---
description: TPO Model Terminology
icon: spell-check
---

# Terminology

To fully utilize the TPO Model, it is essential to understand the market profile concepts it draws and the terms used throughout the settings.

### Auction Market Theory (AMT)

A framework that treats price as the result of a continuous two-way auction between buyers and sellers seeking fair value. The model's profiles are the visual record of that auction: where it paused, where it rejected price, and where it left unfinished business.

### Time Price Opportunity (TPO)

One unit of time spent at a price row. In this model, one TPO block contributes one TPO to every row it traded through. The TPO profile is simply the sum of those blocks across the session.

### TPO Block

The time unit counted as one TPO, set by `Block Size` and defaulting to 30 minutes. A shorter block produces a finer, more granular profile; a longer block smooths the distribution.

### Session

The profile period, set by the model pairing or by a custom timeframe — for example one day or one week. Every completed session becomes the reference for the next one.

### Price Row

A horizontal bin of fixed tick height. Its height is the smallest multiple of the tick size that fits the session range within `Max Rows`.

### Absolute Price Grid

Row boundaries are anchored to price zero, so a given price always falls in the same row across sessions. This is what allows POCs and value-area edges to be compared session to session.

### Profile Engine

The row-store and spread algorithm used to build both profiles. `Modern` is the default; `Classic` is the slower reference implementation and produces the same levels and shapes.

### Intrabar

A lower-timeframe candle inside the current chart bar, used as the raw input for both profiles. Intrabar resolution must be lower than the chart timeframe.

### Point of Control (POC)

The price row with the highest TPO count or highest volume — the market's best estimate of fair value for the session. In this script the POC row is chosen by the highest count, ties resolve to the row closest to the profile centre and then to the upper row, and the plotted POC price is the midpoint of that row.

* **T-POC**: the time-based Point of Control from the TPO profile.
* **V-POC**: the volume-based Point of Control from the volume profile.
* **`V-POC/T-POC`**: a merged label drawn when both profiles place their POC on the same row.

### Value Area (VA)

The contiguous band of rows around the POC that contains the configured share of total TPOs or volume (default 70%). Expansion starts at the POC and continues until the accumulated count reaches `Value Area %`; in `Two-Row Pair` mode the two rows above are compared against the two rows below and the larger pair is added, while `Single Row` mode adds the larger single adjacent row. Ties expand upward.

* **VAH — Value Area High**: the top edge of the highest row in the Value Area.
* **VAL — Value Area Low**: the bottom edge of the lowest row in the Value Area.

### Naked POC (nPOC)

A POC from a completed session that price has not yet touched — also called a virgin POC. In the script it is a finalized session POC that no subsequent bar's high-low range has reached. Untouched POCs tend to act as magnets, because the auction has unfinished business at that price.

* **T-nPOC** and **V-nPOC** name the naked POC from the TPO profile and the volume profile respectively.

### Initial Range (ITR)

The high and low of the first hour of the session, taken as the first 60 minutes after the session opens and marked by a vertical line at the session open.

### Excess

A single-print extreme that shows the auction was rejected at that price — the opposite of a poor extreme.

### Buying Tail (BT) and Selling Tail (ST)

A run of single-print rows at the session low (buying tail) or the session high (selling tail), with a minimum run configurable through `Tails Min Rows` and defaulting to 3. A buying tail shows responsive buying rejected lower prices; a selling tail shows responsive selling rejected higher prices.

### Single Print (SP)

A single-print row inside the profile, away from the extremes. It marks a price zone crossed too quickly for two-way trade, leaving an imbalance the market may revisit.

### Poor High and Poor Low

A session high whose top row printed two or more TPOs, leaving no excess tail, is a poor high — unfinished business above. A session low whose bottom row printed two or more TPOs is a poor low — unfinished business below.

### Balance and Imbalance

A market in **balance** is rotating inside established value. A market in **imbalance** is discovering value outside the previous range. The model's value areas are the reference for telling the two apart.

### Acceptance

Price sustains outside a value boundary. In the dashboard the test is stricter than in the alerts: two consecutive intrabar closes beyond the previous VAH or VAL.

### Rejection

Price probes beyond a boundary but closes back inside. Rejection is the opposite outcome to acceptance and is tracked per boundary in the dashboard and the alerts.

### Failed Auction

An attempt to auction beyond a boundary that is rejected and returns into value.

### 80% Rule

When price opens or trades outside the previous Value Area and then closes back inside twice, the auction has roughly an 80% historical probability of traversing to the opposite boundary.

### HTF Sweep

An HTF candle that trades through a prior HTF candle's high or low but closes back inside its range, indicating a failed liquidity grab. The model requires a sweep before it will look for a structure shift.

### Delivery Leg

The directional sequence of candles that pushed price into the swept extreme. The level that defines the shift is measured against this leg.

### Change in State of Delivery (CISD)

A close beyond the delivery level that produced a sweep, signalling that the prior delivery direction has changed. The level is anchored to the delivery candle's open, and the resulting line is drawn in the configured style.

### Market Structure Shift (MSS)

The same structural change as a CISD, but the level is anchored to the wick of the delivery candle instead of its open, which makes it the more conservative of the two confirmations.

### Pending and Confirmed CISD

A **pending CISD** has formed while the sweeping HTF candle is still open: it is drawn dotted and is not yet confirmed. A CISD is **confirmed** once the sweeping HTF candle closes with the level broken, or once it forms after that candle has closed, and it is drawn solid.

### Invalidated Sweep

A sweep that price has closed back through, which removes the sweep and any CISD built on it.

### Sweep Swing Point

The high or low of the candle that produced the sweep. Taking it out invalidates the CISD.

### Volume Bubble

A right-margin marker for a bar whose volume anomaly exceeds the configured multiple of its 50-bar average.

* **Relative**: compares raw volume against its 50-bar average.
* **Concentrated**: compares volume divided by the bar's high-low range against its 50-bar average.

### Bias

The dashboard's directional score, built from previous-session and current-session value-area interaction plus POC side. Its five outputs are **Bullish**, **Slightly Bullish**, **Neutral**, **Slightly Bearish**, and **Bearish**.

### On-Chart Notation

* **`T-POC` / `V-POC`**: time and volume Points of Control.
* **`T-nPOC` / `V-nPOC`**: untouched time and volume Points of Control.
* **`VAH` / `VAL`**: Value Area High and Low.
* **`ITR`**: Initial Range marker at the session open.
* **`BT` / `ST`**: Buying Tail and Selling Tail.
* **`SP`**: Single Print.
* **`Poor High` / `Poor Low`**: poor session extremes.
* **`❖ <TF> Sweep`**: bullish HTF sweep, while **`✦ <TF> Sweep`** is the bearish one.
* **`<TF> CISD` / `<TF> MSS`**: change in state of delivery or market structure shift on that timeframe.
* **`TPO (partial)` / `Volume (partial)`**: the session lacks intrabar data for part of its range.
* **`Tick volume`**: forex volume is tick-based, not contract volume.

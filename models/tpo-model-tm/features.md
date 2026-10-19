---
description: TPO Model Features
icon: alien-8bit
---

# Features

The CandelaCharts TPO Model turns raw time-at-price data into a complete auction-reading system, from profile construction to confirmed level alerts.

* **Dual Auction Profiles**: Builds a Time Price Opportunity (TPO) profile and an independent Volume profile on the same session, each with its own point of control and value area.
* **Independent Value Areas**: TPO and Volume value areas use separate percentages and separate POC calculations, so you can see where time and volume disagree about fair value.
* **Flexible Value-Area Expansion**: Choose `Two-Row Pair` to reproduce the classical TPO build, or `Single Row` to expand the value area one row at a time.
* **Absolute Price Grid**: Rows are anchored to price zero, so the same price always maps to the same row in every session and profiles stay vertically comparable as you scroll back.
* **Adaptive Row Density**: `Max Rows` (10–200) caps profile resolution, with row height derived from the session range in tick multiples.
* **Histogram or Polyline**: Render the profile as a filled histogram or a thin polyline, with adjustable width as a percentage of session duration.
* **Initial Range (ITR)**: Marks the first hour of the session with a high-to-low range so you can see where the auction established its opening balance.
* **Tails and Single Prints**: Detects buying and selling tails at the session extremes (`BT` / `ST`) and single-print runs inside the profile, with a configurable minimum run.
* **Poor Highs and Lows**: Flags extremes that printed two or more rows instead of a clean single-row tail, a signature of unfinished business.
* **Naked POC Tracking**: Keeps up to 20 untouched POCs per profile type and extends them forward until price revisits them.
* **Model Pairing**: Pairs a profile timeframe with an execution HTF through presets (e.g., `1D - 1H`, `1W - 4H`) or fully custom pairing, with auto pairing from the chart timeframe.
* **Projected HTF Candles**: Draws up to four HTF groups in the right margin — the paired model HTF plus optional HTF I, II, and III — each with its own history and a live close countdown.
* **HTF Sweeps and CISD**: Detects when an HTF candle takes a prior HTF candle's high or low and closes back inside, then the resulting change in state of delivery, marking pending and confirmed structure shifts.
* **Cross-Timeframe Merging**: Merges sweeps and CISDs that land on the same level into one line whose label lists every timeframe that produced it.
* **Volume Bubbles**: Highlights bars whose volume (or volume per unit range) exceeds a multiple of its 50-bar average, sized in four tiers and placed in the right margin.
* **Auction Dashboard**: A compact panel showing the model name, session countdown, latest value-area event, and directional bias, with nine screen positions and ten built-in bull/bear themes.
* **Level and Structure Alerts**: Alerts for POC, VAH, and VAL reach, acceptance outside value, rejection from value, naked POC touches, and CISD pending or confirmed.

---
hidden: true
icon: list-timeline
---

# Footprint

## Volume Footprint

Volume Footprint is a built-in feature of the AMD Model that uses lower timeframe calculations to plot single-candle volume profiles directly on your HTF ghost candles. It reveals where volume concentrated within each HTF candle, helping you identify points of control, volume voids, delta imbalances, and trapped traders — all in the context of the AMD cycle.

When combined with the classic HTF candle structure and CISD levels, the footprint transforms a simple ghost candle into a high-resolution volume map that supports precise entry and exit decisions.

### How It Works

The footprint divides each HTF candle's price range (Low → High) into bins using a configurable **Lot Size** (percentage-based step). It then uses **lower timeframe data** to count how many LTF candle closes fall within each bin and whether those closes were bullish or bearish.

#### Binning Process

1. Starting from the HTF candle's **Low**, the script creates price levels stepping upward by `Low × (Lot Size × n) / 100`
2. Each level defines a bin — a horizontal slice of the candle's range
3. LTF candle data is fetched via `request.security_lower_tf` and each sub-candle's close is assigned to the bin it falls within
4. **Bullish closes** (close > open) add volume; **bearish closes** (close < open) subtract volume

#### Reading the Blocks

Each bin is drawn as colored `▉` blocks inside the transparent footprint candle:

| Block Width        | Meaning                                           |
| ------------------ | ------------------------------------------------- |
| `▉` (1 block)      | Below average activity                            |
| `▉ ▉` (2 blocks)   | Above average activity                            |
| `▉ ▉ ▉` (3 blocks) | Maximum activity (POC or void, depending on mode) |

The **lot count** number beside each level shows exactly how many LTF closes landed in that bin.

{% hint style="info" %}
**Lot Size** is the starting point, always calculated from the Low of the candle. Start with `0.01` and adjust until the bins fill the candle height cleanly. Smaller values create more bins (finer resolution), larger values create fewer bins (coarser view).
{% endhint %}

### Modes

#### Point of Control

The default mode. Highlights the **Point of Control** — the price level with the most LTF closes within the HTF candle.

| Color         | Meaning                                            |
| ------------- | -------------------------------------------------- |
| 🟠 Gold (POC) | Maximum lot count — the most contested price level |
| ⚪ Gray        | Above-average lot count                            |
| ⚫ Dark        | Below-average lot count                            |

**How to read with HTF candles & CISD:**

* A **POC near the Open** of a bearish HTF candle suggests distribution happened early — sellers were in control from the start
* A **POC near the Close** confirms strong directional conviction in that phase
* When the **CISD level aligns with the POC**, it marks a high-probability zone where the market structure shift was backed by significant volume — a strong confirmation signal
* A **POC at the extremes** (near High or Low) acts as a support/resistance zone that price is likely to revisit

#### Delta

Shows **buyer vs. seller dominance** at each price level using net delta volume.

| Color    | Meaning                                |
| -------- | -------------------------------------- |
| 🟢 Green | Net bullish volume (buyers dominated)  |
| 🔴 Red   | Net bearish volume (sellers dominated) |
| ⚫ Dark   | Zero lot count (void)                  |

**How to read with HTF candles & CISD:**

* In a **bullish AMD candle**, look for green delta at the Manipulation low — this shows buyers absorbing the liquidity sweep
* In a **bearish AMD candle**, red delta at the Distribution high confirms sellers are trapping late buyers
* **Mixed delta** (green and red interleaved) near the CISD level suggests the market structure flip was contested — watch for continuation or reversal
* **One-sided delta** through the entire candle indicates strong directional flow with minimal opposition

#### Delta Gradient

A continuous gradient version of Delta mode for smoother visualization.

The color shifts from **red** (strong bearish delta) through neutral to **green** (strong bullish delta), making it easy to visually scan where buying and selling pressure transitions.

**How to read with HTF candles & CISD:**

* Look for **gradient transitions** — where the color shifts from green to red (or vice versa) often marks the exact price level where control changed hands
* This transition point frequently aligns with the **CISD level**, confirming the structural shift
* A **uniformly green/red gradient** through the candle indicates one-sided flow with no structural opposition

#### Total Volume

Displays the **absolute net volume** within each bin using a gradient from low to high.

| Color   | Meaning                 |
| ------- | ----------------------- |
| ⚪ Light | Highest absolute volume |
| 🔘 Gray | Lowest absolute volume  |

**How to read with HTF candles & CISD:**

* **High volume bins** near the CISD level confirm that the market structure shift had institutional participation
* **Low volume bins** in the middle of the candle suggest price moved quickly through those levels — potential future revisit zones
* Compare the volume distribution between the **Accumulation** and **Distribution** phases — institutional accumulation often shows concentrated volume at specific levels

#### POC + Voids

Combines Point of Control with volume void detection. Both POC and voids get maximum block width (3 blocks), making them equally prominent.

| Color   | Meaning                                              |
| ------- | ---------------------------------------------------- |
| 🟠 Gold | POC — maximum lot count                              |
| ⚫ Dark  | Void — zero-close zones (no LTF candles closed here) |
| ⚪ Gray  | Normal activity                                      |

**How to read with HTF candles & CISD:**

* **Voids** are price levels where no LTF candles closed — similar to Fair Value Gaps (FVGs), price tends to return to fill these imbalances
* Voids **above the CISD level** in a bearish candle represent unfilled sell-side imbalance — price may retrace up to fill before continuing lower
* Voids **below the POC** suggest price moved through quickly during manipulation — expect a future fill
* The **distance between POC and the nearest void** indicates how far price might retrace before finding support/resistance

#### Voids

Isolates **volume voids only** — price levels where zero LTF candles closed within the bin.

| Color  | Meaning                                   |
| ------ | ----------------------------------------- |
| 🔴 Red | Void — zero-close zone (maximum 3 blocks) |
| ⚪ Gray | Normal activity (2 blocks)                |
| ⚫ Dark | POC (minimum 1 block — de-emphasized)     |

**How to read with HTF candles & CISD:**

* Pure void mode strips away everything except the imbalances, giving you a clean map of where price needs to return
* **Cluster of voids** in the wick area of the HTF candle marks an aggressive move that will likely be retraced
* Voids that form **between the Manipulation and Distribution phases** are high-probability fill targets
* Use void locations to set **take-profit levels** or identify where price may stall during the next session

### Settings

| Setting          | Default          | Description                                               |
| ---------------- | ---------------- | --------------------------------------------------------- |
| **Footprint**    | Off              | Toggle footprint visibility                               |
| **Mode**         | Point of Control | Select the coloring/display mode                          |
| **Lot Size**     | 0.01             | Percentage step size for bins. Smaller = finer resolution |
| **LTF**          | 5                | Lower timeframe for sub-candle data                       |
| **POC Colors**   | 🟠 ⚪ ⚫           | POC, above-average, below-average                         |
| **Delta Colors** | 🟢 🔴 ⚫          | Bullish, bearish, zero                                    |
| **Total Colors** | ⚪ 🔘 ⚫           | High volume, low volume, background                       |
| **Gaps Colors**  | 🔴 ⚪ ⚫           | Void, normal, POC                                         |
| **Space**        | 5                | Spacing between footprint candles                         |
| **Show Lots**    | On               | Display lot count numbers                                 |

{% hint style="warning" %}
The footprint uses labels for rendering. Pine Script limits labels to **500 per script**. Each candle's footprint uses roughly 40-80 labels depending on lot size. With many HTF candles enabled, you may hit the label budget. Reduce the number of candles or increase the lot size if rendering issues occur.
{% endhint %}

### Correlation with AMD Phases

The footprint's real power emerges when reading it in the context of AMD phases:

#### Accumulation Phase

* Look for a **concentrated POC** near the candle's Open — institutions accumulating positions create a dense volume cluster
* **Delta showing absorption** (green below + red above) confirms smart money is buying the dip / selling the rip

#### Manipulation Phase

* **Voids forming during the sweep** indicate price moved aggressively to grab liquidity without genuine participation
* A **shift in delta** from one color to the other at the manipulation extreme marks the reversal point

#### Distribution Phase

* The **POC shifts toward the Close** as institutions distribute their position
* **Voids left during distribution** become fill targets for the next session
* When the **CISD level sits at or near a void**, it creates a high-conviction entry — the structural shift happened at an imbalanced price level

### Tips

{% hint style="info" %}
**Finding the right Lot Size:**

* Start with `0.01` and increase until the bins fill the candle cleanly
* For crypto (large price values): try `0.05` to `0.25`
* For indices/futures (ES, NQ): try `0.005` to `0.02`
* For forex: try `0.01` to `0.05`
{% endhint %}

{% hint style="info" %}
**LTF Selection:**

* To spot **more voids**, select a LTF close to your chart timeframe
* To spot **fewer voids**, select a LTF further away from your chart timeframe
* Example: on a 5m chart with 1D HTF, try `5` or `3` for LTF
{% endhint %}

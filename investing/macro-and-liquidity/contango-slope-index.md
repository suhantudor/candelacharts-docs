---
icon: blinds-open
---

# Contango Slope Index

{% hint style="info" %}
The Contango Slope Index is available on the <a href="https://www.candelacharts.com/algorithms" class="button secondary medium" data-icon="chart-kanban">CandelaCharts</a> platform as part of Algorithms, in the Professional plan, and on the<a href="https://www.tradingview.com/u/CandelaCharts/" class="button secondary medium" data-icon="display-chart-up">TradingView</a> platform as part of<a href="https://www.candelacharts.com/indicators" class="button secondary medium" data-icon="chart-kanban">CandelaCharts</a> Indicators, in the Investing and Institutional plans.
{% endhint %}

> Measure the steepness and direction of the VIX volatility term structure to spot market complacency, structural stress, and panic-driven reversals.

<figure><img src="../../.gitbook/assets/docs-csi-001.png" alt=""><figcaption></figcaption></figure>

### Introduction

Spot VIX alone only shows what options traders are paying for 30-day volatility right now—it does not tell you how near-term fear compares with longer-term expectations. When short-term implied volatility surges above longer-dated volatility (backwardation), markets are pricing acute panic; when longer-dated volatility trades steadily above short-term volatility (contango), markets are calm and risk-seeking.

The **CandelaCharts – Contango Slope Index** quantifies the annualized slope of the VIX term structure in percentage points per year (`%/yr`) across up to five toggleable CBOE VIX tenors (`VIX1D`, `VIX`, `VIX3M`, `VIX6M`, and `VIX1Y`), defaulting to `VIX6M` and `VIX1Y`. Combined with an optional Moving Average filter and six clear regime classifications, it turns volatility curve dynamics into an actionable macro gauge.

Built for **equity index traders, volatility analysts, and macro allocators**, the oscillator helps distinguish routine contango carry from excessive complacency above **+2.32%/yr** or acute backwardation below **0%**.

{% hint style="info" %}
**TL;DR:** Positive readings indicate **contango** (calm, upward-sloping volatility curve), while negative readings below **0%** indicate **backwardation** (near-term panic exceeding longer-dated volatility, historically a contrarian equity bottoming signal).
{% endhint %}

### How It Works

**CandelaCharts – Contango Slope Index** pulls daily implied volatility across whichever CBOE VIX tenors you enable (`VIX1D`, `VIX`, `VIX3M`, `VIX6M`, and `VIX1Y`) and tracks the annualized steepness of the curve over your `Slope Lookback` window (default `5` days). If only a single tenor is enabled, it smoothly falls back to tracking that single tenor's directional change over the lookback period.

When the optional Moving Average (`MA`, defaulting to `200 SMA`) is evaluated alongside the smoothed slope, the indicator classifies conditions into six distinct regimes—comparing both the curve's sign (contango vs. backwardation) and whether volatility structure is steepening above or flattening below its longer-term trend.

#### Reading the Indicator

The plotted slope line changes color at zero (**Blue** for `>= 0%` contango, **Orange** for `< 0%` backwardation), framed by three dashed reference lines (**+2.32%/yr** Avg Contango, **0** Flat Curve, and **-2.0%/yr** Mild Backwardation) and a subtle **Neutral Zone** band between `-2.0%/yr` and `+2.32%/yr`:

| Regime Label         | Slope Condition     | Trend vs. MA | Right-Edge Badge | Interpretation                                                   |
| -------------------- | ------------------- | ------------ | ---------------- | ---------------------------------------------------------------- |
| **Elevated Risk**    | `> +2.32%/yr`       | Above MA     | Orange           | Steep contango above historical average; rising complacency risk |
| **Cooling Phase**    | `> +2.32%/yr`       | Below MA     | Blue             | Steep contango starting to flatten toward normal                 |
| **Bullish Contango** | `0%` to `+2.32%/yr` | Above MA     | Green            | Healthy upward-sloping curve with improving structure            |
| **Normal**           | `0%` to `+2.32%/yr` | Below MA     | Gray             | Balanced contango with mild softening momentum                   |
| **Recovery**         | `< 0%`              | Above MA     | Green            | Curve still inverted, but steepening out of panic                |
| **Capitulation**     | `< 0%`              | Below MA     | Red              | Deepening backwardation and acute near-term fear                 |

A live label at the latest bar displays the active regime icon, regime name, annualized slope (`%/yr`), and—when `MA` is enabled—the Moving Average value and structural trend direction.

### Features

* **Multi-Tenor VIX Coverage:** Independently toggle `VIX1D`, `VIX` (1M), `VIX3M`, `VIX6M`, and `VIX1Y` (defaulting to `VIX6M` + `VIX1Y`), with automatic single-tenor trend fallback if only one is selected.
* **Annualized Slope Output:** Expresses term-structure steepness in clear annualized percentage points (`%/yr`) alongside the `+2.32%/yr` historical average contango benchmark.
* **Six-Regime Classification:** Combines slope level with Moving Average context (`SMA`, `EMA`, `RMA`, `WMA`, or `VWMA` across lengths `20` to `200`) to distinguish _Capitulation_ from _Recovery_ and _Bullish Contango_ from _Elevated Risk_.
* **Optional MA & Background Shading:** Toggle the Moving Average line, trend-vs-MA fill shading, and full-pane regime background tinting (`Bg`).
* **Six Built-In Alerts:** Covers backwardation entry/exit, elevated complacency above `+2.32%/yr`, and slope-vs-MA momentum crossovers.

### How To Use

#### 1. Spotting Fear Extremes & Capitulation Bottoms (< 0%)

Watch for **Backwardation** when the slope drops below the **0** dashed line into orange territory:

* **Capitulation (Red):** Slope is negative and falling below its Moving Average—near-term fear is still intensifying.
* **Recovery (Green):** Slope remains negative (`< 0%`) but crosses back above its Moving Average, signaling that acute panic is beginning to subside—historically an early inflection point for equity market rebounds.

#### 2. Monitoring Complacency Above +2.32%/yr

When contango expands above the **+2.32%/yr** historical average benchmark into **Elevated Risk**:

* Markets are pricing unusually low near-term risk relative to longer-dated maturities.
* While calm trends can persist, sustained readings above `+2.32%/yr` warn that complacency is elevated and equity pullbacks can unwind quickly if volatility spikes.

#### 3. Customizing Tenors & Moving Average Context

* **Long-End Macro View (Default):** Keeping `VIX6M` and `VIX1Y` enabled filters out brief daily noise and highlights broader institutional volatility regimes.
* **Tactical / Short-Term View:** Enable `VIX` (`1M`) and `VIX3M` (or `VIX1D`) when you want faster sensitivity to sudden front-month volatility shocks, and enable `MA` (`200` or `50` period) to visualize the structural trend line and fill directly on the pane.

### Alerts

**CandelaCharts – Contango Slope Index** includes six built-in TradingView alert conditions:

1. **Backwardation Detected (Bullish Signal):** Fires while the smoothed slope is below `0` (inverted VIX curve).
2. **Exit Backwardation:** Fires when the slope crosses back above `0` (re-entering contango).
3. **Elevated Complacency:** Fires when the slope crosses above `+2.32%/yr` (above historical average contango).
4. **Potential Bullish Setup:** Fires when the slope crosses below `0` into backwardation.
5. **Slope Crosses Above 200EMA:** Fires when the smoothed slope crosses above its configured Moving Average.
6. **Slope Crosses Below 200EMA:** Fires when the smoothed slope crosses below its configured Moving Average.

### FAQs

#### 1. What is the difference between contango and backwardation?

**Contango** (positive slope) means longer-dated VIX expectations are higher than near-term volatility—the normal state during stable or rising markets. **Backwardation** (negative slope) means immediate volatility exceeds longer-term expectations, reflecting acute fear or hedging demand during market sell-offs.

#### 2. Why are VIX6M and VIX1Y enabled by default instead of all five tenors?

`VIX6M` and `VIX1Y` capture clean, structural institutional risk pricing without reacting to every single-day options expiration spike. Enabling `VIX1D`, `VIX`, or `VIX3M` increases responsiveness to fast front-end panics; if you enable only one tenor, the indicator switches to tracking that tenor's change over your `Slope Lookback`.

#### 3. What does the +2.32%/yr reference line represent?

`+2.32%/yr` marks the long-run average contango slope benchmark. Readings above this line indicate an unusually steep upward curve where near-term fear is heavily discounted relative to long-dated volatility—flagging elevated complacency.

#### 4. How does the Moving Average setting affect the indicator?

Even when the `MA` line display is toggled off, the configured Moving Average (default `200 SMA`) is used under the hood to separate improving structure (slope above MA) from weakening structure (slope below MA) in the six-regime badge. Turning `MA` on plots the line and subtle green/red trend fill directly on the pane.

#### 5. Which chart timeframes work best?

All VIX tenor feeds are pulled on daily resolution, making **Daily (`1D`)** and **Weekly (`1W`)** equity index charts (such as `SP:SPX`, `AMEX:SPY`, or `NASDAQ:IXIC`) ideal for consistent macro regime context.

---
icon: square-half-horizontal
---

# Dynamic Exposure Model

{% hint style="info" %}
The Dynamic Exposure Model is part of <a href="https://www.candelacharts.com/algorithms" class="button secondary medium" data-icon="chart-kanban">CandelaCharts</a>Algorithms, available with the Professional plan.
{% endhint %}

> Convert multi-horizon trend momentum and volatility scaling into an actionable 0–100% long-only position size with anti-churn rebalancing bands.

### Introduction

Most trend indicators give binary buy-or-sell signals that treat a calm, textbook uptrend the exact same way as a wild, erratic swing. Without position sizing and volatility control, traders either stay under-exposed during clean trends or hold oversized positions when turbulence doubles.

The **CandelaCharts – Dynamic Exposure Model** converts multi-horizon price momentum into a continuous, **long-only position size from 0% (`FLAT`) to 100% (`HOLD 100%`)**. It automatically scales exposure down when an asset becomes unusually volatile and applies a configurable **Rebalance Threshold** so minor fluctuations never force needless portfolio churn.

Built for **systematic swing traders, trend followers, and crypto/equity investors**, it delivers confirmed bar-close sizing changes, optional chart candle tinting, a compact **HUD Panel**, and real-time trade alerts.

{% hint style="info" %}
**TL;DR:** **Green columns (`Held size %`)** tell you what percentage of a full position to hold on closed bars, the **white step line (`Target size %`)** previews live target sizing, and **Gray (`FLAT`)** means negative or absent trend momentum where the model steps aside into cash.
{% endhint %}

### How It Works

**CandelaCharts – Dynamic Exposure Model** blends normalized returns across a configurable range of short-to-long lookback horizons into a single volatility-adjusted **Momentum Score**, then translates positive scores into a `0%` to `100%` target position size.

When **Volatility Scaling** is enabled, exposure automatically dials back whenever current asset volatility rises above its own normal historical baseline. Held exposure (`Held size %`), main-chart candle tinting, the HUD badge, and built-in alerts update strictly on **confirmed bar closes**—never repainting historical bars—and only adjust when target size drifts past your **Rebalance Threshold (%)** (or moves cleanly between zero and active exposure).

#### Reading the Indicator

Toggle `Pane Shows` between `Size` (default position-sizing columns) and `Score` (raw momentum oscillator):

| Visual Element              | Mode / Color                                                         | How to Read It                                                                                       |
| --------------------------- | -------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| **Held size % Columns**     | Gradient **Gray** (`0%`) to **Green** (`100%`)                       | Confirmed bar-close recommended allocation between `0%` and `100%` (`50%` & `100%` reference lines)  |
| **Target size % Step Line** | Subtle **White** step line (`Size` mode)                             | Real-time un-banded target sizing; shows whether pressure is building toward the next rebalance step |
| **Momentum score**          | **Green** (`> 0`) / **Gray** (`<= 0`) line (`Score` mode)            | Underlying multi-horizon momentum relative to `0` and the **Full size at** threshold line            |
| **Chart Candle Tinting**    | Optional **Gray** (`FLAT`) to **Green** (`HOLD 100%`)                | Paints main price candles directly with current held exposure intensity                              |
| **HUD Panel**               | `Exposure` (`FLAT` / `HOLD XX%`), `Score`, `Volatility` (`x normal`) | Instant at-a-glance sizing, momentum score, and volatility multiplier relative to normal             |

All horizons (`Min / Max`, `Horizon Blend Count`), `Volatility Half-Life`, `Full Exposure Threshold`, `Rebalance Threshold (%)`, `Volatility Scaling`, and colors are customizable in settings.

### Features

* **Continuous 0–100% Position Sizing:** Replaces rigid all-in/all-out guesswork with smooth fractional sizing calibrated to momentum conviction.
* **Automatic Volatility Scaling:** Measures current volatility relative to the asset's own normal baseline (displayed as `x normal` in the HUD) to automatically shrink exposure during turbulent markets.
* **Anti-Churn Rebalance Band:** Filters out noisy micro-adjustments so your held position only changes when target sizing moves meaningfully or enters/exits cash.
* **Non-Repainting Bar-Close Execution:** Separates the live `Target size %` preview from confirmed `Held size %`, candle colors, and alerts so closed signals never shift retroactively.
* **Dual Pane Views & Built-In Alerts:** Inspect `Size` percentages or raw `Momentum score`, mirror exposure onto price candles, and trigger alerts on opens, closes, and size changes.

### How To Use

#### 1. Scaling In and Out Dynamically (`Size` Mode)

Follow the **Held size %** columns and the HUD **Exposure** row (`HOLD XX%` or `FLAT`):

* When **Exposure** steps from `FLAT` into active green bars, initiate a starter position matching the displayed percentage.
* As trend momentum strengthens across multiple horizons and volatility stays tame, step up exposure toward `100%`; when `Target size %` and `Held size %` step down, trim size gradually into strength or fading momentum.

#### 2. Using Volatility Scaling During High-Turbulence Markets

Watch the **Volatility** row in the **HUD Panel** (for example, `1.0x normal` versus `2.0x normal`):

* Even when trend momentum remains positive, a spike well above normal volatility automatically compresses `Held size %` proportionally—keeping dollar risk controlled without requiring manual stop guesswork.

#### 3. Inspecting Underlying Conviction in `Score` Mode

Switch `Pane Shows` to **Score** whenever you want to inspect whether trend momentum is hovering just above `0`, accelerating toward the **Full size at** upper boundary, or remaining deeply negative below zero (`FLAT`).

### Alerts

**CandelaCharts – Dynamic Exposure Model** includes three built-in TradingView alert conditions evaluated on confirmed bar closes:

1. **Position opened:** Fires when held exposure transitions from `0%` (`FLAT`) into an active position.
2. **Position closed:** Fires when held exposure exits completely back to `0%` (`FLAT`).
3. **Size changed:** Fires whenever an already-active held position steps up or down past your rebalance threshold.

### FAQs

#### 1. Does the indicator support short selling when momentum turns negative?

No. **Dynamic Exposure Model** is strictly **long-only**: negative momentum reduces target and held exposure down to **0% (`FLAT`)**, signaling to sit out in cash rather than shorting.

#### 2. Why did `Target size %` move slightly while `Held size %` stayed flat?

That is the **Rebalance Threshold (%)** working as intended. To avoid constant small trades around minor score wiggles, held size updates only when the target moves at least the threshold distance away from your current size (or switches cleanly between `0%` and active exposure).

#### 3. Does this indicator repaint?

No. While the live bar lets `Momentum score` and `Target size %` update with current price, **Held size %**, candle colors, and all three alerts lock strictly on confirmed bar closes.

#### 4. Why does the HUD say `warming up` next to Volatility on newer charts?

When **Volatility Scaling** is enabled, it compares current volatility against a longer baseline history of the asset. Until enough historical bars exist on a young listing, the model relies cleanly on momentum strength alone.

#### 5. Which timeframes and assets work best?

Because horizons and volatility scale dynamically to the series on your chart, **Dynamic Exposure Model** works across **crypto, stocks, ETFs, indexes, and commodities** on **4H, Daily, and Weekly** charts (higher timeframes reduce noise and turnover).

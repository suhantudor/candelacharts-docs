---
icon: omega
---

# Omega Ratio

> Measure return quality without normality assumptions by comparing cumulative excess gains above your target hurdle against cumulative shortfalls below it.

<figure><img src="../../../.gitbook/assets/docs-omega-ratio-002.png" alt=""><figcaption></figcaption></figure>

### Introduction

Most traditional performance ratios summarize risk using a single statistic like standard deviation, which assumes returns follow a clean bell curve. In real markets, returns are skewed and fat-tailed—meaning occasional big gains or sudden drops matter far more than average variance implies.

The **CandelaCharts – Omega Ratio** takes a distribution-free approach. Instead of reducing volatility to standard deviation, it separates every bar's return within a rolling window into **excess gains** above a chosen per-bar target and **shortfalls** below that target, then takes their ratio.

Designed for **active traders, momentum followers, and portfolio allocators**, it turns noisy bar-by-bar return distributions into a clear quality score: values above **1.0** mean cumulative gains above your hurdle outweigh cumulative misses, while values below **1.0** warn that shortfalls dominate.

{% hint style="info" %}
**TL;DR:** An Omega Ratio above **1.0** marks favorable, breakeven-clearing performance; **1.5+** signals good trend quality; and **2.0+** indicates strong, sustained directional compounding.
{% endhint %}

### How It Works

#### Calculation

On every bar, the indicator computes the Omega Ratio across your rolling `Period` window (default `20` bars):

1. **Return & Target Alignment:** Computes per-bar **Simple** (default) or **Log** returns and converts your per-bar `Target Return` (default `0.0`) into the same return space.
2. **Gain vs. Shortfall Separation:** On each bar, any return above the target is recorded as an **Excess Gain**, while any return below the target is recorded as a **Shortfall**.
3. **Rolling Ratio & Thermal Gradient:** Sums excess gains and shortfalls across `Period`, divides total gains by total shortfalls, and colors the line along a smooth **Orange → Gray → Blue** scale up to your `Gradient` ceiling (default `2.0`).

#### Mathematical Formula

**1. Per-Bar Return & Target Adjustment**

```
Simple Return = (Close / Previous Close) - 1
Log Return    = ln(Close / Previous Close)

Target (Simple) = Target Return
Target (Log)    = ln(1 + Target Return)
```

**2. Excess Gains & Shortfalls**

```
Excess Gain = max(Return - Target, 0)
Shortfall   = max(Target - Return, 0)
```

**3. Rolling Omega Ratio**

```
Omega Ratio = Sum(Excess Gain over Period) / Sum(Shortfall over Period)
```

If `Sum(Shortfall)` equals zero across the entire lookback window (meaning every bar met or beat the target), the indicator avoids division by zero and outputs `na` until a shortfall occurs.

#### Visual Guide

The plotted line shifts continuously from **Orange** (`0.0`) through **Gray** (midpoint, default `1.0`) to **Blue** (at or above `Gradient`, default `2.0`), framed by four horizontal reference lines:

| Omega Ratio | Zone Label             | Guide Line           | Interpretation                                |
| ----------- | ---------------------- | -------------------- | --------------------------------------------- |
| `< 0.5`     | Poor                   | Dotted Gray (`0.5`)  | Heavy downside shortfalls dominate gains      |
| `0.5 – 1.0` | Suboptimal             | —                    | Shortfalls still exceed excess gains          |
| `1.0`       | Breakeven              | Solid Orange (`1.0`) | Cumulative gains equal cumulative shortfalls  |
| `1.0 – 1.5` | Acceptable / Favorable | —                    | Excess gains outweigh shortfalls above target |
| `1.5 – 2.0` | Good Performance       | Dashed Teal (`1.5`)  | Clean trend quality with favorable skew       |
| `>= 2.0`    | Strong Performance     | Dotted Blue (`2.0`)  | High-efficiency compounding regime            |

### Features

* **True Distribution-Free Omega:** Computes exact rolling sums of excess gains divided by shortfalls relative to your per-bar target hurdle.
* **Simple & Log Return Support:** Toggle between arithmetic percentage returns (default) and logarithmic returns for symmetric handling of large swings.
* **Dynamic Thermal Gradient:** Smooth **Orange → Gray → Blue** color mapping scaled to a customizable `Gradient` upper bound (default `2.0`).
* **Four Benchmark Guides:** Pre-configured reference lines at `0.5` (Poor), `1.0` (Breakeven), `1.5` (Good), and `2.0` (Strong) for instant visual grading.
* **Built-In Breakeven Alerts:** Includes native `Omega crossed above 1` and `Omega crossed below 1` alert conditions out of the box.

### How To Use

#### 1. Breakeven Regime Filtering (Omega > 1.0)

Use the **1.0** breakeven line as your primary trend-quality filter:

* **Above 1.0:** Cumulative gains above your target exceed shortfalls—conditions favor pro-trend participation and holding winners.
* **Below 1.0:** Losses and misses below target outweigh gains—tighten risk, scale down size, or stand aside until Omega reclaims **1.0**.

#### 2. Calibrating the Per-Bar Target Return

Set `Target Return` as a per-bar decimal hurdle that matches your timeframe:

* **Zero Hurdle (`0.0`):** Measures pure positive-vs-negative return balance (gains vs. losses).
* **Daily Trend Hurdle (`0.0005` – `0.001`):** Requires an average `0.05%` to `0.10%` per daily bar to qualify as excess gain, filtering out flat, sideways chop.
* **Intraday Charts:** Use a smaller hurdle (such as `0.0` to `0.0002`) so normal intraday noise does not keep Omega pinned below **1.0**.

#### 3. Identifying Trend Acceleration (1.5+ and 2.0+)

Watch transitions from the gray breakeven zone into teal and blue territory:

* Crossing above **1.5** confirms that upside momentum is consistently outpacing pullbacks.
* Sustained readings above **2.0** mark high-efficiency trends where pullbacks are shallow and short-lived; a sharp drop back below **1.5** warns that trend momentum is cooling.

### Alerts

**CandelaCharts – Omega Ratio** includes two built-in TradingView alert conditions:

1. Open the **Alerts** menu in TradingView and select **CandelaCharts - Omega Ratio** as the condition.
2. Choose **Omega crossed above 1** to receive a notification when return quality flips favorable, or **Omega crossed below 1** when shortfalls take over.
3. Optionally create manual crossing alerts on the **Omega Ratio** plot at **1.5** or **2.0** to catch strong trend accelerations.

### FAQs

#### 1. What does an Omega Ratio of 1.0 mean?

An Omega Ratio of **1.0** is the exact breakeven threshold relative to your `Target Return`. At **1.0**, total cumulative gains above the target over your lookback period exactly equal total cumulative shortfalls below the target.

#### 2. Why does the Omega line occasionally disappear for a few bars?

If every single bar inside your `Period` window beats `Target Return`, then total shortfalls equal zero (`Sum(Shortfall) = 0`). Because dividing by zero is undefined, the indicator cleanly outputs `na` on those rare bars rather than plotting an infinite spike, and resumes as soon as any bar finishes below the target.

#### 3. How should I choose Target Return for daily vs. intraday charts?

Remember that `Target Return` is measured **per bar** as a decimal (`0.001` = `0.1%` per bar). Leaving it at `0.0` works across every timeframe as a baseline gain-vs-loss ratio. On daily charts, `0.0005` to `0.001` adds a mild upward hurdle; on intraday charts, stick to `0.0` or very small decimals (`0.0001`).

#### 4. How does the Period setting change the indicator?

Shorter values (default `20` bars) make Omega responsive to rapid momentum flips and short-term regime changes. Longer values (`50`–`100` bars) smooth out brief pullbacks and highlight broader structural trends.

#### 5. What does the Gradient setting control?

`Gradient` (default `2.0`) sets the upper ceiling for the line's color scale—not the math itself. The indicator maps `0.0` to **Orange**, the midpoint (`Gradient * 0.5`) to **Gray**, and values at or above `Gradient` to **Blue**. Raise `Gradient` (for example to `3.0`) if your asset or timeframe frequently stays above `2.0`.

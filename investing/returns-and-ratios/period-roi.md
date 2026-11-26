---
icon: circle-small
---

# Period ROI

{% hint style="info" %}
The Period ROI is part of <a href="https://www.candelacharts.com/algorithms" class="button secondary medium" data-icon="chart-kanban">CandelaCharts</a>Algorithms, available with the Professional plan.
{% endhint %}

> Track percentage return over calendar-anchored cycles or rolling day windows across any asset, complete with period dividers, historical averages, and regime alerts.

<figure><img src="../../.gitbook/assets/docs-period-roi-002 (1).png" alt=""><figcaption></figcaption></figure>

### Introduction

Eyeballing a price chart rarely gives an accurate sense of how much an asset has actually gained or lost over a specific horizon. When prices scale exponentially or volatility shifts across cycles, raw dollar moves become misleading without a clear percentage baseline.

The **CandelaCharts – Period ROI** solves this by plotting percentage Return on Investment (ROI) cleanly in a dedicated pane across your chosen horizon—whether **Intraday (Daily Open)**, **1M**, **3M**, **6M**, **1Y** (default), or a **Custom (Days)** lookback. With customizable sign-based shading, period boundary dividers, segment summaries, and an optional external `Asset` selector, you can immediately see whether a market is net positive or negative for the active window.

Designed for **intraday traders, swing traders, and long-term investors**, the indicator also summarizes average historical period performance in a compact dashboard and tracks zero-line crossovers so you never miss a regime flip.

{% hint style="info" %}
**TL;DR:** Readings above **0%** show net positive return for the selected period, while readings below **0%** show net negative return. Switch between calendar-anchored cycles (with `Show Dividers` enabled) and continuous rolling day windows (`Custom (Days)` or `Show Dividers` disabled).
{% endhint %}

### How It Works

**CandelaCharts – Period ROI** measures percentage return from a clear starting price across either calendar-anchored cycles or a continuous rolling day window. When using a calendar preset (`Intraday (Daily Open)`, `1M`, `3M`, `6M`, or `1Y`) with `Show Dividers` enabled, the baseline resets cleanly at each new day, month, quarter, half-year, or year boundary so every cycle starts fresh from **0%**.

When using `Custom (Days)` (default `365`) or disabling `Show Dividers`, the indicator switches to rolling mode and continuously measures performance against the specified number of days prior. You can also target an external `Asset` symbol to monitor benchmark or correlated-market ROI directly beneath your active chart, while an automatic timeframe guard warns you if the chart timeframe is larger than the selected period.

#### Reading the Indicator

The oscillator frames returns around a dotted **0%** baseline with customizable **Positive** (`Teal` default), **Negative** (`Red` default), and **Neutral** (`Gray` default) styling:

| Element                      | Visual Appearance                    | Meaning / What It Shows                                                             |
| ---------------------------- | ------------------------------------ | ----------------------------------------------------------------------------------- |
| **Positive ROI (>= 0%)**     | Teal line + translucent fill         | Asset is trading above the period starting price                                    |
| **Zero Line (0%)**           | Dotted Gray baseline                 | Breakeven threshold separating positive and negative regimes                        |
| **Negative ROI (< 0%)**      | Red line + translucent fill          | Asset is trading below the period starting price                                    |
| **Period Dividers & Labels** | Dashed vertical lines + ▲ / ▼ labels | Marks cycle resets alongside final ROI %, open price, and year/asset tooltip        |
| **Current Value Badge**      | Colored label on latest bar          | Displays live ROI % and the active period's starting price                          |
| **Summary Dashboard**        | Compact 2-column table               | Shows the active `Period` label and historical `Avg Return` across completed cycles |

### Features

* **Six Flexible Time Horizons:** Choose from **Intraday (Daily Open)**, **1M**, **3M**, **6M**, **1Y**, or **Custom (Days)** to match scalping, swing, or macro cycles.
* **Calendar-Anchored & Rolling Modes:** Reset cleanly at calendar boundaries with `Show Dividers` on, or view continuous rolling day-over-day ROI with `Custom (Days)` or dividers turned off.
* **External Asset Tracking:** Leave `Asset` blank to track the current chart symbol, or enter any ticker to compare an external benchmark in the lower pane.
* **Rich Visual Context:** Includes sign-based line and area fills, optional full-background ROI sign tinting (`Color Background by ROI Sign`), period boundary dividers, segment tooltips, and a live last-value label.
* **Historical Avg Return Dashboard:** Automatically tracks completed cycle returns and displays the active `Period` alongside the historical `Avg Return` in a configurable corner table.
* **Built-In Zero-Line Alerts:** Ships with ready-to-use `ROI Crosses Above 0` and `ROI Crosses Below 0` alert conditions.

### How To Use

#### 1. Selecting the Right Horizon (Intraday to 1Y & Custom)

Match `Period Preset` to your trading style:

* **Intraday (Daily Open):** Use on intraday charts (`1m`–`4H`) to track live percentage change relative to the daily open.
* **1M & 3M:** Ideal for tactical momentum and quarterly earnings or macro rotation analysis.
* **6M & 1Y (Default):** Highlights medium- and long-term cycle direction around the **0%** breakeven line.
* **Custom (Days):** Enter any number of calendar days (such as `90` or `365`) for a continuous rolling return benchmark.

#### 2. Reading Calendar-Anchored Cycles vs. Rolling Performance

Use the two modes for different questions:

* Keep **Show Dividers** enabled on calendar presets (`1M`, `3M`, `6M`, `1Y`, or `Intraday`) to compare discrete cycles side-by-side—reading the ▲ / ▼ segment labels at the end of each period to see how every month, quarter, or year finished.
* Turn **Show Dividers** off (or select **Custom (Days)**) when you want an unbroken, continuous oscillator showing trailing performance without periodic resets back to **0%**.

#### 3. Comparing External Assets & Historical Averages

* **Benchmarking:** Enter a market benchmark (such as `SPY` or `BTCUSD`) in the `Asset` input while keeping your primary ticker on the main chart to spot relative performance divergences immediately.
* **Evaluating Typical Returns:** Check the **Dashboard**'s `Avg Return` column to see the average ROI across all completed periods on your chart, and enable **Color Background by ROI Sign** when scanning multiple charts quickly.

### Alerts

**CandelaCharts – Period ROI** includes two built-in TradingView alert conditions:

1. Open the **Alerts** menu in TradingView and select **CandelaCharts - Period ROI** as the condition.
2. Choose **ROI Crosses Above 0** to be notified when performance flips positive (`ROI crossed above 0%`), or **ROI Crosses Below 0** when performance turns negative (`ROI crossed below 0%`).
3. Set **Trigger** to **Once Per Bar Close** (recommended) and click **Create**.

### FAQs

#### 1. What is the difference between calendar-anchored periods and rolling ROI?

When `Show Dividers` is enabled with a calendar preset (`Intraday (Daily Open)`, `1M`, `3M`, `6M`, or `1Y`), ROI resets at each new calendar boundary so you see performance since the start of the current day, month, quarter, half-year, or year. When you select `Custom (Days)` or turn `Show Dividers` off, ROI is measured continuously on a rolling day lookback without resets.

#### 2. Why am I seeing a timeframe warning message on the chart?

The indicator displays a reminder if you select **Intraday (Daily Open)** while viewing a Daily (`1D`) or higher chart, or if your current chart timeframe is larger than the selected ROI period (for example, viewing a `1M` chart with a `1M` or shorter preset). Switch to a lower chart timeframe to resume plotting.

#### 3. What does the Avg Return value in the Dashboard represent?

In calendar-anchored mode, `Avg Return` averages the final ROI percentage of every completed period across the chart's loaded history. If no full calendar period has completed yet (or in rolling mode without dividers), the dashboard displays `N/A`.

#### 4. Can I track a different symbol than the one on my main chart?

Yes. Enter any TradingView ticker in the `Asset` field under the **Main** settings group to display that symbol's Period ROI below your active chart, or leave `Asset` blank to track the chart's own symbol.

#### 5. Which Period Preset should I choose for intraday, swing, or long-term analysis?

Use **Intraday (Daily Open)** on intraday charts for session performance, **1M** or **3M** on `1H`–`1D` charts for swing and quarterly rotation, and **6M** or **1Y** on `1D`–`1W` charts for broader structural trend context.

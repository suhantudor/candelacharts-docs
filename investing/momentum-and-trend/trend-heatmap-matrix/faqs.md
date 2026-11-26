---
description: Trend Heatmap Matrix FAQs
icon: square-question
---

# FAQs

<details>

<summary>What do the different "Trading Profiles" (Scalping, Day Trade, etc.) actually do?</summary>

The Trading Profile automatically adjusts the internal timeframes and resolution settings of the 10 components. "Scalping" speeds up the oscillators to catch micro-trends, while "Investment" slows them down significantly to filter out noise and focus on macro direction.

</details>

<details>

<summary>Why is my matrix stuck on "NEUTRAL"?</summary>

This happens when the market is chopping sideways, causing the underlying indicators (like MACD and RSI) to conflict with each other. A neutral reading is a valid signal: it tells you the market lacks a clear trend and you should avoid trend-following entries.

</details>

<details>

<summary>What does "Allow Repainting?" do?</summary>

If you have multi-timeframe (MTF) resolutions enabled inside your components, MTF data inherently updates until the higher timeframe bar closes. Disabling this forces the indicator to only use confirmed, non-repainting historical data, which is safer for backtesting but may induce slight lag in live trading.

</details>

<details>

<summary>Can I turn off indicators I don't use?</summary>

Yes. In the settings, you can uncheck any component (e.g., "MFI" or "Stochastic"). The Matrix will instantly remove that indicator from the dashboard and recalculate the Bull/Bear percentages using only the indicators you left enabled.

</details>

<details>

<summary>How are the Bar Colors calculated?</summary>

If "Color bars?" is enabled, the indicator will paint your candles based on the aggregate bias. Strong Long prints your primary bullish color, Strong Short prints the primary bearish color, and Neutral/Lean states print modified or translucent versions, visually summarizing the entire matrix directly on your price action.

</details>


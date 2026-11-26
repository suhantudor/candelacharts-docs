---
description: Trend Heatmap Matrix Usage
icon: circle-chevron-right
---

# Usage

The Trend Heatmap Matrix is designed to be your final structural filter before entry, ensuring you have the weight of evidence on your side.

### How it works

The indicator mathematically evaluates the state of every enabled component on every bar. For example, it checks if the MACD line is above its signal line, if price is above the VWAP, and if RSI is trending upwards. Each bullish state adds to the "Bull Score," and each bearish state adds to the "Bear Score." These scores are converted into percentages. If the Bull Percentage is >= 80%, the overall bias is "STRONG LONG." If it's >= 60%, it's "LEAN LONG." The same applies to the downside.

### Interpreting the Matrix Bias

* **STRONG LONG (Bull Score >= 80%)**: The vast majority of momentum, volume, and trend indicators are aligned to the upside. This is a high-probability environment for trend-following long trades and breakouts. Shorting here is highly discouraged.
* **LEAN LONG (Bull Score >= 60%)**: The trend is bullish, but some indicators are flashing warning signs (e.g., overbought oscillators or declining volume). Proceed with normal long setups but exercise caution with position sizing.
* **NEUTRAL (Mixed Scores)**: The market is in equilibrium, consolidating, or transitioning. Trend-following systems typically chop in this environment. It is best to wait for a clear directional shift or rely strictly on mean-reversion boundary trading.
* **LEAN SHORT (Bear Score >= 60%)**: The trend is structurally bearish. Favor short setups or tighten stops on remaining long positions.
* **STRONG SHORT (Bear Score >= 80%)**: The market is in a deep, coordinated downtrend across multiple metrics. Focus entirely on shorting bounces and playing breakdowns.

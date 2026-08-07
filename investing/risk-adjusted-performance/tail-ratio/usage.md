---
description: Tail Ratio Usage
icon: circle-chevron-right
---

# Usage

The Tail Ratio is best used to understand the underlying risk and reward profile of an asset before entering a position or to manage risk on active trades.

### How it works

The indicator calculates the return of each bar over the defined lookback period. It then finds the specified upper percentile (e.g., 90th) and lower percentile (e.g., 10th) of these returns. The Tail Ratio is simply the absolute value of the upper percentile divided by the absolute value of the lower percentile. The resulting value is then optionally smoothed using an EMA to create the final oscillator.

### Interpreting the Ratio

* **Right-tailed / Positive Skew (Above Upper Guide, e.g., > 1.20)**: The right tail is "fatter" than the left. This indicates that extreme upside moves are larger than extreme downside moves. The market has a bullish structural bias and is prone to upside volatility.
* **Symmetric / Normal (Around 1.0)**: The tails are roughly equal. Extreme gains and extreme losses are balanced in magnitude. The market is not showing a strong directional bias in its volatility.
* **Left-tailed / Negative Skew (Below Lower Guide, e.g., < 0.80)**: The left tail is "fatter" than the right. Extreme downside moves are larger than extreme upside moves. The market has a bearish structural bias and is highly susceptible to downside shocks.

---
icon: compass
---

# Bias Magnet

Bias Magnet is an adaptive baseline component that tracks trend direction using half-trend style logic. It provides a clean, responsive line that hugs price without whipsaws, making it ideal for identifying trend direction and strength.

### How It Works

Bias Magnet uses a sophisticated algorithm that:

* Tracks the highest high and lowest low within a dynamic period
* Adjusts the baseline based on price action and moving average relationships
* Calculates trend strength from slope and momentum
* Provides visual feedback through dynamic line transparency

#### **Key Features**

### Adaptive Baseline

The baseline adapts to market conditions, moving up in uptrends and down in downtrends. It acts as dynamic support in bullish trends and dynamic resistance in bearish trends.

### Trend Strength Calculation

Bias Magnet calculates trend strength (0–100) by analyzing:

* **Slope magnitude**: How steep the baseline is moving
* **Momentum**: The rate of change in the baseline direction

This strength value is visualized through line transparency—darker lines indicate stronger trends.

### Flip Signals

When the trend changes direction, Bias Magnet displays visual signals:

* **▲ (Up Arrow)**: Bullish flip signal—trend has changed from bearish to bullish
* **▼ (Down Arrow)**: Bearish flip signal—trend has changed from bullish to bearish

These signals appear on the bar where the flip is confirmed, helping you catch trend changes early.

### Polarity Bars

Polarity bars (☰) appear above or below the baseline to show momentum direction:

* **Above baseline**: Bullish momentum
* **Below baseline**: Bearish momentum

The intensity (transparency) of the bars reflects momentum strength—darker bars indicate stronger momentum. These bars use MFI (Money Flow Index) calculations to determine momentum direction and strength.

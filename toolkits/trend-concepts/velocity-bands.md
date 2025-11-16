---
icon: wave-sine
---

# Velocity Bands

Velocity Bands creates dynamic deviation-based support and resistance levels that adapt to market conditions. Using outlier-filtered standard deviation calculations, it identifies extreme price conditions and provides signals for mean reversion and reversal setups.

### How It Works

Velocity Bands calculates:

* A weighted moving average (WMA) as the center line
* Normalized price deviation from the average
* Outlier filtering to remove extreme spikes
* Standard deviation bands at +1/+2 and -1/-2 levels

The bands dynamically adjust to market volatility, expanding in volatile conditions and contracting in calm markets.

#### Key Features

### Dynamic Bands

Velocity Bands creates four levels:

* **+2 Band (Upper Outer)**: Extreme overbought level
* **+1 Band (Upper Inner)**: Moderate overbought level
* **-1 Band (Lower Inner)**: Moderate oversold level
* **-2 Band (Lower Outer)**: Extreme oversold level

The center line (mean) is displayed as a dotted line, providing a reference point.

### Outlier Filtering

Before calculating bands, Velocity Bands filters out outliers (price moves beyond 4 standard deviations). This ensures the bands aren't distorted by extreme spikes or data errors, creating more stable and reliable levels.

### Gradient Fills

The bands include gradient fills:

* **Base fills**: Subtle gradients between +1/+2 and -1/-2 bands
* **Enhanced fills**: When price is outside the bands, enhanced gradients highlight the extreme condition

### Re-entry Signals

When price returns from extreme zones:

* **▼ (Down Arrow)**: Price re-enters from above the +2 band (bearish mean reversion)
* **▲ (Up Arrow)**: Price re-enters from below the -2 band (bullish mean reversion)

These signals suggest price is returning to normal levels after an extreme move.

### Rejection Signals

When price enters a band but fails to hold:

* **Rejection from upper band**: Price entered the upper band but closed below it (bearish reversal)
* **Rejection from lower band**: Price entered the lower band but closed above it (bullish reversal)

These signals indicate potential reversals when price can't sustain moves into the bands.

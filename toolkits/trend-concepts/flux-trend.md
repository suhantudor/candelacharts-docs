---
icon: chart-scatter-bubble
---

# Flux Trend

Flux Trend uses ATR-based bands to identify trend reversals and continuation setups. It creates dynamic zones that flip between bullish and bearish regimes, providing clear visual signals for trend changes and exit opportunities.

### How It Works

Flux Trend calculates:

* A baseline using a Simple Moving Average (SMA)
* Upper and lower bands based on ATR (Average True Range) multiplied by a distance factor
* Trend state that flips when price crosses the bands
* Gradient-filled zones between the main and secondary bands

The indicator tracks when price enters and exits these zones, providing signals for both reversals and continuations.

#### Key Features

#### Dynamic Trend Bands

Flux Trend creates two bands:

* **Main Band (Band 1)**: The primary trend line that flips position based on trend direction
* **Secondary Band (Band 2)**: Creates a zone with the main band for entry/exit detection

#### Gradient-Filled Zones

The area between the two bands is filled with a gradient that:

* **Bullish trend**: Gradient from outer edge (lighter) to inner edge (darker)
* **Bearish trend**: Gradient from outer edge (lighter) to inner edge (darker)

These zones act as support in bullish trends and resistance in bearish trends.

#### Trend Flip Signals

When the trend changes direction, Flux Trend displays:

* **✦ (Star)**: Bull to bear flip—trend has changed from bullish to bearish
* **❖ (Diamond)**: Bear to bull flip—trend has changed from bearish to bullish

A connecting line shows the transition between the old and new band positions.

#### Exit Signals

Flux Trend detects when price leaves the zone after touching it:

* **✦ outside bands**: Bullish exit signal—price left the zone after touching it in a bullish trend
* **❖ outside bands**: Bearish exit signal—price left the zone after touching it in a bearish trend

These exit signals often indicate continuation in the trend direction.

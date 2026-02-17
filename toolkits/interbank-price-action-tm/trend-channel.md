---
icon: arrow-trend-up
---

# Trend Channel

### Visualizing the Drift <a href="#user-content--visualizing-the-drift" id="user-content--visualizing-the-drift"></a>

The **Trend Channel** tool helps you instantly visualize the market's "flow." Whether the market is trending cleanly or drifting chaotically, these channels provide the boundaries you need to identify overbought (Premium) and oversold (Discount) conditions relative to the trend.

### Channel Types <a href="#user-content-channel-types" id="user-content-channel-types"></a>

We offer two distinct methods for calculating the channel, each with its own advantages:

#### 1. Trendline (Pivot-Based) <a href="#user-content-1-trendline-pivot-based" id="user-content-1-trendline-pivot-based"></a>

* **Logic**: This method finds the most recent Pivot Highs and Pivot Lows and draws dynamic trendlines to connect them.
* **Best For**: Traders who prefer "organic" channels that adapt to Market Structure break points.
* **Visual**: Creates a shape that expands and contracts based on volatility.

#### 2. Channel (Linear Regression) <a href="#user-content-2-channel-linear-regression" id="user-content-2-channel-linear-regression"></a>

* **Logic**: Uses a 5-point linear regression algorithm to mathematically fit a channel around the price action.
* **Best For**: Identifying the statistical "mean" of the trend and its standard deviations.
* **Visual**: Creates a smooth, parallel channel that clearly shows the directional bias.

### Configuration <a href="#user-content-configuration" id="user-content-configuration"></a>

#### Style & Aesthetics <a href="#user-content-style--aesthetics" id="user-content-style--aesthetics"></a>

* **Line Style**: Choose Solid, Dashed, or Dotted lines to differentiate the channel from other tools.
* **Fill**:
  * **Enabled**: Adds a translucent background color between the High and Low lines. This makes it easier to spot when price is "inside" the channel versus "breaking out."
  * **Disabled**: Keey only the lines for a cleaner, minimalist look.

#### Sensitivity <a href="#user-content-sensitivity" id="user-content-sensitivity"></a>

* **Pivot Count (Trendline Mode)**: Determines how many recent pivots to connect. increasing this number creates longer-term trendlines.
* **Length (Channel Mode)**: Defines the lookback period for the regression calculation. A higher length equals a smoother, slower-moving channel.

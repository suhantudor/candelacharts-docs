---
icon: grip-dots
---

# Dashboard

The Order Flow Concepts Dashboard is an on-chart panel that aggregates all the raw order flow and liquidity data into a single, easy-to-read summary. It provides a real-time read on market context, helping you establish a directional bias before looking for entries.

### Configuration

* **Dashboard**: Master toggle to show or hide the panel.
* **Position**: Anchor the dashboard to any of the 9 standard chart positions (e.g., Bottom Center, Top Right).
* **Text Size**: Customize the scale of the dashboard text (Tiny, Small, Normal, Large, Huge, Auto).

### Dashboard Metrics

#### Phase

Displays the current **Market Phase** (e.g., Accumulation, Distribution, Markup, Markdown) based on the balance of liquidity and volume anomalies.

#### Trapped

Displays the status of **Trapped Traders**. If the toolkit recently detected a trap anomaly, this will read "Bulls Trapped" (bearish bias) or "Bears Trapped" (bullish bias), serving as a persistent reminder of who is currently offsides in the market.

#### Algorithm (Mode)

The most powerful feature of the dashboard is its ability to aggregate resting liquidity. You can choose the specific **Algorithm (Mode)** used to calculate the directional pull of the liquidity pools:

* **All Active Levels**: Sums the raw volume of all active liquidity pools on the chart.
* **Time-Weighted (Aged)**: Weights the volume of each pool based on its age (bars since birth). Older, more established pools carry higher weight.
* **Gravity (Inverse Square)**: Applies an inverse-square law to the liquidity. Pools that are physically closer to current price exert a massive gravitational pull, while distant pools are mostly ignored.
* **Proximity-Weighted**: Similar to Gravity, but uses a linear proximity multiplier. Closer pools equal higher weight.
* **Top 3 Largest Pools**: Ignores proximity and simply sums the absolute top 3 largest volume pools on the chart.
* **Top 3 Nearest**: Ignores raw size and sums the volume of the 3 pools closest to current price.
* **Largest Single Pool**: Isolates and tracks only the single largest volume pool on the chart.
* **Closest Single Pool**: Isolates and tracks only the single volume pool closest to current price.
* **Void Detection**: Calculates the distance to the nearest strong liquidity pool, indicating whether the market is currently in a "void" (free to move rapidly) or compressed near liquidity.

---
description: OHLC Range Map Calculation
icon: sigma
---

# Calculation

The **OHLC Range Map** is a sophisticated tool designed to provide deeper insights into market dynamics by analyzing candlestick data using two core statistical methods:

* **Mean**
* **Median**

These methods, coupled with insights into manipulation and distribution phases, empower traders to make more informed decisions based on price action.

### 1. **Mean Method**

The **Mean** method calculates the average of the Open, High, Low, and Close values of a candlestick. This approach provides a balanced representation of price action, helping traders identify central tendencies and equilibrium levels.

Combined with manipulation and distribution insights, the **Mean** offers a clear understanding of price movement within a candlestick.

* **Bullish Candle**:
  * **Manipulation**: Defined as the range between the Open and the Low, representing deceptive price movements intended to mislead traders before the upward trend.
  * **Distribution**: Defined as the range between the Open and the High, representing the true extension of price in the bullish direction.
* **Bearish Candle**:
  * **Manipulation**: Defined as the range between the Open and the High, indicating misleading price movements intended to lure traders before the downward trend.
  * **Distribution**: Defined as the range between the Open and the Low, showing the actual extension of price in the bearish direction.

### 2. **Median Method**

The **Median** method focuses on the middle value within the OHLC dataset, providing a robust measure of price action that minimizes the influence of outliers.

By isolating the most central data point, the **Median** is particularly effective in volatile markets, ensuring the analysis remains unaffected by extreme wicks or spikes.

When applied in conjunction with manipulation and distribution phases, the **Median** highlights stable zones and reliable price levels for potential trade entries or exits.

### Period Options

The algorithm includes a range of configurable period options, allowing traders to adapt statistical calculations to different market conditions. These periods determine how data is aggregated and how the **Mean** and **Median** are calculated over time.

* **5 Candles**: Short-term analysis, ideal for intraday traders seeking immediate price action insights.
* **20 Candles**: Medium-term perspective, suitable for swing traders looking to capture broader trends.
* **40 Candles**: Balanced timeframe for detecting intermediate trends and price levels.
* **60 Candles**: Longer-term view for assessing significant market phases and identifying major support/resistance levels.
* **Custom**: Fully customizable period, enabling traders to tailor the algorithm to specific strategies or unique market conditions.
* **Maximum**: Includes all available candlesticks, offering a comprehensive view of the market's historical behavior.

The chosen period directly affects the statistical outputs and how traders interpret key levels:

* **Short Periods (e.g., 5, 20)**: Highlight recent market activity, making them highly responsive to current trends but more sensitive to noise. Useful for identifying immediate manipulation and distribution ranges.
* **Long Periods (e.g., 40, 60)**: Smooth out short-term fluctuations, offering a clearer picture of underlying trends and significant liquidity levels.
* **Custom and Maximum Periods**: Provide flexibility to capture unique patterns or analyze market behavior over extended durations, enhancing strategy customization.

By integrating the **Mean,** **Median** methods with dynamic period options, the OHLC Range Map Algorithm empowers traders to analyze market behavior with precision and adaptability.

Shorter periods cater to fast-moving markets, while longer and customizable options ensure relevance across varying strategies.

Combined with manipulation and distribution insights, this tool offers a comprehensive framework for understanding and navigating price action effectively.

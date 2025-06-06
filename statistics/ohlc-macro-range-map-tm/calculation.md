---
description: OHLC Macro Range Map Calculation
icon: sigma
---

# Calculation

The **OHLC Macro Range Map** is an advanced tool designed to provide deeper insights into market dynamics by analyzing candlestick data using two key statistical methods:

* **Mean**
* **Median**
* **KDE**

These methods, alongside insights into manipulation and distribution phases, empower traders to make more informed decisions based on price action.&#x20;

### **1. Mean Method**

The **Mean** method calculates the average of the Open, High, Low, and Close values of a candlestick. This approach offers a balanced representation of price action, helping traders identify central tendencies and equilibrium levels. When combined with manipulation and distribution insights, the **Mean** provides a clear understanding of price movement within a candlestick, specific to each session.

* **Bullish Candle:**
  * **Manipulation:** Defined by the range between the Open and the Low, representing deceptive price movements aimed at misleading traders before the upward trend.
  * **Distribution:** Defined by the range between the Open and the High, showing the true extension of price in the bullish direction.
* **Bearish Candle:**
  * **Manipulation:** Defined by the range between the Open and the High, indicating misleading price movements intended to trap traders before the downward trend.
  * **Distribution:** Defined by the range between the Open and the Low, representing the actual extension of price in the bearish direction.

### **2. Median Method**

The **Median** method focuses on the middle value within the OHLC dataset, offering a robust measure of price action that minimizes the influence of outliers. By isolating the most central data point, the **Median** is especially effective in volatile markets, ensuring analysis remains unaffected by extreme wicks or spikes.

When paired with manipulation and distribution phases, the **Median** highlights stable zones and reliable price levels for potential trade entries or exits.

### 3. Kernel Density Estimation

The **Kernel Density Estimation (KDE)** method focuses on identifying the most probable price levels within the OHLC dataset by estimating the underlying distribution of price action. Unlike simple averages or medians, KDE provides a smoothed view of the data, capturing subtle patterns and price clusters while minimizing the impact of outliers.&#x20;

By modeling the distribution with a continuous curve, KDE is particularly effective in volatile markets, as it highlights zones of price stability even amidst rapid fluctuations.&#x20;

When applied in conjunction with manipulation and distribution phases, KDE reveals densely populated price areas, offering reliable zones for potential trade entries or exits.

### **Period Options**

The algorithm includes several customizable period options, allowing traders to adjust statistical calculations to suit different market conditions. These periods determine how data is aggregated and how the **Mean** and **Median** are calculated over time for each specific session or "killzone."

* **5 Candles:** Short-term analysis, ideal for intraday traders seeking immediate price action insights.
* **20 Candles:** Medium-term perspective, suitable for swing traders aiming to capture broader trends.
* **40 Candles:** Balanced timeframe for detecting intermediate trends and price levels.
* **60 Candles:** Longer-term view for assessing significant market phases and identifying major support/resistance levels.
* **Custom:** Fully customizable period, enabling traders to tailor the algorithm to specific strategies or unique market conditions.
* **Maximum:** Includes all available candlesticks, providing a comprehensive view of historical market behavior.

The selected period directly influences the statistical outputs and traders' interpretation of key levels:

* **Short Periods** (e.g., 5, 20): Highlight recent market activity, offering high responsiveness to current trends but more sensitivity to noise. Ideal for identifying immediate manipulation and distribution ranges within specific sessions.
* **Long Periods** (e.g., 40, 60): Smooth out short-term fluctuations, providing a clearer view of underlying trends and significant liquidity levels within each session.
* **Custom and Maximum Periods:** Offer flexibility to capture unique patterns or analyze market behavior over extended durations, enhancing strategy customization.

By combining the **Mean,** **Median and KDE** methods with dynamic period options, the **OHLC Macro Range Map Algorithm** empowers traders to analyze market behavior with precision and flexibility.&#x20;

Shorter periods cater to fast-moving markets, while longer and customizable options ensure relevance across varying strategies.&#x20;

Integrated with manipulation and distribution insights, this tool provides a comprehensive framework for understanding and navigating price action effectively across all key market sessions.

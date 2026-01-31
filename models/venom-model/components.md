---
description: SFP Model Components
icon: diamonds-4
---

# Components

Below is an overview of the visual and analytical components that make up the CandelaCharts SFP Model. Each element is designed to enhance clarity, context, and decision-making by combining precise SFP detection with structural, multi-timeframe, and performance-based insights.

### **SFP Labels & Lines**

The core signal elements — horizontal line at swing level, dotted line at opposing level, thick colored line highlighting the sweep wick, plus a status-colored label showing volume and symbol. Controlled by “Show SFP” setting and “Last N” count.

### **Trendlines (upper and lower)**&#x20;

Lines connecting recent pivot highs and recent pivot lows. Smoothed version used for partial-success evaluation and high-probability filtering. Enabled via Trend → Trendline or Both.

### **Regression Channel (upper and lower)**&#x20;

5-segment linear regression fit used to define stronger success boundaries and high-probability filtering. Enabled via Trend → Channel or Both.

### **Higher Timeframe Candle Group I & II**&#x20;

Miniature candles rendered on the chart showing selected higher timeframes. Includes body, wicks, sweep lines (when valid), timeframe label and remaining close time. Each group can be independently enabled.

### **Liquidity Sweep Lines**&#x20;

Horizontal black lines drawn from HTF sweep points forward until invalidated or the group ends. Only non-removed and non-invalidated sweeps are shown.

### **Dashboard**&#x20;

Optional compact table (position configurable) displaying information about the most recent SFP: type, current status (colored), volume, swing price, opposing channel value, timeframe, asset, market type, and pivot length (in automatic mode).

### **Remaining Time Label**&#x20;

Small label above/below HTF candle group showing formatted time left until the current higher timeframe candle closes.

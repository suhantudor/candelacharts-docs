---
description: Macro Sentiment Index Usage
icon: circle-chevron-right
---

# Usage

### **Interpreting the Index**

* **Above 0**: Net risk-on sentiment\
  &#xNAN;_(Markets favor growth, liquidity, and speculative assets)_
* **Below 0**: Net risk-off sentiment\
  &#xNAN;_(Flight to safety, rising volatility, defensive positioning)_
* **Above +1**: Extreme risk-on / complacency\
  &#xNAN;_(Potential overheating or topping pattern)_
* **Below −1**: Extreme risk-off / fear\
  &#xNAN;_(Stress, capitulation, or strong defensive rotation)_

### **Trading Applications**

<table><thead><tr><th width="223.96875">Strategy</th><th>Application</th></tr></thead><tbody><tr><td><strong>Trend Confirmation</strong></td><td>Use MSI to validate equity or crypto trends. A rising price with rising MSI confirms momentum.</td></tr><tr><td><strong>Divergence Detection</strong></td><td>Price makes new highs but MSI trends lower → bearish divergence.</td></tr><tr><td><strong>Mean Reversion</strong></td><td>Extended stays beyond ±1 may signal overbought/oversold conditions.</td></tr><tr><td><strong>Regime Filtering</strong></td><td>Avoid long-only equity positions when MSI is deeply negative.</td></tr><tr><td><strong>Sector Rotation</strong></td><td>Combine with XLU/XLY or XLP/XLY ratios for defensive/offensive shifts.</td></tr><tr><td><strong>Volatility</strong></td><td>Falling VIX/VVIX ratio + negative MSI suggests suppressed volatility before a spike.</td></tr></tbody></table>

### **Configuration Tips**

* **Shorter lookback (20–40)**: More responsive, suitable for tactical trading
* **Longer lookback (80–120)**: Smoother, better for macro regime identification
* **Enable MA smoothing (50-period EMA)**: Helps filter noise in choppy markets
* **Increase weights** on VIX, MOVE, TED, and HYG for crisis detection
* **Increase BTC, SOXX, QQQ weights** to emphasize tech and crypto liquidity

### **Chart Setup**

Add the indicator to any asset (e.g., SPX, BTCUSD, EURUSD) but interpret within context:

* On **SPX/SPY**: MSI reflects broad equity risk appetite
* On **BTCUSD**: MSI captures global liquidity and risk flow into crypto
* On **USD/JPY**: Helps assess carry trade dynamics

**Best Practice**: Run MSI on a daily chart for macro clarity, or 4H/1H for tactical entries.

---
description: SFP Model Terminology
icon: spell-check
---

# Terminology

These are the core concepts and terms used throughout the CandelaCharts – SFP Model indicator. Understanding them will help you interpret signals, statuses, labels, and tooltips more effectively.

### **SFP**&#x20;

Swing Failure Pattern — price sweeps a recent significant high or low but fails to sustain movement in that direction, often trapping traders.

### **Swing Price**&#x20;

The price level of the recent pivot high or low that was swept / violated.

### **Opposing Price**&#x20;

The extreme price reached during the sweep candle (highest high in a bearish SFP, lowest low in a bullish SFP).

### **Wick Price**&#x20;

The extreme price of the sweep candle itself (high for bearish SFP, low for bullish SFP).

### **Sweep**&#x20;

A liquidity sweep visible on higher timeframe candles — when a candle’s wick extends beyond the previous candle’s extreme but the body does not fully violate it.

### **High Probability SFP**&#x20;

An SFP where at least one of the two relevant wicks (the sweep wick or the formation wick) touches or crosses the current channel or trendline boundary.

### **Trendline boundaries**&#x20;

(pivot-to-pivot trendlines) Lines connecting recent swing highs (upper trendline) and recent swing lows (lower trendline).&#x20;

{% hint style="info" %}
Usually thinner (default width 2), dashed or dotted by default, green color (customizable), drawn between the most recent relevant pivots. They tend to closely follow the latest swing points and change angle more frequently.
{% endhint %}

### **Channel boundaries**&#x20;

(5-segment linear regression channel) Statistically fitted upper and lower lines based on a segmented linear regression over a longer lookback period.&#x20;

{% hint style="info" %}
Noticeably thicker (default width 5), solid or dashed/dotted style (customizable), usually black or dark color for the lines themselves, drawn as straighter, smoother lines that span a wider historical window. They move more slowly and appear more “enveloping” compared to trendlines.
{% endhint %}

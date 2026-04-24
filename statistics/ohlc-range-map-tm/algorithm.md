---
description: OHLC Range Map Calculation
icon: sigma
---

# Calculation

The **OHLC Range Map** is a sophisticated tool designed to provide deeper insights into market dynamics by analyzing candlestick data using two core statistical methods:

* **Mean**
* **Median**
* **Both**

These methods, coupled with insights into manipulation and distribution phases, empower traders to make more informed decisions based on price action.

<figure><img src="../../.gitbook/assets/ohlc-rangemap-021.jpg" alt=""><figcaption></figcaption></figure>

### **Mean vs. Median**

When building a statistical picture of market behavior — say, tracking daily point ranges on NQ — mean and median tell you different things. Knowing which to trust in a given context is what separates clean analysis from misleading data.

### **Mean — The Overall Average**&#x20;

Add all values, divide by the count:

* Values: 132, 197, 198, 210, 350
* Sum = 1087
* Mean = 1087 / 5 = **217.4**

Simple enough — but the problem is sensitivity. That 350-point session, likely driven by a high-impact catalyst like NFP, FOMC, or CPI, pulls the average up and makes the "typical" day look bigger than it actually is.

### **Median — The True Middle**&#x20;

Sort the same values and take the center figure:

* Sorted Values: 132, 197, **198**, 210, 350
* Median = **198**

No weighting, no distortion. The outlier exists in the data set, but it no longer dominates the result. What you're left with is a number that better represents what a normal session actually looks like.



### **The Practical Takeaway**&#x20;

The mean gives you a broad sense of market behavior over time. The median gives you a realistic baseline for what to expect on any given day. When news events are in play, the mean inflates to 217.4 — the median holds steady at 198. For setting your statistical manipulation and distribution targets, the median is the more reliable anchor. Use the mean to understand the full range of possibilities; use the median to plan your trades.

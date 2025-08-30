---
description: Contango Slope Index Usage
icon: circle-chevron-right
---

# Usage

The CSI is plotted as a standalone oscillator beneath the price chart (non-overlay mode). Key interpretation guidelines:

### **Slope Direction**

* **Slope < 0** → Backwardation\
  Indicates near-term volatility is higher than long-term expectations. Historically, this has preceded **equity market rallies**, as panic subsides and fear peaks.
* **Slope > 0** → Contango\
  Reflects normal market conditions where longer-dated volatility is priced higher. Persistent high contango may signal **complacency**.

### **Magnitude of Slope**

* **Slope > 0.0232** (%/yr) → Elevated complacency\
  The term structure is steeper than historical average—caution advised ahead of potential corrections.
* **Slope near 0** → Neutral or transitioning regime\
  Markets may be at inflection points.

### **Slope vs. MA Crossover**

* **Slope crosses above MA** → Improving confidence, potential upside acceleration
* **Slope crosses below MA** → Deteriorating structure, rising stress

### **Default Settings**

| Parameter         | Value                                 |
| ----------------- | ------------------------------------- |
| Lookback Window   | 5 days                                |
| MA Type           | SMA                                   |
| MA Length         | 200                                   |
| Plotted Elements  | Slope line, MA, fill, reference lines |
| Regime Thresholds | 0 (flat), 0.0232 (avg contango)       |

### **Recommended Use Cases**

1. **Equity Strategy Timing**\
   Use backwardation signals (slope < 0) as contrarian buy indicators in S\&P 500 or broad market ETFs.
2. **Risk Management**\
   Watch for elevated contango (>2.32%) as a warning sign before tightening exposure.
3. **Volatility Trading**\
   Trade VIX ETNs (e.g., XIV, ZIV, VXX) based on slope momentum and regime shifts.
4. **Macro Regime Detection**\
   Combine with trend-following models to filter trades during extreme fear/greed phases.

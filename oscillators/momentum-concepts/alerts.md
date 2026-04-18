---
icon: bell
---

# Alerts

Momentum Concepts offers specialized alerts for trend shifts, signals, and statistical reversal signatures.

### Available Alert Types

1. **Momentum Signals**:
   * **Any Buy Signal**: Triggered when any level of buy signal (L1, L2, or L3) occurs.
   * **Any Sell Signal**: Triggered when any level of sell signal (L1, L2, or L3) occurs.
2. **Reversal Probabilities**:
   * **Bottom Probability**: Triggered when the KNN Bottom Reversal Engine confirms a bottoming pattern.
   * **Top Probability**: Triggered when the KNN Top Reversal Engine confirms a topping pattern.

### Advanced Alert Strategy

For maximum efficiency, you can set an alert on the **Any Alert() function call**. This will send a notification for:

* Standard, Strong, and Elite signals.
* Confirmed machine-learning reversals.

### Alert Content

Alerts are pre-configured with descriptive text (e.g., "Momentum Buy Signal (L2) detected") so you can identify the setup directly from your mobile device or desktop notification without opening the chart.

### Frequency

Most alerts are set to **Once Per Bar Close**. This is essential for KNN and Signal analysis to ensure the bar has finished calculating and the momentum transition is sustained.

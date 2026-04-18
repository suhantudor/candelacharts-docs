---
icon: bell
---

# Alerts

The Volume Matrix includes a comprehensive suite of alerts to keep you updated on market shifts and extreme conditions.

### Available Alert Types

1. **Regime Shifts**:
   * **Bullish Regime Shift**: Triggered when the oscillator line crosses above zero.
   * **Bearish Regime Shift**: Triggered when the oscillator line crosses below zero.
2. **Overbought / Oversold**:
   * **Overbought Entry**: Triggered when the line enters the OB zone (> 1.0).
   * **Oversold Entry**: Triggered when the line enters the OS zone (< -1.0).
3. **Price Breakouts**:
   * **Upper Band Breakout**: Triggered when the Price (High) breaks above the outer upper band (`ub_x2`).
   * **Lower Band Breakout**: Triggered when the Price (Low) breaks below the outer lower band (`bb_x2`).

### Setting Up Alerts

* **Alert Dialog**: Open the alert dialog, select the indicator, and choose the specific condition from the list.
* **Any Alert() function call**: If you want to receive all Volume Matrix alerts in a single configuration, select "Any Alert() function call" in the Condition dropdown.

### Frequency

By default, alerts are set to trigger **Once Per Bar Close** to ensure the signal is confirmed by the final price of the candle and to avoid false signals during live volatility.

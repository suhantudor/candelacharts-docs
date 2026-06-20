---
description: Price Action Model Alerts
icon: bell
coverY: 0
---

# Alerts

Missing a setup can be frustrating. The Price Action Model includes built-in alert conditions that integrate seamlessly with TradingView's alert system, allowing you to receive notifications via app, email, or webhook exactly when a mechanical setup forms.

### Available Alert Conditions

* **Bullish Model Formation:**
  * This alert triggers the moment a complete Bullish Price Action Model is validated.
  * **Requirements:** A sell-side liquidity sweep (price breaks below a previous pivot low) must occur, immediately followed by a bullish Change of Character (price breaks structure upward).
* **Bearish Model Formation:**
  * This alert triggers the moment a complete Bearish Price Action Model is validated.
  * **Requirements:** A buy-side liquidity sweep (price breaks above a previous pivot high) must occur, immediately followed by a bearish Change of Character (price breaks structure downward).

### How to Set Up Alerts

1. Open the **Alerts** dialog in TradingView (Alt + A or click the alarm clock icon).
2. Under the **Condition** dropdown, select the **CandelaCharts - Price Action Model** indicator.
3. Choose either the _Bullish Model_ or _Bearish Model_ from the secondary dropdown.
4. Set your preferred expiration time and notification methods (e.g., pop-up, email, webhook to Discord/Telegram).
5. Add a custom message if desired, and click **Create**.

_Tip: For the most reliable signals, configure your alerts on a timeframe where you have established confluence with the MTF Dashboard._

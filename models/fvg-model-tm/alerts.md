---
description: FVG Model Alerts
icon: bell
coverY: 0
---

# Alerts

The FVG Model provides fully customizable alerts that notify you at each critical stage of a model's lifecycle, keeping you informed even when you're away from your charts.

### Alert Settings

* **Enable Alerts**: Master toggle that activates or deactivates the entire alert system. When disabled, no alerts will fire regardless of the individual settings below.

### Alert Types

Each alert type can be independently enabled or disabled:

* **Formed Models**: Triggers the moment a new FVG model is detected and confirmed. This means a sweep has occurred, a market structure shift (CISD/MSS) has been validated, and the HTF FVG has been successfully mapped. Use this alert to be notified the instant a fresh trading opportunity appears.
* **Completed Models**: Triggers when an active model successfully reaches its standard deviation take-profit target. This confirms that the trade thesis played out and price delivered into the projected zone. Useful for tracking performance and logging successful setups.
* **Failed Models**: Triggers when an active model is invalidated — meaning price breached the stop-loss level before reaching the take-profit target. Use this alert to quickly adjust your trade management or close positions if you had entered a trade based on the model.

### Setup Alerts

To set up alerts using the Unicorn Model on TradingView, follow these steps:

1. **Create a New Alert**\
   Click the **“+ Alert”** button located at the top of your TradingView chart interface.
2. **Set the Condition**\
   In the **"Condition"** dropdown menu, select **Unicorn Model** as the indicator you want to trigger the alert.
3. **Choose the Timeframe**\
   Under the **“Interval”** setting, choose your **preferred timeframe** (e.g., 1H, 4H, 1D) based on your trading strategy or the timeframe you want to monitor.
4. **Configure Alert Expiration (Optional)**\
   In the **“Expiration”** section, you can optionally set a date and time for when the alert should stop triggering.
5. **Name Your Alert (Optional)**\
   In the **"Alert Name"** field, provide a **custom name** for your alert. This helps you identify it easily, especially if you're managing multiple alerts.
6. **Create the Alert**\
   Once all settings are configured, click **“Create”** to activate the alert.

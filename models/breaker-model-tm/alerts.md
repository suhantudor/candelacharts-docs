---
description: Breaker Model Alerts
icon: bell
coverY: 0
---

# Alerts

### Available Alerts

Never miss a setup. The Breaker Model features a comprehensive suite of alerts that track the entire lifecycle of a trade.

* **Potential Breaker?**: Fires mid-candle when the logic detects that a liquidity sweep has occurred and a breaker is _currently_ forming, giving you a head-start before the candle closes.
* **Activation?**: Fires the exact moment the setup candle officially closes and confirms the structural shift, signaling that the entry zone is now valid.
* **Target Reached?**: Fires an alert whenever price action successfully hits one of your active R:R target projection lines.
* **Invalidation Hit?**: Fires an alert if a confirmed setup breaches its stop loss / invalidation point, signaling you to manage risk.

{% hint style="info" %}
Ensure the master "Enable Alerts" switch is turned on in the settings to allow any of these specific conditions to trigger.
{% endhint %}

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

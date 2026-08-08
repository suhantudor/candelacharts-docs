---
description: Breaker Model Alerts
icon: bell
coverY: 0
---

# Alerts

Never miss a setup. The Breaker Model features a comprehensive suite of alerts that track the entire lifecycle of a trade.

* **Potential Breaker?**: Fires mid-candle when the logic detects that a liquidity sweep has occurred and a breaker is _currently_ forming, giving you a head-start before the candle closes.
* **Activation?**: Fires the exact moment the setup candle officially closes and confirms the structural shift, signaling that the entry zone is now valid.
* **Target Reached?**: Fires an alert whenever price action successfully hits one of your active R:R target projection lines.
* **Invalidation Hit?**: Fires an alert if a confirmed setup breaches its stop loss / invalidation point, signaling you to manage risk.

{% hint style="info" %}
Ensure the master "Enable Alerts" switch is turned on in the settings to allow any of these specific conditions to trigger.
{% endhint %}

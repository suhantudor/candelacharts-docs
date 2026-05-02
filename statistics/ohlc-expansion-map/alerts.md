---
description: OHLC Expansion Map Alerts
icon: bell
---

# Alerts

Stay on top of every institutional move with real-time **Alerts**. The OHLC Expansion Map allows you to monitor critical behavioral levels even when you are away from your screen.

### Alert Conditions

The indicator is programmed to trigger alerts when price crosses any of the following key levels:

#### 1. Manipulation Zone Entry

Triggered when price enters the Resistance 1 (\[-M]) or Support 1 (\[+M]) zones. This notifies you that a "fake-out" or institutional accumulation/manipulation phase is potentially starting.

#### 2. Distribution Target Hit

Triggered when price reaches the Resistance 2 (\[+D]) or Support 2 (\[-D]) extremes. These are your primary targets or potential reversal areas.

#### 3. Open Price Cross

Notifies you when price returns to the "equilibrium" (the opening price) after an expansion or manipulation phase.

#### 4. Volatility Expansion

Alerts for price entering the ATR-based Volatility Box, signaling potential exhaustion.

### Setting up Alerts in TradingView

1. Click the **Alerts** icon in the TradingView sidebar.
2. Select **CandelaCharts - OHLC Expansion Map** as the "Condition."
3. Choose the specific alert message from the dropdown (e.g., `{{strategy.order.alert_message}}` or use the default message).
4. Set your notification preferences (Pop-up, Email, Webhook, Mobile app).

### Dynamic Placeholders

The indicator uses dynamic strings to provide detailed information in your alert messages:

* **Timeframe:** Identifies which timeframe (1D, 4H, etc.) triggered the alert.
* **Session/Macro Name:** Identifies the specific session or macro (e.g., "London Open").
* **Level Type:** Clearly states whether it was a Manipulation or Distribution level.
* **Price:** Includes the exact price level at the time of the trigger.

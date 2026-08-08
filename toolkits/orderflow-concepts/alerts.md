---
icon: bell
---

# Alerts

The Order Flow Concepts toolkit includes specialized alerts designed to keep you informed of critical liquidity events and traps, even when you aren't actively monitoring the chart.

### Alert Settings

* **Enable Alerts**: The master switch to enable or disable all alerts from this indicator. If this is disabled, no alerts will fire.

### Alert Types

You can independently toggle the following alert conditions:

* **Trapped Traders**: Fires when the model detects that retail traders have been baited into a breakout and immediately trapped by a reversal.
  * This alert is split internally, notifying you specifically if it is "Trapped Bulls" or "Trapped Bears". It is an excellent trigger to look for fading opportunities.
* **Strong Liquidity Reached**: Fires when current price successfully reaches and taps a major active liquidity pool (as defined by your Liquidity Mappings settings).
  * This is your signal to pay attention to the chart and monitor for the reaction: will price absorb the liquidity and reverse, or push through and continue hunting?

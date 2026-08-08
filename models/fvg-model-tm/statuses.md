---
description: FVG Model Statuses
icon: battery-quarter
---

# Statuses

The FVG Model tracks the complete lifecycle of every detected setup, categorizing each model into one of three distinct statuses.

### Active

A model enters the "Active" status the moment a valid FVG model is confirmed — meaning a sweep has occurred, a market structure shift (CISD or MSS) has been validated, and the HTF Fair Value Gap has been mapped onto the LTF chart. The standard deviation projections are drawn and the model is actively being tracked against live price action.

An active model will remain in this state until price either reaches the take-profit level or breaches the stop-loss level.

### Completed

A model transitions to "Completed" when price action successfully reaches the standard deviation take-profit target. This means the trade thesis played out as expected — the sweep was genuine, the structure shift was confirmed, and price delivered into the projected target zone.

Completed models remain visible on the chart (unless filtered out via the Status dropdown) to serve as historical reference for backtesting and pattern recognition.

### Failed

A model becomes "Failed" when price breaches the stop-loss level (1 standard deviation on the opposing side of the anchor) before reaching the take-profit target. This indicates the sweep was either a false signal or the market structure shift was not sustained.

* **Hide Failed Models**: When this toggle is enabled, failed models are automatically removed from the chart, preventing visual clutter and keeping your focus on active and completed setups.

### Status Filter

The **Status** dropdown in the Settings group allows you to filter which models are displayed:

* **All**: Shows every model regardless of status.
* **Active**: Only shows models that are currently live.
* **Completed**: Only shows models that successfully reached their target.
* **Failed**: Only shows models that were invalidated.

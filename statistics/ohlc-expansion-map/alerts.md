---
description: OHLC Expansion Map Alerts
icon: bell
---

# Alerts

The **OHLC Expansion Map** provides real-time notifications when price interacts with key statistical boundaries. These alerts are designed to help traders identify the completion of manipulation phases and the reach of distribution targets without needing to constantly monitor the chart.

### Available Alert Types

The following alert conditions can be enabled within the **Alerts** settings group:

| Alert                       | Condition                                                            | Statistical Context                                                  |
| --------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- |
| **Cross Open (+O)**         | Price crosses the opening level of the current session or timeframe. | Signifies a return to the accumulation baseline.                     |
| **Cross Manipulation (±M)** | Price reaches the Manipulation High or Manipulation Low levels.      | Indicates a potential stop-hunt or trap is in progress.              |
| **Cross Distribution (±D)** | Price reaches the extreme Distribution expansion bands.              | Signals maximum statistical extension and potential exhaustion.      |
| **Cross Avg H/L**           | Price reaches the Average High or Average Low zones.                 | Marks the most common mathematical targets for the distribution leg. |

### Dynamic Alert Logic

The indicator uses advanced logic to ensure alert accuracy based on your chosen calculation settings:

#### 1. Algorithm Adaptability

If you are using the **"Both"** algorithm (Mean + Median), the system automatically identifies the **"Inner Level"** (the boundary closest to the Open). The alert will trigger as soon as price touches this inner boundary to ensure you are notified at the earliest possible confluence.

#### 2. Multi-Timeframe Integration

Alerts can be configured for up to three different timeframes simultaneously (TF1, TF2, and TF3). Each alert message will explicitly state which timeframe triggered the condition (e.g., `(1D)` for Daily or `(1W)` for Weekly).

#### 3. Execution Frequency

All alerts use the `alert.freq_once_per_bar` protocol. This means:

* You receive the notification immediately upon the price cross.
* You will not receive multiple notifications for the same level within the same bar, preventing "spam" during volatile moves.

### Alert Configuration Settings

To ensure your alerts function correctly, verify the following settings:

* **Style Visibility**: Alerts are hard-linked to the visual plots. A level must be toggled **ON** in the **Style** menu to trigger an alert.
* **Timezone Anchor**: Ensure your **Timezone** is set correctly (default is `America/New_York`), as this determines the anchor point for the opening price and subsequent levels.
* **Weighting**: If **Volume** or **Volatility** weighting is enabled, your alert levels will adjust dynamically to market conditions, and notifications will trigger based on these adjusted zones.

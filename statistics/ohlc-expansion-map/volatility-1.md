---
description: OHLC Expansion Map Volume Profile
icon: layer-group
---

# Volume Profile

The **Real Volume Profile** component provides a deep look into the historical volume distribution across specific timeframes or sessions. Unlike standard volume bars, this profile shows "Where" the volume was traded, not just "When."

### Key Components

#### 1. Value Area (VA)

The Value Area represents the price range where a specific percentage (default 70%) of the total volume was traded.

* **VAH (Value Area High):** The upper boundary of the Value Area.
* **VAL (Value Area Low):** The lower boundary of the Value Area.
* **Interpretation:** Price inside the VA is considered "fair value." Price outside the VA is "imbalanced" and may lead to sharp reversals or fast expansions.

#### 2. Point of Control (POC)

The price level with the highest traded volume within the profile. This is the most significant level in any profile and often acts as a powerful "magnet" for price.

### Operation Modes

* **Automatic Mode:** The indicator automatically calculates the volume profile based on the current chart timeframe and session duration.
* **Manual Mode:** You can specify a custom timeframe for the volume calculation (e.g., viewing a 1D Volume Profile while on a 5-minute chart).

### Integration with Expansion Map

The Volume Profile is designed to be used in conjunction with the Behavioral Levels:

* **Mean Reversion:** Look for price to return to the **POC** after reaching a **Distribution (+D/-D)** zone.
* **Breakout Confirmation:** If price breaks out of the **Value Area** and is also entering a **Manipulation** zone, it confirms the "fake-out" logic before a reversal.

### Technical Details

* **Tick Data:** The indicator uses `request.security_lower_tf` to fetch the highest resolution tick/volume data available for precise calculations.
* **Custom Rows:** Adjust the "Rows" setting to increase or decrease the granularity of the profile.
* **Max Width & Offset:** Customize the visual position and size of the profile to avoid overlapping with price action.

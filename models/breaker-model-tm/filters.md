---
description: Breaker Model Filters
icon: filter
---

# Filters

To ensure only premium setups are displayed, the Breaker Model includes a robust suite of filters.

### Size Filters

You can eliminate setups that are too tight to trade or too wide to offer a good Risk-to-Reward ratio.

* **Minimum/Maximum Size**: Define the size boundaries for the Breaker Block.
* **Unit**: Choose to measure the size in `Points`, `Ticks`, or dynamic `ATR` (Average True Range).

### ATR Multiplier Filter

When `Unicorn Mode` is active, the setup requires a Fair Value Gap. By enabling the **ATR Multiplier**, you force the indicator to only validate setups where the FVG height exceeds a specific fraction of the ATR (e.g., `0.5 ATR`), ensuring the displacement was genuinely explosive.

### Time Filters

Institutional setups are highly time-dependent. The Time Filters allow you to strictly restrict the detection of Breaker Blocks to specific liquidity windows, ignoring any sweeps outside of these times.

* **Enable Time Filter?**: Master toggle to turn the time filtering logic on or off.
* **Custom Timezone (Custom Tz)**: Bypass the chart's local time by defining a custom UTC offset. This ensures your sessions are always anchored to a specific global timezone (like EST) regardless of your computer's clock.
  * **Hour Offset**: Set the custom UTC hour deviation (e.g., `-5` for EST).
  * **Minute Offset**: Set the custom UTC minute deviation (useful for timezones like India IST).
* **Session 1, 2, 3**: You can independently toggle and define up to three distinct time windows (e.g., `0830-1200` for NY AM, `1300-1600` for NY PM). Each session has its own enable/disable checkbox and time input field.

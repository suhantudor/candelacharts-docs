---
description: Breaker Model Statuses
icon: battery-quarter
---

# Statuses

The Breaker Model tracks the complete lifecycle of a trade setup, categorizing it into distinct statuses from inception to completion.

### 1. Potential

A setup enters the "Potential" status the moment a Higher Timeframe (HTF) liquidity pool is swept and price begins to reverse. At this stage, the Breaker Block has not yet been confirmed by a candle close.

* _Note: You can enable alerts specifically for when a setup is in this potential phase._

### 2. Confirmed (Active)

A setup becomes "Confirmed" (or Active) once the required structural shift occurs and the candle closes, officially validating the Breaker Block.

* The indicator will draw the Breaker Box in your active color (e.g., solid green or red) and plot the R:R projection targets.
* If `Unicorn Mode` is enabled, the setup will only reach this status if a Fair Value Gap (FVG) is present.

### 3. Target Hit

A confirmed setup transitions to "Target Hit" when price action successfully reaches one of your active Risk-to-Reward projection lines.

* Once this happens, the visual components of the setup (boxes, lines) will fade to your designated inactive color (e.g., gray) to signify the trade has played out.

### 4. Invalidated

A confirmed setup becomes "Invalidated" if price action breaches the stop-loss level before hitting the target.

* Depending on your settings, the stop-loss is either the absolute extreme of the liquidity sweep (`Use Swing as Invalidation`) or the opposite edge of the Breaker Block.
* Upon invalidation, the setup will either turn inactive (fade to gray) or be completely removed from the chart if `Discard Invalidated` is enabled.

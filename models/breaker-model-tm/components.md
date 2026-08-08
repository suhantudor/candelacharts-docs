---
description: Breaker Model Components
icon: diamonds-4
---

# Components

The Breaker Model relies on several interconnected components to validate and display trade setups.

### Liquidity Sourcing

The foundation of the model. It tracks up to 4 discrete HTF sources (`Source A`, `Source B`, `Source C`, `Source D`). You can configure whether these sources look for major Swing Highs/Lows, or static OHLC (Open, High, Low, Close) levels from the higher timeframes. The indicator draws a sweep line when these levels are raided.

### Breaker Detection

Once a liquidity level is swept, it monitors the immediate reaction. It looks for the origin of the sweep and waits for a confirmed candle close that breaks structure and officially forms the Breaker Block.

### Projections & Risk Manager

Upon confirmation of a setup, this component calculates the distance between the entry zone and the invalidation point (the risk). It then projects your predefined Risk-to-Reward multipliers (`Targets: 1, 2, 2.5`) as take-profit lines on the chart.

### Visual Lifecycle Manager

Handles the aesthetics of the setup. It draws the Breaker Box in an "Active" color when formed, and transitions the box to an "Inactive" color (e.g., gray) once the setup either hits its target or breaches its invalidation level. If `Discard Invalidated` is enabled, failed setups are removed from the chart entirely.

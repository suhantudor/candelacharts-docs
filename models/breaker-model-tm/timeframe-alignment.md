---
description: Breaker Model Timeframe Alignment
icon: chess-clock-flip
---

# Timeframe Alignment

Proper timeframe alignment is crucial for high-probability setups. The Breaker Model uses an advanced Multi-Timeframe (MTF) engine.

### Automatic Mode

When `HTF Mode` is set to **Automatic**, the indicator dynamically scales the liquidity sources based on your current chart timeframe. For example, if you are viewing a 5m chart, it will automatically look for liquidity on the 15m, 1H, and 4H charts, ensuring you don't have to manually adjust settings when switching charts.

### Manual Mode

When set to **Manual**, you have granular control over the exact timeframes the indicator tracks for liquidity sweeps.

**Recommended Pairings for Manual Mode:**

* **Execution (Chart): 1m - 3m**
  * Liquidity Sources: 15m, 1H
* **Execution (Chart): 5m - 15m**
  * Liquidity Sources: 1H, 4H, Daily
* **Execution (Chart): 1H**
  * Liquidity Sources: 4H, Daily, Weekly

The logic requires a higher timeframe level to be swept to validate the lower timeframe Breaker formation.

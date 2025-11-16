---
icon: bell
---

# Alerts

Trend Concepts provides alert options for each component's key signals. All alerts fire once per bar close and include the symbol and timeframe in the message format: `[SYMBOL TIMEFRAME] Signal Description`.

### Bias Magnet Alerts

#### BM Bull

**Triggers when:** Bias Magnet trend flips to bullish (baseline crosses above price and confirms)

**Alert message:** `[SYMBOL TIMEFRAME] Bias Magnet — Trend Up [bullish flip]`

#### BM Bear

**Triggers when:** Bias Magnet trend flips to bearish (baseline crosses below price and confirms)

**Alert message:** `[SYMBOL TIMEFRAME] Bias Magnet — Trend Down [bearish flip]`

### Flux Trend Alerts

#### FT Bull

**Triggers when:** Flux Trend flips from bearish to bullish (price crosses above upper band)

**Alert message:** `[SYMBOL TIMEFRAME] Flux Trend — Flip Up [bear to bull]`

#### FT Bear

**Triggers when:** Flux Trend flips from bullish to bearish (price crosses below lower band)

**Alert message:** `[SYMBOL TIMEFRAME] Flux Trend — Flip Down [bull to bear]`

### Surge Waves Alerts

#### SW Bull

**Triggers when:** Surge Waves detects a sustained rising run (5+ consecutive bars rising, confirmed on bar close)

**Alert message:** `[SYMBOL TIMEFRAME] Surge Waves — Rising Signal [sustained rising run detected, bullish]`

#### SW Bear

**Triggers when:** Surge Waves detects a sustained falling run (5+ consecutive bars falling, confirmed on bar close)

**Alert message:** `[SYMBOL TIMEFRAME] Surge Waves — Falling Signal [sustained falling run detected, bearish]`

### Velocity Bands Alerts

#### VB Re-entry Bull

**Triggers when:** Price re-enters Velocity Bands from below the lower -2 band (bullish mean reversion signal)

**Alert message:** `[SYMBOL TIMEFRAME] Velocity Bands — Re-entry from Below [bullish]`

#### VB Re-entry Bear

**Triggers when:** Price re-enters Velocity Bands from above the upper +2 band (bearish mean reversion signal)

**Alert message:** `[SYMBOL TIMEFRAME] Velocity Bands — Re-entry from Above [bearish]`

#### VB Rejection Bull

**Triggers when:** Price enters the lower band but rejects back above it (bullish reversal signal)

**Alert message:** `[SYMBOL TIMEFRAME] Velocity Bands — Rejection from Lower Band [bullish]`

#### VB Rejection Bear

**Triggers when:** Price enters the upper band but rejects back below it (bearish reversal signal)

**Alert message:** `[SYMBOL TIMEFRAME] Velocity Bands — Rejection from Upper Band [bearish]`

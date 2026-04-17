---
icon: bell
---

# Alerts

Oscillator Concepts provides alert options for overbought/oversold conditions and divergence signals. All alerts fire once per bar close and include the symbol and timeframe in the message format: `[SYMBOL TIMEFRAME] Signal Description`.

### Overbought/Oversold Alerts

#### OS/OB Conditions

**Triggers when:** The oscillator enters an extreme zone

* **Overbought**: Oscillator crosses above +1
* **Oversold**: Oscillator crosses below -1

**Alert messages:**

* `[SYMBOL TIMEFRAME] OS/OB Condition — Entered Overbought (> +1) [bearish condition]`
* `[SYMBOL TIMEFRAME] OS/OB Condition — Entered Oversold (< -1) [bullish condition]`

**Use case:** Know when the oscillator enters an extreme state. Useful for identifying when price is in overbought or oversold territory.

#### OS/OB Signals

**Triggers when:** The oscillator returns from an extreme zone back inside the ±1 band

* **From Overbought**: Oscillator crosses back below +1
* **From Oversold**: Oscillator crosses back above -1

**Alert messages:**

* `[SYMBOL TIMEFRAME] OS/OB Signal — Overbought re-entry back inside band (bearish)`
* `[SYMBOL TIMEFRAME] OS/OB Signal — Oversold re-entry back inside band (bullish)`

**Use case:** Mean reversion opportunities. Often used as a potential mean-reversion cue when price returns from extremes.

### Divergence Alerts

#### Divergence Conditions

**Triggers when:** A regular divergence pattern is detected at pivots (raw detection, no high-probability filter)

* **Bullish Divergence**: Price makes lower low (LL) while oscillator makes higher low (HL) at pivot lows
* **Bearish Divergence**: Price makes higher high (HH) while oscillator makes lower high (LH) at pivot highs

**Alert messages:**

* `[SYMBOL TIMEFRAME] Divergence Condition — Bullish Regular Divergence (raw)`
* `[SYMBOL TIMEFRAME] Divergence Condition — Bearish Regular Divergence (raw)`

**Use case:** Early divergence detection. Alerts as soon as a divergence pattern is detected, without filtering.

**Note:** Requires the Divergences component to be enabled in the Components group.

#### Divergence Signals

**Triggers when:** A regular divergence is confirmed by the high-probability filter

* **Bullish Divergence**: Price LL + Oscillator HL, with at least one oscillator pivot outside the ±1 band
* **Bearish Divergence**: Price HH + Oscillator LH, with at least one oscillator pivot outside the ±1 band

**Alert messages:**

* `[SYMBOL TIMEFRAME] Divergence Signal — Bullish Regular Divergence (confirmed)`
* `[SYMBOL TIMEFRAME] Divergence Signal — Bearish Regular Divergence (confirmed)`

**Use case:** High-probability divergence signals. More selective than Conditions alerts, requiring at least one oscillator pivot to be outside the ±1 band. Fewer false positives.

**Note:** Requires the Divergences component to be enabled in the Components group. The high-probability filter can be toggled in the Divergences settings.

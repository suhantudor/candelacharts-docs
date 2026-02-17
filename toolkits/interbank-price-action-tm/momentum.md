---
icon: road-spikes
---

# Momentum

### Measuring Market Intent <a href="#user-content--measuring-market-intent" id="user-content--measuring-market-intent"></a>

Momentum is the engine of price movement. While many indicators lag, **Momentum Impulse** identifies the _initiation_ of a move. It highlights candles that display exceptional strength relative to recent history, often signaling the arrival of institutional volume.

### Impulse Candles <a href="#user-content-impulse-candles" id="user-content-impulse-candles"></a>

Not all large candles are significant. Some are just noise. We filter for true "Impulse Candles" based on specific criteria:

1. **Explosive Range**: The candle's body must be significantly larger than the previous candle's body (based on a dynamic ratio).
2. **Clean Closure**:
   * **Bullish Impulse**: Must close near its high, with very little upper wick.
   * **Bearish Impulse**: Must close near its low, with very little lower wick.

* **Visual**: These candles are highlighted on your chart, alerting you that a strong move has begun.

### Impulse Zones (Support & Resistance) <a href="#user-content--impulse-zones-support--resistance" id="user-content--impulse-zones-support--resistance"></a>

The origin of an impulsive move is a critical level. Institutions often defend these areas if price returns to test them.

* **Bullish Impulse Zone**: Drawn from the Open/Low of a Bullish Impulse Candle.
  * _Usage_: Potential Support. Look for long entries on a retest.
* **Bearish Impulse Zone**: Drawn from the Open/High of a Bearish Impulse Candle.
  * _Usage_: Potential Resistance. Look for short entries on a retest.

### Zone Management <a href="#user-content-zone-management" id="user-content-zone-management"></a>

To keep your chart clean, we manage these zones automatically:

* **Dimming (Mitigation)**: When price touches a zone, it dims. This tells you the zone has been tested and may be weaker.
* **Deletion (break)**: If price closes beyond the zone (invalidating it), the box is removed immediately.
* **Count**: You can limit the number of active momentum boxes on the chart (e.g., last 3) to avoid clutter.

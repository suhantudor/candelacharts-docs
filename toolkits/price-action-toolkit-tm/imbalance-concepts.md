---
icon: chart-bullet
---

# Imbalances

### Market Inefficiencies <a href="#user-content-market-inefficiencies" id="user-content-market-inefficiencies"></a>

**Imbalances**—most commonly known as **Fair Value Gaps (FVG)**—occur when buying or selling pressure is so intense that price "skips" levels, leaving behind unfilled orders.

These gaps act as:

1. **Magnets**: Price often returns to "fill" or "rebalance" the gap.
2. **Support/Resistance**: Once filled, the zone often triggers a reversal.

### Gap Types Explained <a href="#user-content--gap-types-explained" id="user-content--gap-types-explained"></a>

#### 1. Fair Value Gap (FVG) <a href="#user-content-1-fair-value-gap-fvg" id="user-content-1-fair-value-gap-fvg"></a>

The most fundamental imbalance pattern.

* **Structure**: A 3-candle sequence where the wicks of candle 1 and candle 3 do not overlap. The space between them is the gap.
* **Usage**: Wait for price to tap into the FVG (often the 50% level) for a high-probability entry.

#### 2. Inversion FVG (IFVG) <a href="#user-content-2-inversion-fvg-ifvg" id="user-content-2-inversion-fvg-ifvg"></a>

An FVG that has "flipped" its polarity.

* **Scenario**: Price smashes through a Bullish FVG without stopping.
* **Result**: That failed Support zone now becomes **Resistance**. We automatically label this as a **Bearish Inversion FVG**.
* **Power**: These are exceptionally strong signals for trend reversals or continuations.

#### 3. Volume Imbalance (VI) <a href="#user-content-3-volume-imbalance-vi" id="user-content-3-volume-imbalance-vi"></a>

A gap formed by the difference between the **Close** of one candle and the **Open** of the next.

* **Context**: Often seen in low-liquidity environments or during high-volatility news events.

#### 4. Opening Gap (OG) <a href="#user-content-4-opening-gap-og" id="user-content-4-opening-gap-og"></a>

The jump between yesterday's market **Close** and today's market **Open**.

* **Context**: Critical for Daily bias. If price opens huge gap up, the OG often acts as support for the day.

#### 5. Balanced Price Range (BPR) <a href="#user-content-5-balanced-price-range-bpr" id="user-content-5-balanced-price-range-bpr"></a>

A complex pattern where a Bullish FVG and a Bearish FVG overlap.

* **Meaning**: The market has aggressively bought up and then sold down through the same price area. It represents a "knot" of equilibrium that price respects highly.

### Smart Settings <a href="#user-content-smart-settings" id="user-content-smart-settings"></a>

#### Filtering (Reduce Noise) <a href="#user-content--filtering-reduce-noise" id="user-content--filtering-reduce-noise"></a>

* **Threshold (ATR Filter)**: Don't want to see every tiny 1-pip gap? Set a threshold (e.g., 0.5 ATR). We will hide any imbalance smaller than this size.
* **Displacement**: Only show gaps that were created by a _strong_ move (a large candle body). This separates true institutional intent from choppy noise.

#### Mitigation Logic <a href="#user-content--mitigation-logic" id="user-content--mitigation-logic"></a>

What happens when price fills the gap?

* **Dim**: The zone fades out to show it's less significant.
* **Hide**: The zone disappears completely to keep your chart clean.
* **Extend**: Keep the zone active until it is fully closed.

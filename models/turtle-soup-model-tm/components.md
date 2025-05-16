---
description: Turtle Soup Model Components
icon: diamonds-4
---

# Components

**ICT Turtle Soup** is a **liquidity-based reversal setup** taught by the Inner Circle Trader (ICT). It targets traders who follow traditional breakout strategies (like the classic Turtle Trading System) by **fading false breakouts** near key swing highs or lows.

Below are the key components that make up the algorithm:

* **Sweep**
* **D-purge**
* **MSS**
* **PD Arrays**
* **SMT**
* **Projections**
* **Liquidity**

## **Components**

### **1. Sweep**

**Definition:** A Sweep is a candlestick pattern where the price momentarily exceeds the high or low of the previous candle (via the wick) and then closes within that candle’s range.

**Formation:**

* **Bullish Sweep:** The price briefly surpasses the high of the prior candle and closes back within its range.
* **Bearish Sweep:** The price briefly surpasses the low of the prior candle and closes back within its range.

**Invalidation:**

* **Bullish Sweep:**
  * Invalidated if the next candle is bullish and its body closes above the high of the prior candle.
  * Invalidated if any subsequent bullish candle closes above the high of the prior candle.
* **Bearish Sweep:**
  * Invalidated if the next candle is bearish and its body closes below the low of the prior candle.
  * Invalidated if any subsequent bearish candle closes below the low of the prior candle.

{% hint style="warning" %}
Real-time models remove the sweep once the model is invalidated and the candle closes. In other models, the sweep remains unless it is directly invalidated, with any changes clearly shown in the UI.
{% endhint %}

### **2. D-Purge**

**Definition:** A D-purge is a type of Sweep where the price exceeds both the high and low of the previous candle (via wicks) and then closes within the range of the prior candle.

**Formation:** A D-purge Sweep requires two higher-time-frame candles, with both sides of the previous candle being swept. The side that is swept last determines the direction of the D-purge.

**Invalidation:**

* **Bullish D-purge:**
  * Invalidated if the next candle is bullish and closes its body above the high of the prior candle.
  * Invalidated if any subsequent bullish candle closes above the high of the previous candle.
* **Bearish D-purge:**
  * Invalidated if the next candle is bearish and closes its body below the low of the prior candle.
  * Invalidated if any subsequent bearish candle closes below the low of the prior candle.

### **3. MSS**

**Definition:** **Market Structure Shift (MSS)** in trading refers to a significant change in the price pattern or trend direction of an asset, indicating a potential reversal or transition in market sentiment.

**Formation:**

* **Bullish MSS:** Occurs when the price closes above the opening price of a bearish delivery.
* **Bearish MSS:** Occurs when the price closes below the opening price of a bullish delivery.

**Invalidation:**

* N/A (No specific invalidation).

### **4. PD Arrays**

**Definition:** PD Arrays are models that describe how price is likely to be delivered from one liquidity point to another, based on smart money behavior.&#x20;

Model supports following PD Arrays for HTF and LTF:

* **Fair Value Gaps (FVGs):** Imbalances between buying and selling, often acts as a **magnet for price** or a **support/resistance zone**
* **Inversion Fair Value Gaps:** Former FVGs that, once filled or mitigated, reverse roles — acting as support/resistance or continuation zones.

**Formation:**&#x20;

#### Fair Value Gaps (FVG)

An FVG forms when there's a gap between Candle 1 and Candle 3 due to strong buying or selling, leaving an untraded zone.

* **Bullish FVG:** Gap between Candle 1 high and Candle 3 low after a strong up move.
* **Bearish FVG:** Gap between Candle 1 low and Candle 3 high after a strong down move.

#### Inversion Fair Value Gaps (FVG)

An FVG that was filled and later acts as support (bullish) or resistance (bearish) after a market shift.

**Invalidation:**

#### Fair Value Gaps (IFVG)

FVG is invalidated when price fully trades through (closes inside) the gap.

#### Inversion Fair Value Gaps (FVG)

IFVG is invalidated when price breaks through and closes beyond it in the opposite direction.

### **5. SMT**

**Definition:** **Smart Money Technique** refers to strategies used by institutional investors and large entities that have access to advanced insights and market-moving information.

**Formation:** **SMT Divergences** occur when two correlated markets show differing swing highs or lows, signaling a potential shift in market direction.

**Invalidation:** The SMT formation is invalidated if the price moves in the opposite direction, failing to respect the expected pattern.

### **6. Projections**

**Definition:** Projections measures the variation or dispersion of price from a mean, often used to project price swings.

**Formation:** It’s calculated from the CISD level to the price point of a swing manipulation.

**Invalidation:** Once the price reaches the 2 standard deviation level.

### **7. Liquidity**

**Definition:** Liquidity refers to areas of concentrated buy and sell orders at significant price levels, often where price reversals occur (e.g., swing highs and lows).

**Formation:** Liquidity zones are typically formed at swing points, PDH/PDL, PWH/PWL, and similar levels.

**Invalidation:** Once the price hits the liquidity zone.

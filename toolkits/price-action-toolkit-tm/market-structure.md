---
icon: arrow-up-arrow-down
---

# Market Structure

### The Roadmap of Price <a href="#user-content--the-roadmap-of-price" id="user-content--the-roadmap-of-price"></a>

**Market Structure** is the most fundamental concept in technical analysis. It tells you "who is winning" the battle between buyers and sellers. By objectively mapping out the Highs and Lows, you can trade _with_ the dominant flow rather than fighting against it.

<figure><img src="../../.gitbook/assets/docs-ipa-008.png" alt=""><figcaption></figcaption></figure>

This tool automates the tedious process of labeling structure, giving you a clean, objective map of the market in real-time.

### Structure Types <a href="#user-content-structure-types" id="user-content-structure-types"></a>

We separate structure into two distinct layers to help you see both the "Big Picture" and the "Immediate Action."

#### 1. Macro Structure (Swing) <a href="#user-content-1-macro-structure-swing" id="user-content-1-macro-structure-swing"></a>

* **Purpose**: Defines the overall trend bias (Daily/4H style structure).
* **Usage**: Trade in this direction. If Macro is Bullish, look for Longs.
* **Settings**: Controlled by `Macro Length`. A higher number (e.g., 50) filters out noise and shows main pivots.

#### 2. Micro Structure (Internal) <a href="#user-content-2-micro-structure-internal" id="user-content-2-micro-structure-internal"></a>

* **Purpose**: Defines the short-term momentum (15m/5m style structure).
* **Usage**: Used for entries and early warning signals. A Micro CHoCH often precedes a Macro reversal.
* **Settings**: Controlled by `Micro Length`. A lower number (e.g., 5) catches every minor pullback.

### Structural Events <a href="#user-content--structural-events" id="user-content--structural-events"></a>

We automatically detect and label three key events:

#### **BOS (Break of Structure)** <a href="#user-content-bos-break-of-structure" id="user-content-bos-break-of-structure"></a>

<figure><img src="../../.gitbook/assets/docs-ipa-003.png" alt=""><figcaption></figcaption></figure>

* **Meaning**: Trend Continuation.
* **Bullish BOS**: Price breaks above a Higher High. The uptrend is healthy.
* **Bearish BOS**: Price breaks below a Lower Low. The downtrend is healthy.

#### **CHoCH (Change of Character)** <a href="#user-content-choch-change-of-character" id="user-content-choch-change-of-character"></a>

<figure><img src="../../.gitbook/assets/docs-ipa-004.png" alt=""><figcaption></figcaption></figure>

* **Meaning**: The _first_ sign of a potential reversal.
* **Bullish CHoCH**: Price breaks above the last Lower High. The downtrend might be ending.
* **Bearish CHoCH**: Price breaks below the last Higher Low. The uptrend might be ending.

#### **CHoCH+ (Confirmed Change)** <a href="#user-content-choch-confirmed-change" id="user-content-choch-confirmed-change"></a>

<figure><img src="../../.gitbook/assets/docs-ipa-005.png" alt=""><figcaption></figcaption></figure>

* **Meaning**: A higher-probability reversal signal.
* **Logic**: Standard CHoCH can be triggered by a wick. **CHoCH+** requires a **candle close** beyond the structural level to confirm the breakout.

### Visualizing the Swings <a href="#user-content--visualizing-the-swings" id="user-content--visualizing-the-swings"></a>

#### Zigzag <a href="#user-content-zigzag" id="user-content-zigzag"></a>

<figure><img src="../../.gitbook/assets/docs-ipa-006.png" alt=""><figcaption></figcaption></figure>

Connects the Highs and Lows with a line.

* **Benefit**: Instantly visualize the "Wave" of the market. See impulsive moves vs. corrective moves at a glance.

#### Swing Points <a href="#user-content-swing-points" id="user-content-swing-points"></a>

<figure><img src="../../.gitbook/assets/docs-ipa-009.png" alt=""><figcaption></figcaption></figure>

Labels the specific pivots with symbols.

* **HH / HL**: Higher High / Higher Low.
* **LH / LL**: Lower High / Lower Low.
* **Customization**: You can change the shape (Circle, Square, Diamond) to fit your aesthetic.

### Strong vs. Weak Highs/Lows <a href="#user-content--strong-vs-weak-highslows" id="user-content--strong-vs-weak-highslows"></a>

This is a powerful concept for placing Stop Losses and Take Profits.

<figure><img src="../../.gitbook/assets/docs-ipa-007.png" alt=""><figcaption></figcaption></figure>

#### **Strong High/Low**  <a href="#user-content-strong-highlow" id="user-content-strong-highlow"></a>

* **Definition**: A pivot that **caused a Break of Structure**.
  * _Example_: A High that pushed price down to make a new Low.
* **Psychology**: Institutions defended this level and pushed price aggressively. It is likely to hold again.
* **Action**: **Place your Stop Loss here.** It is a safe invalidated point.

#### **Weak High/Low**  <a href="#user-content-weak-highlow" id="user-content-weak-highlow"></a>

* **Definition**: A pivot that **failed to break structure**.
  * _Example_: A High that failed to make a new Low and price reversed.
* **Psychology**: This level failed to do its job. It is "weak." behaviorally, price often returns to "sweep" these levels for liquidity.
* **Action**: **Target this for Take Profit.** Price is likely to trade through it.

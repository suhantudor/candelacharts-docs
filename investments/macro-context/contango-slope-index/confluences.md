---
description: Contango Slope Index Confluences
icon: object-intersect
---

# Confluences

While the **Contango Slope Index (CSI)** provides valuable insights into volatility structure and market sentiment, pairing it with well-established **technical confluences** enhances its reliability and applicability in real-world trading strategies.&#x20;

Below are several **high-impact technical confluences** that align with the CSI's logic and improve signal accuracy.

### **1. 200-Day Moving Average (Price Filter)**

**Confluence Logic**: Use the **S\&P 500 (SPX) 200-day SMA** as a macro trend filter. The CSI performs best when aligned with the broader market trend.

* ✅ **Valid Bullish Signal**: `CSI < 0` (Backwardation) **and** `SPX > 200-day SMA` → High-probability recovery or continuation of bull market.
* 🚫 **Avoid Bullish Signal**: `CSI < 0` but `SPX < 200-day SMA` → May indicate a "bear market rally"—higher risk, shorter duration.
* ⚠️ **Caution Zone**: `CSI > 0.0232` **and** `SPX > 200-day SMA` → Complacency in uptrend—watch for reversal signs.

**Why it works**: Prevents counter-trend entries and improves win rate by filtering signals within structural context.

### **2. RSI Divergence (Momentum Confirmation)**

**Confluence Logic**: Combine CSI regime shifts with **daily RSI(14) price divergence** to detect hidden strength or exhaustion.

* ✅ **Strong Buy Setup**: `CSI crosses below 0` (Backwardation begins) **+** `Price makes new low, RSI does not` (Bullish RSI divergence)
* ✅ **Strong Sell Warning**: `CSI > 0.0232` **+** `Price makes new high, RSI makes lower high` (Bearish divergence)

**Why it works**: Adds momentum layer to volatility structure—confirms whether price action supports the sentiment shift.

### **3. Volume-Weighted Moving Average (VWMA) Breakout**

**Confluence Logic**: Use **VWMA(20)** on SPX as a dynamic support/resistance level. CSI signals gain strength when confirmed by volume-weighted breakout.

* ✅ **High-Confidence Entry**: `CSI enters backwardation` **+** `Price closes above VWMA(20)` on above-average volume\`
* ✅ **Defensive Exit**: `CSI shows elevated contango` **+** `Price closes below VWMA(20)` with expanding volume\`

**Why it works**: Volume confirms institutional participation—separates noise from conviction.

### **4. VIX Spot vs. CSI Divergence**

**Confluence Logic**: Compare the **behavior of spot VIX** with the **CSI trend** to detect shifts in forward expectations.

* ✅ **Early Warning of Regime Change**: `Spot VIX is flat or declining` **but** `CSI slope is becoming more negative` → Forward curve is steepening into backwardation despite calming spot—can precede renewed fear.
* ✅ **Stability Signal**: `Spot VIX spikes` **but** `CSI remains positive and above MA` → Temporary volatility, no structural shift—likely a buying opportunity.

**Why it works**: Decouples spot noise from term structure dynamics.

### **5. Put/Call Ratio (Sentiment Overlay)**

**Confluence Logic**: Use the **CBOE Total Put/Call Ratio (daily)** to validate extreme sentiment.

* ✅ **High-Conviction Buy Signal**: `CSI < 0` **+** `Put/Call Ratio > 1.05` → Fear confirmed by options market.
* ✅ **Overbought Caution**: `CSI > 0.0232` **+** `Put/Call Ratio < 0.85` → Excessive bullishness—risk of correction.

**Why it works**: Adds another layer of market-based sentiment confirmation.

### **6. 52-Week High/Low Percent Indicator**

**Confluence Logic**: Use the percentage of S\&P 500 stocks at **52-week highs vs. lows** (McClellan Oscillator-style) to assess internal strength.

* ✅ **Robust CSI Signal**: `CSI enters backwardation` **+** `% Stocks at 52W Low > % at High` → Broad capitulation confirmed.
* ✅ **Complacency Confirmed**: `CSI > 0.0232` **+** `% Highs > 70%` → Widespread optimism—risk of mean reversion.

**Why it works**: Measures breadth—if only a few stocks drive the move, the CSI signal may be less reliable.

### **7. Yield Curve Slope (10Y-2Y Treasury Spread)**

**Confluence Logic**: Federal Reserve policy impacts volatility structure. The **Treasury term premium** affects VIX contango.

* ✅ **Higher-Probability Backwardation Rally**: `CSI < 0` **+** `Yield curve steepening after inversion`\
  &#x20;→ Macroeconomic support for recovery.
* 🚫 **Caution During Inversion**: `CSI < 0` **but** `10Y-2Y < -0.50%` → Recession risk may override volatility signal.

**Why it works**: Links macro-financial conditions to volatility behavior.

### **8. Dip Index**&#x20;

**Confluence Logic:** Volatility sentiment (CSI) must align with price structure resilience (Dip Index). A fear signal is only actionable if price has stopped reacting to downside shocks.

#### **8.1. Higher-Probability Reversal Setup:**

`CSI < 0` + `Dip Index declining from >7.0` → Fear confirmed, selling exhaustion evident.

**Action**: High-conviction long entry; target 3–6% over 4–8 weeks.

_Example_: March 2020 – CSI dropped to -0.018%/yr while Dip Index fell from 8.4 to 6.2 within two weeks. SPX stabilized and entered strong recovery.

#### **8.2. Recovery Confirmation (Post-Bottom):**

`CSI crosses above 0` + `Dip Index already in downtrend` → Sentiment normalizing as price structure strengthens.

**Action**: Add to long positions; remove hedges. Suitable for trend-following re-entry.

_Rationale_: The Dip Index lead confirms structural healing before CSI turns positive—early confirmation of sustainable rebound.

#### **8.3. Overheat Warning (Blow-Off Risk):**

`CSI > 0.0232` + `Dip Index < 5.0 and stable` → Complacency in options market, minimal pullbacks in price.

**Action**: Reduce risk exposure. Avoid new longs. Consider volatility hedges.

_Historical context_: Late 2017 and January 2021 – both conditions present before sharp corrections.

#### **8.4. Structural Decay (Hidden Fragility):**

`CSI ~ 0 (neutral)` + `Dip Index rising over time` → Market makes higher highs but with deeper corrections.

**Action**: Tighten stops; rotate to defensive sectors; monitor for breadth breakdown.

_Why it matters_: Volatility remains calm (flat CSI), but increasing dip depth reveals weakening demand—a divergence not captured by sentiment alone.

**8.5. False Dip Trap (Don’t Buy the Dip):**

`CSI > 0.0232` + `Dip Index rising` → Complacency persists despite deteriorating price structure.

**Action**: Exit longs on failed breakout. High risk of sharp correction.

_Signal failure mode_: A rally on shallow dips loses integrity when dip depth increases—warning of distribution masked by elevated contango.

### **Optimal Confluence Framework**&#x20;

<table><thead><tr><th>Confluence</th><th width="249.09765625">Bullish Signal (Entry)</th><th>Bearish Warning (Risk)</th></tr></thead><tbody><tr><td><strong>200-day SMA</strong></td><td>CSI &#x3C; 0 &#x26; SPX > SMA200</td><td>CSI > 0.0232 &#x26; SPX &#x3C; SMA200</td></tr><tr><td><strong>RSI(14) Divergence</strong></td><td>Price low, RSI higher</td><td>Price high, RSI lower</td></tr><tr><td><strong>VWMA Breakout</strong></td><td>Close above VWMA(20) on volume</td><td>Close below VWMA(20)</td></tr><tr><td><strong>Spot VIX vs CSI</strong></td><td>VIX flat, CSI falling</td><td>VIX down, CSI rising fast</td></tr><tr><td><strong>Put/Call Ratio</strong></td><td>Ratio > 1.05 + CSI &#x3C; 0</td><td>Ratio &#x3C; 0.85 + CSI > 0.0232</td></tr><tr><td><strong>52W High/Low %</strong></td><td>More lows than highs</td><td>70% at highs</td></tr><tr><td><strong>Yield Curve</strong></td><td>Steepening post-inversion</td><td>Deep inversion</td></tr><tr><td><strong>Dip Index</strong></td><td>Falling from elevated level + CSI &#x3C; 0 or crossing up</td><td>Rising trend + CSI > 0.0232 or flat</td></tr></tbody></table>

The **Contango Slope Index** excels as a **regime-detection engine**, but its predictive power multiplies when combined with **price, volume, sentiment, and macro confluences**.&#x20;

For systematic use, consider a **scoring system**:

* Assign +1 for each confirming confluence
* Only act when **≥3 confluences align**

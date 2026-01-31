---
description: SFP Model Framework
icon: diagram-venn
---

# Framework

<figure><img src="../../.gitbook/assets/docs-sf-model-005.png" alt=""><figcaption></figcaption></figure>

The SFP Model follows this logical sequence for every potential setup:

### **Pivot Detection**&#x20;

A recent significant high (for bearish setups) or low (for bullish setups) is identified using your chosen pivot length:

* one of the 9 preset lengths
* your custom length
* or “Automatic” mode (scans multiple lengths and picks recent high-quality candidates)

### **Sweep Occurs**&#x20;

Price makes a new extreme that goes beyond the pivot level (a “liquidity grab” or fakeout), but the candle body stays on the “safe” side of the pivot:

* Bearish SFP: high goes above previous swing high, but close stays below it
* Bullish SFP: low goes below previous swing low, but close stays above it This creates the classic “failure to follow through” pattern.

### **Confirmation Check**&#x20;

The setup waits for price to close strongly in the reversal direction:

* Bullish → close above the highest point of the sweep candle
* Bearish → close below the lowest point of the sweep candle Once this happens → the SFP is **Confirmed** (turns blue).

### **Outcome Evaluation (after confirmation)**&#x20;

The model now watches how far price moves in the expected direction:

* Price reaches the **trendline** opposing boundary first → **Partial Success** (lime color)
* Price reaches the **channel** opposing boundary (stronger target) → **Successful** (green color)
* Price turns around and breaks the original swing level **or** the sweep wick extreme in the wrong direction → **Failed** (red color)

### **Invalidation (can happen at any stage before full success)**&#x20;

The setup is cancelled and marked **Invalidated** (orange) if any of these occur:

* An opposite-direction SFP appears before confirmation
* Price returns inside the original swing level without confirming
* The pattern becomes too old (roughly >500 bars) or violates internal range rules

### **High-Probability Filter (optional – enabled by default)**&#x20;

When turned on, only SFPs are shown (and alerted) where at least one of the two key wicks — either the sweep wick or the formation/succession wick — actually touches or crosses the active boundary line.

* If both trendline and channel are enabled → the channel is preferred for this check. This significantly reduces noise and focuses on setups with structural context.

This flow ensures every SFP is tracked from birth → confirmation → success/failure/invalidation with clear visual feedback at each stage.

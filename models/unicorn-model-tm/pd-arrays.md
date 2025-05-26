---
description: Unicorn Model HTF & LTF PD Arrays
icon: frame
---

# PD Arrays

The Unicorn Model leverages two tiers of PD Arrays—Higher Time Frame (HTF) and Lower Time Frame (LTF)—to structure both macro-level bias and precise trade entries.

These arrays, referred to as:

* **FVG** (Fair Value Gap)
* **IFVG** (Inverse Fair Value Gap)

forming the foundation for model-based decisions.

### HTF PD Arrays

HTF PD Arrays define **high-probability reversal zones**, typically aligning with major liquidity pools. When a price sweep reaches these levels, the model anticipates a potential reversal or significant reaction. These zones serve as macro-level anchors, helping traders identify when a dominant trend may exhaust or shift.

### LTF PD Arrays

LTF PD Arrays are essential components of the Unicorn Model and must **overlap with the Zigzag Breaker** to form a valid setup. These arrays highlight precise zones of local imbalance or liquidity—typically Fair Value Gaps (FVGs) or Inverse Fair Value Gaps (IFVGs)—that serve as the foundation for low time frame execution.

A Unicorn Model is only considered valid if the Zigzag Breaker and the LTF PD Array **intersect within the same price zone**. This overlap provides structural and liquidity-based confluence, greatly increasing the probability of a successful trade. If there is no alignment between the two, the model is discarded as low-confidence and not tradeable.

By pairing **HTF arrays for directional bias** with **LTF arrays for tactical entries**, the Unicorn Model ensures both clarity and timing in execution—empowering traders to capture meaningful moves with structure and confidence.

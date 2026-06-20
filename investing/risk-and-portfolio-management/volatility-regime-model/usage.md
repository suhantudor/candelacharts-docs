---
description: Volatility Regime Model Usage
icon: circle-chevron-right
---

# Usage

Trading in different volatility states requires adapting your bias dynamically. Follow these steps to properly identify regimes and execute trades safely during high-stress market conditions:

1. **Classification of Regimes**: Rather than viewing the VIX as a continuous oscillator, it is broken into distinct zones:
   * **Low Vol (VIX < 22)**: A stable carry regime characterized by high persistence. Levels near 15 represent an extremely quiet market.
   * **Mid Vol (VIX 22–32)**: A transition or "fragility" zone. Often short-lived.
   * **High Vol (VIX 32–38.3)**: A stress regime indicating significant market uncertainty.
   * **Crisis Cluster (VIX > 38.3)**: Statistically, severe structural market stress begins around this level.
2. **The Persistence Decay**: Volatility is mean-reverting early and becomes persistent if the shock survives.
   * **Days 1–2**: High probability of a downshift (Fade Noise).
   * **Days 3–5**: Edge for a quick "vol crush" begins to decay.
   * **Day 6+**: Persistence begins to dominate. Risk of a regime shift is high (Defensive).
3. **The Validation Layer**: Determining if a spike is a "glitch" or a systemic shift via cross-asset confirmation. If signals do not confirm, fade the move. If they confirm, respect the new trend.

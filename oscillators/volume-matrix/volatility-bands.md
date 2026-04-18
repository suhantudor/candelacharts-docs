---
icon: waves-sine
---

# Volatility Bands

The Volume Matrix uses **Elastic Bands** on the price pane to visualize the statistical boundaries used for the oscillator calculation.

### Band Types

There are four bands plotted on the chart:

1. **Outer Bands (±σ x2)**:
   * **Logic**: Based on the Standard Deviation of the volume-weighted mean.
   * **Purpose**: These represent the extreme boundaries of expected volatility. Price wicking out of these bands is a "Breakout".
2. **Inner Bands (±σ x1)**:
   * **Logic**: Based on the **Robust Sigma** (Mean Absolute Deviation).
   * **Purpose**: These are "Robust" measures that are less sensitive to price spikes but more responsive to sustained volume shifts. They define the "Core" range of the asset.

### Using the Bands

* **Band Expansion**: Indicates a high-volatility environment (Trending).
* **Band Contraction**: Indicates low volatility (Consolidation/Squeeze).
* **Mean Line (Gray Line)**: This is the **ePulse μ** (Elastic Pulse Mean). It's the volume-weighted "Fair Value" of the asset.
* **Shadow Fills**: The areas between the Inner and Outer bands are filled to create "Extreme Heatmaps", helping you quickly identify when the price is entering an over-extended state.

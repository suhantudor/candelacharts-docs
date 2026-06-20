---
description: Volatility Regime Model Features
icon: sparkle
---

# Features

Instead of relying on basic VIX oscillators, the Volatility Regime Model uses advanced persistence tracking and cross-asset confirmation.&#x20;

Below are the unique mechanisms driving this framework:

* **Regime Classification**: Categorizes volatility into 4 distinct states: Low Vol (Stable), Mid Vol (Fragile), High Vol (Stress), and Crisis Cluster.
* **Persistence Tracking**: Measures how many consecutive days the market has spent in an elevated volatility state, adjusting the trading bias based on time-decay (Fade Noise -> Edge Decaying -> Defensive).
* **Cross-Asset Validation**: Automatically cross-references the MOVE Index (bond volatility) and High-Yield Credit Spreads (HY vs IG). If these external markets are widening alongside the VIX, the systemic stress is confirmed.
* **Dynamic Trading Bias**: Synthesizes the regime, persistence, and validation layers to output a clear, actionable trading bias on the dashboard.
* **Visual Ribbon & Dashboard**: Plots the VIX line with dynamic color-coding, a background regime ribbon, and a real-time dashboard summarizing the exact market state.

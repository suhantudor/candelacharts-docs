---
icon: slider
---

# Volume Line

The **Volume Line** is the primary signal generator within the Volume Matrix. It tracks the real-time relative momentum of price, heavily influenced by volume participation.

<figure><img src="../../.gitbook/assets/docs-volume-matrix-001.png" alt=""><figcaption></figcaption></figure>

&#x20;It is designed to act as a "Single Source of Truth" for where price sits within the current volatility context.

### Smoothing

<figure><img src="../../.gitbook/assets/docs-volume-matrix-011.png" alt=""><figcaption></figcaption></figure>

To ensure the signal is usable for traders, the Volume Line includes an optional **Smoothing** feature:

* **Unsmoothed (Raw)**: Captures every tick and micro-shift in momentum. Useful for fast scalpers.
* **Smoothed (EMA)**: Uses an Exponential Moving Average to filter out market noise and wicks. This provides a much clearer view of the "core" trend and reduces the number of false zero-line crossovers.

### Visual Cues

The Volume Line provides instant visual feedback through its color and position:

* **Teal Line (Bullish Regime)**: When the line is above **0.0**, it is colored teal (default), indicating that buyers are in control and the price is in the upper half of its volatility range.
* **Red Line (Bearish Regime)**: When the line is below **0.0**, it is colored red (default), indicating that sellers are in control.
* **Histbase Interaction**: The line is plotted against a histogram area base of 0.0, making it easy to identify **Regime Shifts** (crosses of the zero line).

### Practical Usage

* **Ascension/Descension**: Watch for the _slope_ of the line. A steepening slope indicates accelerating momentum.
* **Zero-Line Rejections**: If the line approaches 0.0 but bounces off it, it confirms that the current regime is very strong and the mean is acting as support/resistance.
* **Crossovers**: A Zero-Line Crossover is a primary signal of a trend change.

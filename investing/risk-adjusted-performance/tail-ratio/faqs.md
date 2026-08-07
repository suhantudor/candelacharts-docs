---
description: Tail Ratio FAQs
icon: square-question
---

# FAQs

<details>

<summary>What is a "good" Tail Ratio to look for?</summary>

A Tail Ratio above 1.0 (and especially above the Upper Guide, like 1.20) generally indicates a favorable risk profile where upside potential outweighs downside risk. However, it should be used in conjunction with other indicators rather than as a standalone buy/sell signal.

</details>

<details>

<summary>Should I use Log Returns or Simple Returns?</summary>

Log returns are generally preferred for financial time series analysis because they are time-additive and symmetric. However, for shorter timeframes, simple returns are often sufficient. We recommend experimenting with both to see which fits your specific asset and timeframe best.

</details>

<details>

<summary>Why is the Tail Ratio sometimes blank or very erratic?</summary>

If the asset has extremely low volatility (e.g., stablecoins or low-volume periods), the lower percentile can approach zero. The indicator has built-in protections against division by zero, which may cause it to temporarily flatline or clamp values to prevent massive, unreadable spikes.

</details>

<details>

<summary>Can I use this for short-term day trading?</summary>

Yes. While it is highly effective on higher timeframes (Daily, Weekly) for structural analysis, you can lower the Lookback Length (e.g., from 60 to 20) to make the oscillator more responsive for lower timeframe day trading.

</details>

<details>

<summary>How do I interpret the colored oscillator line?</summary>

The line changes color based on the neutral 1.0 level. It is colored Teal when the Tail Ratio is above 1.0 (Positive Skew), indicating favorable upside conditions, and Orange when it is below 1.0 (Negative Skew), highlighting increased downside risk.

</details>


---
description: ATH Drawdown FAQs
icon: square-question
---

# FAQs

<details>

<summary>Does this repaint?</summary>

No. The series is based on a running maximum (ATH) and current price. It will update intra-bar as price moves (like any real-time series), then fix at bar close. There is no look-ahead.

</details>

<details>

<summary>Why did my drawdown change after switching symbols or loading more history?</summary>

ATH is computed from the first available bar on your chart. Different symbols/exchanges or added history can reveal an earlier/higher ATH, changing the baseline. Use the feed with the most complete history for consistency.

</details>

<details>

<summary>Close vs. High—what should I choose?</summary>

Close anchors ATH to settled prices (more conservative, fewer false peaks). High includes wicks, catching fleeting spikes—useful for identifying maximum extremes but more sensitive to noise.

</details>

<details>

<summary>What thresholds define a “deep” drawdown?</summary>

There’s no universal rule. Many high-volatility assets historically see −60% to −80% during major cycles, but you should calibrate bands to your asset class and risk model.

</details>

<details>

<summary>How do I reduce noisy alerts?</summary>

Set alerts to Once per bar close, use a higher timeframe, add a small EMA smoothing length (e.g., 3–8), or widen your alert band (e.g., −72% to −78% instead of −70% to −80%).

</details>

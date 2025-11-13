---
description: Sortino Ratio FAQs
icon: square-question
---

# FAQs

<details>

<summary>Sortino vs. Sharpe—when use which?</summary>

Sharpe penalizes total volatility; Sortino penalizes only downside. Use Sortino when negative swings matter more than upside noise.

</details>

<details>

<summary>What should I use for MAR?</summary>

Risk-Free is a robust default. Use a **Custom per-period** hurdle to reflect a strategy target (e.g., 0.05% per bar).

</details>

<details>

<summary>Simple or Log returns?</summary>

Log handles large moves and cross-asset comparisons better; Simple is fine for stable, small step changes.

</details>

<details>

<summary>Do percentile bands repaint?</summary>

No. Bands are computed from the rolling history up to the calibration window; values lock after bar close.

</details>

<details>

<summary>Why does Sortino jump when I change MAR or return type?</summary>

Because both the numerator (excess vs. MAR) and the denominator (downside deviation below MAR) depend on those choices—pick settings that match your objective and keep them consistent across comparisons.

</details>

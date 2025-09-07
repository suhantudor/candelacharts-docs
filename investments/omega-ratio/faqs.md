---
description: Omega Ratio FAQs
icon: square-question
---

# FAQs

<details>

<summary>What does Omega > 1 actually guarantee?</summary>

Nothing deterministic—markets are noisy—but it _does_ mean that over your window, cumulative wins above the hurdle exceed cumulative misses, i.e., better-than-target quality.

</details>

<details>

<summary>How should I choose the Target Return?</summary>

Anchor it to timeframe and asset. Daily: **0.00–0.10%** per bar is common; intraday is smaller. Backtest values that reflect your strategy’s realistic edge.

</details>

<details>

<summary>Should I prefer log returns?</summary>

Use **log** when comparing across assets or dealing with large swings; it treats up/down moves symmetrically. Use **linear** for small, stable bars where differences are negligible.

</details>

<details>

<summary>Does Omega repaint?</summary>

No. It’s a rolling sum over completed bars. Values update intrabar while the bar forms and lock at close—standard indicator behavior.

</details>

<details>

<summary>Why is my Omega chronically low/high?</summary>

Your **target** may be too ambitious/lenient, or your **Period** too short/long. Raise target or shorten the window to lower readings; lower target or lengthen the window to raise/stabilize them.

</details>

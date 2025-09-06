---
description: Mayer Multiple Z-score FAQs
icon: square-question
---

# FAQs

<details>

<summary>What is the Mayer Multiple here?</summary>

It’s \[b]price ÷ SMA\[/b] using your chosen length (default 200). The script then converts that ratio into a Z-Score based on your undervalue/overvalued mapping.

</details>

<details>

<summary>Why use a cumulative-to-rolling SMA?</summary>

Early bars shouldn’t pretend you have a full 200-bar history. The average grows honestly until the lookback is filled, then behaves like a standard SMA—clean and non-repainting.

</details>

<details>

<summary>Do any plots repaint?</summary>

No. The SMA, Z-Score, and its EMA use completed historical data. Values only change intrabar while the bar is forming, then lock after close.

</details>

<details>

<summary>How should I pick the thresholds (0.5 / 2.0)?</summary>

Keep the span at roughly **6σ** for comparability; move the endpoints to match asset class. Higher-vol assets may warrant a higher “overvalued” multiple (e.g., 2.5) and/or a lower “undervalue” multiple.

</details>

<details>

<summary>Will bar coloring affect performance or visibility of other indicators?</summary>

Barcolor is purely visual; if it clashes, disable \[b]Bar Color\[/b] and keep the Z-Score/EMA plots and fills as your primary cues.

</details>

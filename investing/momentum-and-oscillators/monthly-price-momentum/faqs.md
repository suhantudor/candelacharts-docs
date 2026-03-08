---
description: Monthly Price Momentum FAQs
icon: square-question
---

# FAQs

<details>

<summary>Is this time-frame dependent?</summary>

The formula is scale-agnostic, but “30 days” is most natural on Daily charts. On intraday, you’re measuring the last 30 daily closes’ effect—still valid, but interpret accordingly.

</details>

<details>

<summary>Does smoothing add lag?</summary>

Yes, slightly. Smoothing (EMA) improves readability at the cost of a bit of delay. Use a smaller value for quicker reacts, larger for calmer visuals.

</details>

<details>

<summary>How do I choose a good Upper Level?</summary>

Scan history: pick a value that captures strong thrusts without triggering constantly (e.g., +20–25% for low-vol, +30–40% for high-beta).

</details>

<details>

<summary>Can I add a lower threshold line (e.g., −20%)?</summary>

This version exposes only the upper level; you can still monitor a custom negative threshold by eye or with a separate horizontal line on the chart.

</details>

<details>

<summary>Does it repaint?</summary>

No. The ROC% and EMA use completed data and lock after bar close; values update intrabar as normal during formation.

</details>

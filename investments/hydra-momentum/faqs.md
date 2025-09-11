---
description: Hydra Momentum FAQs
icon: square-question
---

# FAQs

<details>

<summary>Is ±1 the same as overbought/oversold?</summary>

Not exactly. It’s a **normalized stretch**. Acceptance beyond ±1 can trend; rejection often mean-reverts.

</details>

<details>

<summary>Why didn’t my alert fire?</summary>

Usually the **Nondirectional** line was **below the filter**, or your **Alert Condition** (Source vs EMA) didn’t match your chosen **thresholds**.

</details>

<details>

<summary>Do Directional checkboxes change divergence logic?</summary>

Yes. The main composite drives divergences, so toggling components changes what can be detected.

</details>

<details>

<summary>How do I tune per timeframe/asset?</summary>

Raise **Overall Length** and **Smoothing** on higher TFs or noisy symbols; bring thresholds toward **±1** when using the EMA trigger or when volatility contracts.

</details>

<details>

<summary>What’s a good starter setup?</summary>

Use defaults, enable **Nondirectional**, keep the filter at **≥ −0.25** (or **0** for stricter), start with **Directional Source** and **±1.25** thresholds, then adapt to your market.

</details>

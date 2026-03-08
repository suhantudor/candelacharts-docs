---
description: MVRV Ratio FAQs
icon: square-question
---

# FAQs

<details>

<summary>What exactly is MVRV?</summary>

It’s the ratio of the network’s market cap to its realized cap (sum of coins priced at last on-chain move). Values above 1 mean market value exceeds holder cost basis; far above 1 often marks frothy phases.

</details>

<details>

<summary>Why those fixed levels (3.5 / 2.5 / 1.0 / 0.8)?</summary>

They’re widely watched cycle landmarks: 1.0 ≈ fair value, 0.8 ≈ stress, 2.5–3.5 ≈ elevated to extreme euphoria. Use them as guides, not guarantees.

</details>

<details>

<summary>Do σ bands repaint?</summary>

No. The bands use historical mean/stdev over a fixed lookback and update only as new bars arrive; completed bars don’t change after close.

</details>

<details>

<summary>Does the script compute MVRV itself?</summary>

No. It reads curated MVRV series for BTC/ETH and plots them with added logic (levels, zones, bands). That keeps the output consistent with trusted data sources.

</details>

<details>

<summary>Why use “lookahead on” in the code?</summary>

To align historical MVRV values precisely with past bars when requesting the series, avoiding off-by-one shifts—visual accuracy matters for threshold touches.

</details>

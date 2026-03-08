---
description: Macro Sentiment Index FAQs
icon: square-question
---

# FAQs

<details>

<summary>How is the Macro Sentiment Index calculated?</summary>

MSI computes z-scores for each component over a lookback period, adjusts directionality (e.g., VIX is inverted), applies user-defined weights, and calculates a weighted average. The result is smoothed optionally with a moving average.

</details>

<details>

<summary>What does a reading of +1.5 mean?</summary>

A score above +1 indicates strong risk-on sentiment. At +1.5, most risk assets are performing well relative to history, potentially signaling euphoria or complacency. Monitor for reversals or volatility spikes.

</details>

<details>

<summary>Can I use MSI for crypto trading?</summary>

Yes. Bitcoin and crypto markets are highly sensitive to global liquidity and risk appetite. MSI serves as an excellent macro filter—avoid aggressive longs when MSI is deeply negative.

</details>

<details>

<summary>Why is the VIX given a negative sign in scoring?</summary>

Because rising VIX reflects fear and risk aversion. In MSI logic, higher fear = lower sentiment, so its z-score is negated to align with the overall scale.

</details>

<details>

<summary>Is MSI leading or lagging?</summary>

It is **primarily coincident**, reflecting current market sentiment. However, due to z-score normalization and aggregation, it can act as a **leading indicator** when divergences appear (e.g., price up, MSI down).

</details>

<details>

<summary>Is CSI suitable for intraday trading?</summary>

No.

</details>

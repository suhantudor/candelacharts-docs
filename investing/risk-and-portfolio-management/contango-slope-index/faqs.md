---
description: Contango Slope Index FAQs
icon: square-question
---

# FAQs

<details>

<summary>What does a negative slope mean?</summary>

A negative slope indicates **backwardation** in the VIX futures curve—near-term volatility is priced higher than longer-term expectations. This often reflects panic or crisis conditions and has historically been a statistically significant predictor of **short-to-medium-term equity market rallies**.

</details>

<details>

<summary>Why is 2.32% the threshold for elevated complacency?</summary>

The **0.0232** value (\~2.32% per year) represents the **long-term average slope** of the VIX term structure under normal market conditions. When the current slope exceeds this level, it suggests that investors are paying a premium for longer-dated protection, which can signal **excessive calm** and increased vulnerability to shocks.

</details>

<details>

<summary>Can I use CSI on instruments other than VIX?</summary>

While the default implementation uses VIX futures, the underlying methodology can be adapted to any futures curve exhibiting contango/backwardation behavior (e.g., oil, gold, crypto perpetuals). However, the thresholds and interpretations may need recalibration.

</details>

<details>

<summary>Does CSI predict market direction?</summary>

The CSI does not predict direction in isolation. It identifies **regimes of fear and complacency** that have shown statistical tendencies to precede certain types of moves. It should be used as part of a broader analytical framework, not as a standalone signal generator.

</details>

<details>

<summary>Why does the slope sometimes jump unexpectedly?</summary>

Sudden jumps can occur due to:

* Data gaps in VIX futures
* Contract rollover effects
* Extreme intraday volatility moves

The forward-filling mechanism minimizes discontinuities, but delays may occur depending on data availability.

</details>

<details>

<summary>Is CSI suitable for intraday trading?</summary>

No.

</details>

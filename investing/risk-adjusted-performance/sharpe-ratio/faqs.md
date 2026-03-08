---
description: Sharpe Ratio FAQs
icon: square-question
---

# FAQs

<details>

<summary>What’s a “good” Sharpe?</summary>

Rough rules: **\~1.0** is investable, **≥ 2.0** is very good, **≥ 3.0** is exceptional. Context matters—timeframe, asset class, and sample length all influence the number.

</details>

<details>

<summary>Why use log returns by default?</summary>

They treat up and down moves symmetrically and behave better for large swings and long horizons. Linear is fine for small, stable step changes.

</details>

<details>

<summary>How should I set Periods/Year?</summary>

Match your return sampling: **252** for daily, **52** for weekly, **12** for monthly, etc. This only affects annualized Sharpe.

</details>

<details>

<summary>Does it repaint?</summary>

No. The ratio uses completed data within rolling windows. Values evolve intrabar and lock at close, which is standard indicator behavior.

</details>

<details>

<summary>Why does my Sharpe jump when I change timeframe?</summary>

Because returns, volatility, and the **periods/year** scaling change with the sampling frequency. Either fix the calculation TF or compare like-for-like across symbols.

</details>

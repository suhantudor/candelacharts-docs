---
description: Macro Credit Model FAQs
icon: square-question
---

# FAQs

<details>

<summary>What does the "Calculate Excess Spread" setting do?</summary>

When enabled (default), the indicator subtracts the Investment Grade spread from the High Yield spread. This isolates the pure "credit risk premium" of junk bonds while stripping out baseline corporate interest rate effects, providing a cleaner signal of systemic stress.

</details>

<details>

<summary>Why do I see an error or no data on lower timeframes?</summary>

The underlying data is sourced from the Federal Reserve Economic Data (FRED) database, which only publishes these specific bond spreads on a daily basis. The indicator will only work on the Daily (1D), Weekly (1W), or Monthly (1M) charts.

</details>

<details>

<summary>What is a Z-Score and why use it instead of the raw spread?</summary>

A Z-Score measures how many standard deviations the current spread is from its historical average. A raw spread of 500 basis points might be "normal" in 2009 but "terrifying" in 2018. The Z-Score normalizes the data, making sure the signal is relative to the current market regime.

</details>

<details>

<summary>How do I trade the "Stress" signals?</summary>

A "Stress" signal (Z-Score > 2.0) is not necessarily a signal to short immediately, but rather a structural mandate to de-risk. It tells you to tighten stop losses, reduce position sizing, and avoid buying dips until credit markets stabilize.

</details>

<details>

<summary>Why is the "Low Risk Zone" colored Teal?</summary>

When credit spreads are low (negative Z-Score), it means borrowing is cheap and credit is flowing freely. This is a highly supportive, bullish environment for stocks, so it is colored Teal to signify a "Risk-On" environment.

</details>


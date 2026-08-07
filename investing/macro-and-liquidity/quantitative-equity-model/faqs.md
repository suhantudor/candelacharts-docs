---
description: Quantitative Equity Model FAQs
icon: square-question
---

# FAQs

<details>

<summary>What do the different "Allocation Types" mean?</summary>

The Allocation Type dictates the baseline aggressiveness of the model. "Risk-Averse" is quick to de-risk and slow to buy back in. "Risk-Seeking" prioritizes keeping money in the market. "Balanced" is in the middle, and "Adaptive" dynamically shifts its aggressiveness based on the current market regime.

</details>

<details>

<summary>Can I change the weight of the five pillars?</summary>

Yes. In the settings, you have full control over the percentage weights of the Market Regime, Risk, Valuation, Sentiment, and Macro pillars. Just ensure that the combined weights equal exactly 100%.

</details>

<details>

<summary>What happens when the model enters "Crisis" mode?</summary>

When the automated crisis engine detects extreme stress (e.g., massive VIX spikes or credit spread blowouts), it overrides the standard pillar calculations and immediately drops the recommended equity allocation toward 0%, urging a rapid shift to cash or safe havens.

</details>

<details>

<summary>How does "Portfolio Risk Scaling" work?</summary>

If you enable risk scaling and input a Target Volatility (e.g., 15%) and Max Drawdown (e.g., 20%), the model will mathematically throttle your equity allocation down to ensure your overall portfolio (Equities + Cash) stays within those specific risk confines.

</details>

<details>

<summary>Why is the allocation stuck at 0% for so long?</summary>

During severe secular bear markets or prolonged economic crises, the model prioritizes capital preservation. It will keep the allocation at or near 0% until multiple pillars (like Valuation and Trend) show structural improvement, helping you avoid "catching a falling knife."

</details>


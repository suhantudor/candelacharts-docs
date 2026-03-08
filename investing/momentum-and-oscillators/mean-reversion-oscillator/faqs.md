---
description: Mean Reversion Oscillator FAQs
icon: square-question
---

# FAQs

<details>

<summary>What does the Mean Reversion Oscillator measure?</summary>

It measures the deviation of price from its moving average, scaled into a 0–100 range. High = stretched above mean; Low = stretched below mean.

</details>

<details>

<summary>Why does the oscillator sometimes stick at 0 or 100?</summary>

Because StdDev Length is too short compared to MA Length, volatility is underestimated. Fix: set **StdDev Length equal to MA Length** or increase it.

</details>

<details>

<summary>How should I set Overbought and Oversold levels?</summary>

* Default: 70/30 works broadly.
* Conservative: 80/20 for fewer, stronger signals.
* Aggressive: 60/40 for more frequent triggers.

</details>

<details>

<summary>Can MRO be used in trending markets?</summary>

Yes, but with a **trend filter**. Strong uptrends can keep MRO overbought for long periods. Use 200 EMA or HTF bias to avoid fading healthy trends.

</details>

<details>

<summary>Can the MRO be used to spot divergences?</summary>

* **Bullish divergence:** Price makes a lower low while MRO forms a higher low → possible reversal upward.
* **Bearish divergence:** Price makes a higher high while MRO forms a lower high → possible reversal downward.\
  These signals are strongest when they align with support/resistance or higher timeframe context.

Yes. Divergences between price and the MRO can signal weakening momentum:

It’s designed for versatility and can be applied to stocks, forex, crypto, futures, and indices across any timeframe.

</details>

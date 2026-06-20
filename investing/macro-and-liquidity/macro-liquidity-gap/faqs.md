---
description: Macro Liquidity Gap FAQs
icon: square-question
---

# FAQs

<details>

<summary><strong>Why is the indicator not loading on intraday charts?</strong></summary>

The Macro Liquidity Gap requires a Daily (1D) or higher timeframe. Central bank money supply data is only updated weekly or monthly, making intraday calculations impossible.

</details>

<details>

<summary><strong>How does the Fed Net Liquidity blend work?</strong></summary>

The indicator allows you to blend standard US M2 with the more precise Fed Net Liquidity formula (Balance Sheet - TGA - Reverse Repo). You can use the slider in the settings to adjust the weighting based on your preference.

</details>

<details>

<summary><strong>Why is China's M2 weight discounted?</strong></summary>

China operates with strict capital controls, meaning a significant portion of its printed money cannot easily flow into global asset markets like the S\&P 500. We discount it by 50% to provide a more realistic picture of "exportable" liquidity.

</details>

<details>

<summary><strong>Can I change the asset the liquidity is compared against?</strong></summary>

Yes, by default it compares against the S\&P 500 (SP:SPX), but you can change the target index or asset in the indicator settings to analyze how liquidity affects Bitcoin, Gold, or other indices.

</details>

<details>

<summary><strong>Does it repaint?</strong></summary>

No, the indicator calculates based on closed data. However, be aware that central bank M2 data is sometimes subject to slight historical revisions by the issuing banks themselves.

</details>

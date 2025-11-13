---
description: Period ROI FAQs
icon: square-question
---

# FAQs

<details>

<summary>What does the “daily reference” mean in practice?</summary>

The indicator fetches a daily series for consistency. On markets that trade every day (e.g., crypto), “days” map one-to-one; on markets with non-trading days, the lookback counts daily bars (not calendar weekends/holidays).

</details>

<details>

<summary>Why is my 1Y ROI not exactly year-over-year on some symbols?</summary>

For instruments without seven-day trading, “365 daily bars” can cover more than 365 calendar days. The benefit is TF-consistency; if you need strict calendar math, set a custom days value appropriate for that market.

</details>

<details>

<summary>Can I use another source than Close?</summary>

Yes—use the **Source** input to compute ROI on your preferred series.

</details>

<details>

<summary>Does it repaint?</summary>

No. The ROI uses completed daily data; values update intrabar while a bar forms and lock after close.

</details>

<details>

<summary>How should I choose the right window?</summary>

Match the window to the decision you’re making: 1M for tactical momentum, 3–6M for rotation, 1Y for business-cycle context. Keep it consistent across comparisons.

</details>

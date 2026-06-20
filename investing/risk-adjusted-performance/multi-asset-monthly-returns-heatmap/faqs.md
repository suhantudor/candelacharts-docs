---
description: Multi-Asset Monthly Returns Heatmap FAQs
icon: square-question
---

# FAQs

<details>

<summary><strong>Why is the heatmap not loading or showing a timeframe error?</strong></summary>

The indicator requires your chart to be set to the 1M (Monthly) timeframe to accurately pull and calculate the monthly data for all 28 assets. Please switch your chart to the 1M timeframe.

</details>

<details>

<summary><strong>Can I change the assets displayed in the heatmap?</strong></summary>

Yes, all 28 assets are fully customizable. You can change the ticker symbol and the display name for each slot in the indicator's settings menu.

</details>

<details>

<summary><strong>What does the "Calc Mode" setting do?</strong></summary>

The Calc Mode determines which statistical metric is calculated and displayed for each month. For example, "Mean" shows the average historical return for that month, while "Max" shows the single highest return ever recorded for that month.

</details>

<details>

<summary><strong>Why do the color intensities change when I switch Calc Modes?</strong></summary>

The indicator features dynamic heatmap scaling. Because different metrics have different typical ranges (e.g., the 'Sum' of all returns will be much larger than the 'Mean'), the indicator automatically adjusts its color intensity thresholds so the heatmap remains visually readable and useful.

</details>

<details>

<summary><strong>Does this indicator slow down TradingView?</strong></summary>

Because it pulls historical data for up to 28 different assets simultaneously and performs complex statistical calculations, it can take a moment to load upon initial application or when changing settings. This is normal and expected behavior for heavy data-aggregation scripts.

</details>

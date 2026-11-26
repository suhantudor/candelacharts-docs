---
description: Investor Tool FAQs
icon: square-question
---

# FAQs

<details>

<summary>How is the MA length computed across different timeframes?</summary>

`ma_length = years × bars_per_year`, where bars/year adapts to the chart: Daily≈365, Weekly≈52, Monthly≈12, Intraday≈252. Your “2 years” remains time-comparable across TFs.

</details>

<details>

<summary>Do WVAPs repaint?</summary>

They’re **cumulative within the active anchor** and **reset at the new anchor** (e.g., new Month/Quarter/Year). They update as new bars arrive but don’t revise completed anchor history after the bar closes.

</details>

<details>

<summary>My WVAP didn’t reset—why?</summary>

Resets occur only when the platform detects a true boundary via `timeframe.change(...)`. If your anchor is Year but you’re on a custom/time-compressed dataset, ensure the chart has full calendar continuity and that the selected anchor granularity is supported on that symbol.

</details>

<details>

<summary>Can I use this on symbols with little or no volume (indices, some CFDs, synthetics)?</summary>

Yes—**Investor MA** and **bands** work normally because they use price only. However, **WVAPs** depend on volume; on symbols without reliable volume they may be `na` or noisy. In that case, disable WVAPs and rely on MA + bands (and anchors on higher-quality proxies, if needed).

</details>

<details>

<summary>Do the MA and bands repaint or change after the bar closes?</summary>

No. The MA (`ta.sma`) and bands (`± multiplier × stdev`) use only past data and **do not repaint** once a bar closes. They will look different when you **change timeframe** because `bars_per_year` adjusts (Daily≈365, Weekly≈52, etc.), and early bars can be `na` until the lookback fills—both expected behavior, not repainting.

</details>

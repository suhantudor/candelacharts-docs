---
description: Volatility Regime Model FAQs
icon: square-question
---

# FAQs

<details>

<summary><strong>Can I change the VIX thresholds for the different regimes?</strong></summary>

Yes, you can fully customize the threshold levels for Low, Mid, High, and Crisis Cluster zones in the settings menu to fit different assets or historical periods.

</details>

<details>

<summary><strong>What is VIX Smoothing and should I use it?</strong></summary>

VIX Smoothing applies a Hull Moving Average (HMA) to the raw VIX data. This filters out intraday noise and prevents rapid switching of states during volatile, choppy sessions.

</details>

<details>

<summary><strong>Which tickers are used for Cross-Asset Validation?</strong></summary>

By default, it uses the MOVE Index for bond volatility and the High-Yield vs Investment Grade corporate bond spread for credit validation. You can customize these tickers in the settings.

</details>

<details>

<summary><strong>How do I interpret the "Fade Noise" vs "Defensive" bias?</strong></summary>

"Fade Noise" appears early in a volatility spike (Days 1-2), suggesting a high probability of mean reversion. "Defensive" appears when the spike persists (Day 6+), indicating a genuine regime shift where fading the volatility is dangerous.

</details>

<details>

<summary><strong>How do I move the dashboard if it blocks price action?</strong></summary>

You can easily adjust the positioning of the real-time summary dashboard to any corner of the chart via the settings panel.

</details>

---
description: Composite Risk Index FAQs
icon: square-question
---

# FAQs

<details>

<summary>Does the indicator repaint?</summary>

No. The Composite Risk Index is strictly coded to execute on the bar close and uses non-repainting historical data referencing. It does not look into the future. All regime shifts are confirmed once the candle closes.

</details>

<details>

<summary>Which timeframes does it work best on?</summary>

It is designed as a macro compass, meaning it performs best on the **Daily (1D)** and **Weekly (1W)** timeframes. Intraday timeframes (like 15m or 1H) will be too noisy for evaluating structural market regimes.

</details>

<details>

<summary>Does it work on both Crypto and Stocks?</summary>

Yes! The indicator automatically detects the asset class you are trading. If you are on an equity, forex, or index chart, it uses CBOE:VIX for external volatility referencing. If you are on a crypto asset, it uses Deribit DVOL.

</details>

<details>

<summary>What exactly do the "Buy Zone" backgrounds mean?</summary>

When the index enters a deep Crisis state (Score below -1.0), the chart background is highlighted. This indicates a period of extreme, irrational market fear—often characterized by capitulation volume. Historically, buying solid spot assets during these specific windows yields the highest long-term returns. It is an accumulation signal, not a shorting signal.

</details>

<details>

<summary>How do I set up alerts for a regime change?</summary>

Simply click the Alert icon in TradingView, select the Composite Risk Index from the dropdown, and choose the "Any alert() function call" condition. This single alert will trigger a dynamic notification containing the ticker, the new regime, and the score every time the regime shifts.

</details>


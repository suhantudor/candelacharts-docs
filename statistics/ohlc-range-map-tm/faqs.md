---
description: OHLC Range Map FAQs
icon: circle-question
---

# FAQs

<details>

<summary><strong>Do I need to create separate alerts for every level?</strong></summary>

No. You only need to create **one** alert in the TradingView "Create Alert" dialog by selecting the indicator and choosing the `Any alert() function call` condition. This will funnel all enabled level crosses into a single alert stream.

</details>

<details>

<summary><strong>What does the alert message look like?</strong></summary>

A typical message follows this format: `[Ticker] ([Timeframe]): Price reached [Level Name] Level`.\
&#xNAN;_&#x45;xample:_ `EURUSD (1D): Price reached Manipulation (+M) Level`

</details>

<details>

<summary><strong>Can I use these for Telegram or Discord bots?</strong></summary>

Yes. Because the indicator uses the `alert()` function, the dynamic messages can be sent via Webhook URL to any third-party automation service or bot.

</details>


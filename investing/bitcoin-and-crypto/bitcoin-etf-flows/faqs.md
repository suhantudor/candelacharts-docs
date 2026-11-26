---
description: Bitcoin ETF Flows FAQs
icon: square-question
---

# FAQs

<details>

<summary>Why does the indicator require a 1D timeframe or higher?</summary>

Spot Bitcoin ETFs report their balances and flows at the end of the trading day. Therefore, intraday data is not available or accurate. The indicator enforces a minimum 1D timeframe to ensure the data is displayed correctly.

</details>

<details>

<summary>Where does the ETF data come from?</summary>

The indicator utilizes professional-grade Glassnode metrics natively integrated into TradingView to pull the exact underlying balances for each specific ETF.

</details>

<details>

<summary>What is the difference between Money and Coins data formats?</summary>

"Money" displays the flows in USD value, which is influenced by the current price of Bitcoin. "Coins" displays the flows in raw BTC amounts, isolating the actual accumulation/distribution behavior regardless of fiat price fluctuations.

</details>

<details>

<summary>How should I use the Z-Score format?</summary>

The Z-Score measures how many standard deviations a recent flow is from the historical average (defined by the Z-Score Length). A Z-Score above +2.0 or below -2.0 indicates a statistically extreme inflow or outflow event, which often marks a point of exhaustion or capitulation.

</details>

<details>

<summary>Can I turn off specific ETFs if I only want to track a few?</summary>

Yes. The settings menu allows you to individually toggle each of the 10 supported ETFs on or off, allowing you to create custom aggregate views or track specific funds in isolation.

</details>


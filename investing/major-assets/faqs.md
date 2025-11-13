---
description: Major Assets FAQs
icon: square-question
---

# FAQs

<details>

<summary>Why does US M2 look “steppy” on intraday charts?</summary>

M2 is a monthly macro series. On lower timeframes you’ll see discrete steps; use it for context, not timing.

</details>

<details>

<summary>Can I use spot crypto instead of futures?</summary>

Yes—change the symbols (e.g., BTCUSD/ETHUSD from your preferred exchange). Futures are provided by default for broader availability.

</details>

<details>

<summary>Do I need volume for this to work?</summary>

No—this indicator uses price only. It handles symbols with sparse data more gracefully than volume-based tools.

</details>

<details>

<summary>Why don’t all series start exactly on my chosen date?</summary>

If a symbol lacks data on that exact bar, the indicator uses the first available bar after the date. That ensures consistent, non-`na` indexing.

</details>

<details>

<summary>Does this indexing include dividends, distributions, or futures roll effects?</summary>

No—index levels are based on the instrument’s **price close** only. Dividends and distributions aren’t added back, and futures may reflect **roll/contract construction** artifacts. If you need total-return style comparisons, use **total-return tickers/indices** (when available) or dividend-adjusted series; for futures, prefer **spot** or a **back-adjusted continuous** contract that matches your methodology.

</details>

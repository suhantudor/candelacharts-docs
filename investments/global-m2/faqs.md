---
description: Global M2 FAQs
icon: square-question
---

# FAQs

<details>

<summary>Why is Australia labeled AUM3 instead of M2?</summary>

Australia commonly publishes **M3** as the broader aggregate comparable to M2 elsewhere; using AUM3 preserves a consistent liquidity proxy.

</details>

<details>

<summary>My YoY shows “na” for a while—what’s happening?</summary>

YoY needs a **52-week** history. If the aggregate (given your current region toggles) lacks enough back data, YoY will be **na** until the lookback is filled.

</details>

<details>

<summary>Can I add alerts for crossings or threshold events?</summary>

The script doesn’t ship with built-in alerts, but you can create **manual alerts** on the Global M2 or its MA (e.g., crossing a value, moving up/down).

</details>

<details>

<summary>Which MA type should I prefer?</summary>

* **SMA** for structural regimes,
* **EMA** for faster inflection capture,
* **WMA** for a weighted middle ground.

Choose based on your asset’s responsiveness and timeframe.

</details>

<details>

<summary>Why don’t totals exactly match external dashboards?</summary>

Differences in **definitions, sources, update timing, and FX treatment** lead to minor discrepancies. This indicator aggregates TradingView ECONOMICS series with spot-like FX conversions at the chart’s resolution.

</details>

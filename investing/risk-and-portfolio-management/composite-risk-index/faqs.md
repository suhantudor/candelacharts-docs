---
description: Composite Risk Index FAQs
icon: square-question
---

# FAQs

<details>

<summary>Why does the indicator use FRED data instead of the standard VIX ticker?</summary>

Using the `FRED:VIXCLS` ticker ensures the data is strictly daily closing data, which provides a cleaner, more robust dataset for calculating long-term statistical standard deviations without the noise of intraday gaps and wicks.

</details>

<details>

<summary>Can I use this indicator on intraday timeframes?</summary>

Because the underlying FRED data is updated daily, this indicator is strictly designed for the Daily (1D) timeframe and higher. It will not display accurate data on lower timeframes like 1H or 5m.

</details>

<details>

<summary>Why is the "Panic" zone colored Blue and "Complacency" colored Orange?</summary>

This contrarian color scheme is deliberate. Blue (cool) reminds you to stay calm and look for buying opportunities when everyone else is panicking. Orange (warm/warning) reminds you to be cautious and alert when everyone else feels perfectly safe. You can change these in the settings.

</details>

<details>

<summary>What does the "Z-Score Length" setting do?</summary>

This determines how many days of history the indicator uses to calculate the average VIX and its standard deviation. The default of 365 days gives a solid 1-year rolling window, ensuring the Z-Score adapts to the current macro environment rather than comparing today's volatility to a completely different market decade.

</details>

<details>

<summary>Does a Z-Score of +2.0 mean I should buy immediately?</summary>

Not necessarily. In a severe crisis (like 2008 or 2020), the VIX can stay elevated for weeks, pushing the Z-Score extremely high. A reading > 2.0 tells you that capitulation is occurring; you should use technical triggers (like a bullish engulfing candle or a break of market structure) to time the actual entry.

</details>


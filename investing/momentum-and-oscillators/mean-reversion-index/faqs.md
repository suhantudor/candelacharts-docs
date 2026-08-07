---
description: Mean Reversion Index FAQs
icon: square-question
---

# FAQs

<details>

<summary>What does the "Lookback (Bars)" setting do?</summary>

The lookback period determines the historical window used to calculate the Z-Score. The default is 730 bars, which represents roughly 2 years of daily trading data in traditional markets. This ensures the indicator has enough historical context to accurately determine what constitutes a "rare" extreme.

</details>

<details>

<summary>Can I use this on intraday timeframes?</summary>

Yes, but you will need to adjust your settings. A 200-period MA on a 5-minute chart represents less than one day of price action. For intraday use, you may want to increase the MA Length and adjust the Lookback to reflect the specific micro-cycle you are trying to trade.

</details>

<details>

<summary>Why did the price keep falling after it entered the Buy Zone?</summary>

A Z-Score below -2σ simply means the move is a statistical outlier (occurring roughly 2.5% of the time in a normal distribution). It does not mean the price must reverse instantly. During severe market panics, price can ride the extreme bands for days or weeks. This is why confluences are necessary for exact timing.

</details>

<details>

<summary>What is the Fractal Map?</summary>

The Fractal Map is a visual tool that tracks the time (in bars) between significant peaks or troughs in the oscillator. By displaying the historical cycle lengths, it helps you identify temporal patterns and estimate when the next major mean reversion event might occur.

</details>

<details>

<summary>How do I enable the Buy Zone on my main chart?</summary>

In the settings menu under "Settings," simply check the box labeled "Show Buy Zones". This will cast the Buy Zone background color directly onto your main price chart whenever the indicator drops below the -2σ threshold, making it impossible to miss.

</details>


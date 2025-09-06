---
description: Momentum Pulse FAQs
icon: square-question
---

# FAQs

<details>

<summary>Does the gradient repaint or shift after the bar closes?</summary>

No. Colors are derived from current momentum and its stdev over the chosen length; values settle at bar close like any standard indicator.

</details>

<details>

<summary>My gradient looks too “hot” or too “cold”—what should I change first?</summary>

Adjust the Multiplier (k). Raise k to widen the color range (less “hot”); lower k to tighten it (more sensitive heat).

</details>

<details>

<summary>How do I pick good Level 1/Level 2 values?</summary>

Scan history: set L1 to catch routine pushes and L2 to capture true thrusts. If L2 triggers too often, increase it; if almost never, decrease it.

</details>

<details>

<summary>What’s the difference between the two MAs?</summary>

“Normal MA” = SMA(close,len); “Smoothed MA” = SMA(src,len). The latter tracks the blended source used by the momentum calculation and typically reduces noise.

</details>

<details>

<summary>Can I use this intraday?</summary>

Yes. The log math is time-scale agnostic. For choppy intraday names, increase Length and/or k, and rely more on L2 and the zero-line to avoid over-trading.

</details>

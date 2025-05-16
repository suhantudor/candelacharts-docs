---
description: Turtle Soup Model Labels
icon: text-size
---

# Labels

The model assigns specific labels based on certain conditions.&#x20;

Below is an explanation of what each label represents.

**C** - _Current Model Label:_ These models are generated and displayed based on the number of candles present on the Higher Time Frame (HTF).

**R** - _Realtime Model Label:_ These models are created on the Lower Time Frame (LTF) for the same HTF candle. Although they may reach 2 standard deviations or the first liquidity level, they can be invalidated later within the same candle.

**H** - _History Model Label:_ These models are derived from historical data.

{% hint style="warning" %}
Models generated on the LFT for the same HTF candle, even if they reach 2 standard deviations or the first liquidity level, may be invalidated later within the same candle if it hasn't closed yet. These are marked as "real-time invalidated models." Be cautious when using these models, as their status could change once the candle closes.
{% endhint %}

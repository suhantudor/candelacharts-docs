---
description: X Model Labels
icon: text-size
---

# Labels

The model displays specific labels under certain conditions. Here’s a breakdown of the meaning behind each label.

**C** - _Current Model Label:_ These models are generated and displayed based on the number of candles present on the Higher Time Frame (HTF).

**R** - _Realtime Model Label:_ These models are created on the Lower Time Frame (LTF) for the same HTF candle. Although they may reach 2 standard deviations or the first liquidity level, they can be invalidated later within the same candle.

**H** - _History Model Label:_ These models are derived from historical data.

{% hint style="warning" %}
Models formed on the LFT for the same HTF candle, even if they reach 2 standard deviations or the first liquidity level, can be invalidated later within the same candle due to the candle not having closed yet. These models are labeled as "real-time invalidated models." Exercise caution when working with these models, as the status may change once the candle closes.
{% endhint %}


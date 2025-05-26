---
description: Unicorn Model Labels
icon: text-size
---

# Labels

The model assigns specific labels based on certain conditions.&#x20;

Below is an explanation of what each label represents.

**C** - _Current Model Label:_ Generated based on the current number of candles available on the Higher Time Frame (HTF). These represent the actively forming model context.

**R** - _Realtime Model Label:_ Formed on the Lower Time Frame (LTF) within the duration of the same HTF candle. These may reach targets like 2 standard deviations or liquidity levels, but can still be invalidated before the HTF candle closes. These are dynamic and require caution.

**H** - _History Model Label:_ Based on fully closed HTF candles and confirmed LTF behavior. These models   reflect completed market structure.

{% hint style="warning" %}
Realtime (R) models that appear valid intrabar can still be retroactively invalidated if the HTF candle closes against them. Use with discretion during live analysis.
{% endhint %}

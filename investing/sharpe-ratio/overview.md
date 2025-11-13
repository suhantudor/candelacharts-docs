---
description: Sharpe Ratio Quick Specs
icon: list-ol
---

# Overview

<figure><img src="../../.gitbook/assets/docs-sharpe-ratio-001.png" alt=""><figcaption></figcaption></figure>

This implementation computes per-period returns from your chosen source and timeframe, subtracts a per-period risk-free hurdle derived from your annual input, and summarizes reward vs. variability over a configurable lookback.&#x20;

{% content-ref url="features.md" %}
[features.md](features.md)
{% endcontent-ref %}

{% content-ref url="usage.md" %}
[usage.md](usage.md)
{% endcontent-ref %}

{% content-ref url="confluences.md" %}
[confluences.md](confluences.md)
{% endcontent-ref %}

{% content-ref url="faqs.md" %}
[faqs.md](faqs.md)
{% endcontent-ref %}

You can smooth the line with a light EMA and read it against well-known guideposts (0, 0.5, 1, 2, 3) with a right-edge label for quick checks.

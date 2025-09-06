---
description: Mayer Multiple Z-score Quick Specs
icon: list-ol
---

# Overview

<figure><img src="../../.gitbook/assets/docs-mayer-multiple-zscore-001.png" alt=""><figcaption></figcaption></figure>

The indicator computes a long-term SMA (cumulative until the lookback is filled, then rolling), divides price by that SMA to form the **Mayer Multiple**, and linearly maps your chosen “undervalue” and “overvalued” multiples (e.g., 0.5× and 2.0×) to **−3σ and +3σ**.&#x20;

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

The result is a standardized **Z-Score** with an optional EMA smoothing layer, optional extreme-zone fills, and an optional bar-color gradient for heat.

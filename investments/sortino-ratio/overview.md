---
description: Sortino Ratio Quick Specs
icon: list-ol
---

# Overview

<figure><img src="../../.gitbook/assets/docs-sortino-ratio-001.png" alt=""><figcaption></figcaption></figure>

This implementation aligns the target (MAR) with your return type, computes excess returns per bar, and divides their average by the _downside_ deviation over a lookback.&#x20;

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

You can annualize for comparability, switch between **Percentile Bands** (P50/P75/P90 etc.) and **Fixed Levels** (0/0.5/1/2/3), and use a right-edge label that summarizes percentile bucket or level.

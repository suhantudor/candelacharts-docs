---
description: Monthly Price Momentum Quick Specs
icon: list-ol
---

# Overview

<figure><img src="../../.gitbook/assets/docs-mpm-001.png" alt=""><figcaption></figcaption></figure>

The indicator computes **ROC% = (Close − Close\[n]) / Close\[n] · 100**, with `n` defaulting to **30 days** (one month on Daily).&#x20;

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

It then applies an **EMA smoothing** and plots two references: a **dashed 0 line** (regime) and a **solid upper level** (default **+30%**) to highlight powerful upside runs. A blue→cyan gradient encodes acceleration.

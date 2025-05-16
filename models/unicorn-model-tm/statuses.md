---
description: Unicorn Model Statuses
icon: battery-quarter
---

# Statuses

The **Turtle Soup Model** follows a well-defined lifecycle, outlining its current state and determining if a trade opportunity is valid.&#x20;

The lifecycle consists of four phases:

* **Formation**
* **Pre-Invalidation**
* **Invalidation**
* **Success**

{% hint style="info" %}
The current status of the model will become visible when you hover your cursor over the associated label (e.g., C1, R1, H1).
{% endhint %}

### **1. Formation**

The **Formation** phase marks the beginning of the Turtle Soup setup. During this phase, the model identifies key components that suggest a potential reversal, such as:

* **Sweeps**: Price moves that capture liquidity, often above or below significant swing points, signaling potential trend shifts.
* **Market Structure Shift (MSS)**: A structural shift that indicates a potential change in market direction.

Once identified, the model calculates **Projections** and **Liquidity Levels**, providing insight into potential price movements and the overall market bias.

{% hint style="warning" %}
The lower timeframe PD Arrays are essential for model formation. In the absence of a LTF PD Array, the model is considered low probability and will not be formed.
{% endhint %}

### **2. Pre-Invalidation**

In the **Pre-Invalidation** phase, the model is considered at risk of failing. This occurs when the price moves above the sweep high but the **sweep itself remains intact** (not fully broken). In this case:

* The model is viewed as **unreliable** but not yet fully invalidated.
* The **sweep high** remains significant, indicating the setup may still be valid, but it’s close to being invalidated.

{% hint style="info" %}
Most setups in this phase do not lead to success, as the market often reverses, and the original trade setup becomes less reliable.
{% endhint %}

### **3. Invalidation**

The **Invalidation** phase occurs when key conditions for the setup are not met, signaling that the trade idea is no longer valid. The model is invalidated if:

* The price **fails to reach** the 2 Standard Deviation level.
* The price **doesn’t hit** the first identified liquidity level.
* The price **breaks above** the sweep high.

When the model is invalidated, it is crucial for traders to **abandon the setup**, as the trade no longer aligns with the expected price behavior.

### **4. Success**

The **Success** phase happens when the trade setup aligns with the expected market movement, confirming that the model is valid. Success is reached when:

* The price **reaches the 2 Standard Deviation level**.
* The price **hits the first identified SSL/BSL liquidity level**.

At this point, the model’s predictions are confirmed, and traders can **execute the trade** with higher confidence.

By understanding the **Formation**, **Pre-Invalidation**, **Invalidation**, and **Success** phases, traders can effectively manage positions and capitalize on high-probability setups identified by the Turtle Soup Model.&#x20;

This structured approach helps reduce risk and increases the likelihood of successful trades.

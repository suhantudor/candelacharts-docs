---
description: Unicorn Model Statuses
icon: battery-quarter
---

# Statuses

The Unicorn Model operates through a structured lifecycle that defines its current state and assesses whether a trade opportunity is valid or actionable.

The lifecycle consists of four phases:

* **Formation**
* **Pre-Invalidation**
* **Invalidation**
* **Success**

{% hint style="info" %}
The current status of the model will become visible when you hover your cursor over the associated label (e.g., C1, R1, H1).
{% endhint %}

### **1. Formation**

The **Formation** phase is the starting point of the Unicorn Model, where key structural elements are identified that indicate a potential market reversal, such as:

* **Sweeps**: Price moves that capture liquidity, often above or below significant swing points, signaling potential trend shifts.
* **Zigzag (Breaker)**: A Zigzag Breaker in the Unicorn Model is a reversal pattern formed when price breaks the structure between the 2nd and 3rd Zigzag points, confirming a shift in order flow and initiating a new directional leg.

Once identified, the model calculates **Standard Deviation,** **Liquidity Levels** and display **Macros**, providing insight into potential price movements and the overall market bias.

### **2. Pre-Invalidation**

In the **Pre-Invalidation** phase, the model is considered at risk of failing. This occurs when the price moves above the sweep high but the **sweep itself remains intact** (not fully broken). In this case:

* The model is viewed as **unreliable** but not yet fully invalidated.
* The **sweep high** remains significant, indicating the setup may still be valid, but it’s close to being invalidated.

{% hint style="info" %}
Most Unicorn Models in this phase fail to follow through, as the market often reverses, making the original trade setup less reliable or invalid.
{% endhint %}

### **3. Invalidation**

The **Invalidation** phase marks the point where the trade setup loses validity due to unmet conditions. A Unicorn Model is invalidated if:

* Price fails to reach the **2 standard deviation** projection,
* Price does not tap the **first liquidity level**, or
* Price breaks above the **sweep high** (or low, depending on direction).

When invalidated, the setup should be discarded, as it no longer reflects the model’s expected market behavior.

### **4. Success**

The **Success** phase confirms the Unicorn Model’s validity when price moves in line with expectations. It is achieved when:

* Price reaches the **2 standard deviation** target, or
* Taps the first **SSL/BSL liquidity level**.

At this stage, the model is confirmed, giving traders greater confidence in executing the setup.

By mastering the **Formation**, **Pre-Invalidation**, **Invalidation**, and **Success** phases, traders can manage risk more effectively and capitalize on high-probability opportunities identified by the Unicorn Model.

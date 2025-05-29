---
description: X Model Statuses
icon: battery-quarter
---

# Statuses

The X Model follows a defined lifecycle that outlines its current status and determines whether a trade opportunity is valid. The lifecycle consists of the following phases:

### **1. Formation**

The Formation phase marks the initiation of the X Model. In this phase, the model identifies key components, including:

* **Sweeps**: Market movements that signal potential trend reversals or shifts.
* **CISD (Change In State of Delivery)**: Structural changes indicating a potential trend shift.

Once these components are identified, the model calculates and visualizes **Projections** and **Fair Value Gaps**, offering insights into potential future price movements and targets.

### **2. Pre-Invalidation**

A model enters the Pre-Invalidation phase when the body of the next candle closes above the sweep line, but the high that created the sweep remains intact. In such cases, the model is typically considered unreliable, as it suggests a likely failure.&#x20;

However, the high of the original sweep still holds importance, implying the model is close to being invalidated but not yet fully. In most cases, these models do not result in successful trades.

### **3. Invalidation**

The X Model is invalidated when the price fails to meet critical conditions, signaling that the initial setup is no longer reliable.&#x20;

Invalidation occurs under the following circumstances:

* The price fails to reach the **2 Standard Deviation** level.
* The price fails to reach the first identified **Fair Value Gap**.
* The price breaks above the high that initiated the **Sweep**.

Once invalidated, the original trade setup is no longer viable, and traders should refrain from executing the trade.

### **4. Success**

The X Model is considered successful when the price meets one of the following criteria:

* The price reaches the **2 Standard Deviation** level.
* The price reaches the first identified **Fair Value Gap**.

When success is achieved, the model's projections align with market movements, confirming the validity of the trade setup and providing a potential signal to execute the trade.

By understanding the phases of **Formation**, **Invalidation**, and **Success**, traders can effectively manage positions, minimize risk, and capitalize on high-probability setups identified by the X Model.

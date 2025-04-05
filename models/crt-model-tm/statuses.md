---
description: CRT Model Statuses
icon: battery-quarter
---

# Statuses

The CRT Model operates through a defined lifecycle that outlines its current state and determines whether a trade opportunity is valid.&#x20;

The lifecycle includes the following phases:

* **Formation**
* **Pre-Invalidation**
* **Invalidation**
* **Success**

### **1. Formation**

The Formation phase marks the initiation of the CRT Model. During this stage, the model identifies and plots critical components like:

* **Sweeps**: Market movements signaling potential trend reversals or shifts.
* **CISD (Change In State of Delivery)**: Structural changes that reveal potential trend shifts.

Once these components are detected, the model calculates and visualizes Projections and Liquidity Levels, providing insights into future price action.

### **2. Pre-Invalidation**

A CRT Model is considered pre-invalidated when the body of the subsequent candle closes above the sweep, yet the high that formed the sweep remains intact.&#x20;

In such cases, the model is typically deemed unreliable, as it suggests a potential failure in most instances.&#x20;

Despite this, the high from the original sweep continues to hold significance, indicating that the model has not yet been fully invalidated but is on the brink of doing so.&#x20;

Most of the time, these models do not result in successful outcomes.

### **3. Invalidation**

The CRT Model is considered invalid when the price fails to meet key conditions, signaling that the initial setup is no longer reliable.&#x20;

Invalidation occurs when:

* The price fails to reach the **2 Standard Deviation** level.
* The price fails to reach the **first identified liquidity** level.
* The price breaks above the high that initiated the Sweep.

When invalidated, the original trade setup is no longer valid, and traders should refrain from acting on it.

### **4. Success**

The CRT Model is deemed successful when the price meets one of the following criteria:

* The price reaches the **2 Standard Deviation** level.
* The price reaches the **first identified liquidity** level.

When success is achieved, the model's predictions align with market movements, confirming the validity of the trade setup and providing a potential signal to execute a trade.

By understanding the phases of **Formation**, **Invalidation**, and **Success**, traders can effectively manage their positions, reduce risk, and take advantage of high-probability setups that the CRT Model identifies.

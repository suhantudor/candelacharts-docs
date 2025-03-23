---
description: Fractal Range Model Framework
icon: diagram-venn
---

# Framework

The **Fractal Range Model** is an advanced trading framework that programmatically detects, visualizes, and invalidates key market concepts such as **Sweeps**, **CISD**, **Projections**, **Liquidity Levels**, **SMT Divergences**, **PD Arrays**, and more.&#x20;

Designed to streamline the trading process, this model integrates multiple components to offer a comprehensive view of the market, helping traders identify key entry and exit points.

## Lifecycle Statuses

The Fractal Range Model follows a specific lifecycle, which highlights the current state of the model and determines whether a trade opportunity is valid.&#x20;

The model's lifecycle includes the following statuses:

1. **Formation**
2. **Invalidation**
3. **Success**

### **1. Formation**

The **Formation** phase marks the initial setup of the Fractal Range Model.&#x20;

<figure><img src="../../.gitbook/assets/docs-frm-006.png" alt=""><figcaption></figcaption></figure>

During this stage, the model identifies and plots key components, such as:

* **Sweeps**: Market movements that indicate a potential reversal or strong shift in trend.
* **CISD (Change In State of Delivery)**: A structural change that provides insight into trend shifts.

Once these components are detected, the model automatically calculates and displays **Projections** and **Liquidity Levels**, offering insights into potential price action movements.

At this stage, the model also identifies and displays the following key elements, provided they are available:

* **HTF PD Arrays** (Higher-Timeframe Price Delivery Arrays)
* **LTF PD Arrays** (Lower-Timeframe Price Delivery Arrays)
* **SMT (Smart Money Technique)**

If any of these elements are present, they will be automatically displayed on the chart.

### **2. Invalidation**

A Fractal Range Model is considered **invalidated** when the price does not reach the **2 Standard Deviation** level or the first identified liquidity level, and when the price breaks above the high that formed the **Sweep**.&#x20;

<figure><img src="../../.gitbook/assets/docs-frm-005.png" alt=""><figcaption></figcaption></figure>

Invalidation signals that the original setup is no longer reliable, and traders should avoid taking action based on the model's original parameters.

**Key Invalidation Conditions**:

* Price fails to reach the **2 Standard Deviation** level.
* Price fails to reach the **first liquidity level**.
* Price breaks the **high/low** that initiated the **Sweep**.

### **3. Success**

A Fractal Range Model is considered **successful** when the price reaches the **2 Standard Deviation** level or the first identified liquidity level.&#x20;

<figure><img src="../../.gitbook/assets/docs-frm-003.png" alt=""><figcaption></figcaption></figure>

This indicates that the model's predictions align with actual market movements, confirming the setup's validity and providing a potential trading signal.

**Key Success Conditions**:

* Price reaches the **2 Standard Deviation** level.
* Price reaches the **first liquidity level**.

By leveraging these phases—**Formation**, **Invalidation**, and **Success**—traders can effectively manage their positions, minimize risk, and capitalize on high-probability setups based on the Fractal Range Model.

## **When to Enter a Trade**

After the **Fractal Range Model** has formed and key components like **Sweep** and **CISD** have been detected, traders can look for entry opportunities based on additional technical signals. The goal is to align the model's formation with other structural clues to optimize the timing of trade entries. Here's a breakdown of when to enter:

### **1. Entry Based on LTF PD Arrays**

Once the model is formed and **Sweep** and **CISD** have been established, the next step is to check for **Low-Timeframe (LTF) PD Arrays**. These arrays are key areas of liquidity or price structure that can give further confirmation for an entry.&#x20;

<figure><img src="../../.gitbook/assets/docs-frm-007.png" alt=""><figcaption></figcaption></figure>

If a **LTF PD Array** is present, traders can place their position in line with this array, as it serves as a strong zone of potential price reversal or continuation.

* **Action**: Look for LTF PD Arrays that align with the Fractal Range Model’s structure.
* **Entry**: If the array provides confluence, place the position near the array with a stop loss below the array zone.

### **2. Entry Using CISD**

If no **LTF PD Arrays** are present, the next best entry signal comes from the **CISD**. When the **CISD** aligns with the model's structure, it can serve as an entry point, signaling that the market is likely to follow the predicted path set by the Fractal Range Model.

* **Action**: Look for a **CISD** that aligns with the broader model and the price structure.
* **Entry**: Place a position near the **CISD** zone, ensuring that the stop loss is set appropriately based on the model's invalidation rules.

### **3. Missed Entries: First C-Area Level**

If a trader misses an entry at the **CISD** or **LTF PD Array**, the next opportunity for entry is at the **first C-Area level**. The **C-Area** represents a critical zone where price action is likely to consolidate, and traders should look for volume confirmation and a lack of divergences for a valid entry.

* **Action**: Wait for price to approach the **first C-Area** level, ensuring that there is consolidation and strong volume present.
* **Confirmation**: Confirm that there are no divergences (e.g., no bearish or bullish divergences that would contradict the price movement). This ensures that the price action is in alignment with the model’s projection.
* **Entry**: If the above conditions are met, place the entry with a stop loss at the end of the **C-Area** zone.

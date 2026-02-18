---
icon: arrows-left-right
---

# Support & Resistance

### Automated Level Detection <a href="#user-content--automated-level-detection" id="user-content--automated-level-detection"></a>

Drawing Support and Resistance (S/R) lines can be subjective and tedious. This tool automates the process by scanning historical price action to find "clusters" where price has reacted multiple times.

<figure><img src="../../.gitbook/assets/docs-ipa-041.png" alt=""><figcaption></figcaption></figure>

It doesn't just draw lines; it identifies **High-Probability Zones** where liquidity and orders are stacked.

### How It Works <a href="#user-content--how-it-works" id="user-content--how-it-works"></a>

1. **Scan**: The script looks back over a defined period (Loopback) to find every Pivot High and Pivot Low.
2. **Cluster**: It analyzes where these pivots stack up at the same price level.
3. **Qualify**: Only levels with a high density of touches are kept. Weak, random levels are filtered out.
4. **Visualize**: The strongest levels are drawn as horizontal zones extending to the right.

### Customization <a href="#user-content-customization" id="user-content-customization"></a>

#### 1. Loopback Period <a href="#user-content-1-loopback-period" id="user-content-1-loopback-period"></a>

* **Short**: Finds S/R levels based on recent price action (good for scalping).
* **Long**: Finds major historical S/R levels that have been respected for a long time (good for swing trading).

#### 2. Zone Attributes <a href="#user-content-2-zone-attributes" id="user-content-2-zone-attributes"></a>

* **Channel Width**: Controls the vertical thickness of the S/R zone.
  * _Tip_: Increase this slightly for volatile assets (like Crypto) to catch wicks.
* **Strength Threshold**: The filter for quality.
  * _Higher Value_: Shows fewer zones, but they are very significant.
  * _Lower Value_: Shows more zones, capturing minor supports.

#### 3. Visuals <a href="#user-content-3-visuals" id="user-content-3-visuals"></a>

* **Colors**: Resistance is Red, Support is Blue/Green (customizable).
* **Mean Line**: Draws a thin line through the center of the zone for precision entries.
* **Labels**: Displays the exact price level on the chart scale so you can set your alerts or limit orders easily.

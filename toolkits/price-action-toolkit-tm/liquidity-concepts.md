---
description: Liquidity Concepts settings
icon: window-minimize
---

# Liquidity

Price Action Toolkit™ encompasses a range of liquidity-related concepts, all accessible through the Liquidity Concepts settings section. Each concept is detailed in the sections below for your reference.

### Settings

<table><thead><tr><th>Name</th><th>Default</th><th>Options<select multiple><option value="FU3l9x4JLwvZ" label="Short Term" color="blue"></option><option value="UMXMzCc5q62R" label="Intermediate Term" color="blue"></option><option value="793RkGng9EhT" label="Long Term" color="blue"></option><option value="5VAOtACoZ4wA" label="Area" color="blue"></option><option value="BCpM6lZgl2a9" label="Line" color="blue"></option></select></th></tr></thead><tbody><tr><td>Show EQH/EQL</td><td>Short Term</td><td><span data-option="FU3l9x4JLwvZ">Short Term, </span><span data-option="UMXMzCc5q62R">Intermediate Term, </span><span data-option="793RkGng9EhT">Long Term</span></td></tr><tr><td>Buyside &#x26; Sellside</td><td>false</td><td><span data-option="5VAOtACoZ4wA">Area, </span><span data-option="BCpM6lZgl2a9">Line</span></td></tr><tr><td>Liquidity Sweeps</td><td>false</td><td></td></tr><tr><td>Liquidity Prints</td><td>false</td><td></td></tr></tbody></table>

### Equal Highs & Lows

The toolkit identifies historical equal highs and lows based on swing points. These equal highs and lows can signal potential reversals and upcoming market structures, such as Change of Character (CHoCH) or Break of Structure (BOS).

To view longer-term equal highs and lows, simply increase the numerical value next to the toggle (default is 3).

{% hint style="info" %}
Equal high’s & low’s requires the detected swing points to be confirmed, which takes an amount of bars equal to the value set in the numerical input. As such it is important to understand these are displayed retrospectively.
{% endhint %}

### Liquidity Prints

Liquidity Prints indicate areas where significant trading activity has occurred in more liquid zones, and are highlighted by the toolkit with distinct colored borders. These grabs can signal potential reversals:

* **Bullish Liquidity Prints**: Highlighted in blue, with borders extending from the price low to the minimum of the candle body. These grabs occur in demand areas and suggest a potential bullish reversal.
* **Bearish Liquidity Prints**: Highlighted in red, with borders extending from the price high to the maximum of the candle body. These grabs occur in supply areas and suggest a potential bearish reversal.

The simultaneous presence of both bullish and bearish liquidity grabs may signal market indecision.

### Liquidity Sweeps

A liquidity sweep is a price movement aimed at capturing liquidity before reversing direction. This typically involves:

* **Targeting Equal Highs**: The price may reach or exceed previous highs to tap into buy-side liquidity but fails to sustain the move, leading to a reversal.
* **Exceeding Highs**: If the price closes above the highs, it may quickly reverse, often accompanied by strong selling momentum.

In both scenarios, the liquidity sweep is designed to capture and exhaust liquidity before the price changes direction.

### Buyside & Sellside

Liquidity refers to the availability of orders at specific price levels that facilitate smooth transactions.

Liquidity often involves stop losses or pending orders, highlighting areas where buy or sell orders are concentrated. Smart money traders, like banks and institutions, target these liquidity pools to manage their positions.

There are two main types of liquidity:

* **Buyside Liquidity:** Levels where short sellers have their stop losses.
* **Sellside Liquidity:** Levels where long traders have their stop losses.

These liquidity pools often act as support or resistance and present trading opportunities.

{% hint style="info" %}
Built-in alerts for liquidity grabs are available to users within Smart Money Concept.
{% endhint %}

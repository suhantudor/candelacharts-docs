---
description: FVG Model Terminology
icon: spell-check
---

# Terminology

To fully utilize the FVG Model, it is essential to understand the core Smart Money Concepts (SMC) it detects and the terms used throughout the settings.

### Fair Value Gap (FVG)

An FVG represents an imbalance in price action, occurring when there is a rapid, explosive displacement in one direction. It is visually identified as a three-candle sequence where there is a literal "gap" between the wick of the first candle and the wick of the third candle. This gap signifies a lack of trading on the opposing side (inefficiency), and price often returns to these gaps to rebalance the market before continuing in the direction of the displacement.

### Consequent Encroachment (CE)

The exact midpoint (50%) of a Fair Value Gap. The CE line represents the equilibrium of the imbalance. Price retracing to or through the CE is considered a sign that the FVG is being partially filled. In this model, the CE line can be optionally displayed inside each mapped FVG.

### Liquidity Sweep (Raid)

A deceptive price movement where the market momentarily pierces a significant old high or low (a liquidity pool). The purpose of this move is to trigger stop-loss orders and trap breakout traders, engineering the necessary liquidity for major market participants to reverse the trend in the opposite direction.

### Change in State of Delivery (CISD)

A specific type of market structure confirmation. A CISD occurs when price transitions from delivering in one direction (e.g., aggressively selling) to delivering in the opposite direction. It is confirmed by a candle that closes beyond the body of the previous opposing candle, signaling a genuine shift in institutional intent.

### Market Structure Shift (MSS)

A broader structural confirmation where price breaks a recent swing high or swing low with a confirmed candle close, indicating that the prevailing trend has been broken. An MSS is typically more aggressive than a CISD and represents a more definitive change in market direction.

### Standard Deviation Projections

Mathematical projections used to estimate take-profit and stop-loss levels. The model calculates the distance between the anchor point (sweep candle wick or body) and the structural break, then projects this distance by a user-defined standard deviation multiplier to determine where price is statistically likely to reach.

### HTF (Higher Timeframe)

The larger timeframe (e.g., 1H, 4H, Daily) used by the indicator to source macro liquidity levels and Fair Value Gaps. The HTF provides the structural context that the model validates on the lower timeframe.

### LTF (Lower Timeframe)

Your execution timeframe (e.g., 1m, 5m, 15m). This is the chart timeframe where the model detects sweeps, market structure shifts, and draws the mapped FVG entry zones. It is where you would actually execute trades.

### HTF Candles

Visual reconstructions of the Higher Timeframe's candlesticks, drawn directly on the Lower Timeframe chart. These candles provide macro context — showing HTF open, high, low, and close — without requiring you to switch timeframes.

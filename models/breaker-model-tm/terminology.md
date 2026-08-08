---
description: Breaker Model Terminology
icon: spell-check
---

# Terminology

To fully utilize the Breaker Model, it is crucial to have a deep understanding of the core Smart Money Concepts (SMC) it detects and the terms used within the settings.

### Breaker Block

A Breaker Block originates as a standard Order Block that failed to hold its ground.

* **Bullish Breaker**: Price makes a lower low (sweeping sell-side liquidity) by pushing through a down-close candle. However, instead of continuing lower, price aggressively reverses and breaks market structure to the upside, closing above that same down-close candle. That original down-close candle is now a Bullish Breaker, acting as a high-probability support zone for future pullbacks.
* **Bearish Breaker**: Price makes a higher high (sweeping buy-side liquidity), pushing through an up-close candle. It then aggressively reverses and breaks structure to the downside. That up-close candle becomes a Bearish Breaker, acting as future resistance.

### Order Block (OB)

The last opposing candle before a strong impulse move that breaks market structure. While this indicator specifically tracks _failed_ order blocks (Breakers), understanding OBs is essential because every Breaker was once an OB.

### Liquidity Sweep (Raid)

A deceptive price movement where the market momentarily pierces a significant old high or low (a liquidity pool). The purpose of this move is to trigger stop-loss orders and trap breakout traders, engineering the necessary liquidity for major market participants to reverse the trend in the opposite direction.

### Fair Value Gap (FVG)

An FVG represents an imbalance in price action, occurring when there is a rapid, explosive displacement in one direction. It is visually identified as a three-candle sequence where there is a literal "gap" between the wick of the first candle and the wick of the third candle. This gap signifies a lack of trading on the opposing side (inefficiency), and price often returns to these gaps to rebalance the market before continuing the trend.

### Unicorn Setup

A rare, ultra-high-probability confluence pattern. It occurs when a newly formed Breaker Block perfectly aligns and overlaps with a newly formed Fair Value Gap (FVG) generated during the market structure shift. The overlapping area between the Breaker and the FVG creates the "Unicorn" entry zone, offering heavy institutional sponsorship.

### Projections (R:R Targets)

Risk-to-Reward (R:R) Projections are dynamic take-profit levels calculated based on your initial risk. `1R` equals the distance between your entry price and your invalidation point.

* **Fixed Projections**: Target lines that are plotted statically based on the original entry zone. They do not move, providing strict, predetermined exit liquidity levels.
* **Trailing Projections**: Dynamic target lines that recalculate and trail behind price as it moves in your favor, ideal for managing active trades and locking in profits.

### Invalidation Point

The precise price level at which the setup's structural logic is deemed to have failed, serving as your hard stop-loss. In the Breaker Model, you can toggle between using the absolute wick extreme of the initial liquidity sweep (safer, wider stop) or the opposite edge of the Breaker Block (tighter stop, higher R:R).

### HTF (Higher Timeframe)

Refers to the larger timeframes (e.g., 1H, 4H, Daily) used by the indicator's engine to source major liquidity pools. The model uses this HTF structural context to validate lower timeframe (LTF) execution patterns, ensuring you are trading in alignment with macro order flow.

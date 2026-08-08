---
description: Breaker Model Features
icon: alien-8bit
---

# Features

The CandelaCharts Breaker Model comes packed with advanced functionalities tailored for precision trading and risk management.

* **Automated Liquidity Tracking**: Automatically sources Higher Timeframe (HTF) liquidity levels (OHLC or Swings) across up to 4 different timeframes (e.g., 15m, 1H, 4H, Daily).
* **Unicorn Mode**: A strict confluence filter that only displays Breaker Blocks that perfectly align with a newly formed Fair Value Gap (FVG).
* **Customizable Invalidation**: Choose whether your stop-loss/invalidation point should be the absolute extreme of the liquidity sweep, or simply the opposite edge of the Breaker Block.
* **Dynamic R:R Projections**: Input your desired Risk-to-Reward targets (e.g., `1, 2, 2.5`), and the indicator will automatically plot projection lines based on your entry and invalidation points.
* **Position Sizing Calculator**: Input your account balance and risk parameters (Percentage or Fixed Amount), and the dashboard will output the exact position size for the current setup.
* **Time and Size Filters**: Restrict setups to specific trading sessions (e.g., NY AM Session) and filter out Breakers that are too large or too small based on ATR, Points, or Ticks.
* **Directional Bias Filtering**: Choose whether to display all setups (Neutral) or restrict the indicator to strictly trace only Bullish or Bearish Breakers based on your higher timeframe bias.
* **Historical Tracking**: Control exactly how many historical setups remain visible on the chart at one time. Set it to '1' for a completely clean chart focused on the present, or increase it for visual backtesting.
* **Trade Lifecycle Tracking**: Visually track a setup from "Potential" to "Confirmed", all the way to "Target Hit" or "Invalidated", with customizable colors for active vs. inactive states.
* **Discard Invalidated**: Keep your charts clutter-free by toggling the option to automatically delete setups that breach their stop-loss point.

---
description: FVG Model Timeframe Alignment
icon: chess-clock-flip
---

# Timeframe Alignment

The FVG Model relies on a precise relationship between your execution timeframe (LTF) and a macro context timeframe (HTF). This pairing determines which candles are drawn as HTF context and where the model sources its liquidity pools.

### Automatic Mode

When set to **Automatic**, the indicator detects your current chart timeframe and automatically selects the optimal HTF pairing from its internal mapping. This is the recommended mode for most traders — it ensures the ratio between LTF and HTF is always appropriate for reliable model detection.

| Chart Timeframe | Paired HTF |
| --------------- | ---------- |
| 15s             | 5m         |
| 1m              | 15m        |
| 2m              | 20m        |
| 3m              | 30m        |
| 5m              | 1H         |
| 15m             | 4H         |
| 30m             | 12H        |
| 1H              | 1D         |
| 2H              | 2D         |
| 3H              | 3D         |
| 4H              | 1W         |
| 8H              | 2W         |
| 12H             | 3W         |
| 1D              | 1M         |
| 2D              | 2M         |
| 3D              | 1M         |
| 1W              | 3M         |
| 2W              | 6M         |
| 3W              | 9M         |
| 1M              | 12M        |

### Preset Pairings

For more control, you can manually select from 25+ preset LTF/HTF combinations directly from the dropdown.

| LTF | HTF |
| --- | --- |
| 15s | 5m  |
| 1m  | 15m |
| 1m  | 30m |
| 2m  | 20m |
| 3m  | 30m |
| 3m  | 1H  |
| 5m  | 1H  |
| 15m | 4H  |
| 15m | 8H  |
| 30m | 9H  |
| 30m | 12H |
| 1H  | 1D  |
| 2H  | 2D  |
| 3H  | 3D  |
| 4H  | 1W  |
| 8H  | 2W  |
| 12H | 3W  |
| 1D  | 1M  |
| 2D  | 1M  |
| 2D  | 2M  |
| 3D  | 1M  |
| 3D  | 3M  |
| 1W  | 3M  |
| 2W  | 6M  |
| 3W  | 9M  |
| 1M  | 12M |

### Custom Mode

When set to **Custom**, two timeframe input fields become active, allowing you to define your own LTF and HTF pair with full flexibility. Use this when you want to test unconventional pairings or when your chart timeframe does not appear in the preset list.

### Length Filter

The **Length** setting controls the maximum allowed distance (in HTF candles) between the FVG and the Sweep that triggers the model. If the FVG and the sweep are too far apart, the setup may lack confluence. Setting this to `5` means the sweep must occur within 5 HTF candles of the FVG. You can uncheck this filter to allow any distance.

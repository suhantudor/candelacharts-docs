---
description: FVG Model Components
icon: diamonds-4
---

# Components

The FVG Model is built from several interconnected visual and analytical components that work together to identify, confirm, and manage trade setups.

### HTF Candles

The foundation of the model's multi-timeframe capability. HTF candles are reconstructed and drawn directly on your LTF chart, providing macro structural context.

* **HTF I**: The primary HTF candle layer. You control how many candles are displayed (up to 20).
* **HTF II**: An optional secondary HTF candle layer from an independent timeframe (e.g., Daily candles on a 5m chart that already shows 1H as HTF I), giving you two layers of macro context simultaneously.
* **Labels**: Toggle and customize the labels displayed on HTF candles, including text size and color.
* **Offset**: Controls the horizontal distance (in bars) between the HTF candle drawing and your live chart.
* **Space**: Adjusts the spacing between individual HTF candle bodies.
* **Margin**: Controls the gap between the HTF candle section and the main chart area.
* **Size**: Sets the visual width of the HTF candle bodies (Tiny, Small, Medium, Large, Huge).
* **Coloring**: Fully customizable bull, bear, and wick/border colors.

### Fair Value Gaps

Once a model is confirmed, the HTF Fair Value Gap is mapped onto the LTF chart as a colored box representing the imbalance zone.

* **Map to LTF**: Toggle that controls whether HTF FVGs are projected onto the lower timeframe chart.
* **CE Line**: Optionally display the Consequent Encroachment (midpoint) line inside each FVG, with customizable style (solid, dashed, dotted) and width.
* **Border**: Optionally show a border around the FVG box with configurable line style and width.
* **Coloring**: Independent bull and bear FVG colors with adjustable transparency.

### Sweeps

Visual indicators of where HTF liquidity was raided. The sweep component draws lines marking the exact price levels that were taken out.

* **Sweeps**: Toggle visibility and customize the line style (solid, dashed, dotted), width, and separate bull/bear colors.
* **Invalidated Sweeps**: Optionally display sweeps that were later invalidated, with their own distinct style and color (typically gray/dashed) so you can distinguish between active and dead sweeps.

### Market Structure

The structural confirmation layer that validates the sweep. This component draws the CISD or MSS break line on your chart.

* **Type**: Choose between CISD (Change in State of Delivery) or MSS (Market Structure Shift) as the required structural confirmation method.
* **Line Style**: Customize the style (solid, dashed, dotted) and width of the market structure break line.
* **Coloring**: Independent bull and bear colors for the structure break lines.

### LTF Open/Close Lines

Optional horizontal lines drawn at the Open and Close prices of HTF candles on the LTF chart, providing additional structural reference levels.

* **O/C Line**: Toggle visibility with customizable line style, width, and color.

### Standard Deviations (Projections)

The trade management component. Once a model is confirmed, standard deviation projections are calculated and drawn as take-profit and stop-loss zones.

* **Anchor**: Choose whether projections are measured from the sweep candle's Wick (wider range, conservative) or Body (tighter range, aggressive).
* **Take Profit Level**: Set the standard deviation multiplier for the take-profit target (e.g., `-2.5`). The negative value projects in the direction of the trade.
* **Show TP Labels**: Toggle visibility of labels on the take-profit projection lines.
* **Coloring**: Separate colors for bullish take-profit, bearish take-profit, and stop-loss zones.

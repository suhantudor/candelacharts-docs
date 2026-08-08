---
icon: objects-column
---

# Stacked Imbalances

Stacked Imbalances are powerful visual confirmations of aggressive institutional participation. They occur when market participants execute large market orders in a single direction, overwhelming the limit orders and leaving behind a "stack" of consecutive price levels with one-sided volume.

When the toolkit detects a stacked imbalance, it highlights the zone on your chart, providing a clear visual representation of aggressive buying or selling pressure. These zones often act as strong support or resistance on subsequent retracements.

### Configuration

* **Show Stacked Imbalances**: Master toggle to enable or disable the highlighting of stacked imbalance zones.
* **Threshold %**: This setting defines how aggressive the volume must be to qualify as an imbalance. For example, a threshold of `300%` means the buying volume at a specific price level must be at least 3x (300%) greater than the selling volume (or vice versa) to be flagged as an imbalance.
* **Min Levels**: Defines how many consecutive imbalanced price levels must stack on top of each other to draw the zone. The default is `3`, meaning you need at least three back-to-multi-level imbalances in a row to confirm strong directional conviction. A lower number (e.g., 2) will show more zones but with less conviction, while a higher number (e.g., 4 or 5) will only highlight extreme momentum.

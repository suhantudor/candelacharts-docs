---
description: FVG Model Filters
icon: filter
---

# Filters

The FVG Model provides session-based time filters to restrict model detection to specific institutional trading windows. Unlike size-based filters, the FVG Model focuses on temporal precision — ensuring setups only form during the hours that historically produce the highest probability moves.

### Session Filters

Each session can be independently enabled or disabled, and their time windows are fully customizable:

* **Asia**: Covers the Asian session (default `2000-0000`). Useful for identifying setups during the quieter, accumulation-heavy Asian hours.
* **London**: Covers the London open and pre-NY overlap (default `0200-0500`). This is when European institutional flow begins and often produces the first major displacement of the day.
* **NY AM**: Covers the New York AM session (default `0930-1100`). This is the most volatile window of the day, where NYSE and CME open and major liquidity events occur.
* **NY LA (NY Launch)**: Covers the New York Launch window (default `1200-1300`). A transitional period where the London close overlaps with NY afternoon flow.
* **NY PM**: Covers the New York PM session (default `1330-1600`). The afternoon session where reversals, continuations, and end-of-day positioning often take place.
* **Custom**: A fully user-defined session window (default `0000-0001`). Use this for any non-standard trading hours, overnight scalping sessions, or crypto-specific time windows.

When one or more sessions are enabled, the indicator will strictly ignore any model formations that occur outside of the defined windows. If no session filters are enabled, all models across the entire trading day are considered valid.

{% hint style="info" %}
Session filters are only available when the paired LTF is 1H or below. On higher timeframes, individual bars span multiple sessions, making session-based filtering impractical.
{% endhint %}

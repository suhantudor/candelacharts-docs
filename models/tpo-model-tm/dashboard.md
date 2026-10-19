---
description: TPO Model Dashboard
icon: game-board-simple
---

# Dashboard

The dashboard is a compact four-row heads-up display anchored to your chart. Its job is to provide real-time situational awareness at a glance, answering two questions without cluttering your screen:

1. _How is price interacting with fair value right now?_
2. _Which way is the auction bias leaning?_

### Row 1 — Model Pairing

Row 1 shows the active profile timeframe and paired higher timeframe.

* If you use a preset like `1D - 1H`, it displays `1D - 1H Model`.
* If you use a custom pairing, it shows the resolved intervals (for example, `Custom Model (D - 60)`).

**Practical Use**: This acts as a sanity check before executing trades. If you sit down expecting to trade an intraday daily profile but the dashboard reads `1W - 4H Model`, your timeframe alignment is mismatched before you enter a position.

### Row 2 — Remaining Time

Row 2 displays a live, tick-by-tick countdown tracking the time left before the current profile session closes.

* Formatted as `HH:MM:SS` (or `Xd HH:MM:SS` for multi-day profiles).
* Reaches `00:00:00` at the session boundary, at which point the current session finalizes, resting levels become historical references, and a fresh profile begins building.

**Practical Use**: Prevents the common mistake of initiating new trades right before session settlement, when historical value boundaries freeze and session-reset volatility can produce unexpected whipsaws.

### Row 3 — Value Area Event

The Event row is an automated state classifier. It tracks intrabar price action to determine how price is interacting with the **previous session's Value Area**:

* **Accepted Above VAH** — Price broke above the previous Value Area High and printed two or more consecutive intrabar closes above it. This confirms bullish range expansion and upward price discovery.
* **Accepted Below VAL** — Price broke below the previous Value Area Low and printed two or more consecutive intrabar closes below it. This confirms bearish range expansion and downward price discovery.
* **Testing VAH / Testing VAL** — Price has probed beyond a boundary, but has not yet printed two consecutive closes outside. The auction is probing for liquidity; acceptance or rejection is not yet decided.
* **Rejected VAH (In VA)** — Price traded above VAH, encountered responsive sellers, and closed back inside the Value Area. This marks a failed breakout and initiates the classic 80% Rule setup toward the POC and VAL.
* **Rejected VAL (In VA)** — Price traded below VAL, encountered responsive buyers, and closed back inside. This marks a failed breakdown toward the POC and VAH.
* **Rejected Both (In VA)** — A two-sided failed auction. Both the high and low boundaries were probed and rejected, leaving price back inside the value band.
* **Inside VA** — Price is rotating comfortably within the previous session's boundaries. The label indicates whether price is currently trading above or below the previous POC (for example, `Inside VA (Bullish)` or `Inside VA (Bearish)`).
* **Pending** — Early in a new session when not enough intrabar data has accumulated to classify an interaction.

{% hint style="info" %}
**Why two closes matter**: A single wick beyond VAH or VAL is not acceptance. The model requires two consecutive intrabar closes beyond the boundary to prevent false breakout whipsaws.
{% endhint %}

### Row 4 — Directional Bias

Row 4 translates auction interaction into an objective directional score. It is not a lagging oscillator or moving average; it is a deterministic calculation that evaluates price position against both the previous session and the developing session.

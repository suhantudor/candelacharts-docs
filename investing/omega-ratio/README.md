---
icon: omega
---

# Omega Ratio

Quality of returns compounds; the **Omega Ratio** tells you whether gains above your hurdle outpace misses below it.

Instead of averaging returns or assuming a normal distribution, Omega evaluates the _entire return distribution_ relative to a user-defined **target return per bar**. For each bar, it counts how much you beat the target (**excess gains**) and how much you fell short (**shortfalls**). Over a rolling window, **Omega = Σ(excess gains) / Σ(shortfalls)**.

* **Intuition:** An Omega of **1.0** means gains above your hurdle roughly match the losses below it (breakeven quality). **> 1.5** suggests favorable conditions; **> 2.0** signals strong quality. **< 1.0** means setbacks dominate.
* **Why Omega vs. Sharpe/Sortino?** Omega uses _all_ moments of the distribution around a **user-chosen threshold** (not just mean and variance), making it robust when returns are skewed or heavy-tailed—and directly aligned to your objective (e.g., “beat 0.05% per bar”).
* **Target choice matters:** On Daily charts, typical per-bar targets range from **0.00% to 0.10%**; intraday usually needs smaller targets. Higher targets demand more edge and will reduce Omega; lower targets do the opposite.
* **Log vs. linear:** Choose **log returns** for large moves/cross-asset comparability; **linear** is fine for small, steady bars.\
  Use Omega as a **quality gate**: require Omega > 1 (or > 1.5) before deploying capital, then layer your usual entries/exits.


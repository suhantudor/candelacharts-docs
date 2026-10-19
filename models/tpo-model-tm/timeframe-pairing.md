---
description: TPO Model Timeframe Alignment
icon: chess-clock-flip
---

# Timeframe Alignment

The model runs on two clocks:

* The **profile clock** decides how much price action makes up one session, its Value Area, and its POC.
* The **HTF clock** decides which candles are projected into the right margin and which timeframe supplies sweeps and CISD detection.

`Model Pairing` sets both at once.

### Model pairing presets

| Preset     | Profile (session) timeframe     | HTF overlay       | Typical use                                        |
| ---------- | ------------------------------- | ----------------- | -------------------------------------------------- |
| `Auto`     | Chosen from the chart timeframe | Chosen with it    | First look; adapts on load                         |
| `1D - 1H`  | 1 day                           | 1 hour            | Intraday execution inside a daily profile          |
| `1D - 4H`  | 1 day                           | 4 hours           | Intraday with a slower execution clock             |
| `1D - 6H`  | 1 day                           | 6 hours           | Intraday with two to three HTF candles per session |
| `3D - 4H`  | 3 days                          | 4 hours           | Multi-day swing context                            |
| `3D - 6H`  | 3 days                          | 6 hours           | Multi-day swing context                            |
| `3D - 12H` | 3 days                          | 12 hours          | Multi-day with two HTF candles per session         |
| `1W - 4H`  | 1 week                          | 4 hours           | Weekly profile, intraday execution                 |
| `1W - 6H`  | 1 week                          | 6 hours           | Weekly profile, intraday execution                 |
| `1W - 12H` | 1 week                          | 12 hours          | Weekly profile with two HTF candles per day        |
| `1W - 1D`  | 1 week                          | 1 day             | Weekly profile, daily execution                    |
| `1M - 1D`  | 1 month                         | 1 day             | Monthly profile, daily execution                   |
| `12M - 1W` | 1 year                          | 1 week            | Annual profile, weekly execution                   |
| `12M - 1M` | 1 year                          | 1 month           | Annual profile, monthly execution                  |
| `12M - 3M` | 1 year                          | 3 months          | Annual profile, quarterly execution                |
| `Custom`   | Your `Custom TPO TF`            | Your `Custom HTF` | Any pairing the presets do not cover               |

### Auto mapping

`Auto` reads the chart timeframe when the script loads:

| Chart timeframe                   | Selected pairing        |
| --------------------------------- | ----------------------- |
| 1–5 minutes                       | `1D - 1H`               |
| 6–15 minutes                      | `1D - 4H`               |
| 16–30 minutes                     | `3D - 6H`               |
| 31–60 minutes                     | `1W - 12H`              |
| 61–240 minutes                    | `1M - 1D`               |
| Daily                             | `12M - 1W`              |
| Weekly, monthly, or anything else | Falls back to `1D - 1H` |

{% hint style="info" %}
`Auto` can select a profile timeframe far above the chart timeframe. That is intentional: you may execute on a 1-hour chart while profiling the week. It also means the chart timeframe does not have to equal the session timeframe.
{% endhint %}

### Custom pairing

Select `Custom` to expose:

| Input           | Default | Meaning                                                      |
| --------------- | ------- | ------------------------------------------------------------ |
| `Custom TPO TF` | `D`     | Session timeframe used for both profiles                     |
| `Custom HTF`    | `60`    | Timeframe for the primary HTF candle group, sweeps, and CISD |

The two are independent. For example, a `12H` profile with a `1H` HTF is valid, as is a `W` profile with a `D` HTF.

### Alignment constraints

| Constraint                            | Behaviour                                                                                     |
| ------------------------------------- | --------------------------------------------------------------------------------------------- |
| Intrabar Resolution ≥ chart timeframe | Runtime error; the script stops and explains the requirement                                  |
| 1-minute chart                        | Needs a seconds resolution (where supported); otherwise no lower timeframe exists             |
| HTF lower than chart timeframe        | Not blocked, but produces misleading projection; keep the HTF at or above the chart timeframe |
| Insufficient intrabar history         | Session labelled `TPO (partial)` / `Volume (partial)`                                         |
| Too many HTF groups or candles        | Drawing objects may be truncated by TradingView limits                                        |
| Forex symbols                         | Volume is tick volume; a notice is displayed                                                  |

### Choosing a pairing

| If you…                       | Start with                                         |
| ----------------------------- | -------------------------------------------------- |
| Scalp intraday index futures  | `1D - 1H` or `1D - 4H`                             |
| Day trade with a session bias | `1D - 1H`, History 3–5                             |
| Swing trade over days         | `1W - 4H` or `1W - 1D`                             |
| Analyse macro value           | `1M - 1D` or `12M - 1W`                            |
| Want a clean chart            | One profile, paired HTF only, extra HTF groups off |

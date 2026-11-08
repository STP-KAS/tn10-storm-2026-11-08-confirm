> **Experimental. We are just trying this.** [Disclaimer](DISCLAIMER.md) · Kaspa Testnet-10 only; tKAS has no value. **This is a plan, not a run. No date is set.** Mainnet: **not tested (label B)**.
>
> **Part of [tn-master](https://github.com/STP-KAS/tn-master)**, the map of every TN10 storm. Named by the [11 Oct naming rule](https://github.com/STP-KAS/tn-master/blob/main/repos/INDEX.md): a plan stays `tn10-storm-plan-*` until the day is chosen, then it is renamed to `tn10-storm-YYYY-MM-DD`.

# tn10-storm-plan-confirm

**History of every storm: [MASTER.md](https://github.com/STP-KAS/tn-master/blob/main/history/MASTER.md)** (in tn-master).

**Previous storm:** [tn10-storm-2026-11-08](https://github.com/STP-KAS/tn10-storm-2026-11-08). That repo is the rehearsal. It stands on its own. This plan does not move that clock.

**The date is blank.** Pulse chooses the day. Until both pastes contain that same calendar day, and this repo has been renamed, a read of either paste does not start a runner.

## The two pastes

One story. One file for each computer. Paste the file that names the machine in front of you. The first sentence must be that machine. If it names the other one, stop and paste the other file.

| Machine | Paste | First sentence |
|---|---|---|
| **desk** | [GO-DESK.md](GO-DESK.md) | DESK. I send and I count. |
| **Mini** | [GO-MINI.md](GO-MINI.md) | MINI. I count. I do not send. |

Each file is the whole plan. Grok Build does not guess the machine from its own name. The pasted file is the machine. [GO.md](GO.md) is the map. It does not start a session. Bot may read either file. Bot watches and does not send. The run does not wait for bot.

## Clock, once the day exists

Times are UTC first, on the chosen day. Desk local is CET (UTC+1). The offsets are the 8 Nov rehearsal.

| | UTC | CET |
|---|---|---|
| Both machines have read their paste | **00:20** | **01:20** |
| Genesis, eight families | 00:35 | 01:35 |
| Counts on | 00:38 | 01:38 |
| **START (T0)** | **00:40** | **01:40** |
| First sends finished | 02:10 | 03:10 |
| First count off | 02:40 | 03:40 |
| 32-family load | 02:55–03:40 | 03:55–04:40 |
| Load count off | 03:55 | 04:55 |
| Sixteen families, if the earlier part finished clean | **04:15–04:30** | **05:15–05:30** |
| Sixteen-family count off | 04:45 | 05:45 |

The steps are in [plan/PLAN.md](plan/PLAN.md). The same clock is in both pastes.

## What and why

**What.** One desk sender. The same shape as the 8 Nov rehearsal. Steps of 15 minutes at 1 family, then 2, then 4, then 8 if 4 held the line, with 5-minute gaps. Then a 10-minute ramp. Offer 1.2 hop/s per family. Line 1.14, which is 1,026 hops per family over 900 seconds. Then one 32-family load, 45 minutes, same offer. Then one 16-family step, 15 minutes, same offer. The desk sends and counts, and the desk runner publishes [counts/desk/](counts/desk/README.md). Mini counts, and Mini's runner publishes [counts/mini/](counts/mini/README.md). Each hash file records the time the rows reached GitHub. Bot watches. Miners stay off.

**Why.** The 8 Nov desk procedure finished on its clock. The missing piece of the standard was the publish: Mini's paste had told him not to commit, and the desk runner never wrote a count file of its own. Both of those are now in the 8 Nov pastes, and Mini's three files are on that repo. This plan runs the same measurement again so both publishers fire on a live clock, and so the hash file shows the origin time in the same night. The full why is [WHY.md](WHY.md).

**Already measured, and not folded into this clock.** The other drafts are listed in [plan/LATER.md](plan/LATER.md). They stay their own nights. Mixing them into this clock would change the measurement.

## Map

| Path | What is in it |
|---|---|
| [BENCHMARK.md](BENCHMARK.md) | What this plan copies from the 8 Nov pattern |
| [DISCLAIMER.md](DISCLAIMER.md) | Experimental. Certainty labels A / B / C |
| [WHY.md](WHY.md) | Why this confirmation, and what it does not test |
| [GO.md](GO.md) | Map of the two pastes. Does not start a machine |
| [GO-DESK.md](GO-DESK.md) | Desk paste. The whole story. Desk sends and counts |
| [GO-MINI.md](GO-MINI.md) | Mini paste. The same story. Mini counts |
| [go/README.md](go/README.md) | Which paste goes on which computer |
| [plan/PLAN.md](plan/PLAN.md) | The shape, the offsets, the funding rule |
| [plan/COUNT.md](plan/COUNT.md) | How a hop is counted, and where each file is published |
| [plan/SIXTEEN.md](plan/SIXTEEN.md) | Why sixteen families are in this confirmation |
| [plan/LATER.md](plan/LATER.md) | Drafts that were checked and left for another night |
| [hashes/README.md](hashes/README.md) | Three hash files. Absent until the desk runner writes them |
| [counts/desk/README.md](counts/desk/README.md) | The desk's three count files |
| [counts/mini/README.md](counts/mini/README.md) | Mini's three count files |
| [logs/README.md](logs/README.md) | Where the method log will land after the run |

## Results

None. The day is not chosen. A number from the 8 Nov rehearsal stays in that repo. It is one desk reading.

Counts only. No key, seed, txid, covenant id, address, host or port in this repo.

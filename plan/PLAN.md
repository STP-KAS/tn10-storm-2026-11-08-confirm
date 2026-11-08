> **Experimental. We are just trying this.** [Disclaimer](../DISCLAIMER.md) · This page does not start a machine.

# Plan

The day is **Sun 8 Nov 2026**. The shape is the 8 Nov 2026 rehearsal. T0 is 12:00 UTC. Both pastes carry this clock. This is a new run. The repo name is `tn10-storm-2026-11-08-confirm`, because the rehearsal already holds `tn10-storm-2026-11-08`. The standing rule is [RULES.md](../RULES.md).

## Shape

One sender. The desk. Offer 1.2 hop/s per family. Boson. Stagger 0. No phase offset.

| UTC | What | How long |
|---|---|---|
| 12:00–12:15 | 1 family | 15 min |
| 12:20–12:35 | 2 families | 15 min |
| 12:40–12:55 | 4 families | 15 min |
| 13:00–13:15 | 8 families, only if 4 held 1.14 | 15 min |
| 13:20–13:30 | Ramp, 50 s on / 10 s off, +0.1 from 1.2 toward 2.1 | 10 min |
| 14:15–15:00 | 32 families, offer 1.2 | 45 min |
| 15:35–15:50 | 16 families, offer 1.2, only if the earlier part finished clean | 15 min |

If 4 does not hold the line, skip 8 and start the ramp at 13:00 UTC. The load stays at 14:15. Sixteen stays at 15:35.

The early ramp may share the 8-family clock. It runs only when 4 does not hold the line. The gate writes the SKIP file in the five-minute gap, after the step that decides and before the next step opens. The later ramp runs only when the 8-family step runs. Do not add a third row on a clock that is already taken.

The ramp stops when two gains in a row are under 3%. The test uses the unrounded gain. A printed 3.0 can still be under 3%.

## Counts

Both machines count the same three windows and each publishes its own folder.

| File | On | Off | Desk | Mini |
|---|---|---|---|---|
| FIRST.md | 11:58 | 14:00 | counts/desk/ | counts/mini/ |
| LOAD.md | 14:13 | 15:15 | counts/desk/ | counts/mini/ |
| SIXTEEN.md | 15:33 | 16:05 | counts/desk/ | counts/mini/ |

The rule is [COUNT.md](COUNT.md).

## Hashes

| File | Before |
|---|---|
| hashes/EIGHT.md | 12:00 |
| hashes/THIRTYTWO.md | 14:15 |
| hashes/SIXTEEN.md | 15:35, and after the load has spent its funding coins |

Each file gets an On origin time from the commit that put the rows on GitHub. The rule is [hashes/README.md](../hashes/README.md). No proved file, no send.

## Funding

Before the first genesis, every key the night will use has one eligible coin per genesis that night. The eight-family genesis uses one coin. The load uses a second. A key that has only those two coins is not used for the sixteen-family genesis. Sixteen hashes are published after the load, so the published row and the later genesis name the same remaining coin. Do not spend a mining coin at or above 100,000 tKAS. Do not print a balance, a key, or an id.

## Abort

2,500 coins and 18,000 usable tKAS, checked before genesis and again before 43a. Fee stays where the counted windows left it. A fee reject stops that part. Faults: sender-off, pool-low, node-drop, proc-exit. A start of 43a after 17:20 UTC does not happen.

One process on the desk chains the eight-family window, then the load, then sixteen. A later phase starts only if the earlier phase log ended on the window, with no launch abort and no family drop. The quiet load gate is not swapped in while the eight-family process is still running.

## What this plan does not change

The 8 Nov repo stays the rehearsal. This plan does not edit that clock and does not start a sender for it. 43b is [LATER.md](LATER.md).

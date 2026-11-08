> **Experimental. We are just trying this.** [Disclaimer](../DISCLAIMER.md) · This page does not start a machine. The date is blank.

# Plan

The day is **DATE**. The offsets are the 8 Nov 2026 rehearsal. T0 is 00:40 UTC on the chosen day. Both pastes carry this clock. A runner starts only after DATE has been replaced by that day in both pastes, and the repo has been renamed to `tn10-storm-YYYY-MM-DD`.

## Shape

One sender. The desk. Offer 1.2 hop/s per family. Boson. Stagger 0. No phase offset.

| UTC | What | How long |
|---|---|---|
| 00:40–00:55 | 1 family | 15 min |
| 01:00–01:15 | 2 families | 15 min |
| 01:20–01:35 | 4 families | 15 min |
| 01:40–01:55 | 8 families, only if 4 held 1.14 | 15 min |
| 02:00–02:10 | Ramp, 50 s on / 10 s off, +0.1 from 1.2 toward 2.1 | 10 min |
| 02:55–03:40 | 32 families, offer 1.2 | 45 min |
| 04:15–04:30 | 16 families, offer 1.2, only if the earlier part finished clean | 15 min |

If 4 does not hold the line, skip 8 and start the ramp at 01:40 UTC. The load stays at 02:55. Sixteen stays at 04:15.

The early ramp may share the 8-family clock. It runs only when 4 does not hold the line. The gate writes the SKIP file in the five-minute gap, after the step that decides and before the next step opens. The later ramp runs only when the 8-family step runs. Do not add a third row on a clock that is already taken.

The ramp stops when two gains in a row are under 3%. The test uses the unrounded gain. A printed 3.0 can still be under 3%.

## Counts

Both machines count the same three windows and each publishes its own folder.

| File | On | Off | Desk | Mini |
|---|---|---|---|---|
| FIRST.md | 00:38 | 02:40 | counts/desk/ | counts/mini/ |
| LOAD.md | 02:53 | 03:55 | counts/desk/ | counts/mini/ |
| SIXTEEN.md | 04:13 | 04:45 | counts/desk/ | counts/mini/ |

The rule is [COUNT.md](COUNT.md).

## Hashes

| File | Before |
|---|---|
| hashes/EIGHT.md | 00:40 |
| hashes/THIRTYTWO.md | 02:55 |
| hashes/SIXTEEN.md | 04:15, and after the load has spent its funding coins |

Each file gets an On origin time from the commit that put the rows on GitHub. The rule is [hashes/README.md](../hashes/README.md). No proved file, no send.

## Funding

Before the first genesis, every key the night will use has one eligible coin per genesis that night. The eight-family genesis uses one coin. The load uses a second. A key that has only those two coins is not used for the sixteen-family genesis. Sixteen hashes are published after the load, so the published row and the later genesis name the same remaining coin. Do not spend a mining coin at or above 100,000 tKAS. Do not print a balance, a key, or an id.

## Abort

2,500 coins and 18,000 usable tKAS, checked before genesis and again before 43a. Fee stays where the counted windows left it. A fee reject stops that part. Faults: sender-off, pool-low, node-drop, proc-exit. A start of 43a after 06:00 UTC does not happen.

One process on the desk chains the eight-family window, then the load, then sixteen. A later phase starts only if the earlier phase log ended on the window, with no launch abort and no family drop. The quiet load gate is not swapped in while the eight-family process is still running.

## What this plan does not change

The 8 Nov repo stays the rehearsal. This plan does not edit that clock and does not start a sender for it. 43b is [LATER.md](LATER.md).

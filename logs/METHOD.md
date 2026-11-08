> **Experimental. We are just trying this.** [Disclaimer](../DISCLAIMER.md) · [tn-master](https://github.com/STP-KAS/tn-master) · One desk reading and one Mini reading. Not averaged. Not Kaspa Pulse's count.

# Method, 8 Nov 2026 confirmation

Sun 8 Nov 2026. Start 12:00 UTC (13:00 CET). Same shape as the 8 Nov 00:40 rehearsal. The 10:40 waiter was stopped before its hash. This clock replaced it. Desk sends and counts. Mini counts. One process on the desk, from the 11:47 restart through `NIGHT_DONE` at 16:10:08 UTC. Exits 0.

The eight-hash rows reached the repo at 11:45. The proof line failed to push, and the runner stopped. The publish was fixed and the same clock started again at 11:47, before the 11:53 cutoff. The proof that stands is the second one.

## Hashes

| File | On origin | Commit |
|---|---|---|
| [hashes/EIGHT.md](../hashes/EIGHT.md) | 2026-11-08T11:47:03Z | `43010f8` |
| [hashes/THIRTYTWO.md](../hashes/THIRTYTWO.md) | 2026-11-08T13:32:09Z | `412aba3` |
| [hashes/SIXTEEN.md](../hashes/SIXTEEN.md) | 2026-11-08T15:20:11Z | `6ae79c9` |

## Desk

Header time. Every minute was read in full. No family drop. Each phase ended `reason=window`.

| File | Counter | Accepted hops | On origin |
|---|---|---|---|
| [counts/desk/FIRST.md](../counts/desk/FIRST.md) | 11:58–14:00 | 20,156 | 2026-11-08T14:00:01Z, `39307a1` |
| [counts/desk/LOAD.md](../counts/desk/LOAD.md) | 14:13–15:15 | 96,217 | 2026-11-08T15:20:06Z, `3044e7c` |
| [counts/desk/SIXTEEN.md](../counts/desk/SIXTEEN.md) | 15:33–16:05 | 17,777 | 2026-11-08T16:10:05Z, `1ad569c` |

The early ramp was skipped, so the eight-family step ran. The later ramp stopped after r6, when the gain fell below the line.

The 32-family load, rows before 15:00 UTC: 32 families, min 2,918, max 3,197, mean 3,006.8 over 2,700 seconds. The line is 3,078. The mean is under it. The step ran its full time.

The sixteen-family step, rows before 15:50 UTC: 16 families, min 1,080, max 1,172, mean 1,111.1 over 900 seconds. The line is 1,026. Every family is above it.

## Mini

Mini's own files. The last minute of each counter has no read mark. No minute is marked unread in full.

| File | In the window | After the window | No read mark | Commit |
|---|---|---|---|---|
| [counts/mini/FIRST.md](../counts/mini/FIRST.md) | 96,802 | 14,523 | 13:59 | `8258e4f` at 14:00:06Z |
| [counts/mini/LOAD.md](../counts/mini/LOAD.md) | 260,582 | 7,554 | 15:14 | `5931c91` at 15:15:02Z |
| [counts/mini/SIXTEEN.md](../counts/mini/SIXTEEN.md) | 53,442 | 7,606 | 16:04 | `2376cb7` at 16:05:04Z |

Both publishers fired on this clock. This is not the Tuesday count.

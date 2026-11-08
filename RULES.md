> **Experimental. We are just trying this.** [Disclaimer](DISCLAIMER.md) · Kaspa Testnet-10 only. Counts only.
>
> This page is the rule. It does not start a machine.

# Rules

Every storm from the 8 Nov 2026 rehearsal on keeps these rules. The pastes point here. A chat note does not replace this page.

This repo is a new run. It is not a restart of the 00:40 UTC rehearsal. That clock is closed in [tn10-storm-2026-11-08](https://github.com/STP-KAS/tn10-storm-2026-11-08). The rule page there is the same rule, on that closed clock.

## Who publishes

The desk sends and counts. The desk runner publishes three files when each window has closed:

| File | Counter on | Counter off |
|---|---|---|
| [counts/desk/FIRST.md](counts/desk/README.md) | 11:58 UTC | 14:00 UTC |
| [counts/desk/LOAD.md](counts/desk/README.md) | 14:13 UTC | 15:15 UTC |
| [counts/desk/SIXTEEN.md](counts/desk/README.md) | 15:33 UTC | 16:05 UTC |

Mini counts and does not send. Mini's runner publishes the same three windows under [counts/mini/](counts/mini/README.md). Each machine writes only its own folder. The chat does not publish either folder. Bot does not write them.

A hop is in the file when the accepting block's header time is inside that counter. The row does not carry a txid, a key, a seed, an address, a host, a port, or a covenant id. The accepting block hash may sit on the row. The family label may be a sha256 already stored. The covenant id stays off the file. A minute that was not read in full stays marked. The gap is not filled.

The 8 Nov desk scores stay in that rehearsal's method log. They are not copied here.

## Hashes

The desk writes each hash file before the matching send. Fixed is the local write time. On origin is the commit time of the commit that put the rows on GitHub. After that push succeeds, the same runner reads the time from origin and writes it into the file, then pushes that one line. The time comes from origin. The runner does not invent it. A file with rows and no On origin line is not proof the push happened. No proved file, no send.

| File | Before |
|---|---|
| [hashes/EIGHT.md](hashes/README.md) | the 12:00 UTC send |
| [hashes/THIRTYTWO.md](hashes/README.md) | the 14:15 UTC load |
| [hashes/SIXTEEN.md](hashes/README.md) | the 15:35 UTC step, and after the load |

The 8 Nov origin times stay in that rehearsal. They are not this run's proof.

## Git

Call git by its full path. Keep the errors. Empty output is a failed read. Read once more with the same path. If that read fails too, stop. One commit per file that just closed. If the push fails, try the same push once more. Then stop and say the git error.

## One runner

One runner on the desk. One runner on Mini. The runner is a process with a log. The chat is not the runner. A second runner is a fault. A scheduled task is not the arm. The 7 Nov tasks stay unused.

## This clock

The day is Sun 8 Nov 2026. Start is 12:00 UTC (13:00 CET). Both pastes carry that day. A read of [GO-MINI.md](GO-MINI.md) on Mini starts Mini's runner, and Mini's first push is `logs/MINI-ARMED.md`. The desk hashes only when that line is on origin. A quiet chat does not stop the desk. [GO.md](GO.md) does not start a machine. After 11:40 UTC the pastes stay as they are. The 10:40 UTC waiter stays stopped.

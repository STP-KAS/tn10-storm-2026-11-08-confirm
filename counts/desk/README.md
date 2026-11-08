> **Experimental. We are just trying this.** [Disclaimer](../../DISCLAIMER.md) · Counts only. No key, seed, txid, covenant id, address, host, or port.
>
> The desk's count files will live here. Mini does not write this folder. The paste is [GO-DESK.md](../../GO-DESK.md). The date is blank, so the files are absent.

# Desk counts

The desk counts. Previous counted storms already counted on the sending machine. On the live clock the desk runner writes three files here and publishes each one at the window end. The chat is not the publisher.

| File | Counter on | Counter off |
|---|---|---|
| FIRST.md | 00:38 UTC | 02:40 UTC |
| LOAD.md | 02:53 UTC | 03:55 UTC |
| SIXTEEN.md | 04:13 UTC | 04:45 UTC |

A hop is in a file when the accepting block's header time is inside that counter. That header time is the clock. The desk's notice time is not the clock. A minute the desk did not read in full stays marked. The gap is not filled. Genesis is not a hop. A conflicting spend is not a hop. Hops after the window are listed apart.

The accepting block hash may sit on a row. A txid, a key, a seed, an address, a host, a port, and a covenant id do not.

The runner resolves git once, keeps that full path, and uses only that path. Empty output is a failed read. It is not an empty count. Read once more. If that read fails too, stop and say the read failed. The local file stays. Do not invent a count. Do not start a second runner. Mini's folder is [counts/mini/](../mini/README.md). The desk does not write it.

While the paste says DATE, the runner stays down. The 8 Nov desk scores stay in [that rehearsal's method log](https://github.com/STP-KAS/tn10-storm-2026-11-08/blob/main/logs/METHOD.md). They are not copied here.

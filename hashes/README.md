> **Experimental. We are just trying this.** [Disclaimer](../DISCLAIMER.md) · Kaspa Testnet-10 only. No covenant id in this folder.
>
> Nothing here is a result. The files below are written by the desk runner before the matching submit. Until then they are absent on purpose. The date is blank, so they are absent now.

# Hashes

| File | When it has to be here | What it covers |
|---|---|---|
| EIGHT.md | before 00:40 UTC on the chosen day | the 1-to-8 shape |
| THIRTYTWO.md | before 02:55 UTC | the 32-family load |
| SIXTEEN.md | before 04:15 UTC, and after the load | the sixteen-family step |

Each row is a sha256 of a lowercase hex covenant id. The id stays off this repo. The desk paste is [GO-DESK.md](../GO-DESK.md). No file, no send.

Fixed is the time the runner wrote the file on the desk. On origin is the commit time of the commit that put those rows on GitHub. The runner writes the rows, pushes, reads that commit time from origin, writes it into the file, and pushes that one line. The time comes from origin. The runner does not invent it. A file with rows and no On origin line is not proof the push happened. Empty git output is a failed read. Read once more. If that read fails too, stop.

On the 8 Nov rehearsal the rows reached origin at these times. They live in that repo, not in this one.

| File | On origin/main of the rehearsal |
|---|---|
| EIGHT | 2026-11-08T00:07:21Z, commit 430e905 |
| THIRTYTWO | 2026-11-08T02:30:02Z, commit 180529c |
| SIXTEEN | 2026-11-08T04:00:04Z, commit abb8ac5 |

Source: [the rehearsal hash page](https://github.com/STP-KAS/tn10-storm-2026-11-08/blob/main/hashes/README.md).

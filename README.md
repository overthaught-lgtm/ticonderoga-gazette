-Craig Gazette- RE-introducing facts & truth
# The Ticonderoga Gazette

**Live at:** [gazette.ticonderoga.online](https://gazette.ticonderoga.online)
**Published by:** Ticonderoga Systems Holdings LLC · Craig, Colorado
**Byline:** Rigby Donovan (Ticon Recon vertical: Cora)

-----

## ▲ Versioning & Archive Standard (TEAKWOOD Protocol)

This repository follows the **TEAKWOOD Protocol** — Truth-first, Event-immutable,
Audit-locked, Kinetic-zero drift, Write-once, Operational truth, On-premises
sovereign, Drift-zero.

In practice, this means:

- `index.html` at the repo root is **always the current live issue** — this is
  the file Vercel deploys to `gazette.ticonderoga.online`.
- Every time a new issue replaces the live one, the **outgoing issue is
  archived** into `/issues/vN-YYYY-MM/` *before* it is overwritten. Nothing is
  deleted or silently lost.
- Each archived issue is a frozen, complete snapshot — exactly what was live,
  exactly when it was live.

This creates a permanent, ordered record of every public version of the
Gazette: what it said, when it said it, and in what order.

-----

## ▲ Archive Index

|Version|Folder               |Status  |Live Window                 |
|-------|---------------------|--------|----------------------------|
|v1     |`/issues/v1-2026-05/`|Archived|May 2026 → (until v2 deploy)|
|v2     |`/issues/v2-2026-0X/`|Pending |TBD                         |
|v3     |`/issues/v3-2026-0X/`|Pending |TBD                         |

*(Live windows and folder names get filled in as each version goes live and
is superseded.)*

-----

## ▲ Minting / Chain-of-Record (Intent)

Each archived issue is intended to eventually receive a **timestamped,
tamper-evident record** — a content hash + publish date, logged permanently
once an issue is retired from live status. This record is the “minting” step:
it confirms an issue existed, in this exact form, at this exact time, and
locks it against revision.

**Mechanism: not yet decided.** Candidates under consideration include the
TicoJitsu ledger, an on-chain record via the TSH wallet on Base, or a simple
hash/timestamp log committed to this repo (`/issues/ledger.yaml` or similar).
This section will be updated once the mechanism is selected — until then,
archival into `/issues/` is the operative record-keeping step.

-----

## ▲ Repo Structure

```
ticonderoga-gazette/
├── index.html              ← current live issue (deployed to gazette.ticonderoga.online)
├── README.md                ← this file
└── issues/
    ├── v1-2026-05/
    │   └── index.html       ← frozen snapshot of v1
    ├── v2-2026-0X/
    │   └── index.html       ← frozen snapshot of v2 (once superseded)
    └── v3-2026-0X/
        └── index.html
```

-----

© 2026 Ticonderoga Systems Holdings LLC · Craig, Colorado · Moffat County
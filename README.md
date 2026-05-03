# Hardwired Terminal

A working surface for the Hardwired framework. v3.1 methodology, database-driven.

## Files

```
hardwired/
├── index.html       public terminal — read-only
├── eval.html        v3 migration terminal — Ed's working surface
├── data.json        the published dataset
├── methodology.md   v3.1 methodology specification
└── README.md
```

## Current phase: V3 migration

The framework recently moved from v2 to v3 methodology, then refined to v3.1
to operationalise the era evaluation. The eval terminal contains 64 v2
records that need to be walked through v3.1 review one by one. As records
are validated, they accumulate in `eval.html`'s localStorage.

When all 64 records are v3.1-validated, Ed runs `publish` in `eval.html`,
which downloads a fresh `data.json` containing the locked dataset. He drags
that file onto github.com to replace the existing `data.json`. The public
terminal then reads the new locked data.

Until that moment, `data.json` contains only the records already validated
under v3.1, and the public terminal shows those.

## Architecture

- **index.html** — public terminal. Reads `data.json`. Untouched during migration.
- **eval.html** — v3 migration terminal. Self-contained: 64 v2 records baked in,
  6 v3 records carry forward on first boot, all working state in localStorage.
  No GitHub fetch. No second input file.
- **data.json** — current public dataset. Will be replaced once migration completes.
- **methodology.md** — v3.1 specification. The authoritative document.

## V3.1 review procedure

`review <TICKER>` walks the v3.1 methodology procedure:

1. Show the v2 reading at each step
2. Three named differences
3. Verdict (the honest answer to v3's three questions)
4. Pool, mediation, cluster, durability classification
5. Grade decision (drift-toward-charity warning if migrating downward)
6. MINI test (named figure, named moment, result)
7. Financial-trajectory check (3 prompts + validity)
8. Era evaluation (v3.1 — four-step):
   - Agent-callability — present, absent, what philosophy authorises
   - Agent-readability — name a structural commitment models could cite
   - Four hedges — direct relationships, category identity,
     capital authority, institutional trust
   - Era verdict — one closing line
9. Re-score triggers
10. Research notes (optional, private)

The wizard preserves the v2 headline, reasoning bullets, chips, category, and
position into the v3.1 record so the published surface keeps the strong v2
writing alongside the v3.1 apparatus.

## What v3.1 changes from v3.0

The era evaluation, previously an implicit consequence of era-relevance and
mediation exposure, is now named explicitly and operationalised as three tests
plus the four-hedges check from the substrates document:

- **Synthesis layer** — what frontier models surface about the company
- **Agent-callability** — can an agent complete a commercial path with the
  company under its philosophy (split into present / absent / authorised)
- **Agent-readability** — structural commitments models could cite

The four hedges (direct customer relationships, category identity LLMs
describe as canonical, capital authority for partnerships, institutional
trust signals) are surfaced as a check during review. A company strong on at
least two hedges is structurally defended at the agent layer.

Mediation exposure is now connected to the agent-era ledger logic: low
mediation = direct relationships = brand becomes an entry in the buyer's
operating context. High mediation = the retailer becomes the ledger entry.

No grades require revision under v3.1. The change is operational, not
doctrinal.

## Methodology

v3.1 · May 2026 · Inverness Consulting · always in beta.

The framework asks three questions of every company: what are the differences,
is the company protecting them, is the company capitalising where it can.
Grade is the honest answer, validated by financial evidence.

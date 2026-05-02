# Hardwired Terminal

A working surface for the Hardwired framework. v3.0 methodology, database-driven.

## Files

```
hardwired-terminal/
├── index.html    public terminal — read-only, fetches data.json on load
├── eval.html     analyst terminal — read/write (Phase 2, in progress)
└── data.json     single source of truth — every company record lives here
```

## Architecture

One JSON, two surfaces.

- **index.html** is what subscribers see. It fetches `data.json` and renders.
- **eval.html** is what Ed uses to score, update, and maintain records.
- **data.json** is the only file with content. Edit it, commit it, GitHub Pages
  republishes within a minute.

## Hosting

GitHub Pages, free, version-controlled. Every change to `data.json` is a git
commit, which automatically gives the publication a dated audit trail —
satisfying the v3 discipline of *every grade is dated and methodology-stamped*
without Ed having to remember to log anything.

## Workflow

To add or update a company:

1. Open `eval.html` (Phase 2)
2. Run `add MSFT` or `edit SBUX`
3. Walk through the v3 procedure
4. Run `export` — downloads a fresh `data.json`
5. Replace `data.json` in the repo
6. Commit and push
7. Public terminal updates within ~1 minute

## Schema

`data.json` has three top-level blocks:

- `_meta` — methodology version, last published date, publisher
- `_index` — light index of every record (ticker, grade, pool, mediation,
  durability, cell, scoredOn). Used for list, grid, and filter views.
- `records` — full v3 record per company, keyed by ticker

Each record carries the full v3 apparatus: 9 dimensions, 5 gates, MINI test,
adversarial flags, financial check, programs and constraints, era evaluation,
re-score triggers, methodology stamp, scored-on date.

## Methodology

v3.0 · April 2026 · Inverness Consulting · always in beta.

The framework asks three questions of every company: what are the differences,
is the company protecting them, is the company capitalising where it can.
Grade is the honest answer, validated by financial evidence.

---
title: Experiment logging & branch discipline
type: doc-concept
provenance: doc
source: program.md
updated: 2026-07-04
status: fresh
---
# Experiment logging & branch discipline

## Definition
Every autonomous run is recorded two ways: as **git history on a dedicated branch** and as a row in an
untracked **`results.tsv`** ledger. Together they give the human a readable record of what was tried and
what worked, and give the agent a durable memory across a long unattended session.

## In autoresearch (grounded)
- **Branch per run.** Setup creates `autoresearch/<tag>` (e.g. `autoresearch/mar5`) from master; the branch
  must not already exist, guaranteeing a fresh run. The keep/revert rule from the
  [experiment loop](autonomous-experiment-loop.md) *advances* this branch on improvement and `git reset`s it
  on a regression, so the branch tip always points at the best model so far.
- **`results.tsv` ledger.** A tab-separated file (commas would break descriptions) with five columns:
  `commit`, `val_bpb`, `memory_gb`, `status`, `description`. `status` is `keep`, `discard`, or `crash`;
  crashes record `0.000000` / `0.0`. The `val_bpb` column is exactly the
  [`val_bpb`](../catalog/train.md#val_bpb) printed by [train.py](../concepts/train.md), and `memory_gb` is
  [`peak_vram_mb`](../catalog/train.md#peak_vram_mb) divided by 1024. `program.md` insists `results.tsv`
  stay **untracked by git** — it is a run-local scratch ledger, not committed state.
- **The summary block** the agent parses is printed at the end of a run — `val_bpb`, `training_seconds`,
  `peak_vram_mb`, `mfu_percent`, `total_tokens_M`, `num_steps`, `num_params_M`, `depth` — extracted with
  `grep "^val_bpb:" run.log`.

## Why it matters / when it applies
The ledger is what makes an overnight batch of ~100 experiments legible to a human in the morning, and the
branch discipline is what lets the agent hill-climb without losing its best result. `program.md` also sets
operational guardrails around logging: a **10-minute hard timeout** per experiment (kill and treat as a
failure — the run should be ~5 min plus startup), and a crash policy of "fix if it's something dumb like a
typo, otherwise log `crash` and move on."

## Connections
- Related doc-concepts: [the autonomous experiment loop](autonomous-experiment-loop.md),
  [the fixed time budget](fixed-time-budget.md).
- Code concepts: [train.py](../concepts/train.md) (source of the summary metrics logged here).
- Module catalogs: [train](../catalog/train.md).

## Source
Extracted from `program.md` (kept in place).

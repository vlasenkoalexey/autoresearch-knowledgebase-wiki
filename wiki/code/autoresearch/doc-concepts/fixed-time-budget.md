---
title: The fixed time budget
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# The fixed time budget

## Definition
Training always runs for a **fixed 5-minute wall-clock budget** (excluding startup/compilation), regardless
of the model, batch size, or hardware. This single design choice is what makes autonomous experiments
directly comparable and what turns the search into an optimization for *the best model achievable in 5
minutes on this machine*.

## In autoresearch (grounded)
The budget is the frozen constant [`TIME_BUDGET`](../catalog/prepare.md#TIME_BUDGET) (300s) in
[prepare.py](../concepts/prepare.md), imported by [train.py](../concepts/train.md). The training loop
accumulates only steady-state wall time into [`total_training_time`](../catalog/train.md#total_training_time)
and stops when it reaches the budget — but only *after* `step > 10`, so `torch.compile` warm-up isn't
charged against it. The time-sensitive schedules are functions of [`progress`](../catalog/train.md#progress)
= elapsed / budget rather than a step count: the LR multiplier
[`get_lr_multiplier`](../catalog/train.md#get_lr_multiplier) and the weight-decay decay key off it, which is
the only way to land a warmdown exactly at the buzzer when the number of steps is unknown in advance. (Muon
momentum is the one exception, warming up over the first ~300 steps.)

## Why it matters / when it applies
Two upsides, per the README: (1) experiments are directly comparable no matter what the agent changes
(model size, architecture, optimizer), because they all get the same clock; and (2) the search converges on
the most capable model for *your* platform within the budget. The tradeoff: results are not comparable
across different compute platforms. The budget also removes "how long to train" from the agent's decision
space entirely — the only objective left is the score, [`val_bpb`](../catalog/train.md#val_bpb), scored by
the frozen [`evaluate_bpb`](../catalog/prepare.md#evaluate_bpb) at a fixed [`MAX_SEQ_LEN`](../catalog/prepare.md#MAX_SEQ_LEN)
and [`EVAL_TOKENS`](../catalog/prepare.md#EVAL_TOKENS). VRAM ([`peak_vram_mb`](../catalog/train.md#peak_vram_mb))
is a *soft* constraint — some growth is fine for a real gain, but it shouldn't blow up.

## Connections
- Code concepts: [train.py](../concepts/train.md) (time-indexed schedules, budget check),
  [prepare.py](../concepts/prepare.md) (the frozen budget/metric constants).
- Module catalogs: [prepare](../catalog/prepare.md), [train](../catalog/train.md).
- Related doc-concepts: [the autonomous experiment loop](autonomous-experiment-loop.md),
  [single-file agent edits](single-file-agent-edits.md).

## Source
Extracted from `README.md` (kept in place; see also `program.md`).

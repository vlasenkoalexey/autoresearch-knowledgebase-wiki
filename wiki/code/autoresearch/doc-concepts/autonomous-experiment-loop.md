---
title: The autonomous experiment loop
type: doc-concept
provenance: doc
source: program.md
updated: 2026-07-04
status: fresh
---
# The autonomous experiment loop

## Definition
The core of autoresearch is a **forever-loop** in which an AI agent plays the role of an autonomous
researcher: it hacks an idea into `train.py`, commits, runs one fixed-budget training experiment, reads the
resulting score, and then **keeps or discards** the change based on whether the metric improved — with no
human in the loop. `program.md` is the lightweight "skill" that instructs the agent how to run this loop;
the human iterates on `program.md`, the agent iterates on `train.py`.

## In autoresearch (grounded)
Each iteration edits [`train.py`](../concepts/train.md) — the only mutable file — and runs it, producing a
single scalar [`val_bpb`](../catalog/train.md#val_bpb) after exactly [`TIME_BUDGET`](../catalog/prepare.md#TIME_BUDGET)
seconds of training. The loop (from `program.md`) is:

1. Look at the current git branch/commit.
2. Tune `train.py` with one experimental idea (architecture, optimizer, hyperparameters, batch size, model
   size — all fair game; the primary capacity knob is `DEPTH`, consumed by
   [`build_model_config`](../catalog/train.md#build_model_config)).
3. `git commit`.
4. Run `uv run train.py > run.log 2>&1` (redirect everything — never flood the agent's context).
5. `grep "^val_bpb:\|^peak_vram_mb:" run.log` to read the result.
6. Empty grep ⇒ the run crashed; `tail -n 50 run.log`, attempt a fix a few times, else give up.
7. Record the row in `results.tsv` (see [experiment logging](experiment-logging.md)).
8. If [`val_bpb`](../catalog/train.md#val_bpb) improved (lower), **advance** the branch (keep the commit).
9. If equal or worse, `git reset` back to where the iteration started.

The improvement signal is honest because the score is produced by the frozen
[`evaluate_bpb`](../catalog/prepare.md#evaluate_bpb) in [prepare.py](../concepts/prepare.md), which the
agent may not modify.

## Why it matters / when it applies
This loop is what turns a single training script into *research*: keep-if-better/revert-if-worse is
hill-climbing over the space of code edits, and because each experiment is a fixed 5 minutes (~12/hour,
~100 over a night's sleep), a human can leave the agent running unattended and wake to a log of experiments
plus a better model. `program.md` is explicit that the agent must **NEVER STOP** to ask permission mid-loop —
if it runs out of ideas it should read the papers referenced in the code, re-read the in-scope files, or try
more radical changes, and only halt when manually interrupted.

## Connections
- Code concepts: [train.py — the experiment substrate](../concepts/train.md) (what the agent edits and how a
  run works), [prepare.py — the frozen substrate](../concepts/prepare.md) (why the metric can't be gamed).
- Module catalogs: [train](../catalog/train.md), [prepare](../catalog/prepare.md).
- Related doc-concepts: [experiment logging & branch discipline](experiment-logging.md),
  [the fixed time budget](fixed-time-budget.md), [single-file agent edits](single-file-agent-edits.md).

## Source
Extracted from `program.md` (kept in place).

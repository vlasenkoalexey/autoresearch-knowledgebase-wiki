---
title: Single-file agent edits (mutable vs. frozen)
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Single-file agent edits (mutable vs. frozen)

## Definition
autoresearch deliberately has **only three files that matter**, and the agent is allowed to edit exactly
one of them. `train.py` is fair game in its entirety; `prepare.py` is read-only; `program.md` is edited by
the human, not the agent. Constraining the agent to a single file keeps scope manageable and every diff
reviewable, while quarantining the experimental conditions from the thing being optimized.

## In autoresearch (grounded)
- **`train.py` — mutable.** The full GPT model, the Muon+AdamW optimizer, and the training loop live here;
  everything is fair game (architecture, hyperparameters, optimizer, batch size, model size). See
  [train.py — the experiment substrate](../concepts/train.md). The main capacity knob is `DEPTH`, turned
  into a config by [`build_model_config`](../catalog/train.md#build_model_config).
- **`prepare.py` — frozen.** Fixed constants, data prep, tokenizer, dataloader, and — most importantly — the
  evaluation harness [`evaluate_bpb`](../catalog/prepare.md#evaluate_bpb), the ground-truth metric. The agent
  may not modify it, install new packages, or change the evaluation. See
  [prepare.py — the frozen substrate](../concepts/prepare.md).
- **`program.md` — human-authored.** The agent's instruction "skill" describing the
  [experiment loop](autonomous-experiment-loop.md); the human iterates on it to shape the research org.

## Why it matters / when it applies
The mutable/frozen split is the scientific control: because the agent can only change the model and never
the test, "lower [`val_bpb`](../catalog/train.md#val_bpb)" is guaranteed to mean "better model" rather than
"easier benchmark." The README frames the design as *single file to modify* (reviewable diffs, manageable
scope), *fixed budget* (comparability — see [the fixed time budget](fixed-time-budget.md)), and
*self-contained* (one GPU, one file, one metric — no distributed training, no complex configs). A
**simplicity criterion** also governs edits: all else equal, simpler is better, and deleting code for equal
or better score is an outright win.

## Connections
- Code concepts: [train.py](../concepts/train.md), [prepare.py](../concepts/prepare.md).
- Module catalogs: [train](../catalog/train.md), [prepare](../catalog/prepare.md).
- Related doc-concepts: [the autonomous experiment loop](autonomous-experiment-loop.md),
  [the fixed time budget](fixed-time-budget.md), [experiment logging](experiment-logging.md).

## Source
Extracted from `README.md` (kept in place).

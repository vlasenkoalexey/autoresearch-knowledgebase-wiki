---
title: LogWriter / StepRecord — the log as replayable ground truth
type: concept
provenance: mixed
concept: arc3-logwriter
concepts: [verification-independence]
updated: 2026-08-12
status: fresh
---
# LogWriter / StepRecord — the log as replayable ground truth

<!-- connect:up:begin -->
> **Cross-repo concept:** part of [verification-independence](../../../concepts/verification-independence.md) across this wiki's repos.
<!-- connect:up:end -->
## Overview

Every step Retrodict takes is written to a text log as a [`StepRecord`](../catalog/src/arc3/logwriter.md#StepRecord) —
*"One environment step as written to and parsed from the log"* — and [`parse_log`](../catalog/src/arc3/logwriter.md#parse_log)
can reconstruct the exact same records back out of that text. This round-trip is what makes
[`GameRunner._restore`](arc3-runner.md) possible: the log isn't a human-readable side effect, it's a
serialization format the agent's own state can be rebuilt from after a context reset.

## Design rationale (why it's built this way)

**Parsing deliberately skips derived content.** [`parse_log`](../catalog/src/arc3/logwriter.md#parse_log)'s
docstring is explicit — *"Parse step sections back out of a log; derived [DIFF] and [PLAN] blocks are
skipped"* — meaning the log carries both the durable record (`StepRecord` fields) and transient
presentation content (diffs, plan text) in the same file, and replay only trusts the former. This is what
keeps a re-parse of a growing log cheap and keeps `_restore` from re-deriving stale reasoning rather than
raw fact.

**`StepRecord` is frozen.** It's declared `@dataclass(frozen=True)` — a logged step, once written, is not a
mutable object anyone downstream can quietly edit; [`_finish`](../catalog/src/arc3/logwriter.md#_finish)
builds one from an in-progress `_StepBuilder` only at the point the step is actually complete.

**`BoardDiff` is an explicit type alias** (`list[tuple[int, int, int, int]]`), and
[`append_step`](../catalog/src/arc3/logwriter.md#LogWriter.append_step) accepts an optional `diff` alongside
the record — the log can carry a compact description of *what changed* on the board this step, not just the
raw frame, which is what lets a later reader (human or the retrodiction check itself) see the delta without
diffing two full frames by hand.

## Entry points
- [`LogWriter.append_step`](../catalog/src/arc3/logwriter.md#LogWriter.append_step) — writes one step
  section to the log file, called from [`GameRunner._log_frame`](arc3-runner.md).
- [`parse_log`](../catalog/src/arc3/logwriter.md#parse_log) — reads a log's text back into a list of
  `StepRecord`, called from [`GameRunner._restore`](arc3-runner.md).

## Mechanism (step-by-step)
1. As each action resolves, [`GameRunner._log_frame`](../catalog/src/arc3/runner.md#GameRunner._log_frame)
   builds the step's data and calls [`append_step`](../catalog/src/arc3/logwriter.md#LogWriter.append_step),
   which formats it (via [`format_diff`](../catalog/src/arc3/logwriter.md#format_diff) for any board delta)
   and appends it to the on-disk log through [`_append`](../catalog/src/arc3/logwriter.md#LogWriter._append).
2. On resume, [`parse_log`](../catalog/src/arc3/logwriter.md#parse_log) reads the full log text, splits it
   into step sections, and reconstructs each as a [`StepRecord`](../catalog/src/arc3/logwriter.md#StepRecord)
   via [`_finish`](../catalog/src/arc3/logwriter.md#_finish) — skipping the derived `[DIFF]`/`[PLAN]`
   annotations.
3. [`GameRunner._restore`](../catalog/src/arc3/runner.md#GameRunner._restore) replays those records through
   the real environment to rebuild live state, and
   [`_seed_level_signals`](../catalog/src/arc3/runner.md#GameRunner._seed_level_signals) derives the current
   level's stuck-detection signals from the same replayed sequence.

## Key data structures
- [`StepRecord`](../catalog/src/arc3/logwriter.md#StepRecord) — `step`, `action`,
  [`frames`](../catalog/src/arc3/logwriter.md#StepRecord.frames),
  [`levels_completed`](../catalog/src/arc3/logwriter.md#StepRecord.levels_completed),
  [`state`](../catalog/src/arc3/logwriter.md#StepRecord.state), `x`/`y` — the durable, replayable unit.
- `BoardDiff` — a list of `(row, col, old_value, new_value)` tuples, the compact per-step board delta.

## See also
- [`arc3-runner`](arc3-runner.md) — the writer (`_log_frame`) and reader (`_restore`) of this log format.

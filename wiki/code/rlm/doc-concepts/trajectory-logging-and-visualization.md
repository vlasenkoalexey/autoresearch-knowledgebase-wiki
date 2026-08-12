---
title: Trajectory logging and visualization
type: doc-concept
provenance: doc
source: README.md
updated: 2026-08-12
status: fresh
---
# Trajectory logging and visualization

## Definition
The README documents two logging modes: **in-memory only** (`logger=RLMLogger()`, trajectory reachable via
`completion.metadata`) and **also-save-to-disk** (`RLMLogger(log_dir="./logs")`, writing one JSONL file per
completion), plus a Node.js/shadcn visualizer web app for browsing those JSONL files interactively.

## In rlm (grounded)
The two modes map directly onto [`RLMLogger.log_file_path`](../catalog/rlm/logger/rlm_logger.md#RLMLogger.log_file_path) —
set or unset depending on whether `log_dir` was passed — gating whether
[`RLMLogger.log`](../catalog/rlm/logger/rlm_logger.md#RLMLogger.log) persists to disk in addition to holding
the trajectory in memory. The visualizer itself is grounded in
[`visualizer-src-lib-types.ts`](../concepts/visualizer-src-lib-types.ts.md), whose `RLMIteration` TypeScript
interface mirrors the Python dataclass these JSONL files serialize.

## Why it matters / when it applies
This is the concrete implementation of `RLMChatCompletion.metadata` — described in the README as holding
"the full trajectory (run config + all iterations and sub-calls) so you can reconstruct the run" — which is
what lets a recursive, potentially deeply-nested completion be inspected after the fact rather than only
observed live via `verbose=True` (see [`rlm-logger-verbose`](../concepts/rlm-logger-verbose.md)).

## Connections
- Code concepts: [`rlm-logger-rlm_logger`](../concepts/rlm-logger-rlm_logger.md),
  [`rlm-logger-verbose`](../concepts/rlm-logger-verbose.md),
  [`visualizer-src-lib-types.ts`](../concepts/visualizer-src-lib-types.ts.md),
  [`rlm-core-types`](../concepts/rlm-core-types.md)
- Module catalogs: [`logger/rlm_logger`](../catalog/rlm/logger/rlm_logger.md)
- Related doc-concepts: [repl-environment-taxonomy](repl-environment-taxonomy.md)

## Source
Extracted from `README.md` (kept in place).

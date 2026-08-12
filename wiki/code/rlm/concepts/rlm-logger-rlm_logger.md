---
title: RLMLogger — trajectory capture across recursion
type: concept
provenance: mixed
concept: rlm-logger-rlm_logger
updated: 2026-08-12
status: fresh
---
# RLMLogger — trajectory capture across recursion

## Overview

[`RLMLogger`](../catalog/rlm/logger/rlm_logger.md#RLMLogger) captures the full trajectory of one
`completion()` call — run metadata plus every iteration — and is the mechanism behind
`RLMChatCompletion.metadata` being populated on a call that had a logger attached. It is optionally
propagated from a parent RLM to any child RLM spawned via `_subcall` (see
[`rlm-core-rlm`](rlm-core-rlm.md)'s Dynamics section, which the tests here directly exercise).

## Design rationale (why it's built this way)

**Metadata and iterations are logged separately, on separate calls** ([`log_metadata`](../catalog/rlm/logger/rlm_logger.md#RLMLogger.log_metadata)
vs. [`log`](../catalog/rlm/logger/rlm_logger.md#RLMLogger.log)), because run metadata (backend, model,
`max_depth`, `max_iterations`, environment type/kwargs — visible on
[`RLM._persistent_env`](rlm-core-rlm.md)'s construction path) is known once at the start of a call, while
iterations accumulate one at a time as the loop runs. Both paths funnel through the same
`_save_to_disk`/`log_file_path` mechanism, so a logger can be file-backed or purely in-memory depending on
whether `log_file_path` is set.

## Entry points
- [`RLMLogger.log`](../catalog/rlm/logger/rlm_logger.md#RLMLogger.log) — called once per iteration from
  `RLM.completion`'s loop.
- [`RLMLogger.log_metadata`](../catalog/rlm/logger/rlm_logger.md#RLMLogger.log_metadata) — called once, at
  the start of a completion, to record run configuration.

## Mechanism (step-by-step)
1. [`RLM.completion`](../catalog/rlm/core/rlm.md#RLM.completion) clears any prior iterations at the start of
   a call (`logger.clear_iterations()` — see [`rlm-core-rlm`](rlm-core-rlm.md)).
2. Run metadata (backend, model config, depth limits, environment config) is captured once via
   [`log_metadata`](../catalog/rlm/logger/rlm_logger.md#RLMLogger.log_metadata), serialized through
   `RLMMetadata.to_dict`.
3. Each completed [`RLMIteration`](../catalog/rlm/core/types.md#RLMIteration) is appended via
   [`log`](../catalog/rlm/logger/rlm_logger.md#RLMLogger.log), and if
   [`log_file_path`](../catalog/rlm/logger/rlm_logger.md#RLMLogger.log_file_path) is set, persisted
   incrementally rather than only held in memory.
4. If a logger is attached to a parent RLM, a child RLM spawned via
   [`_subcall`](../catalog/rlm/core/rlm.md#RLM._subcall) also receives a logger, so the resulting
   `RLMChatCompletion.metadata` carries the child's own full trajectory nested inside the parent's.

## Edge cases
- A leaf-depth sub-call (one that degrades to a plain LM completion rather than spawning a real child RLM)
  carries **no metadata at all**, logger or not — there is no child trajectory to capture because no child
  RLM ran.

## See also
- [`rlm-core-rlm`](rlm-core-rlm.md) — the caller and the logger-propagation-across-`_subcall` behavior.
- [`rlm-core-types`](rlm-core-types.md) — `RLMIteration`, `RLMMetadata`, the shapes being logged.
- [`rlm-logger-verbose`](rlm-logger-verbose.md) — the console-printing counterpart to this file-backed logger.

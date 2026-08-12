---
title: VerbosePrinter — console rendering of one iteration
type: concept
provenance: mixed
concept: rlm-logger-verbose
updated: 2026-08-12
status: fresh
---
# VerbosePrinter — console rendering of one iteration

## Overview

`VerbosePrinter` is the `verbose=True` path's console output — a human-readable rendering of the same
[`RLMIteration`](../catalog/rlm/core/types.md#RLMIteration) data [`RLMLogger`](rlm-logger-rlm_logger.md)
persists to disk. It exists purely for interactive debugging of a running RLM session; it does not affect
what gets logged or returned.

## Design rationale

**It walks the same tree structure `RLMLogger` captures, but renders instead of serializes.**
[`print_iteration`](../catalog/rlm/logger/verbose.md#VerbosePrinter.print_iteration) prints a complete
iteration (model response plus every code execution triggered), delegating each code block to
[`print_code_execution`](../catalog/rlm/logger/verbose.md#VerbosePrinter.print_code_execution), which shows
`stdout`/`stderr` and any nested `rlm_calls` a code block made — so a verbose run visibly shows recursion
happening in real time, one sub-call at a time, rather than only after the whole completion returns.

## Entry points
- [`VerbosePrinter.print_iteration`](../catalog/rlm/logger/verbose.md#VerbosePrinter.print_iteration) — one
  call per iteration in `RLM.completion`'s loop when `verbose=True`.

## See also
- [`rlm-logger-rlm_logger`](rlm-logger-rlm_logger.md) — the persistent counterpart.
- [`rlm-core-types`](rlm-core-types.md) — the data being rendered.

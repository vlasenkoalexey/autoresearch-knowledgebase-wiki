---
title: Visualizer types — the log-viewer's read of RLMIteration
type: concept
provenance: mixed
concept: visualizer-src-lib-types.ts
updated: 2026-08-12
status: fresh
---
# Visualizer types — the log-viewer's read of RLMIteration

## Overview

`visualizer/` is a small TypeScript web viewer for RLM trajectory logs — the browser-side counterpart to
[`VerbosePrinter`](rlm-logger-verbose.md)'s console rendering. Its
[`RLMIteration`](../catalog/visualizer/src/lib/types.ts.md#RLMIteration) interface is a hand-mirrored
TypeScript shape of the Python dataclass of the same name (see [`rlm-core-types`](rlm-core-types.md)),
consumed after a JSONL trajectory file (written by [`RLMLogger`](rlm-logger-rlm_logger.md)) is parsed.

## Mechanism
[`parseJSONL`](../catalog/visualizer/src/lib/parse-logs.ts.md#parseJSONL) reads a log file into an array of
`RLMIteration` objects; [`computeMetadata`](../catalog/visualizer/src/lib/parse-logs.ts.md#computeMetadata)
and [`extractContextQuestion`](../catalog/visualizer/src/lib/parse-logs.ts.md#extractContextQuestion) derive
summary views (walking `code_blocks` and each block's `result`) for display — the same tree the Python
logger captured, read back for a human browsing a completed run rather than watching one live.

## See also
- [`rlm-core-types`](rlm-core-types.md) — the Python-side dataclass this interface mirrors.
- [`rlm-logger-rlm_logger`](rlm-logger-rlm_logger.md) — the writer of the JSONL this module reads.

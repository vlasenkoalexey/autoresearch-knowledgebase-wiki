---
title: 'Module: packages/coding-agent/src/core/logging.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/logging.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`logging.ts`/
symbols:
  installFileLogSink: installFileLogSink().
  setLogContext: setLogContext().
  context: context.
  AGENT_LOG_MAX_BYTES: AGENT_LOG_MAX_BYTES.
---
# Module: [`packages/coding-agent/src/core/logging.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/logging.ts)

## Functions
- `installFileLogSink(fields?: Record<string, unknown> | undefined)` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/logging.ts#L18) — Route all structured logging (coding-agent and pi-ai) to the shared JSONL
- `setLogContext(fields: Record<string, unknown>)` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/logging.ts#L9) — Merge late-bound fields (e.g. mode, sessionId) into every subsequent log entry.

## Module values
- `AGENT_LOG_MAX_BYTES` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/logging.ts#L4)
- `context` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/logging.ts#L6)


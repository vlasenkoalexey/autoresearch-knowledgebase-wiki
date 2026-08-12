---
title: 'Module: packages/coding-agent/src/core/usage.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/usage.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`usage.ts`/
symbols:
  emptyUsage: emptyUsage().
  cloneUsage: cloneUsage().
  addAssistantUsage: addAssistantUsage().
  subtractAssistantUsage: subtractAssistantUsage().
---
# Module: [`packages/coding-agent/src/core/usage.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/usage.ts)

## Functions
- `addAssistantUsage(total: Usage, usage: Usage)` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/usage.ts#L20)
- `cloneUsage(usage: Usage)` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/usage.ts#L47)
- `emptyUsage()` — [`L3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/usage.ts#L3)
- `subtractAssistantUsage(total: Usage, usage: Usage)` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/usage.ts#L34) — Remove a previously added usage, clamping at zero to absorb attribution drift.


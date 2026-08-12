---
title: 'Module: packages/coding-agent/test/suite/agent-session-compaction.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/agent-session-compaction.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/`agent-session-compaction.test.ts`/
symbols:
  createAssistant.options-typeLiteral14.timestamp: createAssistant().(options)typeLiteral14:timestamp.
  createAssistant.options-typeLiteral14.stopReason: createAssistant().(options)typeLiteral14:stopReason.
  createAssistant: createAssistant().
  SessionWithCompactionInternals: SessionWithCompactionInternals#
  createAssistant.options-typeLiteral14.totalTokens: createAssistant().(options)typeLiteral14:totalTokens.
  SessionWithCompactionInternals.typeLiteral0._checkCompaction: SessionWithCompactionInternals#typeLiteral0:_checkCompaction.
  failingGateCommand: failingGateCommand().
  SessionWithCompactionInternals.typeLiteral0._shouldStopAfterTurn: SessionWithCompactionInternals#typeLiteral0:_shouldStopAfterTurn.
  SessionWithCompactionInternals.typeLiteral0._runAutoCompaction: SessionWithCompactionInternals#typeLiteral0:_runAutoCompaction.
  createAssistant.options-typeLiteral14.errorMessage: createAssistant().(options)typeLiteral14:errorMessage.
  SessionWithCompactionInternals.typeLiteral0._persistCompactionOutcome: SessionWithCompactionInternals#typeLiteral0:_persistCompactionOutcome.
  createUsage: createUsage().
---
# Module: [`packages/coding-agent/test/suite/agent-session-compaction.test.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compaction.test.ts)

## Classes
### `SessionWithCompactionInternals`
- def: [`packages/coding-agent/test/suite/agent-session-compaction.test.ts:8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compaction.test.ts#L8)
- signature: `type SessionWithCompactionInternals`
- protocol/private: `_checkCompaction`[`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compaction.test.ts#L9), `_persistCompactionOutcome`[`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compaction.test.ts#L16), `_runAutoCompaction`[`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compaction.test.ts#L14), `_shouldStopAfterTurn`[`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compaction.test.ts#L15)
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../../ai/src/types.ts.md#AssistantMessage), [`ShouldStopAfterTurnContext`](../../../agent/src/types.ts.md#ShouldStopAfterTurnContext)
- used by: (1 test-only callers)

## Functions
- `createAssistant(harness: Harness, options: { stopReason?: StopReason | undefined; errorMessage?: string | undefined; totalTokens?: number | undefined; timestamp?: number | undefined; })` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compaction.test.ts#L34)
- `createUsage(totalTokens: number)` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compaction.test.ts#L23)
- `failingGateCommand()` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compaction.test.ts#L57)

## Module values
- `errorMessage` — [`L38`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compaction.test.ts#L38)
- `stopReason` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compaction.test.ts#L37)
- `timestamp` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compaction.test.ts#L40)
- `totalTokens` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compaction.test.ts#L39)


---
title: 'Module: packages/coding-agent/test/suite/agent-session-compact-skill.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/agent-session-compact-skill.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/`agent-session-compact-skill.test.ts`/
symbols:
  setStreaming: setStreaming().
  createAssistant.options-typeLiteral6.errorMessage: createAssistant().(options)typeLiteral6:errorMessage.
  createAssistant: createAssistant().
  SessionInternals.typeLiteral0._checkCompaction: SessionInternals#typeLiteral0:_checkCompaction.
  SessionInternals: SessionInternals#
  extensionCompaction: extensionCompaction().
  createAssistant.options-typeLiteral6.stopReason: createAssistant().(options)typeLiteral6:stopReason.
  SessionInternals.typeLiteral0._shouldStopAfterTurn: SessionInternals#typeLiteral0:_shouldStopAfterTurn.
  SessionInternals.typeLiteral0._createKernelHostHandlers: SessionInternals#typeLiteral0:_createKernelHostHandlers.
---
# Module: [`packages/coding-agent/test/suite/agent-session-compact-skill.test.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compact-skill.test.ts)

## Classes
### `SessionInternals`
- def: [`packages/coding-agent/test/suite/agent-session-compact-skill.test.ts:6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compact-skill.test.ts#L6)
- signature: `type SessionInternals`
- protocol/private: `_checkCompaction`[`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compact-skill.test.ts#L7), `_createKernelHostHandlers`[`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compact-skill.test.ts#L9), `_shouldStopAfterTurn`[`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compact-skill.test.ts#L8)
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../../ai/src/types.ts.md#AssistantMessage), [`ShouldStopAfterTurnContext`](../../../agent/src/types.ts.md#ShouldStopAfterTurnContext)
- used by: (1 test-only callers)

## Functions
- `createAssistant(harness: Harness, options?: { stopReason?: StopReason | undefined; errorMessage?: string | undefined; })` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compact-skill.test.ts#L12)
- `extensionCompaction()` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compact-skill.test.ts#L34) — Extension that supplies compaction content so no provider call is needed.
- `setStreaming(harness: Harness, streaming: boolean)` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compact-skill.test.ts#L29)

## Module values
- `errorMessage` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compact-skill.test.ts#L14)
- `stopReason` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-compact-skill.test.ts#L14)


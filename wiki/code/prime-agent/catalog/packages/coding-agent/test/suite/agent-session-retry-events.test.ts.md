---
title: 'Module: packages/coding-agent/test/suite/agent-session-retry-events.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/agent-session-retry-events.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/`agent-session-retry-events.test.ts`/
symbols:
  normalizeEventOrder: normalizeEventOrder().
  structuredProviderFailure: structuredProviderFailure().
  SessionRetryCompactionInternals.typeLiteral71._checkCompaction: SessionRetryCompactionInternals#typeLiteral71:_checkCompaction.
  SessionRetryCompactionInternals.typeLiteral71._retryAttempt: SessionRetryCompactionInternals#typeLiteral71:_retryAttempt.
  SessionRetryCompactionInternals.typeLiteral71._processAgentEvent: SessionRetryCompactionInternals#typeLiteral71:_processAgentEvent.
  SessionRetryCompactionInternals: SessionRetryCompactionInternals#
  SessionRetryCompactionInternals.typeLiteral71._retryPromise: SessionRetryCompactionInternals#typeLiteral71:_retryPromise.
  SessionRetryCompactionInternals.typeLiteral71._retryResolve: SessionRetryCompactionInternals#typeLiteral71:_retryResolve.
  SessionRetryCompactionInternals.typeLiteral71._autoCompactionAbortController: SessionRetryCompactionInternals#typeLiteral71:_autoCompactionAbortController.
  SessionRetryCompactionInternals.typeLiteral71._postCompactionContinuationScheduled: SessionRetryCompactionInternals#typeLiteral71:_postCompactionContinuationScheduled.
  SessionRetryCompactionInternals.typeLiteral71._schedulePostCompactionContinue: SessionRetryCompactionInternals#typeLiteral71:_schedulePostCompactionContinue.
  SessionRetryCompactionInternals.typeLiteral71._cancelPostCompactionContinue: SessionRetryCompactionInternals#typeLiteral71:_cancelPostCompactionContinue.
---
# Module: [`packages/coding-agent/test/suite/agent-session-retry-events.test.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-retry-events.test.ts)

## Classes
### `SessionRetryCompactionInternals`
- def: [`packages/coding-agent/test/suite/agent-session-retry-events.test.ts:40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-retry-events.test.ts#L40)
- signature: `type SessionRetryCompactionInternals`
- protocol/private: `_autoCompactionAbortController`[`L44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-retry-events.test.ts#L44), `_cancelPostCompactionContinue`[`L49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-retry-events.test.ts#L49), `_checkCompaction`[`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-retry-events.test.ts#L47), `_postCompactionContinuationScheduled`[`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-retry-events.test.ts#L45), `_processAgentEvent`[`L46`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-retry-events.test.ts#L46), `_retryAttempt`[`L41`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-retry-events.test.ts#L41), `_retryPromise`[`L42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-retry-events.test.ts#L42), `_retryResolve`[`L43`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-retry-events.test.ts#L43), `_schedulePostCompactionContinue`[`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-retry-events.test.ts#L48)
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../../ai/src/types.ts.md#AssistantMessage), [`AgentEvent`](../../../agent/src/types.ts.md#AgentEvent)
- used by: (1 test-only callers)

## Functions
- `normalizeEventOrder(events: AgentSessionEvent[])` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-retry-events.test.ts#L7)
- `structuredProviderFailure(kind: "refusal" | "auth" | "invalid_request")` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-retry-events.test.ts#L24)


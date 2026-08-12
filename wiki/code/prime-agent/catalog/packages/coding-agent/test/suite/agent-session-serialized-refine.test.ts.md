---
title: 'Module: packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/`agent-session-serialized-refine.test.ts`/
symbols:
  SerializedInternals: SerializedInternals#
  SerializedInternals.typeLiteral0._assistantTurnsSinceAutoRefine: SerializedInternals#typeLiteral0:_assistantTurnsSinceAutoRefine.
  emptyRefinementResult: emptyRefinementResult().
  SerializedInternals.typeLiteral0._runSerializedRefineCheckpoint: SerializedInternals#typeLiteral0:_runSerializedRefineCheckpoint().
  mockSerializedRefine: mockSerializedRefine().
  SerializedInternals.typeLiteral0._pendingRequestedRefine: SerializedInternals#typeLiteral0:_pendingRequestedRefine.
  SerializedInternals.typeLiteral0._serializedPlanInFlight: SerializedInternals#typeLiteral0:_serializedPlanInFlight.
  SerializedInternals.typeLiteral0._autoRefineBranchVersion: SerializedInternals#typeLiteral0:_autoRefineBranchVersion.
  SerializedInternals.typeLiteral0._compactAutoRefinePending: SerializedInternals#typeLiteral0:_compactAutoRefinePending.
  SerializedInternals.typeLiteral0._lastAutoRefineReviewAt: SerializedInternals#typeLiteral0:_lastAutoRefineReviewAt.
  SerializedInternals.typeLiteral0._applyRefine: SerializedInternals#typeLiteral0:_applyRefine().
  SerializedInternals.typeLiteral0._drainPendingRefinementForDisposal: SerializedInternals#typeLiteral0:_drainPendingRefinementForDisposal().
  SerializedInternals.typeLiteral0._shouldStopAfterTurn: SerializedInternals#typeLiteral0:_shouldStopAfterTurn().
  makeCtx: makeCtx().
  SerializedInternals.typeLiteral0._agentEventQueue: SerializedInternals#typeLiteral0:_agentEventQueue.
  SerializedInternals.typeLiteral0._refineAbortController: SerializedInternals#typeLiteral0:_refineAbortController.
  SerializedInternals.typeLiteral0._lastAssistantMessage: SerializedInternals#typeLiteral0:_lastAssistantMessage.
  SerializedInternals.typeLiteral0._handleAgentEvent: SerializedInternals#typeLiteral0:_handleAgentEvent().
  SerializedInternals.typeLiteral0._handleAgentEvent.event-typeLiteral15.type: SerializedInternals#typeLiteral0:_handleAgentEvent().(event)typeLiteral15:type.
  SerializedInternals.typeLiteral0._handleAgentEvent.event-typeLiteral15.messages: SerializedInternals#typeLiteral0:_handleAgentEvent().(event)typeLiteral15:messages.
  SerializedInternals.typeLiteral0._scheduleAutoRefineAfterCompaction: SerializedInternals#typeLiteral0:_scheduleAutoRefineAfterCompaction().
  SerializedInternals.typeLiteral0._runSerializedRefine: SerializedInternals#typeLiteral0:_runSerializedRefine().
  SerializedInternals.typeLiteral0._runSerializedRefine.options-typeLiteral3.instructions: SerializedInternals#typeLiteral0:_runSerializedRefine().(options)typeLiteral3:instructions.
  SerializedInternals.typeLiteral0._compactionOperation: SerializedInternals#typeLiteral0:_compactionOperation.
  SerializedInternals.typeLiteral0._refineInFlight: SerializedInternals#typeLiteral0:_refineInFlight.
  SerializedInternals.typeLiteral0._disposed: SerializedInternals#typeLiteral0:_disposed.
  SerializedInternals.typeLiteral0._consumeSerializedBackgroundPlan: SerializedInternals#typeLiteral0:_consumeSerializedBackgroundPlan().
  SerializedInternals.typeLiteral0._runSerializedAutoRefineReview: SerializedInternals#typeLiteral0:_runSerializedAutoRefineReview().
  SerializedInternals.typeLiteral0._planRefine: SerializedInternals#typeLiteral0:_planRefine().
  SerializedInternals.typeLiteral0._createPreparedTurnAction: SerializedInternals#typeLiteral0:_createPreparedTurnAction().
  SerializedInternals.typeLiteral0._admitSessionInput: SerializedInternals#typeLiteral0:_admitSessionInput().
  SerializedInternals.typeLiteral0._refinePlanInFlight: SerializedInternals#typeLiteral0:_refinePlanInFlight.
  SerializedInternals.typeLiteral0._autoRefineReviewAbort: SerializedInternals#typeLiteral0:_autoRefineReviewAbort.
  SerializedInternals.typeLiteral0._branchSummaryOperation: SerializedInternals#typeLiteral0:_branchSummaryOperation.
  SerializedInternals.typeLiteral0._planRefine.options-typeLiteral7.instructions: SerializedInternals#typeLiteral0:_planRefine().(options)typeLiteral7:instructions.
  SerializedInternals.typeLiteral0._serializedRefine: SerializedInternals#typeLiteral0:_serializedRefine.
  SerializedInternals.typeLiteral0._getRequiredRequestAuth.Promise.typeLiteral16.apiKey: SerializedInternals#typeLiteral0:_getRequiredRequestAuth().Promise:typeLiteral16:apiKey.
  SerializedInternals.typeLiteral0._performCompaction.Promise.typeLiteral17.summary: SerializedInternals#typeLiteral0:_performCompaction().Promise:typeLiteral17:summary.
  SerializedInternals.typeLiteral0._performCompaction.Promise.typeLiteral17.firstKeptEntryId: SerializedInternals#typeLiteral0:_performCompaction().Promise:typeLiteral17:firstKeptEntryId.
  SerializedInternals.typeLiteral0._performCompaction.Promise.typeLiteral17.tokensBefore: SerializedInternals#typeLiteral0:_performCompaction().Promise:typeLiteral17:tokensBefore.
  SerializedInternals.typeLiteral0._autoRefineOperations: SerializedInternals#typeLiteral0:_autoRefineOperations.
  SerializedInternals.typeLiteral0._shouldStopAfterTurn.context-typeLiteral1.message: SerializedInternals#typeLiteral0:_shouldStopAfterTurn().(context)typeLiteral1:message.
  SerializedInternals.typeLiteral0._shouldStopAfterTurn.context-typeLiteral1.message.typeLiteral2.stopReason: SerializedInternals#typeLiteral0:_shouldStopAfterTurn().(context)typeLiteral1:message.typeLiteral2:stopReason.
  SerializedInternals.typeLiteral0._shouldStopAfterTurn.context-typeLiteral1.message.typeLiteral2.content: SerializedInternals#typeLiteral0:_shouldStopAfterTurn().(context)typeLiteral1:message.typeLiteral2:content.
  SerializedInternals.typeLiteral0._shouldStopAfterTurn.context-typeLiteral1.message.typeLiteral2.role: SerializedInternals#typeLiteral0:_shouldStopAfterTurn().(context)typeLiteral1:message.typeLiteral2:role.
  SerializedInternals.typeLiteral0._shouldStopAfterTurn.context-typeLiteral1.message.typeLiteral2.usage: SerializedInternals#typeLiteral0:_shouldStopAfterTurn().(context)typeLiteral1:message.typeLiteral2:usage.
  SerializedInternals.typeLiteral0._shouldStopAfterTurn.context-typeLiteral1.message.typeLiteral2.timestamp: SerializedInternals#typeLiteral0:_shouldStopAfterTurn().(context)typeLiteral1:message.typeLiteral2:timestamp.
  SerializedInternals.typeLiteral0._shouldStopAfterTurn.context-typeLiteral1.toolResults: SerializedInternals#typeLiteral0:_shouldStopAfterTurn().(context)typeLiteral1:toolResults.
  SerializedInternals.typeLiteral0._shouldStopAfterTurn.context-typeLiteral1.context: SerializedInternals#typeLiteral0:_shouldStopAfterTurn().(context)typeLiteral1:context.
  SerializedInternals.typeLiteral0._shouldStopAfterTurn.context-typeLiteral1.newMessages: SerializedInternals#typeLiteral0:_shouldStopAfterTurn().(context)typeLiteral1:newMessages.
  SerializedInternals.typeLiteral0._runSerializedRefine.options-typeLiteral3.global: SerializedInternals#typeLiteral0:_runSerializedRefine().(options)typeLiteral3:global.
  SerializedInternals.typeLiteral0._consumePendingRequestedRefine: SerializedInternals#typeLiteral0:_consumePendingRequestedRefine().
  SerializedInternals.typeLiteral0._maybeAutoRefine: SerializedInternals#typeLiteral0:_maybeAutoRefine().
  SerializedInternals.typeLiteral0._reviewAutoRefine: SerializedInternals#typeLiteral0:_reviewAutoRefine().
  SerializedInternals.typeLiteral0._reviewAutoRefine.context-typeLiteral6.reason: SerializedInternals#typeLiteral0:_reviewAutoRefine().(context)typeLiteral6:reason.
  SerializedInternals.typeLiteral0._reviewAutoRefine.context-typeLiteral6.turnsSinceLastReview: SerializedInternals#typeLiteral0:_reviewAutoRefine().(context)typeLiteral6:turnsSinceLastReview.
  SerializedInternals.typeLiteral0._planRefine.options-typeLiteral7.global: SerializedInternals#typeLiteral0:_planRefine().(options)typeLiteral7:global.
  SerializedInternals.typeLiteral0._applyRefine.options-typeLiteral8.instructions: SerializedInternals#typeLiteral0:_applyRefine().(options)typeLiteral8:instructions.
  SerializedInternals.typeLiteral0._applyRefine.options-typeLiteral8.global: SerializedInternals#typeLiteral0:_applyRefine().(options)typeLiteral8:global.
  SerializedInternals.typeLiteral0._admitSessionInput.options-typeLiteral9.wake: SerializedInternals#typeLiteral0:_admitSessionInput().(options)typeLiteral9:wake.
  SerializedInternals.typeLiteral0._admitSessionInput.typeLiteral10.accepted: SerializedInternals#typeLiteral0:_admitSessionInput().typeLiteral10:accepted.
  SerializedInternals.typeLiteral0._autoRefineInProgress: SerializedInternals#typeLiteral0:_autoRefineInProgress.
  SerializedInternals.typeLiteral0._disposing: SerializedInternals#typeLiteral0:_disposing.
  SerializedInternals.typeLiteral0._scheduleAutoRefineAfterAgentEnd: SerializedInternals#typeLiteral0:_scheduleAutoRefineAfterAgentEnd().
  SerializedInternals.typeLiteral0._checkCompaction: SerializedInternals#typeLiteral0:_checkCompaction().
  SerializedInternals.typeLiteral0.requestAbort: SerializedInternals#typeLiteral0:requestAbort().
  SerializedInternals.typeLiteral0.abortCompaction: SerializedInternals#typeLiteral0:abortCompaction().
  SerializedInternals.typeLiteral0.abortBranchSummary: SerializedInternals#typeLiteral0:abortBranchSummary().
  SerializedInternals.typeLiteral0._pendingMessageResumeRequested: SerializedInternals#typeLiteral0:_pendingMessageResumeRequested.
  SerializedInternals.typeLiteral0._pendingMessageResumeEpoch: SerializedInternals#typeLiteral0:_pendingMessageResumeEpoch.
  SerializedInternals.typeLiteral0._pendingMessageResumeQueue: SerializedInternals#typeLiteral0:_pendingMessageResumeQueue.
  SerializedInternals.typeLiteral0._schedulePendingMessageResume: SerializedInternals#typeLiteral0:_schedulePendingMessageResume().
  SerializedInternals.typeLiteral0._maybeStartSerializedBackgroundPlan: SerializedInternals#typeLiteral0:_maybeStartSerializedBackgroundPlan.
  SerializedInternals.typeLiteral0._scheduleAutoRefine: SerializedInternals#typeLiteral0:_scheduleAutoRefine().
  SerializedInternals.typeLiteral0._getRequiredRequestAuth: SerializedInternals#typeLiteral0:_getRequiredRequestAuth().
  SerializedInternals.typeLiteral0._getRequiredRequestAuth.Promise.typeLiteral16.headers: SerializedInternals#typeLiteral0:_getRequiredRequestAuth().Promise:typeLiteral16:headers.
  SerializedInternals.typeLiteral0._performCompaction: SerializedInternals#typeLiteral0:_performCompaction().
---
# Module: [`packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts)

## Classes
### `SerializedInternals`
- def: [`packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts:7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L7)
- signature: `type SerializedInternals`
- members:
  - `abortBranchSummary(method)` — [`L56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L56)
  - `abortCompaction(method)` — [`L55`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L55)
  - `requestAbort(method)` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L54)
  - `accepted` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L34)
  - `apiKey` — [`L65`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L65)
  - `content` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L9)
  - `context` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L11)
  - `firstKeptEntryId` — [`L68`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L68)
  - `global` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L15)
  - `global` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L21)
  - `global` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L24)
  - `headers` — [`L65`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L65)
  - `instructions` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L15)
  - `instructions` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L21)
  - `instructions` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L24)
  - `message` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L9)
  - `messages` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L48)
  - `newMessages` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L12)
  - `reason` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L20)
  - `role` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L9)
  - `stopReason` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L9)
  - `summary` — [`L67`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L67)
  - `timestamp` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L9)
  - `tokensBefore` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L69)
  - `toolResults` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L10)
  - `turnsSinceLastReview` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L20)
  - `type` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L48)
  - `usage` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L9)
  - `wake` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L34)
- protocol/private: `_admitSessionInput`[`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L34), `_agentEventQueue`[`L49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L49), `_applyRefine`[`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L22), `_assistantTurnsSinceAutoRefine`[`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L36), `_autoRefineBranchVersion`[`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L39), `_autoRefineInProgress`[`L38`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L38), `_autoRefineOperations`[`L72`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L72), `_autoRefineReviewAbort`[`L50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L50), `_branchSummaryOperation`[`L53`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L53), `_checkCompaction`[`L46`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L46), `_compactAutoRefinePending`[`L62`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L62), `_compactionOperation`[`L52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L52), `_consumePendingRequestedRefine`[`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L18), `_consumeSerializedBackgroundPlan`[`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L16), `_createPreparedTurnAction`[`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L28), `_disposed`[`L44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L44), `_disposing`[`L43`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L43), `_drainPendingRefinementForDisposal`[`L71`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L71), `_getRequiredRequestAuth`[`L65`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L65), `_handleAgentEvent`[`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L48), `_lastAssistantMessage`[`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L47), `_lastAutoRefineReviewAt`[`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L37), `_maybeAutoRefine`[`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L19), `_maybeStartSerializedBackgroundPlan`[`L61`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L61), `_pendingMessageResumeEpoch`[`L58`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L58), `_pendingMessageResumeQueue`[`L59`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L59), `_pendingMessageResumeRequested`[`L57`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L57), `_pendingRequestedRefine`[`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L35), `_performCompaction`[`L66`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L66), `_planRefine`[`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L21), `_refineAbortController`[`L51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L51), `_refineInFlight`[`L40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L40), `_refinePlanInFlight`[`L41`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L41), `_reviewAutoRefine`[`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L20), `_runSerializedAutoRefineReview`[`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L17), `_runSerializedRefine`[`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L15), `_runSerializedRefineCheckpoint`[`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L14), `_scheduleAutoRefine`[`L63`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L63), `_scheduleAutoRefineAfterAgentEnd`[`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L45), `_scheduleAutoRefineAfterCompaction`[`L64`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L64), `_schedulePendingMessageResume`[`L60`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L60), `_serializedPlanInFlight`[`L42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L42), `_serializedRefine`[`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L27), `_shouldStopAfterTurn`[`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L8)
- used by: (2 test-only callers)

## Functions
- `emptyRefinementResult()` — [`L75`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L75)
- `makeCtx(text: string)` — [`L86`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L86)
- `mockSerializedRefine(harness: Harness)` — [`L102`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-serialized-refine.test.ts#L102) — Mock _planRefine and _applyRefine so _runSerializedRefine completes without real LLM calls.


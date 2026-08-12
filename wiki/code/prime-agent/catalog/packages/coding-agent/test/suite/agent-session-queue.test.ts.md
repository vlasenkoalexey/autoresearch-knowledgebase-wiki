---
title: 'Module: packages/coding-agent/test/suite/agent-session-queue.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/agent-session-queue.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/`agent-session-queue.test.ts`/
symbols:
  heartbeatJob: heartbeatJob().
  createAutoRefineHarness: createAutoRefineHarness().
  emptyRefinementResult: emptyRefinementResult().
  AutoRefineInternals: AutoRefineInternals#
  AutoRefineInternals.typeLiteral0._maybeAutoRefine: AutoRefineInternals#typeLiteral0:_maybeAutoRefine().
  agentPromptText: agentPromptText().
  AutoRefineReason: AutoRefineReason#
  AutoRefineInternals.typeLiteral0._assistantTurnsSinceAutoRefine: AutoRefineInternals#typeLiteral0:_assistantTurnsSinceAutoRefine.
  AutoRefineInternals.typeLiteral0._postCompactionContinuationScheduled: AutoRefineInternals#typeLiteral0:_postCompactionContinuationScheduled.
  AutoRefineInternals.typeLiteral0._pendingAutoRefineReview: AutoRefineInternals#typeLiteral0:_pendingAutoRefineReview.
  refinePlanJson: refinePlanJson().
  AutoRefineInternals.typeLiteral0._lastAutoRefineReviewAt: AutoRefineInternals#typeLiteral0:_lastAutoRefineReviewAt.
  AutoRefineInternals.typeLiteral0._compactAutoRefinePending: AutoRefineInternals#typeLiteral0:_compactAutoRefinePending.
  SteeringStopInternals.typeLiteral1._steeringStopPending: SteeringStopInternals#typeLiteral1:_steeringStopPending.
  AutoRefineInternals.typeLiteral0._scheduleAutoRefineAfterAgentEnd: AutoRefineInternals#typeLiteral0:_scheduleAutoRefineAfterAgentEnd().
  AutoRefineInternals.typeLiteral0._schedulePostCompactionContinue: AutoRefineInternals#typeLiteral0:_schedulePostCompactionContinue().
  skipReviewer: skipReviewer.
  AutoRefineInternals.typeLiteral0._scheduleAutoRefineAfterCompaction: AutoRefineInternals#typeLiteral0:_scheduleAutoRefineAfterCompaction().
  SteeringStopInternals: SteeringStopInternals#
  AutoRefineInternals.typeLiteral0._scheduleAutoRefine: AutoRefineInternals#typeLiteral0:_scheduleAutoRefine().
  AutoRefineInternals.typeLiteral0._turnIntervalAutoRefinePending: AutoRefineInternals#typeLiteral0:_turnIntervalAutoRefinePending.
  AutoRefineInternals.typeLiteral0._autoRefineInProgress: AutoRefineInternals#typeLiteral0:_autoRefineInProgress.
  AutoRefineInternals.typeLiteral0._invalidatePendingAutoRefineForBranchChange: AutoRefineInternals#typeLiteral0:_invalidatePendingAutoRefineForBranchChange().
  AutoRefineInternals.typeLiteral0._cancelPostCompactionContinue: AutoRefineInternals#typeLiteral0:_cancelPostCompactionContinue().
  SteeringStopInternals.typeLiteral1._clearQueuedGoalContexts: SteeringStopInternals#typeLiteral1:_clearQueuedGoalContexts().
  AutoRefineInternals.typeLiteral0._autoRefineBranchVersion: AutoRefineInternals#typeLiteral0:_autoRefineBranchVersion.
---
# Module: [`packages/coding-agent/test/suite/agent-session-queue.test.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts)

## Classes
### `AutoRefineInternals`
- def: [`packages/coding-agent/test/suite/agent-session-queue.test.ts:33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L33)
- signature: `type AutoRefineInternals`
- protocol/private: `_assistantTurnsSinceAutoRefine`[`L41`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L41), `_autoRefineBranchVersion`[`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L48), `_autoRefineInProgress`[`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L47), `_cancelPostCompactionContinue`[`L40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L40), `_compactAutoRefinePending`[`L43`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L43), `_invalidatePendingAutoRefineForBranchChange`[`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L39), `_lastAutoRefineReviewAt`[`L42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L42), `_maybeAutoRefine`[`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L34), `_pendingAutoRefineReview`[`L46`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L46), `_postCompactionContinuationScheduled`[`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L45), `_scheduleAutoRefine`[`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L35), `_scheduleAutoRefineAfterAgentEnd`[`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L37), `_scheduleAutoRefineAfterCompaction`[`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L36), `_schedulePostCompactionContinue`[`L38`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L38), `_turnIntervalAutoRefinePending`[`L44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L44)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `AutoRefineReason`
- def: [`packages/coding-agent/test/suite/agent-session-queue.test.ts:31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L31)
- signature: `type AutoRefineReason`
- used by: (3 test-only callers)

### `SteeringStopInternals`
- def: [`packages/coding-agent/test/suite/agent-session-queue.test.ts:51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L51)
- signature: `type SteeringStopInternals`
- protocol/private: `_clearQueuedGoalContexts`[`L53`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L53), `_steeringStopPending`[`L52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L52)
- used by: (1 test-only callers)

## Functions
- `agentPromptText(id: string, body: string)` — [`L80`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L80)
- `createAutoRefineHarness(options?: HarnessOptions | undefined)` — [`L76`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L76)
- `emptyRefinementResult()` — [`L56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L56)
- `heartbeatJob()` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L84)
- `refinePlanJson(summary: string, edits?: unknown[])` — [`L67`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L67)

## Module values
- `skipReviewer` — [`L102`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-queue.test.ts#L102)


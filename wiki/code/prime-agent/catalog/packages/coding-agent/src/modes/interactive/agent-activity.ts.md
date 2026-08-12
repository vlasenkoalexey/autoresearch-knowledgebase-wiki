---
title: 'Module: packages/coding-agent/src/modes/interactive/agent-activity.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/agent-activity.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/`agent-activity.ts`/
symbols:
  AgentActivityTracker.handleEvent: AgentActivityTracker#handleEvent().
  AgentActivityTracker.getStatus: AgentActivityTracker#getStatus().
  AgentActivityTracker: AgentActivityTracker#
  AgentActivityTracker.reset: AgentActivityTracker#reset().
  formatTokenCount: formatTokenCount().
  AgentActivityTracker.activity: AgentActivityTracker#activity.
  AgentActivityStatus.tokens: AgentActivityStatus#tokens.
  AgentActivityStatus.activity: AgentActivityStatus#activity.
  AgentActivityTracker.currentTokens: AgentActivityTracker#currentTokens().
  AgentActivityTracker.estimatedStreamingTokens: AgentActivityTracker#estimatedStreamingTokens().
  AgentActivityTracker.runningToolCount: AgentActivityTracker#runningToolCount.
  AgentActivityTracker.streamingUsageTokens: AgentActivityTracker#streamingUsageTokens.
  AgentActivityTracker.streamingChars: AgentActivityTracker#streamingChars.
  AGENT_ACTIVITY_LABELS: AGENT_ACTIVITY_LABELS.
  AgentActivityStatus.direction: AgentActivityStatus#direction.
  AgentActivityTracker.reportedTokens: AgentActivityTracker#reportedTokens.
  AgentActivity: AgentActivity#
  AgentActivityTracker.completedTokens: AgentActivityTracker#completedTokens.
  AgentActivityStatus: AgentActivityStatus#
  CHARS_PER_TOKEN_ESTIMATE: CHARS_PER_TOKEN_ESTIMATE.
---
# Module: [`packages/coding-agent/src/modes/interactive/agent-activity.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts)

## Classes
### `AgentActivity`
- def: [`packages/coding-agent/src/modes/interactive/agent-activity.ts:4`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L4)
- signature: `type AgentActivity`
- used by: [`activity`](agent-activity.ts.md#AgentActivityTracker.activity), [`activity`](agent-activity.ts.md#AgentActivityStatus.activity), [`AGENT_ACTIVITY_LABELS`](agent-activity.ts.md#AGENT_ACTIVITY_LABELS)

### `AgentActivityStatus`
- def: [`packages/coding-agent/src/modes/interactive/agent-activity.ts:6`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L6)
- signature: `interface AgentActivityStatus`
- members:
  - `activity` — [`L7`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L7)
  - `direction` — [`L9`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L9) — "down" while receiving model output, "up" while sending (request in flight or tool executing).
  - `tokens` — [`L11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L11) — Output tokens accumulated since the user's last message.
- uses (calls/refs, reference-scoped): [`AgentActivity`](agent-activity.ts.md#AgentActivity)
- used by: [`getStatus`](agent-activity.ts.md#AgentActivityTracker.getStatus), [`getConnectionContextUsage`](interactive-mode.ts.md#InteractiveMode.getConnectionContextUsage), [`refreshConnectionContextUsage`](interactive-mode.ts.md#InteractiveMode.refreshConnectionContextUsage), [`getWorkingLoaderMessage`](interactive-mode.ts.md#InteractiveMode.getWorkingLoaderMessage), [`applyOptimisticContextUsage`](interactive-mode.ts.md#InteractiveMode.applyOptimisticContextUsage)  (1 test-only)

### `AgentActivityTracker`
- def: [`packages/coding-agent/src/modes/interactive/agent-activity.ts:30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L30)
- doc: Derives what the agent is doing right now (and how many output tokens it has
- signature: `class AgentActivityTracker`
- members:
  - `currentTokens(method)` — [`L119`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L119)
  - `estimatedStreamingTokens(method)` — [`L132`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L132)
  - `getStatus(method)` — [`L111`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L111)
  - `handleEvent(method)` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L41)
  - `reset(method)` — [`L123`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L123)
  - `activity` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L31)
  - `completedTokens` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L32)
  - `reportedTokens` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L39)
  - `runningToolCount` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L35)
  - `streamingChars` — [`L34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L34)
  - `streamingUsageTokens` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L33)
- uses (calls/refs, reference-scoped): [`role`](../../../../ai/src/types.ts.md#AssistantMessage.role), [`role`](../../../../ai/src/types.ts.md#ToolResultMessage.role), [`role`](../../../../ai/src/types.ts.md#UserMessage.role), [`role`](../../core/messages.ts.md#CustomMessage.role), [`role`](../../core/messages.ts.md#BashExecutionMessage.role), [`role`](../../core/messages.ts.md#BranchSummaryMessage.role), [`role`](../../core/messages.ts.md#CompactionSummaryMessage.role), [`usage`](../../../../ai/src/types.ts.md#AssistantMessage.usage), [`output`](../../../../ai/src/types.ts.md#Usage.output), [`AgentConnectionSessionEvent`](../agent-connection/types.ts.md#AgentConnectionSessionEvent), [`isAgentSessionMessage`](../../core/agent-messages.ts.md#isAgentSessionMessage), [`tokens`](agent-activity.ts.md#AgentActivityStatus.tokens), [`activity`](agent-activity.ts.md#AgentActivityStatus.activity), [`direction`](agent-activity.ts.md#AgentActivityStatus.direction), [`AgentActivity`](agent-activity.ts.md#AgentActivity), [`AgentActivityStatus`](agent-activity.ts.md#AgentActivityStatus), [`CHARS_PER_TOKEN_ESTIMATE`](agent-activity.ts.md#CHARS_PER_TOKEN_ESTIMATE)
- used by: [`interactive-mode.ts`](interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`handleEvent`](interactive-mode.ts.md#InteractiveMode.handleEvent), [`resetCurrentSessionRenderState`](interactive-mode.ts.md#InteractiveMode.resetCurrentSessionRenderState), [`getConnectionContextUsage`](interactive-mode.ts.md#InteractiveMode.getConnectionContextUsage), [`refreshConnectionContextUsage`](interactive-mode.ts.md#InteractiveMode.refreshConnectionContextUsage), [`getWorkingLoaderMessage`](interactive-mode.ts.md#InteractiveMode.getWorkingLoaderMessage), [`applyOptimisticContextUsage`](interactive-mode.ts.md#InteractiveMode.applyOptimisticContextUsage), [`activityTracker`](interactive-mode.ts.md#InteractiveMode.activityTracker)  (9 test-only)

## Functions
- `formatTokenCount(count: number)` — [`L138`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L138)

## Module values
- `AGENT_ACTIVITY_LABELS` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L14)
- `CHARS_PER_TOKEN_ESTIMATE` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/agent-activity.ts#L23) — Fallback estimate for providers that only report usage when the message completes.


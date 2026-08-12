---
title: 'Module: packages/coding-agent/src/core/goals.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/goals.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`goals.ts`/
symbols:
  GoalState.status: GoalState#status.
  goalHostResponse: goalHostResponse().
  GoalState: GoalState#
  createGoalContextMessage: createGoalContextMessage().
  GoalState.tokensUsed: GoalState#tokensUsed.
  emptyGoalState: emptyGoalState().
  GoalState.objective: GoalState#objective.
  GoalState.timeUsedSeconds: GoalState#timeUsedSeconds.
  GoalState.tokenBudget: GoalState#tokenBudget.
  GoalState.active: GoalState#active.
  normalizeGoalState: normalizeGoalState().
  GoalState.continuationsUsed: GoalState#continuationsUsed.
  continuationPrompt: continuationPrompt().
  budgetLimitPrompt: budgetLimitPrompt().
  objectiveUpdatedPrompt: objectiveUpdatedPrompt().
  goalContextPrompt: goalContextPrompt().
  GoalState.lastReason: GoalState#lastReason.
  formatGoalUsage: formatGoalUsage().
  completionBudgetReport: completionBudgetReport().
  GoalHostResponse.typeLiteral1.goal: GoalHostResponse#typeLiteral1:goal.
  GOAL_CONTEXT_CUSTOM_TYPE: GOAL_CONTEXT_CUSTOM_TYPE.
  GoalState.goalId: GoalState#goalId.
  GoalState.lastError: GoalState#lastError.
  goalTokenDeltaForUsage: goalTokenDeltaForUsage().
  GoalStatus: GoalStatus#
  GoalContextDetails: GoalContextDetails#
  validateGoalObjective: validateGoalObjective().
  GOAL_STATE_CUSTOM_TYPE: GOAL_STATE_CUSTOM_TYPE.
  GoalHostResponse: GoalHostResponse#
  isPersistedGoalState: isPersistedGoalState().
  GOAL_CONTEXT_PREVIEW_LABEL: GOAL_CONTEXT_PREVIEW_LABEL.
  SerializedGoal.typeLiteral0.status: SerializedGoal#typeLiteral0:status.
  GoalContextDetails.kind: GoalContextDetails#kind.
  GoalContextKind: GoalContextKind#
  GoalState.updatedAt: GoalState#updatedAt.
  SerializedGoal.typeLiteral0.goal_id: SerializedGoal#typeLiteral0:goal_id.
  GoalHostResponse.typeLiteral1.remaining_tokens: GoalHostResponse#typeLiteral1:remaining_tokens.
  GoalHostResponse.typeLiteral1.completion_budget_report: GoalHostResponse#typeLiteral1:completion_budget_report.
  validateGoalBudget: validateGoalBudget().
  escapeXmlText: escapeXmlText().
  GoalContextDetails.status: GoalContextDetails#status.
  GOAL_SKILL_NAME: GOAL_SKILL_NAME.
  MAX_THREAD_GOAL_OBJECTIVE_CHARS: MAX_THREAD_GOAL_OBJECTIVE_CHARS.
  GoalState.createdAt: GoalState#createdAt.
  SerializedGoal: SerializedGoal#
  SerializedGoal.typeLiteral0.time_used_seconds: SerializedGoal#typeLiteral0:time_used_seconds.
  GoalContextDetails.objective: GoalContextDetails#objective.
  SerializedGoal.typeLiteral0.objective: SerializedGoal#typeLiteral0:objective.
  SerializedGoal.typeLiteral0.token_budget: SerializedGoal#typeLiteral0:token_budget.
  SerializedGoal.typeLiteral0.tokens_used: SerializedGoal#typeLiteral0:tokens_used.
  SerializedGoal.typeLiteral0.created_at: SerializedGoal#typeLiteral0:created_at.
  SerializedGoal.typeLiteral0.updated_at: SerializedGoal#typeLiteral0:updated_at.
  goalTokenDeltaForUsage.usage-typeLiteral5.input: goalTokenDeltaForUsage().(usage)typeLiteral5:input.
  goalTokenDeltaForUsage.usage-typeLiteral5.output: goalTokenDeltaForUsage().(usage)typeLiteral5:output.
  GoalContextDetails.goalId: GoalContextDetails#goalId.
  GoalContextDetails.continuationsUsed: GoalContextDetails#continuationsUsed.
---
# Module: [`packages/coding-agent/src/core/goals.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts)

## Classes
### `GoalContextDetails`
- def: [`packages/coding-agent/src/core/goals.ts:47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L47)
- signature: `interface GoalContextDetails`
- members:
  - `continuationsUsed` — [`L52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L52)
  - `goalId` — [`L49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L49)
  - `kind` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L48)
  - `objective` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L50)
  - `status` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L51)
- uses (calls/refs, reference-scoped): [`GoalStatus`](goals.ts.md#GoalStatus), [`GoalContextKind`](goals.ts.md#GoalContextKind)
- used by: [`injected-prompt-message.ts`](../modes/interactive/components/injected-prompt-message.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-injected-prompt-message.ts), [`createGoalContextMessage`](goals.ts.md#createGoalContextMessage), [`headerText`](../modes/interactive/components/injected-prompt-message.ts.md#InjectedPromptMessageComponent.headerText), [`metaText`](../modes/interactive/components/injected-prompt-message.ts.md#InjectedPromptMessageComponent.metaText), [`InjectedPromptDetails`](../modes/interactive/components/injected-prompt-message.ts.md#InjectedPromptDetails), [`goalLabel`](../modes/interactive/components/injected-prompt-message.ts.md#goalLabel)

### `GoalContextKind`
- def: [`packages/coding-agent/src/core/goals.ts:11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L11)
- signature: `type GoalContextKind`
- used by: [`createGoalContextMessage`](goals.ts.md#createGoalContextMessage), [`goalContextPrompt`](goals.ts.md#goalContextPrompt), [`kind`](goals.ts.md#GoalContextDetails.kind)

### `GoalHostResponse`
- def: [`packages/coding-agent/src/core/goals.ts:41`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L41)
- doc: Reply payload for goal.* host requests from the IPython kernel.
- signature: `type GoalHostResponse`
- members:
  - `completion_budget_report` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L44)
  - `goal` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L42)
  - `remaining_tokens` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L43)
- uses (calls/refs, reference-scoped): [`SerializedGoal`](goals.ts.md#SerializedGoal)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`goalHostResponse`](goals.ts.md#goalHostResponse), [`handleGoalHostRequest`](agent-session.ts.md#AgentSession.handleGoalHostRequest)  (1 test-only)

### `GoalState`
- def: [`packages/coding-agent/src/core/goals.ts:13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L13)
- signature: `interface GoalState`
- members:
  - `active` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L14)
  - `continuationsUsed` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L21)
  - `createdAt` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L22)
  - `goalId` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L16)
  - `lastError` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L25)
  - `lastReason` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L24)
  - `objective` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L17)
  - `status` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L15)
  - `timeUsedSeconds` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L20)
  - `tokenBudget` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L18)
  - `tokensUsed` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L19)
  - `updatedAt` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L23)
- uses (calls/refs, reference-scoped): [`GoalStatus`](goals.ts.md#GoalStatus)
- used by: [`interactive-mode.ts`](../modes/interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`acpUpdatesForSessionEvent`](../modes/acp/acp-events.ts.md#acpUpdatesForSessionEvent), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`_buildRuntime`](agent-session.ts.md#AgentSession._buildRuntime), [`rpc-types.ts`](../modes/rpc/rpc-types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-types.ts), [`AgentConnectionSessionEvent`](../modes/agent-connection/types.ts.md#AgentConnectionSessionEvent), [`goalHostResponse`](goals.ts.md#goalHostResponse), [`_loadPersistedGoalState`](agent-session.ts.md#AgentSession._loadPersistedGoalState), [`<get>goalState`](agent-session.ts.md#AgentSession.-get-goalState), [`abort`](agent-session.ts.md#AgentSession.abort), [`createGoalContextMessage`](goals.ts.md#createGoalContextMessage), [`_executeQueuedSessionCommand`](agent-session.ts.md#AgentSession._executeQueuedSessionCommand), [`_goalState`](agent-session.ts.md#AgentSession._goalState), [`AgentSessionEvent`](agent-session.ts.md#AgentSessionEvent), [`_startGoal`](agent-session.ts.md#AgentSession._startGoal), [`_accountGoalUsageForAssistantMessage`](agent-session.ts.md#AgentSession._accountGoalUsageForAssistantMessage), [`abortForUpdateRestart`](agent-session.ts.md#AgentSession.abortForUpdateRestart), [`_handleGoalSlashCommand`](agent-session.ts.md#AgentSession._handleGoalSlashCommand), [`emptyGoalState`](goals.ts.md#emptyGoalState), [`_runOrQueueGoalContext`](agent-session.ts.md#AgentSession._runOrQueueGoalContext), [`_getGoalContinuationMessages`](agent-session.ts.md#AgentSession._getGoalContinuationMessages), [`_setGoalState`](agent-session.ts.md#AgentSession._setGoalState), [`goalAnnouncementSnapshot`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.goalAnnouncementSnapshot), [`_resumeGoal`](agent-session.ts.md#AgentSession._resumeGoal), [`handleSessionEvent`](../cli/daemon-command.ts.md#DaemonAttachTerminal.handleSessionEvent), [`_completeGoalFromHost`](agent-session.ts.md#AgentSession._completeGoalFromHost), [`_pauseGoal`](agent-session.ts.md#AgentSession._pauseGoal), [`_finishGoalWithError`](agent-session.ts.md#AgentSession._finishGoalWithError), [`formatGoalStatus`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.formatGoalStatus), [`shouldAnnounceGoalUpdate`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.shouldAnnounceGoalUpdate), [`updateGoalTrayTimer`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.updateGoalTrayTimer), [`_finishGoalForTerminalAssistantMessage`](agent-session.ts.md#AgentSession._finishGoalForTerminalAssistantMessage), [`handleGoalUpdate`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleGoalUpdate), [`normalizeGoalState`](goals.ts.md#normalizeGoalState), [`getGoalState`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.getGoalState), [`budgetLimitPrompt`](goals.ts.md#budgetLimitPrompt), [`continuationPrompt`](goals.ts.md#continuationPrompt), [`objectiveUpdatedPrompt`](goals.ts.md#objectiveUpdatedPrompt)  (+15 more; 7 test-only)

### `GoalStatus`
- def: [`packages/coding-agent/src/core/goals.ts:10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L10)
- signature: `type GoalStatus`
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`status`](goals.ts.md#GoalState.status), [`_resumeGoal`](agent-session.ts.md#AgentSession._resumeGoal), [`status`](goals.ts.md#SerializedGoal.typeLiteral0.status), [`status`](goals.ts.md#GoalContextDetails.status)

### `SerializedGoal`
- def: [`packages/coding-agent/src/core/goals.ts:29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L29)
- doc: Goal payload returned to the kernel-side goal skill. Keys are Python-conventional snake_case.
- signature: `type SerializedGoal`
- members:
  - `created_at` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L36)
  - `goal_id` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L30)
  - `objective` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L31)
  - `status` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L32)
  - `time_used_seconds` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L35)
  - `token_budget` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L33)
  - `tokens_used` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L34)
  - `updated_at` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L37)
- uses (calls/refs, reference-scoped): [`GoalStatus`](goals.ts.md#GoalStatus)
- used by: [`goalHostResponse`](goals.ts.md#goalHostResponse), [`goal`](goals.ts.md#GoalHostResponse.typeLiteral1.goal)  (1 test-only)

## Functions
- `budgetLimitPrompt(goal: GoalState)` — [`L232`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L232)
- `completionBudgetReport(goal: GoalState)` — [`L274`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L274)
- `continuationPrompt(goal: GoalState)` — [`L207`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L207)
- `createGoalContextMessage(goal: GoalState, kind: GoalContextKind, images?: ImageContent[] | undefined)` — [`L154`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L154)
- `emptyGoalState()` — [`L55`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L55)
- `escapeXmlText(input: string)` — [`L288`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L288)
- `formatGoalUsage(goal: GoalState)` — [`L182`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L182)
- `goalContextPrompt(goal: GoalState, kind: GoalContextKind)` — [`L192`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L192)
- `goalHostResponse(goal: GoalState, includeCompletionReport: boolean)` — [`L125`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L125)
- `goalTokenDeltaForUsage(usage: { input: number; output: number; })` — [`L96`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L96)
- `isPersistedGoalState(value: unknown)` — [`L100`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L100)
- `normalizeGoalState(goal: GoalState)` — [`L65`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L65)
- `objectiveUpdatedPrompt(goal: GoalState)` — [`L253`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L253)
- `validateGoalBudget(value: number | undefined)` — [`L86`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L86)
- `validateGoalObjective(value: string)` — [`L75`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L75)

## Module values
- `GOAL_CONTEXT_CUSTOM_TYPE` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L5)
- `GOAL_CONTEXT_PREVIEW_LABEL` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L6)
- `GOAL_SKILL_NAME` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L7)
- `GOAL_STATE_CUSTOM_TYPE` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L4)
- `MAX_THREAD_GOAL_OBJECTIVE_CHARS` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L8)
- `input` — [`L96`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L96)
- `output` — [`L96`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/goals.ts#L96)


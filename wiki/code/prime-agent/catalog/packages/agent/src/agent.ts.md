---
title: 'Module: packages/agent/src/agent.ts'
type: catalog
provenance: extracted
module: packages/agent/src/agent.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-agent-core 0.7.2 src/`agent.ts`/
symbols:
  Agent.-get-state: Agent#`<get>state`().
  Agent.-constructor: Agent#`<constructor>`().
  Agent.createLoopConfig: Agent#createLoopConfig().
  Agent.waitForIdle: Agent#waitForIdle().
  Agent.handleRunFailure: Agent#handleRunFailure().
  Agent.continue: Agent#continue().
  Agent.normalizePromptInput: Agent#normalizePromptInput().
  Agent.prompt: Agent#prompt().
  Agent.processEvents: Agent#processEvents().
  Agent._state: Agent#_state.
  DEFAULT_MODEL: DEFAULT_MODEL.
  createMutableAgentState: createMutableAgentState().
  Agent.subscribe: Agent#subscribe().
  Agent.createContextSnapshot: Agent#createContextSnapshot().
  defaultConvertToLlm: defaultConvertToLlm().
  Agent.runPromptMessages: Agent#runPromptMessages().
  Agent: Agent#
  Agent.runWithLifecycle: Agent#runWithLifecycle().
  Agent.followUp: Agent#followUp().
  Agent.abort: Agent#abort().
  Agent.runContinuation: Agent#runContinuation().
  Agent.hasQueuedMessages: Agent#hasQueuedMessages().
  Agent.removeQueuedMessages: Agent#removeQueuedMessages().
  PendingMessageQueue.batches: PendingMessageQueue#batches.
  Agent.activeRun: Agent#activeRun.
  Agent.reset: Agent#reset().
  Agent.steeringQueue: Agent#steeringQueue.
  Agent.followUpQueue: Agent#followUpQueue.
  Agent.steer: Agent#steer().
  Agent.convertToLlm: Agent#convertToLlm.
  PendingMessageQueue.drain: PendingMessageQueue#drain().
  Agent.onPayload: Agent#onPayload.
  Agent.onResponse: Agent#onResponse.
  Agent.getContinuationMessages: Agent#getContinuationMessages.
  Agent.streamFn: Agent#streamFn.
  Agent.finishRun: Agent#finishRun().
  Agent.beforeToolCall: Agent#beforeToolCall.
  Agent.afterToolCall: Agent#afterToolCall.
  Agent.-get-signal: Agent#`<get>signal`().
  QueueMode: QueueMode#
  MutableAgentState: MutableAgentState#
  PendingMessageQueue.enqueue: PendingMessageQueue#enqueue().
  PendingMessageQueue.removeWhere: PendingMessageQueue#removeWhere().
  Agent.-set-steeringMode: Agent#`<set>steeringMode`().
  Agent.-get-steeringMode: Agent#`<get>steeringMode`().
  Agent.-set-followUpMode: Agent#`<set>followUpMode`().
  Agent.-get-followUpMode: Agent#`<get>followUpMode`().
  Agent.clearSteeringQueue: Agent#clearSteeringQueue().
  Agent.clearFollowUpQueue: Agent#clearFollowUpQueue().
  Agent.clearAllQueues: Agent#clearAllQueues().
  Agent.transformContext: Agent#transformContext.
  Agent.transport: Agent#transport.
  Agent.toolExecution: Agent#toolExecution.
  AgentOptions.convertToLlm: AgentOptions#convertToLlm.
  AgentOptions.onPayload: AgentOptions#onPayload.
  AgentOptions.onResponse: AgentOptions#onResponse.
  AgentOptions.beforeToolCall: AgentOptions#beforeToolCall.
  AgentOptions.afterToolCall: AgentOptions#afterToolCall.
  AgentOptions.getContinuationMessages: AgentOptions#getContinuationMessages.
  Agent.sessionId: Agent#sessionId.
  Agent.listeners: Agent#listeners.
  Agent.shouldStopAfterTurn: Agent#shouldStopAfterTurn.
  Agent.thinkingBudgets: Agent#thinkingBudgets.
  PendingMessageQueue.-constructor: PendingMessageQueue#`<constructor>`().
  PendingMessageQueue.hasItems: PendingMessageQueue#hasItems().
  PendingMessageQueue.clear: PendingMessageQueue#clear().
  ActiveRun.typeLiteral60.abortController: ActiveRun#typeLiteral60:abortController.
  Agent.getApiKey: Agent#getApiKey.
  AgentOptions.initialState: AgentOptions#initialState.
  AgentOptions.transformContext: AgentOptions#transformContext.
  AgentOptions.streamFn: AgentOptions#streamFn.
  AgentOptions.shouldStopAfterTurn: AgentOptions#shouldStopAfterTurn.
  AgentOptions.steeringMode: AgentOptions#steeringMode.
  AgentOptions.followUpMode: AgentOptions#followUpMode.
  AgentOptions.thinkingBudgets: AgentOptions#thinkingBudgets.
  AgentOptions.transport: AgentOptions#transport.
  AgentOptions.toolExecution: AgentOptions#toolExecution.
  Agent.shouldStopBeforeTurn: Agent#shouldStopBeforeTurn.
  Agent.maxRetryDelayMs: Agent#maxRetryDelayMs.
  PendingMessageQueue: PendingMessageQueue#
  ActiveRun.typeLiteral60.promise: ActiveRun#typeLiteral60:promise.
  ActiveRun.typeLiteral60.resolve: ActiveRun#typeLiteral60:resolve.
  EMPTY_USAGE: EMPTY_USAGE.
  AgentOptions: AgentOptions#
  AgentOptions.getApiKey: AgentOptions#getApiKey.
  AgentOptions.shouldStopBeforeTurn: AgentOptions#shouldStopBeforeTurn.
  AgentOptions.sessionId: AgentOptions#sessionId.
  AgentOptions.maxRetryDelayMs: AgentOptions#maxRetryDelayMs.
  ActiveRun: ActiveRun#
  Agent.createLoopConfig.options-typeLiteral139.skipInitialSteeringPoll: Agent#createLoopConfig().(options)typeLiteral139:skipInitialSteeringPoll.
  Agent.runPromptMessages.options-typeLiteral118.skipInitialSteeringPoll: Agent#runPromptMessages().(options)typeLiteral118:skipInitialSteeringPoll.
---
# Module: [`packages/agent/src/agent.ts`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts)

## Classes
### `ActiveRun`
- def: [`packages/agent/src/agent.ts:170`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L170)
- signature: `type ActiveRun`
- members:
  - `abortController` — [`L173`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L173)
  - `promise` — [`L171`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L171)
  - `resolve` — [`L172`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L172)
- used by: [`waitForIdle`](agent.ts.md#Agent.waitForIdle), [`processEvents`](agent.ts.md#Agent.processEvents), [`runWithLifecycle`](agent.ts.md#Agent.runWithLifecycle), [`abort`](agent.ts.md#Agent.abort), [`activeRun`](agent.ts.md#Agent.activeRun), [`finishRun`](agent.ts.md#Agent.finishRun), [`<get>signal`](agent.ts.md#Agent.-get-signal)

### `Agent`
- def: [`packages/agent/src/agent.ts:182`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L182)
- doc: Stateful wrapper around the low-level agent loop.
- signature: `class Agent`
- members:
  - `<constructor>(options?: AgentOptions)` — [`L220`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L220) — Stateful wrapper around the low-level agent loop.
  - `<get>followUpMode` — [`L280`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L280) — Controls how queued follow-up messages are drained.
  - `<get>signal` — [`L321`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L321) — Active abort signal for the current run, if any.
  - `<get>state` — [`L262`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L262) — Current agent state.
  - `<get>steeringMode` — [`L271`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L271) — Controls how queued steering messages are drained.
  - `<set>followUpMode` — [`L276`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L276) — Controls how queued follow-up messages are drained.
  - `<set>steeringMode` — [`L267`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L267) — Controls how queued steering messages are drained.
  - `abort(method)` — [`L326`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L326) — Abort the current run, if one is active.
  - `clearAllQueues(method)` — [`L305`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L305) — Remove all queued steering and follow-up messages.
  - `clearFollowUpQueue(method)` — [`L300`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L300) — Remove all queued follow-up messages.
  - `clearSteeringQueue(method)` — [`L295`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L295) — Remove all queued steering messages.
  - `continue(method)` — [`L364`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L364) — Continue from the current transcript. The last message must be a user or tool-result message.
  - `createContextSnapshot(method)` — [`L463`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L463)
  - `createLoopConfig(method)` — [`L471`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L471)
  - `finishRun(method)` — [`L550`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L550)
  - `followUp(method)` — [`L290`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L290) — Queue a message batch to run only after the agent would otherwise stop.
  - `handleRunFailure(method)` — [`L529`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L529)
  - `hasQueuedMessages(method)` — [`L316`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L316) — Returns true when either queue still contains pending messages.
  - `normalizePromptInput(method)` — [`L416`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L416)
  - `processEvents(method)` — [`L565`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L565) — Reduce internal state for a loop event, then await listeners.
  - `prompt(method)` — [`L351`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L351) — Start a new prompt from text, a single message, or a batch of messages.
  - `removeQueuedMessages(method)` — [`L311`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L311) — Remove queued batches containing a message matching the predicate from both queues.
  - `reset(method)` — [`L340`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L340) — Clear transcript state, runtime state, and queued messages.
  - `runContinuation(method)` — [`L451`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L451)
  - `runPromptMessages(method)` — [`L435`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L435)
  - `runWithLifecycle(method)` — [`L504`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L504)
  - `steer(method)` — [`L285`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L285) — Queue a message batch to be injected after the current assistant turn finishes.
  - `subscribe(method)` — [`L252`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L252) — Subscribe to agent lifecycle events.
  - `waitForIdle(method)` — [`L335`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L335) — Resolve when the current run and all awaited event listeners have finished.
  - `activeRun` — [`L208`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L208)
  - `afterToolCall` — [`L198`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L198)
  - `beforeToolCall` — [`L194`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L194)
  - `convertToLlm` — [`L188`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L188)
  - `followUpQueue` — [`L186`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L186)
  - `getApiKey` — [`L191`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L191)
  - `getContinuationMessages` — [`L204`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L204)
  - `listeners` — [`L184`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L184)
  - `maxRetryDelayMs` — [`L216`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L216) — Optional cap for provider-requested retry delays.
  - `onPayload` — [`L192`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L192)
  - `onResponse` — [`L193`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L193)
  - `sessionId` — [`L210`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L210) — Session identifier forwarded to providers for cache-aware backends.
  - `shouldStopAfterTurn` — [`L202`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L202)
  - `shouldStopBeforeTurn` — [`L203`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L203)
  - `skipInitialSteeringPoll` — [`L437`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L437)
  - `skipInitialSteeringPoll` — [`L471`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L471)
  - `steeringQueue` — [`L185`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L185)
  - `streamFn` — [`L190`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L190)
  - `thinkingBudgets` — [`L212`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L212) — Optional per-level thinking token budgets forwarded to the stream function.
  - `toolExecution` — [`L218`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L218) — Tool execution strategy for assistant messages that contain multiple tool calls.
  - `transformContext` — [`L189`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L189)
  - `transport` — [`L214`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L214) — Preferred transport forwarded to the stream function.
- protocol/private: `_state`[`L183`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L183)
- uses (calls/refs, reference-scoped): [`id`](../../ai/src/types.ts.md#Model.id), [`provider`](../../ai/src/types.ts.md#Model.provider), [`api`](../../ai/src/types.ts.md#Model.api), [`role`](../../ai/src/types.ts.md#AssistantMessage.role), [`role`](../../ai/src/types.ts.md#ToolResultMessage.role), [`role`](../../ai/src/types.ts.md#UserMessage.role), [`type`](../../ai/src/types.ts.md#TextContent.type), [`role`](../../coding-agent/src/core/messages.ts.md#CustomMessage.role), [`role`](../../coding-agent/src/core/messages.ts.md#BashExecutionMessage.role), [`role`](../../coding-agent/src/core/messages.ts.md#BranchSummaryMessage.role), [`role`](../../coding-agent/src/core/messages.ts.md#CompactionSummaryMessage.role), [`type`](../../ai/src/types.ts.md#ToolCall.type), [`type`](../../ai/src/types.ts.md#ThinkingContent.type), [`timestamp`](../../ai/src/types.ts.md#AssistantMessage.timestamp), [`AgentMessage`](types.ts.md#AgentMessage), [`timestamp`](../../ai/src/types.ts.md#ToolResultMessage.timestamp), [`timestamp`](../../ai/src/types.ts.md#UserMessage.timestamp), [`type`](../../ai/src/types.ts.md#ImageContent.type), [`timestamp`](../../coding-agent/src/core/messages.ts.md#CustomMessage.timestamp), [`ImageContent`](../../ai/src/types.ts.md#ImageContent), [`timestamp`](../../coding-agent/src/core/messages.ts.md#BashExecutionMessage.timestamp), [`errorMessage`](../../ai/src/types.ts.md#AssistantMessage.errorMessage), [`<get>messages`](types.ts.md#AgentState.-get-messages), [`<set>messages`](types.ts.md#AgentState.-set-messages), [`timestamp`](../../coding-agent/src/core/messages.ts.md#CompactionSummaryMessage.timestamp), [`TextContent`](../../ai/src/types.ts.md#TextContent), [`timestamp`](../../coding-agent/src/core/messages.ts.md#BranchSummaryMessage.timestamp), [`Message`](../../ai/src/types.ts.md#Message), [`SimpleStreamOptions`](../../ai/src/types.ts.md#SimpleStreamOptions), [`AgentEvent`](types.ts.md#AgentEvent), [`streamSimple`](../../ai/src/stream.ts.md#streamSimple), [`messages`](types.ts.md#AgentContext.messages), [`AgentContext`](types.ts.md#AgentContext), [`AgentLoopConfig`](types.ts.md#AgentLoopConfig), [`tools`](types.ts.md#AgentContext.tools), [`model`](types.ts.md#AgentLoopConfig.model), [`convertToLlm`](types.ts.md#AgentLoopConfig.convertToLlm), [`systemPrompt`](types.ts.md#AgentContext.systemPrompt), [`runAgentLoopContinue`](agent-loop.ts.md#runAgentLoopContinue), [`reasoning`](../../ai/src/types.ts.md#SimpleStreamOptions.reasoning)  (+73 more)
- used by: [`agent-session.ts`](../../coding-agent/src/core/agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`handleCommand`](../../coding-agent/src/modes/daemon/daemon-mode.ts.md#AgentDaemon.handleCommand), [`createAgentSession`](../../coding-agent/src/core/sdk.ts.md#createAgentSession), [`agent`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.agent), [`<constructor>`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.-constructor), [`summaryEntry`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`_bindExtensionCore`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._bindExtensionCore), [`_createInlineRlmSubagentRuntime`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._createInlineRlmSubagentRuntime), [`startSideQuestion`](../../coding-agent/src/core/side-question.ts.md#startSideQuestion), [`<get>messages`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.-get-messages), [`_processAgentEvent`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._processAgentEvent), [`_startPreparedTurnActions`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._startPreparedTurnActions), [`dispose`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.dispose), [`sdk.ts`](../../coding-agent/src/core/sdk.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-sdk.ts), [`_pumpSessionInputs`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._pumpSessionInputs), [`signal`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`sendCustomMessage`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.sendCustomMessage), [`_installAgentToolHooks`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._installAgentToolHooks), [`_applyRefine`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._applyRefine), [`_checkCompaction`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._checkCompaction), [`compact`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.compact), [`waitForIdle`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.waitForIdle), [`_cancelSessionActions`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._cancelSessionActions), [`_handleAgentEvent`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._handleAgentEvent), [`<get>model`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.-get-model), [`_runAutoCompaction`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._runAutoCompaction), [`cancelled`](../../coding-agent/src/core/agent-session-runtime.ts.md#AgentSessionRuntime.newSession.Promise.typeLiteral136.cancelled), [`setModel`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.setModel), [`createInteractiveModeLocalSessionHost`](../../coding-agent/src/modes/interactive/interactive-mode-services.ts.md#createInteractiveModeLocalSessionHost), [`refine`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.refine), [`_handleRetryableError`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._handleRetryableError), [`clearQueue`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.clearQueue), [`clearQueuedUserMessagesMatching`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.clearQueuedUserMessagesMatching), [`recordBashResult`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.recordBashResult), [`setRlmMaxDepth`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.setRlmMaxDepth), [`_cycleScopedModel`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._cycleScopedModel), [`requestAbort`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.requestAbort), [`<get>isStreaming`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.-get-isStreaming), [`_notifyKernelStateAfterCompaction`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._notifyKernelStateAfterCompaction), [`_cycleAvailableModel`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._cycleAvailableModel)  (+44 more; 48 test-only)

### `AgentOptions`
- def: [`packages/agent/src/agent.ts:98`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L98)
- doc: Options for constructing an {@link Agent}.
- signature: `interface AgentOptions`
- members:
  - `afterToolCall` — [`L107`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L107)
  - `beforeToolCall` — [`L106`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L106)
  - `convertToLlm` — [`L100`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L100)
  - `followUpMode` — [`L112`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L112)
  - `getApiKey` — [`L103`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L103)
  - `getContinuationMessages` — [`L110`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L110)
  - `initialState` — [`L99`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L99)
  - `maxRetryDelayMs` — [`L116`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L116)
  - `onPayload` — [`L104`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L104)
  - `onResponse` — [`L105`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L105)
  - `sessionId` — [`L113`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L113)
  - `shouldStopAfterTurn` — [`L108`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L108)
  - `shouldStopBeforeTurn` — [`L109`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L109)
  - `steeringMode` — [`L111`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L111)
  - `streamFn` — [`L102`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L102)
  - `thinkingBudgets` — [`L114`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L114)
  - `toolExecution` — [`L117`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L117)
  - `transformContext` — [`L101`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L101)
  - `transport` — [`L115`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L115)
- uses (calls/refs, reference-scoped): [`AgentMessage`](types.ts.md#AgentMessage), [`Message`](../../ai/src/types.ts.md#Message), [`SimpleStreamOptions`](../../ai/src/types.ts.md#SimpleStreamOptions), [`Transport`](../../ai/src/types.ts.md#Transport), [`onResponse`](../../ai/src/types.ts.md#StreamOptions.onResponse), [`onPayload`](../../ai/src/types.ts.md#StreamOptions.onPayload), [`StreamFn`](types.ts.md#StreamFn), [`ShouldStopAfterTurnContext`](types.ts.md#ShouldStopAfterTurnContext), [`ToolExecutionMode`](types.ts.md#ToolExecutionMode), [`ThinkingBudgets`](../../ai/src/types.ts.md#ThinkingBudgets), [`GetContinuationMessagesContext`](types.ts.md#GetContinuationMessagesContext), [`AgentState`](types.ts.md#AgentState), [`QueueMode`](agent.ts.md#QueueMode), [`AfterToolCallContext`](types.ts.md#AfterToolCallContext), [`AfterToolCallResult`](types.ts.md#AfterToolCallResult), [`BeforeToolCallContext`](types.ts.md#BeforeToolCallContext), [`BeforeToolCallResult`](types.ts.md#BeforeToolCallResult)
- used by: [`<constructor>`](agent.ts.md#Agent.-constructor)

### `MutableAgentState`
- def: [`packages/agent/src/agent.ts:60`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L60)
- signature: `type MutableAgentState`
- uses (calls/refs, reference-scoped): [`AgentMessage`](types.ts.md#AgentMessage), [`AgentState`](types.ts.md#AgentState)
- used by: [`_state`](agent.ts.md#Agent._state), [`createMutableAgentState`](agent.ts.md#createMutableAgentState)

### `PendingMessageQueue`
- def: [`packages/agent/src/agent.ts:120`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L120)
- signature: `class PendingMessageQueue`
- members:
  - `<constructor>(mode: QueueMode)` — [`L123`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L123)
  - `clear(method)` — [`L151`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L151)
  - `drain(method)` — [`L136`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L136)
  - `enqueue(method)` — [`L125`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L125)
  - `hasItems(method)` — [`L132`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L132)
  - `removeWhere(method)` — [`L155`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L155)
  - `batches` — [`L121`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L121)
- uses (calls/refs, reference-scoped): [`AgentMessage`](types.ts.md#AgentMessage), [`QueueMode`](agent.ts.md#QueueMode)
- used by: [`<constructor>`](agent.ts.md#Agent.-constructor), [`createLoopConfig`](agent.ts.md#Agent.createLoopConfig), [`continue`](agent.ts.md#Agent.continue), [`followUp`](agent.ts.md#Agent.followUp), [`hasQueuedMessages`](agent.ts.md#Agent.hasQueuedMessages), [`removeQueuedMessages`](agent.ts.md#Agent.removeQueuedMessages), [`followUpQueue`](agent.ts.md#Agent.followUpQueue), [`steer`](agent.ts.md#Agent.steer), [`steeringQueue`](agent.ts.md#Agent.steeringQueue), [`clearFollowUpQueue`](agent.ts.md#Agent.clearFollowUpQueue), [`clearSteeringQueue`](agent.ts.md#Agent.clearSteeringQueue)

### `QueueMode`
- def: [`packages/agent/src/agent.ts:58`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L58)
- signature: `type QueueMode`
- used by: [`<get>followUpMode`](agent.ts.md#Agent.-get-followUpMode), [`<get>steeringMode`](agent.ts.md#Agent.-get-steeringMode), [`<set>followUpMode`](agent.ts.md#Agent.-set-followUpMode), [`<set>steeringMode`](agent.ts.md#Agent.-set-steeringMode), [`<constructor>`](agent.ts.md#PendingMessageQueue.-constructor), [`followUpMode`](agent.ts.md#AgentOptions.followUpMode), [`steeringMode`](agent.ts.md#AgentOptions.steeringMode)

## Functions
- `createMutableAgentState(initialState?: Partial<Omit<AgentState, "errorMessage" | "pendingToolCalls" | "isStreaming" | "streamingMessage">> | undefined)` — [`L67`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L67)
- `defaultConvertToLlm(messages: AgentMessage[])` — [`L30`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L30)

## Module values
- `DEFAULT_MODEL` — [`L45`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L45)
- `EMPTY_USAGE` — [`L36`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent.ts#L36)


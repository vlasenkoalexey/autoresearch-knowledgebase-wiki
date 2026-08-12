---
title: 'Module: packages/agent/src/types.ts'
type: catalog
provenance: extracted
module: packages/agent/src/types.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-agent-core 0.7.2 src/`types.ts`/
symbols:
  AgentMessage: AgentMessage#
  AgentState.-set-messages: AgentState#`<set>messages`().
  AgentState.-get-messages: AgentState#`<get>messages`().
  ThinkingLevel: ThinkingLevel#
  AgentTool.execute: AgentTool#execute.
  AgentTool: AgentTool#
  AgentEvent: AgentEvent#
  AgentContext.messages: AgentContext#messages.
  AgentContext: AgentContext#
  AgentLoopConfig: AgentLoopConfig#
  AgentTool.label: AgentTool#label.
  AgentContext.tools: AgentContext#tools.
  AgentToolResult.details: AgentToolResult#details.
  AgentLoopConfig.model: AgentLoopConfig#model.
  AgentToolResult.content: AgentToolResult#content.
  AgentLoopConfig.convertToLlm: AgentLoopConfig#convertToLlm.
  AgentContext.systemPrompt: AgentContext#systemPrompt.
  AgentState.systemPrompt: AgentState#systemPrompt.
  AgentToolResult: AgentToolResult#
  AgentState.model: AgentState#model.
  ShouldStopAfterTurnContext.message: ShouldStopAfterTurnContext#message.
  AgentState.isStreaming: AgentState#isStreaming.
  AgentState.-set-tools: AgentState#`<set>tools`().
  AgentState.-get-tools: AgentState#`<get>tools`().
  AgentToolCall: AgentToolCall#
  StreamFn: StreamFn#
  AgentState.serviceTier: AgentState#serviceTier.
  ShouldStopAfterTurnContext: ShouldStopAfterTurnContext#
  AgentState.thinkingLevel: AgentState#thinkingLevel.
  ToolExecutionMode: ToolExecutionMode#
  AgentLoopConfig.getSteeringMessages: AgentLoopConfig#getSteeringMessages.
  AgentLoopConfig.getContinuationMessages: AgentLoopConfig#getContinuationMessages.
  ShouldStopAfterTurnContext.context: ShouldStopAfterTurnContext#context.
  AgentLoopConfig.beforeToolCall: AgentLoopConfig#beforeToolCall.
  ShouldStopAfterTurnContext.toolResults: ShouldStopAfterTurnContext#toolResults.
  ShouldStopAfterTurnContext.newMessages: ShouldStopAfterTurnContext#newMessages.
  GetContinuationMessagesContext: GetContinuationMessagesContext#
  AgentLoopConfig.toolExecution: AgentLoopConfig#toolExecution.
  AgentState.streamingMessage: AgentState#streamingMessage.
  AgentToolUpdateCallback: AgentToolUpdateCallback#
  AgentLoopConfig.afterToolCall: AgentLoopConfig#afterToolCall.
  AgentState: AgentState#
  AgentState.errorMessage: AgentState#errorMessage.
  AgentTool.executionMode: AgentTool#executionMode.
  AgentLoopConfig.shouldStopAfterTurn: AgentLoopConfig#shouldStopAfterTurn.
  AgentLoopConfig.getFollowUpMessages: AgentLoopConfig#getFollowUpMessages.
  AgentLoopConfig.transformContext: AgentLoopConfig#transformContext.
  AfterToolCallResult.content: AfterToolCallResult#content.
  AgentLoopConfig.shouldStopBeforeTurn: AgentLoopConfig#shouldStopBeforeTurn.
  AgentState.pendingToolCalls: AgentState#pendingToolCalls.
  AgentTool.prepareArguments: AgentTool#prepareArguments.
  BeforeToolCallContext.toolCall: BeforeToolCallContext#toolCall.
  AfterToolCallContext.toolCall: AfterToolCallContext#toolCall.
  AfterToolCallContext.result: AfterToolCallContext#result.
  BeforeToolCallResult: BeforeToolCallResult#
  AfterToolCallResult: AfterToolCallResult#
  BeforeToolCallContext: BeforeToolCallContext#
  AfterToolCallContext: AfterToolCallContext#
  AgentLoopConfig.getApiKey: AgentLoopConfig#getApiKey.
  BeforeToolCallContext.assistantMessage: BeforeToolCallContext#assistantMessage.
  BeforeToolCallContext.context: BeforeToolCallContext#context.
  AfterToolCallContext.assistantMessage: AfterToolCallContext#assistantMessage.
  AfterToolCallContext.context: AfterToolCallContext#context.
  BeforeToolCallContext.args: BeforeToolCallContext#args.
  AgentLoopConfig.getSystemPrompt: AgentLoopConfig#getSystemPrompt.
  AgentToolResult.terminate: AgentToolResult#terminate.
  AfterToolCallContext.args: AfterToolCallContext#args.
  AfterToolCallContext.isError: AfterToolCallContext#isError.
  CustomAgentMessages: CustomAgentMessages#
  BeforeToolCallResult.block: BeforeToolCallResult#block.
  BeforeToolCallResult.reason: BeforeToolCallResult#reason.
  AfterToolCallResult.details: AfterToolCallResult#details.
  AfterToolCallResult.isError: AfterToolCallResult#isError.
  AfterToolCallResult.terminate: AfterToolCallResult#terminate.
  AgentToolCall.Extract.typeLiteral2.type: AgentToolCall#Extract:typeLiteral2:type.
---
# Module: [`packages/agent/src/types.ts`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts)

## Classes
### `AfterToolCallContext`
- def: [`packages/agent/src/types.ts:89`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L89)
- doc: Context passed to `afterToolCall`.
- signature: `interface AfterToolCallContext`
- members:
  - `args` — [`L95`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L95) — Validated tool arguments for the target tool schema.
  - `assistantMessage` — [`L91`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L91) — The assistant message that requested the tool call.
  - `context` — [`L101`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L101) — Current agent context at the time the tool call is finalized.
  - `isError` — [`L99`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L99) — Whether the executed tool result is currently treated as an error.
  - `result` — [`L97`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L97) — The executed tool result before any `afterToolCall` overrides are applied.
  - `toolCall` — [`L93`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L93) — The raw tool call block from `assistantMessage.content`.
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../ai/src/types.ts.md#AssistantMessage), [`AgentContext`](types.ts.md#AgentContext), [`AgentToolResult`](types.ts.md#AgentToolResult), [`AgentToolCall`](types.ts.md#AgentToolCall)
- used by: [`_installAgentToolHooks`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._installAgentToolHooks), [`agent.ts`](agent.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent.ts), [`finalizeExecutedToolCall`](agent-loop.ts.md#finalizeExecutedToolCall), [`afterToolCall`](types.ts.md#AgentLoopConfig.afterToolCall), [`afterToolCall`](agent.ts.md#Agent.afterToolCall), [`afterToolCall`](agent.ts.md#AgentOptions.afterToolCall)

### `AfterToolCallResult`
- def: [`packages/agent/src/types.ts:65`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L65)
- doc: Partial override returned from `afterToolCall`.
- signature: `interface AfterToolCallResult`
- members:
  - `content` — [`L66`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L66)
  - `details` — [`L67`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L67)
  - `isError` — [`L68`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L68)
  - `terminate` — [`L73`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L73) — Hint that the agent should stop after the current tool batch.
- uses (calls/refs, reference-scoped): [`ImageContent`](../../ai/src/types.ts.md#ImageContent), [`TextContent`](../../ai/src/types.ts.md#TextContent)
- used by: [`agent.ts`](agent.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent.ts), [`finalizeExecutedToolCall`](agent-loop.ts.md#finalizeExecutedToolCall), [`afterToolCall`](types.ts.md#AgentLoopConfig.afterToolCall), [`afterToolCall`](agent.ts.md#Agent.afterToolCall), [`afterToolCall`](agent.ts.md#AgentOptions.afterToolCall)

### `AgentContext`
- def: [`packages/agent/src/types.ts:390`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L390)
- doc: Context snapshot passed into the low-level agent loop.
- signature: `interface AgentContext`
- members:
  - `messages` — [`L394`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L394) — Transcript visible to the model.
  - `systemPrompt` — [`L392`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L392) — System prompt included with the request.
  - `tools` — [`L396`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L396) — Tools available for this run.
- uses (calls/refs, reference-scoped): [`AgentMessage`](types.ts.md#AgentMessage), [`AgentTool`](types.ts.md#AgentTool)
- used by: [`agent-session.ts`](../../coding-agent/src/core/agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`runLoop`](agent-loop.ts.md#runLoop), [`agent.ts`](agent.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent.ts), [`streamAssistantResponse`](agent-loop.ts.md#streamAssistantResponse), [`finalizeExecutedToolCall`](agent-loop.ts.md#finalizeExecutedToolCall), [`executeToolCallsParallel`](agent-loop.ts.md#executeToolCallsParallel), [`executeToolCallsSequential`](agent-loop.ts.md#executeToolCallsSequential), [`agentLoop`](agent-loop.ts.md#agentLoop), [`prepareToolCall`](agent-loop.ts.md#prepareToolCall), [`agentLoopContinue`](agent-loop.ts.md#agentLoopContinue), [`agent-loop.ts`](agent-loop.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent-loop.ts), [`executeToolCalls`](agent-loop.ts.md#executeToolCalls), [`runAgentLoopContinue`](agent-loop.ts.md#runAgentLoopContinue), [`createContextSnapshot`](agent.ts.md#Agent.createContextSnapshot), [`runAgentLoop`](agent-loop.ts.md#runAgentLoop), [`_ensureGoalRuntimeActive`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._ensureGoalRuntimeActive), [`context`](types.ts.md#ShouldStopAfterTurnContext.context), [`context`](types.ts.md#AfterToolCallContext.context), [`context`](types.ts.md#BeforeToolCallContext.context)  (5 test-only)

### `AgentEvent`
- def: [`packages/agent/src/types.ts:406`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L406)
- doc: Events emitted by the Agent for UI updates.
- signature: `type AgentEvent`
- uses (calls/refs, reference-scoped): [`AgentMessage`](types.ts.md#AgentMessage), [`ToolResultMessage`](../../ai/src/types.ts.md#ToolResultMessage), [`AssistantMessageEvent`](../../ai/src/types.ts.md#AssistantMessageEvent)
- used by: [`agent-session.ts`](../../coding-agent/src/core/agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`types.ts`](../../coding-agent/src/modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`_processAgentEvent`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._processAgentEvent), [`_emitExtensionEvent`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._emitExtensionEvent), [`_handleAgentEvent`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._handleAgentEvent), [`rpc-client.ts`](../../coding-agent/src/modes/rpc/rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`rpc-types.ts`](../../coding-agent/src/modes/rpc/rpc-types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-types.ts), [`AgentConnectionSessionEvent`](../../coding-agent/src/modes/agent-connection/types.ts.md#AgentConnectionSessionEvent), [`agent.ts`](agent.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent.ts), [`agentLoop`](agent-loop.ts.md#agentLoop), [`AgentSessionEvent`](../../coding-agent/src/core/agent-session.ts.md#AgentSessionEvent), [`agentLoopContinue`](agent-loop.ts.md#agentLoopContinue), [`agent-loop.ts`](agent-loop.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent-loop.ts), [`processEvents`](agent.ts.md#Agent.processEvents), [`_addLoginGuidanceToAuthError`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._addLoginGuidanceToAuthError), [`subscribe`](agent.ts.md#Agent.subscribe), [`_createRetryPromiseForAgentEnd`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._createRetryPromiseForAgentEnd), [`promptAndWait`](../../coding-agent/src/modes/rpc/rpc-client.ts.md#RpcClient.promptAndWait), [`handleLine`](../../coding-agent/src/modes/rpc/rpc-client.ts.md#RpcClient.handleLine), [`AgentEventSink`](agent-loop.ts.md#AgentEventSink), [`createAgentStream`](agent-loop.ts.md#createAgentStream), [`endAgentStreamOnError`](agent-loop.ts.md#endAgentStreamOnError), [`collectEvents`](../../coding-agent/src/modes/rpc/rpc-client.ts.md#RpcClient.collectEvents), [`RpcEventListener`](../../coding-agent/src/modes/rpc/rpc-client.ts.md#RpcEventListener), [`RpcObservedSessionEvent`](../../coding-agent/src/modes/rpc/rpc-types.ts.md#RpcObservedSessionEvent), [`listeners`](agent.ts.md#Agent.listeners)  (9 test-only)

### `AgentLoopConfig`
- def: [`packages/agent/src/types.ts:119`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L119)
- signature: `interface AgentLoopConfig`
- members:
  - `afterToolCall` — [`L277`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L277) — Called after a tool finishes executing, before `tool_execution_end` and tool-result message events are emitted.
  - `beforeToolCall` — [`L263`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L263) — Called before a tool is executed, after arguments have been validated.
  - `convertToLlm` — [`L148`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L148) — Converts AgentMessage[] to LLM-compatible Message[] before each LLM call.
  - `getApiKey` — [`L183`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L183) — Resolves an API key dynamically for each LLM call.
  - `getContinuationMessages` — [`L244`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L244) — Returns continuation messages when the agent would otherwise stop.
  - `getFollowUpMessages` — [`L230`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L230) — Returns follow-up messages to process after the agent would otherwise stop.
  - `getSteeringMessages` — [`L217`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L217) — Returns steering messages to inject into the conversation mid-run.
  - `getSystemPrompt` — [`L173`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L173) — Resolves the system prompt immediately before each LLM call.
  - `model` — [`L120`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L120)
  - `shouldStopAfterTurn` — [`L195`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L195) — Called after each turn fully completes and `turn_end` has been emitted.
  - `shouldStopBeforeTurn` — [`L204`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L204) — Called synchronously after a completed turn and before polling work for another turn.
  - `toolExecution` — [`L255`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L255) — Tool execution mode.
  - `transformContext` — [`L170`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L170) — Optional transform applied to the context before `convertToLlm`.
- uses (calls/refs, reference-scoped): [`Model`](../../ai/src/types.ts.md#Model), [`AgentMessage`](types.ts.md#AgentMessage), [`Message`](../../ai/src/types.ts.md#Message), [`SimpleStreamOptions`](../../ai/src/types.ts.md#SimpleStreamOptions), [`ShouldStopAfterTurnContext`](types.ts.md#ShouldStopAfterTurnContext), [`ToolExecutionMode`](types.ts.md#ToolExecutionMode), [`GetContinuationMessagesContext`](types.ts.md#GetContinuationMessagesContext), [`AfterToolCallContext`](types.ts.md#AfterToolCallContext), [`AfterToolCallResult`](types.ts.md#AfterToolCallResult), [`BeforeToolCallContext`](types.ts.md#BeforeToolCallContext), [`BeforeToolCallResult`](types.ts.md#BeforeToolCallResult)
- used by: [`createLoopConfig`](agent.ts.md#Agent.createLoopConfig), [`runLoop`](agent-loop.ts.md#runLoop), [`agent.ts`](agent.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent.ts), [`streamAssistantResponse`](agent-loop.ts.md#streamAssistantResponse), [`finalizeExecutedToolCall`](agent-loop.ts.md#finalizeExecutedToolCall), [`executeToolCallsParallel`](agent-loop.ts.md#executeToolCallsParallel), [`executeToolCallsSequential`](agent-loop.ts.md#executeToolCallsSequential), [`createAbortedAssistantMessage`](agent-loop.ts.md#createAbortedAssistantMessage), [`agentLoop`](agent-loop.ts.md#agentLoop), [`prepareToolCall`](agent-loop.ts.md#prepareToolCall), [`agentLoopContinue`](agent-loop.ts.md#agentLoopContinue), [`agent-loop.ts`](agent-loop.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent-loop.ts), [`executeToolCalls`](agent-loop.ts.md#executeToolCalls), [`runAgentLoopContinue`](agent-loop.ts.md#runAgentLoopContinue), [`runAgentLoop`](agent-loop.ts.md#runAgentLoop)  (2 test-only)

### `AgentMessage`
- def: [`packages/agent/src/types.ts:310`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L310) — documented in [packages-agent-src-types.ts](../../../../concepts/packages-agent-src-types.ts.md)
- doc: AgentMessage: Union of LLM messages + custom messages.
- signature: `type AgentMessage`
- uses (calls/refs, reference-scoped): [`Message`](../../ai/src/types.ts.md#Message), [`CustomAgentMessages`](../../coding-agent/src/core/messages.ts.md#CustomAgentMessages), [`CustomAgentMessages`](types.ts.md#CustomAgentMessages)
- used by: [`interactive-mode.ts`](../../coding-agent/src/modes/interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`agent-session.ts`](../../coding-agent/src/core/agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`createAgentSession`](../../coding-agent/src/core/sdk.ts.md#createAgentSession), [`daemon-agent-connection.ts`](../../coding-agent/src/modes/agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](../../coding-agent/src/modes/agent-connection/in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`types.ts`](../../coding-agent/src/core/extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`addMessageToChat`](../../coding-agent/src/modes/interactive/interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`daemon-protocol.ts`](../../coding-agent/src/modes/daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`startSideQuestion`](../../coding-agent/src/core/side-question.ts.md#startSideQuestion), [`<get>messages`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.-get-messages), [`buildConversationComponents`](../../coding-agent/src/modes/interactive/components/conversation-components.ts.md#buildConversationComponents), [`runner.ts`](../../coding-agent/src/core/extensions/runner.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-runner.ts), [`types.ts`](../../coding-agent/src/modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`buildSessionContext`](../../coding-agent/src/core/session-manager.ts.md#buildSessionContext), [`session-manager.ts`](../../coding-agent/src/core/session-manager.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-session-manager.ts), [`DaemonOutbound`](../../coding-agent/src/modes/daemon/daemon-protocol.ts.md#DaemonOutbound), [`_startPreparedTurnActions`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._startPreparedTurnActions), [`sdk.ts`](../../coding-agent/src/core/sdk.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-sdk.ts), [`<get>messages`](types.ts.md#AgentState.-get-messages), [`<set>messages`](types.ts.md#AgentState.-set-messages), [`conversation-components.ts`](../../coding-agent/src/modes/interactive/components/conversation-components.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-conversation-components.ts), [`planRefinement`](../../coding-agent/src/core/refinement/refinement.ts.md#planRefinement), [`_handleAgentEvent`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._handleAgentEvent), [`daemon-session-list.ts`](../../coding-agent/src/modes/daemon/daemon-session-list.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-session-list.ts), [`prepareCompaction`](../../coding-agent/src/core/compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](../../coding-agent/src/core/compaction/branch-summarization.ts.md#getMessageFromEntry), [`rpc-client.ts`](../../coding-agent/src/modes/rpc/rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`convertToLlm`](../../coding-agent/src/core/messages.ts.md#convertToLlm), [`messages`](../../coding-agent/src/core/session-manager.ts.md#SessionContext.messages), [`reviewAutoRefine`](../../coding-agent/src/core/refinement/refinement.ts.md#reviewAutoRefine), [`daemon-command.ts`](../../coding-agent/src/cli/daemon-command.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-daemon-command.ts), [`rpc-types.ts`](../../coding-agent/src/modes/rpc/rpc-types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-types.ts), [`injected-prompt-message.ts`](../../coding-agent/src/modes/interactive/components/injected-prompt-message.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-injected-prompt-message.ts), [`createAgentObserveMessagePreview`](../../coding-agent/src/core/agent-observe.ts.md#createAgentObserveMessagePreview), [`prepareBranchEntries`](../../coding-agent/src/core/compaction/branch-summarization.ts.md#prepareBranchEntries), [`runLoop`](agent-loop.ts.md#runLoop), [`getMessageFromEntry`](../../coding-agent/src/core/compaction/compaction.ts.md#getMessageFromEntry), [`AgentEvent`](types.ts.md#AgentEvent), [`acp-mode.ts`](../../coding-agent/src/modes/acp/acp-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-acp-acp-mode.ts), [`agent.ts`](agent.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent.ts)  (+141 more; 79 test-only)

### `AgentState`
- def: [`packages/agent/src/types.ts:318`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L318)
- doc: Public agent state.
- signature: `interface AgentState`
- members:
  - `<get>messages` — [`L332`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L332) — Conversation transcript. Assigning a new array copies the top-level array. — documented in [packages-agent-src-types.ts](../../../../concepts/packages-agent-src-types.ts.md)
  - `<get>tools` — [`L329`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L329) — Available tools. Assigning a new array copies the top-level array.
  - `<set>messages` — [`L331`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L331) — Conversation transcript. Assigning a new array copies the top-level array. — documented in [packages-agent-src-types.ts](../../../../concepts/packages-agent-src-types.ts.md)
  - `<set>tools` — [`L328`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L328) — Available tools. Assigning a new array copies the top-level array.
  - `errorMessage` — [`L344`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L344) — Error message from the most recent failed or aborted assistant turn, if any.
  - `isStreaming` — [`L338`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L338) — True while the agent is processing a prompt or continuation.
  - `model` — [`L322`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L322) — Active model used for future turns.
  - `pendingToolCalls` — [`L342`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L342) — Tool call ids currently executing.
  - `serviceTier` — [`L326`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L326) — Requested provider service tier for future turns.
  - `streamingMessage` — [`L340`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L340) — Partial assistant message for the current streamed response, if any.
  - `systemPrompt` — [`L320`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L320) — System prompt sent with each model request.
  - `thinkingLevel` — [`L324`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L324) — Requested reasoning level for future turns.
- uses (calls/refs, reference-scoped): [`Model`](../../ai/src/types.ts.md#Model), [`AgentMessage`](types.ts.md#AgentMessage), [`ThinkingLevel`](types.ts.md#ThinkingLevel), [`AgentTool`](types.ts.md#AgentTool), [`ServiceTier`](../../ai/src/types.ts.md#ServiceTier)
- used by: [`agent-session.ts`](../../coding-agent/src/core/agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`createAgentSession`](../../coding-agent/src/core/sdk.ts.md#createAgentSession), [`<constructor>`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.-constructor), [`summaryForActiveSession`](../../coding-agent/src/modes/daemon/daemon-session-list.ts.md#summaryForActiveSession), [`<get>state`](agent.ts.md#Agent.-get-state), [`summaryEntry`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`startSideQuestion`](../../coding-agent/src/core/side-question.ts.md#startSideQuestion), [`<get>messages`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.-get-messages), [`_processAgentEvent`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._processAgentEvent), [`_startPreparedTurnActions`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._startPreparedTurnActions), [`_pumpSessionInputs`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._pumpSessionInputs), [`signal`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`createAgentObserveSummary`](../../coding-agent/src/modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentObserveSummary), [`rlmChildSnapshotForActiveSession`](../../coding-agent/src/modes/daemon/daemon-session-list.ts.md#rlmChildSnapshotForActiveSession), [`sendCustomMessage`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.sendCustomMessage), [`createLoopConfig`](agent.ts.md#Agent.createLoopConfig), [`_applyRefine`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._applyRefine), [`getSessionStats`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.getSessionStats), [`_checkCompaction`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._checkCompaction), [`waitForIdle`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.waitForIdle), [`_cancelSessionActions`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._cancelSessionActions), [`_handleAgentEvent`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._handleAgentEvent), [`<get>model`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.-get-model), [`_runAutoCompaction`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._runAutoCompaction), [`cancelled`](../../coding-agent/src/core/agent-session-runtime.ts.md#AgentSessionRuntime.newSession.Promise.typeLiteral136.cancelled), [`setModel`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.setModel), [`_handleRetryableError`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._handleRetryableError), [`agent.ts`](agent.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent.ts), [`recordBashResult`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.recordBashResult), [`setRlmMaxDepth`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.setRlmMaxDepth), [`exportSessionToHtml`](../../coding-agent/src/core/export-html/index.ts.md#exportSessionToHtml), [`_cycleScopedModel`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._cycleScopedModel), [`handleRunFailure`](agent.ts.md#Agent.handleRunFailure), [`<get>isStreaming`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.-get-isStreaming), [`summarize`](../../coding-agent/src/modes/daemon/daemon-session-summarizer.ts.md#DaemonSessionSummarizer.summarize), [`_notifyKernelStateAfterCompaction`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._notifyKernelStateAfterCompaction), [`waitForHeadlessCompletion`](../../coding-agent/src/modes/headless-completion.ts.md#waitForHeadlessCompletion), [`_cycleAvailableModel`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._cycleAvailableModel), [`_planRefine`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._planRefine), [`extendResourcesFromExtensions`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.extendResourcesFromExtensions)  (+32 more; 24 test-only)

### `AgentTool`
- def: [`packages/agent/src/types.ts:364`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L364)
- doc: Tool definition used by the agent runtime.
- signature: `interface AgentTool`
- members:
  - `execute` — [`L373`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L373) — Execute the tool call. Throw on failure instead of encoding errors in `content`.
  - `executionMode` — [`L386`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L386) — Per-tool execution mode override.
  - `label` — [`L366`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L366) — Human-readable label for UI display.
  - `prepareArguments` — [`L371`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L371) — Optional compatibility shim for raw tool-call arguments before schema validation.
- uses (calls/refs, reference-scoped): [`Tool`](../../ai/src/types.ts.md#Tool), [`AgentToolResult`](types.ts.md#AgentToolResult), [`ToolExecutionMode`](types.ts.md#ToolExecutionMode), [`AgentToolUpdateCallback`](types.ts.md#AgentToolUpdateCallback)
- used by: [`agent-session.ts`](../../coding-agent/src/core/agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`bash.ts`](../../coding-agent/src/core/tools/bash.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-bash.ts), [`index.ts`](../../coding-agent/src/core/tools/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`edit.ts`](../../coding-agent/src/core/tools/edit.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-edit.ts), [`ipython.ts`](../../coding-agent/src/core/tools/ipython.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-ipython.ts), [`_refreshToolRegistry`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._refreshToolRegistry), [`agent.ts`](agent.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent.ts), [`AgentContext`](types.ts.md#AgentContext), [`wrapToolDefinition`](../../coding-agent/src/core/tools/tool-definition-wrapper.ts.md#wrapToolDefinition), [`agent-loop.ts`](agent-loop.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent-loop.ts), [`createBashTool`](../../coding-agent/src/core/tools/bash.ts.md#createBashTool), [`createToolDefinitionFromAgentTool`](../../coding-agent/src/core/tools/tool-definition-wrapper.ts.md#createToolDefinitionFromAgentTool), [`executeToolCalls`](agent-loop.ts.md#executeToolCalls), [`executePreparedToolCall`](agent-loop.ts.md#executePreparedToolCall), [`createMutableAgentState`](agent.ts.md#createMutableAgentState), [`setActiveToolsByName`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.setActiveToolsByName), [`createEditTool`](../../coding-agent/src/core/tools/edit.ts.md#createEditTool), [`wrapper.ts`](../../coding-agent/src/core/extensions/wrapper.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-wrapper.ts), [`wrapRegisteredTools`](../../coding-agent/src/core/extensions/wrapper.ts.md#wrapRegisteredTools), [`createIpythonTool`](../../coding-agent/src/core/tools/ipython.ts.md#createIpythonTool), [`tool-definition-wrapper.ts`](../../coding-agent/src/core/tools/tool-definition-wrapper.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-tool-definition-wrapper.ts), [`wrapRegisteredTool`](../../coding-agent/src/core/extensions/wrapper.ts.md#wrapRegisteredTool), [`<get>tools`](types.ts.md#AgentState.-get-tools), [`<set>tools`](types.ts.md#AgentState.-set-tools), [`wrapToolDefinitions`](../../coding-agent/src/core/tools/tool-definition-wrapper.ts.md#wrapToolDefinitions), [`prepareToolCallArguments`](agent-loop.ts.md#prepareToolCallArguments), [`_toolRegistry`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._toolRegistry), [`_baseToolsOverride`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._baseToolsOverride), [`baseToolsOverride`](../../coding-agent/src/core/agent-session.ts.md#AgentSessionConfig.baseToolsOverride), [`Tool`](../../coding-agent/src/core/tools/index.ts.md#Tool), [`tool`](agent-loop.ts.md#PreparedToolCall.typeLiteral278.tool)  (38 test-only)

### `AgentToolCall`
- def: [`packages/agent/src/types.ts:40`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L40)
- doc: A single tool call content block emitted by an assistant message.
- signature: `type AgentToolCall`
- members:
  - `type` — [`L40`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L40)
- uses (calls/refs, reference-scoped): [`content`](../../ai/src/types.ts.md#AssistantMessage.content), [`AssistantMessage`](../../ai/src/types.ts.md#AssistantMessage)
- used by: [`executeToolCallsParallel`](agent-loop.ts.md#executeToolCallsParallel), [`executeToolCallsSequential`](agent-loop.ts.md#executeToolCallsSequential), [`prepareToolCall`](agent-loop.ts.md#prepareToolCall), [`agent-loop.ts`](agent-loop.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent-loop.ts), [`prepareToolCallArguments`](agent-loop.ts.md#prepareToolCallArguments), [`toolCall`](agent-loop.ts.md#FinalizedToolCallOutcome.typeLiteral280.toolCall), [`toolCall`](agent-loop.ts.md#PreparedToolCall.typeLiteral278.toolCall), [`toolCall`](types.ts.md#AfterToolCallContext.toolCall), [`toolCall`](types.ts.md#BeforeToolCallContext.toolCall)

### `AgentToolResult`
- def: [`packages/agent/src/types.ts:348`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L348)
- doc: Final or partial result produced by a tool.
- signature: `interface AgentToolResult`
- members:
  - `content` — [`L350`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L350) — Text or image content returned to the model.
  - `details` — [`L352`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L352) — Arbitrary structured details for logs or UI rendering.
  - `terminate` — [`L357`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L357) — Hint that the agent should stop after the current tool batch.
- uses (calls/refs, reference-scoped): [`ImageContent`](../../ai/src/types.ts.md#ImageContent), [`TextContent`](../../ai/src/types.ts.md#TextContent)
- used by: [`index.ts`](../../coding-agent/src/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../../coding-agent/src/core/extensions/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-index.ts), [`index.ts`](../../coding-agent/src/core/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`types.ts`](../../coding-agent/src/core/extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`createBashToolDefinition`](../../coding-agent/src/core/tools/bash.ts.md#createBashToolDefinition), [`createIpythonToolDefinition`](../../coding-agent/src/core/tools/ipython.ts.md#createIpythonToolDefinition), [`execute`](types.ts.md#AgentTool.execute), [`_installAgentToolHooks`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._installAgentToolHooks), [`tool-execution.ts`](../../coding-agent/src/modes/interactive/components/tool-execution.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-tool-execution.ts), [`finalizeExecutedToolCall`](agent-loop.ts.md#finalizeExecutedToolCall), [`mountRenderers`](../../coding-agent/src/modes/interactive/components/tool-execution.ts.md#ToolExecutionComponent.mountRenderers), [`execute`](../../coding-agent/src/core/extensions/types.ts.md#ToolDefinition.execute), [`agent-loop.ts`](agent-loop.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent-loop.ts), [`createToolResultMessage`](agent-loop.ts.md#createToolResultMessage), [`renderResult`](../../coding-agent/src/core/extensions/types.ts.md#ToolDefinition.renderResult), [`createErrorToolResult`](agent-loop.ts.md#createErrorToolResult), [`renderResult`](../../coding-agent/src/modes/interactive/components/tool-execution.ts.md#ToolExecutionRendererDefinition.renderResult), [`AgentToolUpdateCallback`](types.ts.md#AgentToolUpdateCallback), [`shouldTerminateToolBatch`](agent-loop.ts.md#shouldTerminateToolBatch), [`result`](agent-loop.ts.md#FinalizedToolCallOutcome.typeLiteral280.result), [`result`](agent-loop.ts.md#ImmediateToolCallOutcome.typeLiteral279.result), [`result`](types.ts.md#AfterToolCallContext.result), [`result`](agent-loop.ts.md#ExecutedToolCallOutcome.typeLiteral322.result)  (23 test-only)

### `AgentToolUpdateCallback`
- def: [`packages/agent/src/types.ts:361`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L361)
- doc: Callback used by tools to stream partial execution updates.
- signature: `type AgentToolUpdateCallback`
- uses (calls/refs, reference-scoped): [`AgentToolResult`](types.ts.md#AgentToolResult)
- used by: [`index.ts`](../../coding-agent/src/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../../coding-agent/src/core/extensions/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-index.ts), [`index.ts`](../../coding-agent/src/core/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`types.ts`](../../coding-agent/src/core/extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`execute`](types.ts.md#AgentTool.execute), [`execute`](../../coding-agent/src/core/extensions/types.ts.md#ToolDefinition.execute)

### `BeforeToolCallContext`
- def: [`packages/agent/src/types.ts:77`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L77)
- doc: Context passed to `beforeToolCall`.
- signature: `interface BeforeToolCallContext`
- members:
  - `args` — [`L83`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L83) — Validated tool arguments for the target tool schema.
  - `assistantMessage` — [`L79`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L79) — The assistant message that requested the tool call.
  - `context` — [`L85`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L85) — Current agent context at the time the tool call is prepared.
  - `toolCall` — [`L81`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L81) — The raw tool call block from `assistantMessage.content`.
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../ai/src/types.ts.md#AssistantMessage), [`AgentContext`](types.ts.md#AgentContext), [`AgentToolCall`](types.ts.md#AgentToolCall)
- used by: [`_installAgentToolHooks`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._installAgentToolHooks), [`agent.ts`](agent.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent.ts), [`prepareToolCall`](agent-loop.ts.md#prepareToolCall), [`beforeToolCall`](types.ts.md#AgentLoopConfig.beforeToolCall), [`beforeToolCall`](agent.ts.md#Agent.beforeToolCall), [`beforeToolCall`](agent.ts.md#AgentOptions.beforeToolCall)  (1 test-only)

### `BeforeToolCallResult`
- def: [`packages/agent/src/types.ts:48`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L48)
- doc: Result returned from `beforeToolCall`.
- signature: `interface BeforeToolCallResult`
- members:
  - `block` — [`L49`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L49)
  - `reason` — [`L50`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L50)
- used by: [`agent.ts`](agent.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent.ts), [`prepareToolCall`](agent-loop.ts.md#prepareToolCall), [`beforeToolCall`](types.ts.md#AgentLoopConfig.beforeToolCall), [`beforeToolCall`](agent.ts.md#Agent.beforeToolCall), [`beforeToolCall`](agent.ts.md#AgentOptions.beforeToolCall)

### `CustomAgentMessages`
- def: [`packages/agent/src/types.ts:301`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L301)
- doc: Extensible interface for custom app messages.
- signature: `interface CustomAgentMessages`
- used by: [`AgentMessage`](types.ts.md#AgentMessage)

### `GetContinuationMessagesContext`
- def: [`packages/agent/src/types.ts:117`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L117)
- doc: Context passed to `getContinuationMessages`.
- signature: `type GetContinuationMessagesContext`
- uses (calls/refs, reference-scoped): [`ShouldStopAfterTurnContext`](types.ts.md#ShouldStopAfterTurnContext)
- used by: [`agent-session.ts`](../../coding-agent/src/core/agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`agent.ts`](agent.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent.ts), [`_getContinuationMessages`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._getContinuationMessages), [`_getGoalContinuationMessages`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._getGoalContinuationMessages), [`getContinuationMessages`](types.ts.md#AgentLoopConfig.getContinuationMessages), [`getContinuationMessages`](agent.ts.md#Agent.getContinuationMessages), [`getContinuationMessages`](agent.ts.md#AgentOptions.getContinuationMessages)

### `ShouldStopAfterTurnContext`
- def: [`packages/agent/src/types.ts:105`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L105)
- doc: Context passed to `shouldStopAfterTurn`.
- signature: `interface ShouldStopAfterTurnContext`
- members:
  - `context` — [`L111`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L111) — Current agent context after the turn's assistant message and tool results have been appended.
  - `message` — [`L107`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L107) — The assistant message that completed the turn.
  - `newMessages` — [`L113`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L113) — Messages that this loop invocation will return if it exits at this point. Prompt runs include the initial prompt messages; continuation runs do not include pre-existing context messages.
  - `toolResults` — [`L109`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L109) — Tool result messages passed to the preceding `turn_end` event.
- uses (calls/refs, reference-scoped): [`AgentMessage`](types.ts.md#AgentMessage), [`AssistantMessage`](../../ai/src/types.ts.md#AssistantMessage), [`ToolResultMessage`](../../ai/src/types.ts.md#ToolResultMessage), [`AgentContext`](types.ts.md#AgentContext)
- used by: [`agent-session.ts`](../../coding-agent/src/core/agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`runLoop`](agent-loop.ts.md#runLoop), [`agent.ts`](agent.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent.ts), [`_getContinuationMessages`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._getContinuationMessages), [`_shouldStopAfterTurn`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._shouldStopAfterTurn), [`_thresholdCompactionNeeded`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._thresholdCompactionNeeded), [`_shouldStopForThresholdCompaction`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._shouldStopForThresholdCompaction), [`_getGoalContinuationMessages`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._getGoalContinuationMessages), [`GetContinuationMessagesContext`](types.ts.md#GetContinuationMessagesContext), [`shouldStopAfterTurn`](types.ts.md#AgentLoopConfig.shouldStopAfterTurn), [`shouldStopAfterTurn`](agent.ts.md#Agent.shouldStopAfterTurn), [`shouldStopAfterTurn`](agent.ts.md#AgentOptions.shouldStopAfterTurn)  (6 test-only)

### `StreamFn`
- def: [`packages/agent/src/types.ts:25`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L25)
- doc: Stream function used by the agent loop.
- signature: `type StreamFn`
- uses (calls/refs, reference-scoped): [`streamSimple`](../../ai/src/stream.ts.md#streamSimple)
- used by: [`runLoop`](agent-loop.ts.md#runLoop), [`agent.ts`](agent.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent.ts), [`streamAssistantResponse`](agent-loop.ts.md#streamAssistantResponse), [`agentLoop`](agent-loop.ts.md#agentLoop), [`agentLoopContinue`](agent-loop.ts.md#agentLoopContinue), [`agent-loop.ts`](agent-loop.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent-loop.ts), [`runAgentLoopContinue`](agent-loop.ts.md#runAgentLoopContinue), [`runAgentLoop`](agent-loop.ts.md#runAgentLoop), [`streamFn`](agent.ts.md#Agent.streamFn), [`streamFn`](agent.ts.md#AgentOptions.streamFn)  (1 test-only)

### `ThinkingLevel`
- def: [`packages/agent/src/types.ts:285`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L285) — documented in [packages-agent-src-types.ts](../../../../concepts/packages-agent-src-types.ts.md)
- doc: Thinking/reasoning level for models that support it.
- signature: `type ThinkingLevel`
- used by: [`interactive-mode.ts`](../../coding-agent/src/modes/interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`agent-session.ts`](../../coding-agent/src/core/agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`createAgentSession`](../../coding-agent/src/core/sdk.ts.md#createAgentSession), [`DaemonCommand`](../../coding-agent/src/modes/daemon/daemon-protocol.ts.md#DaemonCommand), [`daemon-agent-connection.ts`](../../coding-agent/src/modes/agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](../../coding-agent/src/modes/agent-connection/in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`types.ts`](../../coding-agent/src/core/extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`daemon-protocol.ts`](../../coding-agent/src/modes/daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`types.ts`](../../coding-agent/src/modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`<constructor>`](../../coding-agent/src/modes/interactive/components/settings-selector.ts.md#SettingsSelectorComponent.-constructor), [`sdk.ts`](../../coding-agent/src/core/sdk.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-sdk.ts), [`agent-session-services.ts`](../../coding-agent/src/core/agent-session-services.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-services.ts), [`planRefinement`](../../coding-agent/src/core/refinement/refinement.ts.md#planRefinement), [`model`](../../coding-agent/src/core/agent-session.ts.md#AgentSession._createRlmSubagentRuntimeOptions.options-typeLiteral3607.model), [`modelRegistry`](../../coding-agent/src/core/model-resolver.ts.md#findInitialModel.options-typeLiteral257.modelRegistry), [`daemon-session-list.ts`](../../coding-agent/src/modes/daemon/daemon-session-list.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-session-list.ts), [`rpc-client.ts`](../../coding-agent/src/modes/rpc/rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`reviewAutoRefine`](../../coding-agent/src/core/refinement/refinement.ts.md#reviewAutoRefine), [`rpc-types.ts`](../../coding-agent/src/modes/rpc/rpc-types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-types.ts), [`AgentConnectionSessionEvent`](../../coding-agent/src/modes/agent-connection/types.ts.md#AgentConnectionSessionEvent), [`compaction.ts`](../../coding-agent/src/core/compaction/compaction.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-compaction-compaction.ts), [`settings-selector.ts`](../../coding-agent/src/modes/interactive/components/settings-selector.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-settings-selector.ts), [`compact`](../../coding-agent/src/core/compaction/compaction.ts.md#compact), [`model-resolver.ts`](../../coding-agent/src/core/model-resolver.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-model-resolver.ts), [`AgentSessionEvent`](../../coding-agent/src/core/agent-session.ts.md#AgentSessionEvent), [`refineHarness`](../../coding-agent/src/core/refinement/refinement.ts.md#refineHarness), [`generateSummary`](../../coding-agent/src/core/compaction/compaction.ts.md#generateSummary), [`RpcResponse`](../../coding-agent/src/modes/rpc/rpc-types.ts.md#RpcResponse), [`setThinkingLevel`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.setThinkingLevel), [`resolveModelScopeFromModels`](../../coding-agent/src/core/model-resolver.ts.md#resolveModelScopeFromModels), [`rlm-runtime.ts`](../../coding-agent/src/core/rlm-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-rlm-runtime.ts), [`generateTurnPrefixSummary`](../../coding-agent/src/core/compaction/compaction.ts.md#generateTurnPrefixSummary), [`refinement.ts`](../../coding-agent/src/core/refinement/refinement.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-refinement-refinement.ts), [`thinking-selector.ts`](../../coding-agent/src/modes/interactive/components/thinking-selector.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-thinking-selector.ts), [`<constructor>`](../../coding-agent/src/modes/interactive/components/thinking-selector.ts.md#ThinkingSelectorComponent.-constructor), [`agent-session-config.ts`](../../coding-agent/src/core/agent-session-config.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-config.ts), [`showThinkingSelector`](../../coding-agent/src/modes/interactive/interactive-mode.ts.md#InteractiveMode.showThinkingSelector), [`<get>thinkingLevel`](../../coding-agent/src/core/agent-session.ts.md#AgentSession.-get-thinkingLevel), [`applyThinkingLevel`](../../coding-agent/src/modes/interactive/interactive-mode.ts.md#InteractiveMode.applyThinkingLevel), [`thinkingLevel`](../../coding-agent/src/core/model-resolver.ts.md#ParsedModelResult.thinkingLevel)  (+56 more; 12 test-only)

### `ToolExecutionMode`
- def: [`packages/agent/src/types.ts:37`](../../../../../../../raw/code/prime-agent/packages/agent/src/types.ts#L37)
- doc: Configuration for how tool calls from a single assistant message are executed.
- signature: `type ToolExecutionMode`
- used by: [`index.ts`](../../coding-agent/src/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../../coding-agent/src/core/extensions/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-index.ts), [`types.ts`](../../coding-agent/src/core/extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`agent.ts`](agent.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent.ts), [`toolExecution`](types.ts.md#AgentLoopConfig.toolExecution), [`executionMode`](types.ts.md#AgentTool.executionMode), [`executionMode`](../../coding-agent/src/core/extensions/types.ts.md#ToolDefinition.executionMode), [`toolExecution`](agent.ts.md#Agent.toolExecution), [`toolExecution`](agent.ts.md#AgentOptions.toolExecution)  (1 test-only)


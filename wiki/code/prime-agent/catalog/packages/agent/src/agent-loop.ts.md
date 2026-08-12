---
title: 'Module: packages/agent/src/agent-loop.ts'
type: catalog
provenance: extracted
module: packages/agent/src/agent-loop.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-agent-core 0.7.2 src/`agent-loop.ts`/
symbols:
  runLoop: runLoop().
  streamAssistantResponse: streamAssistantResponse().
  finalizeExecutedToolCall: finalizeExecutedToolCall().
  executeToolCallsParallel: executeToolCallsParallel().
  executeToolCallsSequential: executeToolCallsSequential().
  createAbortedAssistantMessage: createAbortedAssistantMessage().
  agentLoop: agentLoop().
  prepareToolCall: prepareToolCall().
  agentLoopContinue: agentLoopContinue().
  createToolResultMessage: createToolResultMessage().
  executeToolCalls: executeToolCalls().
  runAgentLoopContinue: runAgentLoopContinue().
  executePreparedToolCall: executePreparedToolCall().
  EMPTY_USAGE: EMPTY_USAGE.
  runAgentLoop: runAgentLoop().
  emitToolExecutionEnd: emitToolExecutionEnd().
  createErrorToolResult: createErrorToolResult().
  cloneAssistantContent: cloneAssistantContent().
  maybePromiseWithAbort: maybePromiseWithAbort().
  AgentEventSink: AgentEventSink#
  endAgentStreamOnError: endAgentStreamOnError().
  createAgentStream: createAgentStream().
  prepareToolCallArguments: prepareToolCallArguments().
  shouldTerminateToolBatch: shouldTerminateToolBatch().
  settlePostTurn: settlePostTurn().
  FinalizedToolCallOutcome: FinalizedToolCallOutcome#
  cloneUsage: cloneUsage().
  PreparedToolCall.typeLiteral278.toolCall: PreparedToolCall#typeLiteral278:toolCall.
  FinalizedToolCallOutcome.typeLiteral280.toolCall: FinalizedToolCallOutcome#typeLiteral280:toolCall.
  FinalizedToolCallOutcome.typeLiteral280.result: FinalizedToolCallOutcome#typeLiteral280:result.
  pollMessagesUnlessAborted: pollMessagesUnlessAborted().
  raceWithAbort: raceWithAbort().
  emitToolResultMessage: emitToolResultMessage().
  throwIfAborted: throwIfAborted().
  isAbortError: isAbortError().
  getTerminalMessage: getTerminalMessage().
  createAbortError: createAbortError().
  ImmediateToolCallOutcome.typeLiteral279.result: ImmediateToolCallOutcome#typeLiteral279:result.
  FinalizedToolCallOutcome.typeLiteral280.isError: FinalizedToolCallOutcome#typeLiteral280:isError.
  ExecutedToolCallBatch.typeLiteral140.messages: ExecutedToolCallBatch#typeLiteral140:messages.
  PreparedToolCall.typeLiteral278.tool: PreparedToolCall#typeLiteral278:tool.
  ExecutedToolCallOutcome.typeLiteral322.result: ExecutedToolCallOutcome#typeLiteral322:result.
  FinalizedToolCallEntry: FinalizedToolCallEntry#
  ABORT_ERROR_MESSAGE: ABORT_ERROR_MESSAGE.
  ExecutedToolCallBatch: ExecutedToolCallBatch#
  PreparedToolCall: PreparedToolCall#
  PostTurnResult: PostTurnResult#
  PreparedToolCall.typeLiteral278.kind: PreparedToolCall#typeLiteral278:kind.
  PreparedToolCall.typeLiteral278.args: PreparedToolCall#typeLiteral278:args.
  ImmediateToolCallOutcome.typeLiteral279.kind: ImmediateToolCallOutcome#typeLiteral279:kind.
  ImmediateToolCallOutcome.typeLiteral279.isError: ImmediateToolCallOutcome#typeLiteral279:isError.
  ExecutedToolCallOutcome: ExecutedToolCallOutcome#
  ExecutedToolCallBatch.typeLiteral140.terminate: ExecutedToolCallBatch#typeLiteral140:terminate.
  ImmediateToolCallOutcome: ImmediateToolCallOutcome#
  ExecutedToolCallOutcome.typeLiteral322.isError: ExecutedToolCallOutcome#typeLiteral322:isError.
  getTerminalMessage.event-Extract.typeLiteral35.type: getTerminalMessage().(event)Extract:typeLiteral35:type.
---
# Module: [`packages/agent/src/agent-loop.ts`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts)

## Classes
### `AgentEventSink`
- def: [`packages/agent/src/agent-loop.ts:26`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L26)
- signature: `type AgentEventSink`
- uses (calls/refs, reference-scoped): [`AgentEvent`](types.ts.md#AgentEvent)
- used by: [`runLoop`](agent-loop.ts.md#runLoop), [`streamAssistantResponse`](agent-loop.ts.md#streamAssistantResponse), [`executeToolCallsParallel`](agent-loop.ts.md#executeToolCallsParallel), [`executeToolCallsSequential`](agent-loop.ts.md#executeToolCallsSequential), [`executeToolCalls`](agent-loop.ts.md#executeToolCalls), [`runAgentLoopContinue`](agent-loop.ts.md#runAgentLoopContinue), [`executePreparedToolCall`](agent-loop.ts.md#executePreparedToolCall), [`runAgentLoop`](agent-loop.ts.md#runAgentLoop), [`emitToolExecutionEnd`](agent-loop.ts.md#emitToolExecutionEnd), [`emitToolResultMessage`](agent-loop.ts.md#emitToolResultMessage)

### `ExecutedToolCallBatch`
- def: [`packages/agent/src/agent-loop.ts:625`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L625)
- signature: `type ExecutedToolCallBatch`
- members:
  - `messages` — [`L626`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L626)
  - `terminate` — [`L627`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L627)
- uses (calls/refs, reference-scoped): [`ToolResultMessage`](../../ai/src/types.ts.md#ToolResultMessage)
- used by: [`runLoop`](agent-loop.ts.md#runLoop), [`executeToolCallsParallel`](agent-loop.ts.md#executeToolCallsParallel), [`executeToolCallsSequential`](agent-loop.ts.md#executeToolCallsSequential), [`executeToolCalls`](agent-loop.ts.md#executeToolCalls)

### `ExecutedToolCallOutcome`
- def: [`packages/agent/src/agent-loop.ts:764`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L764)
- signature: `type ExecutedToolCallOutcome`
- members:
  - `isError` — [`L766`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L766)
  - `result` — [`L765`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L765)
- uses (calls/refs, reference-scoped): [`AgentToolResult`](types.ts.md#AgentToolResult)
- used by: [`finalizeExecutedToolCall`](agent-loop.ts.md#finalizeExecutedToolCall), [`executePreparedToolCall`](agent-loop.ts.md#executePreparedToolCall)

### `FinalizedToolCallEntry`
- def: [`packages/agent/src/agent-loop.ts:775`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L775)
- signature: `type FinalizedToolCallEntry`
- uses (calls/refs, reference-scoped): [`FinalizedToolCallOutcome`](agent-loop.ts.md#FinalizedToolCallOutcome)
- used by: [`executeToolCallsParallel`](agent-loop.ts.md#executeToolCallsParallel)

### `FinalizedToolCallOutcome`
- def: [`packages/agent/src/agent-loop.ts:769`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L769)
- signature: `type FinalizedToolCallOutcome`
- members:
  - `isError` — [`L772`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L772)
  - `result` — [`L771`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L771)
  - `toolCall` — [`L770`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L770)
- uses (calls/refs, reference-scoped): [`AgentToolResult`](types.ts.md#AgentToolResult), [`AgentToolCall`](types.ts.md#AgentToolCall)
- used by: [`finalizeExecutedToolCall`](agent-loop.ts.md#finalizeExecutedToolCall), [`executeToolCallsParallel`](agent-loop.ts.md#executeToolCallsParallel), [`executeToolCallsSequential`](agent-loop.ts.md#executeToolCallsSequential), [`createToolResultMessage`](agent-loop.ts.md#createToolResultMessage), [`emitToolExecutionEnd`](agent-loop.ts.md#emitToolExecutionEnd), [`shouldTerminateToolBatch`](agent-loop.ts.md#shouldTerminateToolBatch), [`FinalizedToolCallEntry`](agent-loop.ts.md#FinalizedToolCallEntry)

### `ImmediateToolCallOutcome`
- def: [`packages/agent/src/agent-loop.ts:758`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L758)
- signature: `type ImmediateToolCallOutcome`
- members:
  - `isError` — [`L761`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L761)
  - `kind` — [`L759`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L759)
  - `result` — [`L760`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L760)
- uses (calls/refs, reference-scoped): [`AgentToolResult`](types.ts.md#AgentToolResult)
- used by: [`executeToolCallsParallel`](agent-loop.ts.md#executeToolCallsParallel), [`executeToolCallsSequential`](agent-loop.ts.md#executeToolCallsSequential), [`prepareToolCall`](agent-loop.ts.md#prepareToolCall)

### `PostTurnResult`
- def: [`packages/agent/src/agent-loop.ts:106`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L106)
- signature: `type PostTurnResult`
- used by: [`runLoop`](agent-loop.ts.md#runLoop), [`settlePostTurn`](agent-loop.ts.md#settlePostTurn)

### `PreparedToolCall`
- def: [`packages/agent/src/agent-loop.ts:751`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L751)
- signature: `type PreparedToolCall`
- members:
  - `args` — [`L755`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L755)
  - `kind` — [`L752`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L752)
  - `tool` — [`L754`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L754)
  - `toolCall` — [`L753`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L753)
- uses (calls/refs, reference-scoped): [`AgentTool`](types.ts.md#AgentTool), [`AgentToolCall`](types.ts.md#AgentToolCall)
- used by: [`finalizeExecutedToolCall`](agent-loop.ts.md#finalizeExecutedToolCall), [`executeToolCallsParallel`](agent-loop.ts.md#executeToolCallsParallel), [`executeToolCallsSequential`](agent-loop.ts.md#executeToolCallsSequential), [`prepareToolCall`](agent-loop.ts.md#prepareToolCall), [`executePreparedToolCall`](agent-loop.ts.md#executePreparedToolCall)

## Functions
- `agentLoop(prompts: AgentMessage[], context: AgentContext, config: AgentLoopConfig, signal?: AbortSignal | undefined, streamFn?: StreamFn | undefined)` — [`L181`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L181) — Start an agent loop with a new prompt message.
- `agentLoopContinue(context: AgentContext, config: AgentLoopConfig, signal?: AbortSignal | undefined, streamFn?: StreamFn | undefined)` — [`L215`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L215) — Continue an agent loop from the current context without adding a new message.
- `cloneAssistantContent(content: (TextContent | ThinkingContent | ToolCall)[])` — [`L119`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L119)
- `cloneUsage(usage: Usage)` — [`L128`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L128)
- `createAbortError()` — [`L38`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L38)
- `createAbortedAssistantMessage(config: AgentLoopConfig, partialMessage: AssistantMessage | null)` — [`L132`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L132)
- `createAgentStream()` — [`L297`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L297)
- `createErrorToolResult(message: string)` — [`L954`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L954)
- `createToolResultMessage(finalized: FinalizedToolCallOutcome)` — [`L971`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L971)
- `emitToolExecutionEnd(finalized: FinalizedToolCallOutcome, emit: AgentEventSink)` — [`L961`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L961)
- `emitToolResultMessage(toolResultMessage: ToolResultMessage<any>, emit: AgentEventSink)` — [`L983`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L983)
- `endAgentStreamOnError(stream: EventStream<AgentEvent, AgentMessage[]>, promise: Promise<AgentMessage[]>)` — [`L153`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L153)
- `executePreparedToolCall(prepared: PreparedToolCall, signal: AbortSignal | undefined, emit: AgentEventSink)` — [`L850`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L850)
- `executeToolCalls(currentContext: AgentContext, assistantMessage: AssistantMessage, config: AgentLoopConfig, signal: AbortSignal | undefined, emit: AgentEventSink)` — [`L608`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L608) — Execute tool calls from an assistant message.
- `executeToolCallsParallel(currentContext: AgentContext, assistantMessage: AssistantMessage, toolCalls: ToolCall[], config: AgentLoopConfig, signal: AbortSignal | undefined, emit: AgentEventSink)` — [`L690`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L690)
- `executeToolCallsSequential(currentContext: AgentContext, assistantMessage: AssistantMessage, toolCalls: ToolCall[], config: AgentLoopConfig, signal: AbortSignal | undefined, emit: AgentEventSink)` — [`L630`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L630)
- `finalizeExecutedToolCall(currentContext: AgentContext, assistantMessage: AssistantMessage, prepared: PreparedToolCall, executed: ExecutedToolCallOutcome, config: AgentLoopConfig, signal: AbortSignal | undefined)` — [`L906`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L906)
- `getTerminalMessage(event: { type: "done"; reason: "stop" | "length" | "toolUse"; message: AssistantMessage; } | { type: "error"; reason: "error" | "aborted"; error: AssistantMessage; })` — [`L149`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L149)
- `isAbortError(error: unknown)` — [`L102`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L102)
- `maybePromiseWithAbort(operation: T | Promise<T>, signal: AbortSignal | undefined, onAbort?: (() => void) | undefined)` — [`L94`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L94)
- `pollMessagesUnlessAborted(poll: (() => AgentMessage[] | Promise<AgentMessage[]>) | undefined, signal: AbortSignal | undefined)` — [`L167`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L167)
- `prepareToolCall(currentContext: AgentContext, assistantMessage: AssistantMessage, toolCall: ToolCall, config: AgentLoopConfig, signal: AbortSignal | undefined)` — [`L795`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L795)
- `prepareToolCallArguments(tool: AgentTool<any, any>, toolCall: ToolCall)` — [`L781`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L781)
- `raceWithAbort(operation: Promise<T>, signal: AbortSignal | undefined, onAbort?: (() => void) | undefined)` — [`L48`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L48)
- `runAgentLoop(prompts: AgentMessage[], context: AgentContext, config: AgentLoopConfig, emit: AgentEventSink, signal?: AbortSignal | undefined, streamFn?: StreamFn | undefined)` — [`L247`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L247)
- `runAgentLoopContinue(context: AgentContext, config: AgentLoopConfig, emit: AgentEventSink, signal?: AbortSignal | undefined, streamFn?: StreamFn | undefined)` — [`L272`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L272)
- `runLoop(currentContext: AgentContext, newMessages: AgentMessage[], config: AgentLoopConfig, signal: AbortSignal | undefined, emit: AgentEventSink, streamFn?: StreamFn | undefined)` — [`L307`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L307) — Main loop logic shared by agentLoop and agentLoopContinue.
- `settlePostTurn(operation: Promise<T>, signal: AbortSignal | undefined)` — [`L108`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L108)
- `shouldTerminateToolBatch(finalizedCalls: FinalizedToolCallOutcome[])` — [`L777`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L777)
- `streamAssistantResponse(context: AgentContext, config: AgentLoopConfig, signal: AbortSignal | undefined, emit: AgentEventSink, streamFn?: StreamFn | undefined)` — [`L467`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L467) — Stream an assistant response from the LLM.
- `throwIfAborted(signal: AbortSignal | undefined)` — [`L42`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L42)

## Module values
- `ABORT_ERROR_MESSAGE` — [`L28`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L28)
- `EMPTY_USAGE` — [`L29`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L29)
- `type` — [`L149`](../../../../../../../raw/code/prime-agent/packages/agent/src/agent-loop.ts#L149)


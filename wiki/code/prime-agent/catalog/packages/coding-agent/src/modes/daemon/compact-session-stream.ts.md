---
title: 'Module: packages/coding-agent/src/modes/daemon/compact-session-stream.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/compact-session-stream.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`compact-session-stream.ts`/
symbols:
  CompactAssistantStreamReconstructor.reconstruct: CompactAssistantStreamReconstructor#reconstruct().
  createCompactAssistantDelta: createCompactAssistantDelta().
  CompactAssistantStreamReconstructor.observe: CompactAssistantStreamReconstructor#observe().
  compactToolCallArguments: compactToolCallArguments().
  compactContentStart: compactContentStart().
  CompactAssistantDelta.contentStart: CompactAssistantDelta#contentStart.
  CompactAssistantMessageEvent: CompactAssistantMessageEvent#
  CompactAssistantStreamReconstructor.seed: CompactAssistantStreamReconstructor#seed().
  CompactAssistantStreamReconstructor.clear: CompactAssistantStreamReconstructor#clear().
  CompactAssistantStreamReconstructor.partialMessages: CompactAssistantStreamReconstructor#partialMessages.
  CompactAssistantStreamReconstructor: CompactAssistantStreamReconstructor#
  CompactAssistantStreamReconstructor.toolCallJson: CompactAssistantStreamReconstructor#toolCallJson.
  CompactAssistantDelta.activeSessionId: CompactAssistantDelta#activeSessionId.
  MessageUpdateEvent: MessageUpdateEvent#
  CompactAssistantDelta.meta: CompactAssistantDelta#meta.
  isCompactAssistantDelta: isCompactAssistantDelta().
  SessionEvent: SessionEvent#
  WithoutPartial: WithoutPartial#
  CompactAssistantDelta.assistantMessageEvent: CompactAssistantDelta#assistantMessageEvent.
  CompactAssistantDelta: CompactAssistantDelta#
  CompactAssistantStreamReconstructor.toolCallKey: CompactAssistantStreamReconstructor#toolCallKey().
  CompactAssistantDelta.toolCallArguments: CompactAssistantDelta#toolCallArguments.
  MessageUpdateEvent.Extract.typeLiteral7.type: MessageUpdateEvent#Extract:typeLiteral7:type.
  CompactAssistantDelta.type: CompactAssistantDelta#type.
---
# Module: [`packages/coding-agent/src/modes/daemon/compact-session-stream.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts)

## Classes
### `CompactAssistantDelta`
- def: [`packages/coding-agent/src/modes/daemon/compact-session-stream.ts:9`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L9)
- signature: `interface CompactAssistantDelta`
- members:
  - `activeSessionId` — [`L11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L11)
  - `assistantMessageEvent` — [`L12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L12)
  - `contentStart` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L13)
  - `meta` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L15)
  - `toolCallArguments` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L14)
  - `type` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L10)
- uses (calls/refs, reference-scoped): [`content`](../../../../ai/src/types.ts.md#AssistantMessage.content), [`AssistantMessage`](../../../../ai/src/types.ts.md#AssistantMessage), [`DaemonEventMeta`](daemon-protocol.ts.md#DaemonEventMeta), [`CompactAssistantMessageEvent`](compact-session-stream.ts.md#CompactAssistantMessageEvent)
- used by: [`reconstruct`](compact-session-stream.ts.md#CompactAssistantStreamReconstructor.reconstruct), [`createCompactAssistantDelta`](compact-session-stream.ts.md#createCompactAssistantDelta), [`isCompactAssistantDelta`](compact-session-stream.ts.md#isCompactAssistantDelta)

### `CompactAssistantMessageEvent`
- def: [`packages/coding-agent/src/modes/daemon/compact-session-stream.ts:7`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L7)
- signature: `type CompactAssistantMessageEvent`
- uses (calls/refs, reference-scoped): [`MessageUpdateEvent`](compact-session-stream.ts.md#MessageUpdateEvent), [`WithoutPartial`](compact-session-stream.ts.md#WithoutPartial)
- used by: [`createCompactAssistantDelta`](compact-session-stream.ts.md#createCompactAssistantDelta), [`compactToolCallArguments`](compact-session-stream.ts.md#compactToolCallArguments), [`compactContentStart`](compact-session-stream.ts.md#compactContentStart), [`assistantMessageEvent`](compact-session-stream.ts.md#CompactAssistantDelta.assistantMessageEvent)

### `CompactAssistantStreamReconstructor`
- def: [`packages/coding-agent/src/modes/daemon/compact-session-stream.ts:72`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L72)
- signature: `class CompactAssistantStreamReconstructor`
- members:
  - `clear(method)` — [`L188`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L188)
  - `observe(method)` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L80)
  - `reconstruct(method)` — [`L100`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L100)
  - `seed(method)` — [`L76`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L76)
  - `toolCallKey(method)` — [`L197`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L197)
  - `partialMessages` — [`L73`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L73)
  - `toolCallJson` — [`L74`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L74)
- uses (calls/refs, reference-scoped): [`role`](../../../../ai/src/types.ts.md#AssistantMessage.role), [`role`](../../../../ai/src/types.ts.md#ToolResultMessage.role), [`role`](../../../../ai/src/types.ts.md#UserMessage.role), [`type`](../../../../ai/src/types.ts.md#TextContent.type), [`content`](../../../../ai/src/types.ts.md#AssistantMessage.content), [`role`](../../core/messages.ts.md#CustomMessage.role), [`role`](../../core/messages.ts.md#BashExecutionMessage.role), [`role`](../../core/messages.ts.md#BranchSummaryMessage.role), [`role`](../../core/messages.ts.md#CompactionSummaryMessage.role), [`type`](../../../../ai/src/types.ts.md#ToolCall.type), [`type`](../../../../ai/src/types.ts.md#ThinkingContent.type), [`AssistantMessage`](../../../../ai/src/types.ts.md#AssistantMessage), [`DaemonOutbound`](daemon-protocol.ts.md#DaemonOutbound), [`text`](../../../../ai/src/types.ts.md#TextContent.text), [`arguments`](../../../../ai/src/types.ts.md#ToolCall.arguments), [`thinking`](../../../../ai/src/types.ts.md#ThinkingContent.thinking), [`parseStreamingJson`](../../../../ai/src/utils/json-parse.ts.md#parseStreamingJson), [`contentStart`](compact-session-stream.ts.md#CompactAssistantDelta.contentStart), [`activeSessionId`](compact-session-stream.ts.md#CompactAssistantDelta.activeSessionId), [`MessageUpdateEvent`](compact-session-stream.ts.md#MessageUpdateEvent), [`meta`](compact-session-stream.ts.md#CompactAssistantDelta.meta), [`assistantMessageEvent`](compact-session-stream.ts.md#CompactAssistantDelta.assistantMessageEvent), [`CompactAssistantDelta`](compact-session-stream.ts.md#CompactAssistantDelta), [`toolCallArguments`](compact-session-stream.ts.md#CompactAssistantDelta.toolCallArguments)
- used by: [`daemon-supervisor.ts`](daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`handleWorkerFrame`](daemon-supervisor.ts.md#DaemonSupervisor.handleWorkerFrame), [`type`](daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type), [`refreshWorkerSummaries`](daemon-supervisor.ts.md#DaemonSupervisor.refreshWorkerSummaries), [`streamReconstructor`](daemon-supervisor.ts.md#DaemonSupervisor.streamReconstructor)  (1 test-only)

### `MessageUpdateEvent`
- def: [`packages/coding-agent/src/modes/daemon/compact-session-stream.ts:5`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L5)
- signature: `type MessageUpdateEvent`
- members:
  - `type` — [`L5`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L5)
- uses (calls/refs, reference-scoped): [`SessionEvent`](compact-session-stream.ts.md#SessionEvent)
- used by: [`reconstruct`](compact-session-stream.ts.md#CompactAssistantStreamReconstructor.reconstruct), [`CompactAssistantMessageEvent`](compact-session-stream.ts.md#CompactAssistantMessageEvent)

### `SessionEvent`
- def: [`packages/coding-agent/src/modes/daemon/compact-session-stream.ts:4`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L4)
- signature: `type SessionEvent`
- uses (calls/refs, reference-scoped): [`DaemonOutbound`](daemon-protocol.ts.md#DaemonOutbound)
- used by: [`MessageUpdateEvent`](compact-session-stream.ts.md#MessageUpdateEvent)

### `WithoutPartial`
- def: [`packages/coding-agent/src/modes/daemon/compact-session-stream.ts:6`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L6)
- signature: `type WithoutPartial`
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../../../ai/src/types.ts.md#AssistantMessage)
- used by: [`CompactAssistantMessageEvent`](compact-session-stream.ts.md#CompactAssistantMessageEvent)

## Functions
- `compactContentStart(message: AssistantMessage, event: CompactAssistantMessageEvent)` — [`L52`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L52)
- `compactToolCallArguments(message: AssistantMessage, event: CompactAssistantMessageEvent)` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L41)
- `createCompactAssistantDelta(message: DaemonOutbound)` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L18)
- `isCompactAssistantDelta(value: unknown)` — [`L202`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/compact-session-stream.ts#L202)


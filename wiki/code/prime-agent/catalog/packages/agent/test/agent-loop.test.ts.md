---
title: 'Module: packages/agent/test/agent-loop.test.ts'
type: catalog
provenance: extracted
module: packages/agent/test/agent-loop.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-agent-core 0.7.2 test/`agent-loop.test.ts`/
symbols:
  createModel: createModel().
  createAssistantMessage: createAssistantMessage().
  identityConverter: identityConverter().
  createUserMessage: createUserMessage().
  MockAssistantStream.-constructor: MockAssistantStream#`<constructor>`().
  MockAssistantStream: MockAssistantStream#
  ThrowingResultStream: ThrowingResultStream#
  DelayedResultStream.-constructor: DelayedResultStream#`<constructor>`().
  DelayedResultStream: DelayedResultStream#
  DelayedResultStream.result: DelayedResultStream#result().
  ThrowingResultStream.result: ThrowingResultStream#result().
  ThrowingResultStream.-constructor: ThrowingResultStream#`<constructor>`().
  createUsage: createUsage().
---
# Module: [`packages/agent/test/agent-loop.test.ts`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent-loop.test.ts)

## Classes
### `DelayedResultStream`  ·  implements/extends AsyncIterable, EventStream, MockAssistantStream
- def: [`packages/agent/test/agent-loop.test.ts:28`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent-loop.test.ts#L28)
- signature: `class DelayedResultStream`
- members:
  - `<constructor>(getDelayedResult: () => Promise<AssistantMessage>)` — [`L29`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent-loop.test.ts#L29)
  - `result(method)` — [`L33`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent-loop.test.ts#L33)
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../ai/src/types.ts.md#AssistantMessage)  (1 test-only)
- used by: [`result`](../../ai/src/utils/event-stream.ts.md#EventStream.result), [`EventStream`](../../ai/src/utils/event-stream.ts.md#EventStream)  (2 test-only)

### `MockAssistantStream`  ·  implements/extends AsyncIterable, EventStream
- def: [`packages/agent/test/agent-loop.test.ts:15`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent-loop.test.ts#L15)
- signature: `class MockAssistantStream`
- members:
  - `<constructor>()` — [`L16`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent-loop.test.ts#L16)
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../ai/src/types.ts.md#AssistantMessage), [`AssistantMessageEvent`](../../ai/src/types.ts.md#AssistantMessageEvent), [`EventStream`](../../ai/src/utils/event-stream.ts.md#EventStream)  (2 test-only)
- used by: [`EventStream`](../../ai/src/utils/event-stream.ts.md#EventStream)  (3 test-only)

### `ThrowingResultStream`  ·  implements/extends AsyncIterable, EventStream, MockAssistantStream
- def: [`packages/agent/test/agent-loop.test.ts:38`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent-loop.test.ts#L38)
- signature: `class ThrowingResultStream`
- members:
  - `<constructor>(onResult: () => void, error: Error)` — [`L39`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent-loop.test.ts#L39)
  - `result(method)` — [`L52`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent-loop.test.ts#L52)
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../ai/src/types.ts.md#AssistantMessage), [`AssistantMessageEvent`](../../ai/src/types.ts.md#AssistantMessageEvent)  (1 test-only)
- used by: [`result`](../../ai/src/utils/event-stream.ts.md#EventStream.result), [`EventStream`](../../ai/src/utils/event-stream.ts.md#EventStream)  (2 test-only)

## Functions
- `createAssistantMessage(content: (TextContent | ThinkingContent | ToolCall)[], stopReason?: StopReason)` — [`L84`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent-loop.test.ts#L84)
- `createModel()` — [`L69`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent-loop.test.ts#L69)
- `createUsage()` — [`L58`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent-loop.test.ts#L58)
- `createUserMessage(text: string)` — [`L100`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent-loop.test.ts#L100)
- `identityConverter(messages: AgentMessage[])` — [`L109`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent-loop.test.ts#L109)


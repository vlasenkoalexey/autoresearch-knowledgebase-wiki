---
title: 'Module: packages/agent/test/agent.test.ts'
type: catalog
provenance: extracted
module: packages/agent/test/agent.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-agent-core 0.7.2 test/`agent.test.ts`/
symbols:
  createAssistantMessage: createAssistantMessage().
  createToolUseMessage: createToolUseMessage().
  MockAssistantStream.-constructor: MockAssistantStream#`<constructor>`().
  MockAssistantStream: MockAssistantStream#
  createDeferred: createDeferred().
  createDeferred.typeLiteral33.promise: createDeferred().typeLiteral33:promise.
  createDeferred.typeLiteral33.resolve: createDeferred().typeLiteral33:resolve.
---
# Module: [`packages/agent/test/agent.test.ts`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent.test.ts)

## Classes
### `MockAssistantStream`  ·  implements/extends AsyncIterable, EventStream
- def: [`packages/agent/test/agent.test.ts:14`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent.test.ts#L14)
- signature: `class MockAssistantStream`
- members:
  - `<constructor>()` — [`L15`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent.test.ts#L15)
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../ai/src/types.ts.md#AssistantMessage), [`AssistantMessageEvent`](../../ai/src/types.ts.md#AssistantMessageEvent), [`EventStream`](../../ai/src/utils/event-stream.ts.md#EventStream)
- used by: [`EventStream`](../../ai/src/utils/event-stream.ts.md#EventStream)  (1 test-only)

## Functions
- `createAssistantMessage(text: string)` — [`L27`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent.test.ts#L27)
- `createDeferred()` — [`L55`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent.test.ts#L55)
- `createToolUseMessage(toolName: string)` — [`L47`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent.test.ts#L47)

## Module values
- `promise` — [`L56`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent.test.ts#L56)
- `resolve` — [`L57`](../../../../../../../raw/code/prime-agent/packages/agent/test/agent.test.ts#L57)


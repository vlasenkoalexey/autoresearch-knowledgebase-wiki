---
title: 'Module: packages/coding-agent/test/agent-session-concurrent.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/agent-session-concurrent.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`agent-session-concurrent.test.ts`/
symbols:
  createAssistantMessage: createAssistantMessage().
  MockAssistantStream: MockAssistantStream#
  MockAssistantStream.-constructor: MockAssistantStream#`<constructor>`().
---
# Module: [`packages/coding-agent/test/agent-session-concurrent.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-concurrent.test.ts)

## Classes
### `MockAssistantStream`  ·  implements/extends AsyncIterable, EventStream
- def: [`packages/coding-agent/test/agent-session-concurrent.test.ts:28`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-concurrent.test.ts#L28)
- signature: `class MockAssistantStream`
- members:
  - `<constructor>()` — [`L29`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-concurrent.test.ts#L29)
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../ai/src/types.ts.md#AssistantMessage), [`AssistantMessageEvent`](../../ai/src/types.ts.md#AssistantMessageEvent), [`EventStream`](../../ai/src/utils/event-stream.ts.md#EventStream)
- used by: [`EventStream`](../../ai/src/utils/event-stream.ts.md#EventStream)  (1 test-only)

## Functions
- `createAssistantMessage(text: string)` — [`L41`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-concurrent.test.ts#L41)


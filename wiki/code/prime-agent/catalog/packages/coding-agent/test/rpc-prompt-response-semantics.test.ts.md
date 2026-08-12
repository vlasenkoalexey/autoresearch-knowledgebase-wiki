---
title: 'Module: packages/coding-agent/test/rpc-prompt-response-semantics.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/rpc-prompt-response-semantics.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`rpc-prompt-response-semantics.test.ts`/
symbols:
  createRuntimeHost.typeLiteral69.cleanup: createRuntimeHost().typeLiteral69:cleanup.
  createAssistantMessage: createAssistantMessage().
  startRpcMode: startRpcMode().
  rpcIo: rpcIo.
  getPromptResponses: getPromptResponses().
  MockAssistantStream: MockAssistantStream#
  parseOutputLines: parseOutputLines().
  createRuntimeHost.typeLiteral69.runtimeHost: createRuntimeHost().typeLiteral69:runtimeHost.
  createRuntimeHost.typeLiteral69.session: createRuntimeHost().typeLiteral69:session.
  startRpcMode.Promise.typeLiteral108.session: startRpcMode().Promise:typeLiteral108:session.
  startRpcMode.options-typeLiteral107.withAuth: startRpcMode().(options)typeLiteral107:withAuth.
  startRpcMode.options-typeLiteral107.responseDelayMs: startRpcMode().(options)typeLiteral107:responseDelayMs.
  startRpcMode.Promise.typeLiteral108.lineHandler: startRpcMode().Promise:typeLiteral108:lineHandler.
  startRpcMode.Promise.typeLiteral108.cleanup: startRpcMode().Promise:typeLiteral108:cleanup.
  createRuntimeHost.options-typeLiteral68.model: createRuntimeHost().(options)typeLiteral68:model.
  startRpcMode.options-typeLiteral107.model: startRpcMode().(options)typeLiteral107:model.
  ParsedOutputLine: ParsedOutputLine#
  MockAssistantStream.-constructor: MockAssistantStream#`<constructor>`().
  sleep: sleep().
  createRuntimeHost: createRuntimeHost().
  createRuntimeHost.options-typeLiteral68.withAuth: createRuntimeHost().(options)typeLiteral68:withAuth.
  createRuntimeHost.options-typeLiteral68.responseDelayMs: createRuntimeHost().(options)typeLiteral68:responseDelayMs.
---
# Module: [`packages/coding-agent/test/rpc-prompt-response-semantics.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts)

## Classes
### `MockAssistantStream`  ·  implements/extends AsyncIterable, EventStream
- def: [`packages/coding-agent/test/rpc-prompt-response-semantics.test.ts:44`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L44)
- signature: `class MockAssistantStream`
- members:
  - `<constructor>()` — [`L45`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L45)
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../ai/src/types.ts.md#AssistantMessage), [`AssistantMessageEvent`](../../ai/src/types.ts.md#AssistantMessageEvent), [`EventStream`](../../ai/src/utils/event-stream.ts.md#EventStream)
- used by: [`EventStream`](../../ai/src/utils/event-stream.ts.md#EventStream)  (1 test-only)

### `ParsedOutputLine`
- def: [`packages/coding-agent/test/rpc-prompt-response-semantics.test.ts:77`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L77)
- signature: `type ParsedOutputLine`
- used by: (2 test-only callers)

## Functions
- `createAssistantMessage(text: string)` — [`L57`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L57)
- `createRuntimeHost(options: { withAuth: boolean; responseDelayMs: number; model?: Model<any> | undefined; })` — [`L96`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L96)
- `getPromptResponses(outputLines: string[], id: string)` — [`L86`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L86)
- `parseOutputLines(outputLines: string[])` — [`L79`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L79)
- `sleep(ms: number)` — [`L92`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L92)
- `startRpcMode(options: { withAuth: boolean; responseDelayMs: number; model?: Model<any> | undefined; })` — [`L173`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L173)

## Module values
- `cleanup` — [`L99`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L99)
- `cleanup` — [`L176`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L176)
- `lineHandler` — [`L174`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L174)
- `model` — [`L96`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L96)
- `model` — [`L173`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L173)
- `responseDelayMs` — [`L96`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L96)
- `responseDelayMs` — [`L173`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L173)
- `rpcIo` — [`L22`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L22)
- `runtimeHost` — [`L97`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L97)
- `session` — [`L98`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L98)
- `session` — [`L175`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L175)
- `withAuth` — [`L96`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L96)
- `withAuth` — [`L173`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/rpc-prompt-response-semantics.test.ts#L173)


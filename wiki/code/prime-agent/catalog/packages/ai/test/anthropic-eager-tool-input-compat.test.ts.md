---
title: 'Module: packages/ai/test/anthropic-eager-tool-input-compat.test.ts'
type: catalog
provenance: extracted
module: packages/ai/test/anthropic-eager-tool-input-compat.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 test/`anthropic-eager-tool-input-compat.test.ts`/
symbols:
  createModel: createModel().
  createContext: createContext().
  captureAnthropicRequest: captureAnthropicRequest().
  tool: tool.
  CapturedRequest.headers: CapturedRequest#headers.
  CapturedRequest.body: CapturedRequest#body.
  CapturedRequest: CapturedRequest#
  getFirstTool: getFirstTool().
  readRequestBody: readRequestBody().
  writeEmptySseResponse: writeEmptySseResponse().
---
# Module: [`packages/ai/test/anthropic-eager-tool-input-compat.test.ts`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-compat.test.ts)

## Classes
### `CapturedRequest`
- def: [`packages/ai/test/anthropic-eager-tool-input-compat.test.ts:8`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-compat.test.ts#L8)
- signature: `interface CapturedRequest`
- members:
  - `body` — [`L10`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-compat.test.ts#L10)
  - `headers` — [`L9`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-compat.test.ts#L9)
- used by: (2 test-only callers)

## Functions
- `captureAnthropicRequest(compat: AnthropicMessagesCompat | undefined, context: Context)` — [`L55`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-compat.test.ts#L55)
- `createContext(tools?: Tool<TSchema>[])` — [`L35`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-compat.test.ts#L35)
- `createModel(baseUrl: string, compat?: AnthropicMessagesCompat | undefined)` — [`L13`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-compat.test.ts#L13)
- `getFirstTool(body: Record<string, unknown>)` — [`L93`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-compat.test.ts#L93)
- `readRequestBody(request: IncomingMessage)` — [`L42`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-compat.test.ts#L42)
- `writeEmptySseResponse(response: ServerResponse<IncomingMessage>)` — [`L50`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-compat.test.ts#L50)

## Module values
- `tool` — [`L29`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-compat.test.ts#L29)


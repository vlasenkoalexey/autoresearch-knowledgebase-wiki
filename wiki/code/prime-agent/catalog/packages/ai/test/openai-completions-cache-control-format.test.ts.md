---
title: 'Module: packages/ai/test/openai-completions-cache-control-format.test.ts'
type: catalog
provenance: extracted
module: packages/ai/test/openai-completions-cache-control-format.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 test/`openai-completions-cache-control-format.test.ts`/
symbols:
  runCompletion.Promise.typeLiteral27.result: runCompletion().Promise:typeLiteral27:result.
  expectAnthropicCacheMarkers: expectAnthropicCacheMarkers().
  expectNoAnthropicCacheMarkers: expectNoAnthropicCacheMarkers().
  runCompletion: runCompletion().
  runCompletion.Promise.typeLiteral27.params: runCompletion().Promise:typeLiteral27:params.
  getInstructionMessage: getInstructionMessage().
  mockState: mockState.
  CapturedParams.messages.Array.typeLiteral0.content: CapturedParams#messages.Array:typeLiteral0:content.
  capturePayload.options-typeLiteral40.cacheRetention: capturePayload().(options)typeLiteral40:cacheRetention.
  CapturedParams: CapturedParams#
  CapturedParams.tools: CapturedParams#tools.
  capturePayload: capturePayload().
  CapturedParams.messages: CapturedParams#messages.
  TextPart.cache_control: TextPart#cache_control.
  ToolWithCacheControl: ToolWithCacheControl#
  CacheControl: CacheControl#
  TextPart: TextPart#
  CapturedParams.messages.Array.typeLiteral0.role: CapturedParams#messages.Array:typeLiteral0:role.
  ToolWithCacheControl.cache_control: ToolWithCacheControl#cache_control.
  CacheControl.type: CacheControl#type.
  CacheControl.ttl: CacheControl#ttl.
  TextPart.type: TextPart#type.
  TextPart.text: TextPart#text.
  ToolWithCacheControl.type: ToolWithCacheControl#type.
  runCompletion.options-typeLiteral26.cacheRetention: runCompletion().(options)typeLiteral26:cacheRetention.
---
# Module: [`packages/ai/test/openai-completions-cache-control-format.test.ts`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts)

## Classes
### `CacheControl`
- def: [`packages/ai/test/openai-completions-cache-control-format.test.ts:7`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L7)
- signature: `interface CacheControl`
- members:
  - `ttl` — [`L9`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L9)
  - `type` — [`L8`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L8)
- used by: (3 test-only callers)

### `CapturedParams`
- def: [`packages/ai/test/openai-completions-cache-control-format.test.ts:23`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L23)
- signature: `interface CapturedParams`
- members:
  - `content` — [`L26`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L26)
  - `messages` — [`L24`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L24)
  - `role` — [`L25`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L25)
  - `tools` — [`L28`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L28)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (6 test-only callers)

### `TextPart`
- def: [`packages/ai/test/openai-completions-cache-control-format.test.ts:12`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L12)
- signature: `interface TextPart`
- members:
  - `cache_control` — [`L15`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L15)
  - `text` — [`L14`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L14)
  - `type` — [`L13`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L13)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `ToolWithCacheControl`
- def: [`packages/ai/test/openai-completions-cache-control-format.test.ts:18`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L18)
- signature: `interface ToolWithCacheControl`
- members:
  - `cache_control` — [`L20`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L20)
  - `type` — [`L19`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L19)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (3 test-only callers)

## Functions
- `capturePayload(model: Model<"openai-completions">, options?: { cacheRetention?: "none" | "short" | "long" | undefined; } | undefined)` — [`L109`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L109)
- `expectAnthropicCacheMarkers(params: CapturedParams, expectedCacheControl?: CacheControl)` — [`L120`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L120)
- `expectNoAnthropicCacheMarkers(params: CapturedParams)` — [`L138`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L138)
- `getInstructionMessage(params: CapturedParams)` — [`L116`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L116)
- `runCompletion(model: Model<"openai-completions">, options?: { cacheRetention?: "none" | "short" | "long" | undefined; } | undefined)` — [`L78`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L78)

## Module values
- `cacheRetention` — [`L80`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L80)
- `cacheRetention` — [`L111`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L111)
- `mockState` — [`L31`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L31)
- `params` — [`L81`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L81)
- `result` — [`L81`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-cache-control-format.test.ts#L81)


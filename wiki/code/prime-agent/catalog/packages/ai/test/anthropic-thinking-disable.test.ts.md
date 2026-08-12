---
title: 'Module: packages/ai/test/anthropic-thinking-disable.test.ts'
type: catalog
provenance: extracted
module: packages/ai/test/anthropic-thinking-disable.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 test/`anthropic-thinking-disable.test.ts`/
symbols:
  makeE2EContext: makeE2EContext().
  runWithoutReasoning: runWithoutReasoning().
  capturePayload: capturePayload().
  makePayloadCaptureContext: makePayloadCaptureContext().
  AnthropicThinkingPayload.thinking: AnthropicThinkingPayload#thinking.
  AnthropicThinkingPayload.output_config: AnthropicThinkingPayload#output_config.
  AnthropicThinkingPayload: AnthropicThinkingPayload#
  AnthropicThinkingPayload.temperature: AnthropicThinkingPayload#temperature.
  RunResult: RunResult#
  RunResult.thinkingEventCount: RunResult#thinkingEventCount.
  RunResult.thinkingCharCount: RunResult#thinkingCharCount.
  RunResult.text: RunResult#text.
  RunResult.contentTypes: RunResult#contentTypes.
  countPongs: countPongs().
  AnthropicThinkingPayload.thinking.typeLiteral0.type: AnthropicThinkingPayload#thinking.typeLiteral0:type.
  AnthropicThinkingPayload.thinking.typeLiteral0.budget_tokens: AnthropicThinkingPayload#thinking.typeLiteral0:budget_tokens.
  AnthropicThinkingPayload.thinking.typeLiteral0.display: AnthropicThinkingPayload#thinking.typeLiteral0:display.
  AnthropicThinkingPayload.output_config.typeLiteral1.effort: AnthropicThinkingPayload#output_config.typeLiteral1:effort.
---
# Module: [`packages/ai/test/anthropic-thinking-disable.test.ts`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts)

## Classes
### `AnthropicThinkingPayload`
- def: [`packages/ai/test/anthropic-thinking-disable.test.ts:6`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L6)
- signature: `interface AnthropicThinkingPayload`
- members:
  - `budget_tokens` — [`L7`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L7)
  - `display` — [`L7`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L7)
  - `effort` — [`L8`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L8)
  - `output_config` — [`L8`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L8)
  - `temperature` — [`L9`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L9)
  - `thinking` — [`L7`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L7)
  - `type` — [`L7`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L7)
- used by: (2 test-only callers)

### `RunResult`
- def: [`packages/ai/test/anthropic-thinking-disable.test.ts:46`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L46)
- signature: `interface RunResult`
- members:
  - `contentTypes` — [`L50`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L50)
  - `text` — [`L49`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L49)
  - `thinkingCharCount` — [`L48`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L48)
  - `thinkingEventCount` — [`L47`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L47)
- used by: (2 test-only callers)

## Functions
- `capturePayload(model: Model<"anthropic-messages">, options?: SimpleStreamOptions | undefined)` — [`L18`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L18)
- `countPongs(text: string)` — [`L67`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L67)
- `makeE2EContext()` — [`L53`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L53)
- `makePayloadCaptureContext()` — [`L12`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L12)
- `runWithoutReasoning(model: Model<"anthropic-messages">)` — [`L71`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-thinking-disable.test.ts#L71)


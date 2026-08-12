---
title: 'Module: packages/ai/test/openai-completions-thinking-as-text.test.ts'
type: catalog
provenance: extracted
module: packages/ai/test/openai-completions-thinking-as-text.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 test/`openai-completions-thinking-as-text.test.ts`/
symbols:
  compat: compat.
  buildModel: buildModel().
  buildContext: buildContext().
  emptyUsage: emptyUsage.
  buildAssistant: buildAssistant().
  collectEvents: collectEvents().
  ChatCompletionsRequestBody: ChatCompletionsRequestBody#
  ChatCompletionsRequestBody.messages: ChatCompletionsRequestBody#messages.
  ChatCompletionsRequestBody.model: ChatCompletionsRequestBody#model.
  ChatCompletionsRequestBody.messages.Array.typeLiteral10.role: ChatCompletionsRequestBody#messages.Array:typeLiteral10:role.
  ChatCompletionsRequestBody.messages.Array.typeLiteral10.content: ChatCompletionsRequestBody#messages.Array:typeLiteral10:content.
  ChatCompletionsRequestBody.stream: ChatCompletionsRequestBody#stream.
  ChatCompletionsRequestBody.stream_options: ChatCompletionsRequestBody#stream_options.
  ChatCompletionsRequestBody.stream_options.typeLiteral11.include_usage: ChatCompletionsRequestBody#stream_options.typeLiteral11:include_usage.
---
# Module: [`packages/ai/test/openai-completions-thinking-as-text.test.ts`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-thinking-as-text.test.ts)

## Classes
### `ChatCompletionsRequestBody`
- def: [`packages/ai/test/openai-completions-thinking-as-text.test.ts:93`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-thinking-as-text.test.ts#L93)
- signature: `interface ChatCompletionsRequestBody`
- members:
  - `content` — [`L95`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-thinking-as-text.test.ts#L95)
  - `include_usage` — [`L97`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-thinking-as-text.test.ts#L97)
  - `messages` — [`L95`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-thinking-as-text.test.ts#L95)
  - `model` — [`L94`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-thinking-as-text.test.ts#L94)
  - `role` — [`L95`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-thinking-as-text.test.ts#L95)
  - `stream` — [`L96`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-thinking-as-text.test.ts#L96)
  - `stream_options` — [`L97`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-thinking-as-text.test.ts#L97)
- used by: (1 test-only callers)

## Functions
- `buildAssistant(content: (TextContent | ThinkingContent | ToolCall)[])` — [`L62`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-thinking-as-text.test.ts#L62)
- `buildContext(assistant: AssistantMessage)` — [`L75`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-thinking-as-text.test.ts#L75)
- `buildModel(baseUrl?: string)` — [`L46`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-thinking-as-text.test.ts#L46)
- `collectEvents(stream: AsyncIterable<AssistantMessageEvent>)` — [`L85`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-thinking-as-text.test.ts#L85)

## Module values
- `compat` — [`L24`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-thinking-as-text.test.ts#L24)
- `emptyUsage` — [`L15`](../../../../../../../raw/code/prime-agent/packages/ai/test/openai-completions-thinking-as-text.test.ts#L15)


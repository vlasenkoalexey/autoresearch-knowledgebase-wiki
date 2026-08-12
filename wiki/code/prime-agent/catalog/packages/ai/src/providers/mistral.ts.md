---
title: 'Module: packages/ai/src/providers/mistral.ts'
type: catalog
provenance: extracted
module: packages/ai/src/providers/mistral.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/providers/`mistral.ts`/
symbols:
  consumeChatStream: consumeChatStream().
  streamMistral: streamMistral.
  createOutput: createOutput().
  toChatMessages: toChatMessages().
  streamSimpleMistral: streamSimpleMistral.
  buildChatPayload: buildChatPayload().
  MistralOptions: MistralOptions#
  buildRequestOptions: buildRequestOptions().
  toFunctionTools: toFunctionTools().
  mapReasoningEffort: mapReasoningEffort().
  formatMistralError: formatMistralError().
  usesPromptModeReasoning: usesPromptModeReasoning().
  deriveMistralToolCallId: deriveMistralToolCallId().
  usesReasoningEffort: usesReasoningEffort().
  mapToolChoice: mapToolChoice().
  stripSymbolKeys: stripSymbolKeys().
  createMistralToolCallIdNormalizer: createMistralToolCallIdNormalizer().
  mapChatStopReason: mapChatStopReason().
  MistralReasoningEffort: MistralReasoningEffort#
  MistralOptions.toolChoice: MistralOptions#toolChoice.
  MistralOptions.promptMode: MistralOptions#promptMode.
  MistralOptions.reasoningEffort: MistralOptions#reasoningEffort.
  MISTRAL_TOOL_CALL_ID_LENGTH: MISTRAL_TOOL_CALL_ID_LENGTH.
  MAX_MISTRAL_ERROR_BODY_CHARS: MAX_MISTRAL_ERROR_BODY_CHARS.
  truncateErrorText: truncateErrorText().
  safeJsonStringify: safeJsonStringify().
  buildToolResultText: buildToolResultText().
---
# Module: [`packages/ai/src/providers/mistral.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts)

## Classes
### `MistralOptions`
- def: [`packages/ai/src/providers/mistral.ts:41`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L41)
- signature: `interface MistralOptions`
- members:
  - `promptMode` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L43)
  - `reasoningEffort` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L44)
  - `toolChoice` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L42)
- uses (calls/refs, reference-scoped): [`StreamOptions`](../types.ts.md#StreamOptions), [`MistralReasoningEffort`](mistral.ts.md#MistralReasoningEffort)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`mistral.ts`](mistral.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-mistral.ts), [`register-builtins.ts`](register-builtins.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-register-builtins.ts), [`streamMistral`](mistral.ts.md#streamMistral), [`streamSimpleMistral`](mistral.ts.md#streamSimpleMistral), [`buildChatPayload`](mistral.ts.md#buildChatPayload), [`loadMistralProviderModule`](register-builtins.ts.md#loadMistralProviderModule), [`buildRequestOptions`](mistral.ts.md#buildRequestOptions), [`mistralProviderModulePromise`](register-builtins.ts.md#mistralProviderModulePromise), [`mapToolChoice`](mistral.ts.md#mapToolChoice), [`streamMistral`](register-builtins.ts.md#MistralProviderModule.streamMistral)

### `MistralReasoningEffort`
- def: [`packages/ai/src/providers/mistral.ts:39`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L39)
- doc: Provider-specific options for the Mistral API.
- signature: `type MistralReasoningEffort`
- used by: [`MistralOptions`](mistral.ts.md#MistralOptions), [`mapReasoningEffort`](mistral.ts.md#mapReasoningEffort)

## Functions
- `buildChatPayload(model: Model<"mistral-conversations">, context: Context, messages: Message[], options?: MistralOptions | undefined)` — [`L243`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L243)
- `buildRequestOptions(model: Model<"mistral-conversations">, options?: MistralOptions | undefined)` — [`L216`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L216)
- `buildToolResultText(text: string, hasImages: boolean, supportsImages: boolean, isError: boolean)` — [`L575`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L575)
- `consumeChatStream(model: Model<"mistral-conversations">, output: AssistantMessage, stream: AssistantMessageEventStream, mistralStream: AsyncIterable<CompletionEvent>)` — [`L272`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L272)
- `createMistralToolCallIdNormalizer()` — [`L156`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L156)
- `createOutput(model: Model<"mistral-conversations">)` — [`L136`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L136)
- `deriveMistralToolCallId(id: string, attempt: number)` — [`L178`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L178)
- `formatMistralError(error: unknown)` — [`L188`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L188)
- `mapChatStopReason(reason: string | null)` — [`L624`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L624)
- `mapReasoningEffort(model: Model<"mistral-conversations">, level: ThinkingLevel)` — [`L604`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L604)
- `mapToolChoice(choice: "auto" | "none" | "any" | "required" | { type: "function"; function: { name: string; }; } | undefined)` — [`L611`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L611)
- `safeJsonStringify(value: unknown)` — [`L207`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L207)
- `stripSymbolKeys(value: unknown)` — [`L472`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L472)
- `toChatMessages(messages: Message[], supportsImages: boolean)` — [`L488`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L488)
- `toFunctionTools(tools: Tool<TSchema>[])` — [`L460`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L460)
- `truncateErrorText(text: string, maxChars: number)` — [`L202`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L202)
- `usesPromptModeReasoning(model: Model<"mistral-conversations">)` — [`L600`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L600)
- `usesReasoningEffort(model: Model<"mistral-conversations">)` — [`L596`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L596)

## Module values
- `MAX_MISTRAL_ERROR_BODY_CHARS` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L34)
- `MISTRAL_TOOL_CALL_ID_LENGTH` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L33)
- `streamMistral` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L50) — Stream responses from Mistral using `chat.stream`.
- `streamSimpleMistral` — [`L113`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/mistral.ts#L113) — Maps provider-agnostic `SimpleStreamOptions` to Mistral options.


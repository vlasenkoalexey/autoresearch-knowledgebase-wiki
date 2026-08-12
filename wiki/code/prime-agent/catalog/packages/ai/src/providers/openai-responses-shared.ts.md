---
title: 'Module: packages/ai/src/providers/openai-responses-shared.ts'
type: catalog
provenance: extracted
module: packages/ai/src/providers/openai-responses-shared.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/providers/`openai-responses-shared.ts`/
symbols:
  processResponsesStream: processResponsesStream().
  convertResponsesMessages: convertResponsesMessages().
  convertResponsesTools: convertResponsesTools().
  encodeTextSignatureV1: encodeTextSignatureV1().
  parseTextSignature: parseTextSignature().
  OpenAIResponsesStreamOptions.applyServiceTierPricing: OpenAIResponsesStreamOptions#applyServiceTierPricing.
  mapStopReason: mapStopReason().
  OpenAIResponsesStreamOptions.serviceTier: OpenAIResponsesStreamOptions#serviceTier.
  OpenAIResponsesStreamOptions.resolveServiceTier: OpenAIResponsesStreamOptions#resolveServiceTier.
  ConvertResponsesToolsOptions.strict: ConvertResponsesToolsOptions#strict.
  OpenAIResponsesStreamOptions: OpenAIResponsesStreamOptions#
  ConvertResponsesMessagesOptions: ConvertResponsesMessagesOptions#
  ConvertResponsesMessagesOptions.includeSystemPrompt: ConvertResponsesMessagesOptions#includeSystemPrompt.
  ConvertResponsesToolsOptions: ConvertResponsesToolsOptions#
---
# Module: [`packages/ai/src/providers/openai-responses-shared.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses-shared.ts)

## Classes
### `ConvertResponsesMessagesOptions`
- def: [`packages/ai/src/providers/openai-responses-shared.ts:79`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses-shared.ts#L79)
- signature: `interface ConvertResponsesMessagesOptions`
- members:
  - `includeSystemPrompt` — [`L80`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses-shared.ts#L80)
- used by: [`convertResponsesMessages`](openai-responses-shared.ts.md#convertResponsesMessages)

### `ConvertResponsesToolsOptions`
- def: [`packages/ai/src/providers/openai-responses-shared.ts:83`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses-shared.ts#L83)
- signature: `interface ConvertResponsesToolsOptions`
- members:
  - `strict` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses-shared.ts#L84)
- used by: [`convertResponsesTools`](openai-responses-shared.ts.md#convertResponsesTools)

### `OpenAIResponsesStreamOptions`
- def: [`packages/ai/src/providers/openai-responses-shared.ts:67`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses-shared.ts#L67)
- signature: `interface OpenAIResponsesStreamOptions`
- members:
  - `applyServiceTierPricing` — [`L73`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses-shared.ts#L73)
  - `resolveServiceTier` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses-shared.ts#L69)
  - `serviceTier` — [`L68`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses-shared.ts#L68)
- uses (calls/refs, reference-scoped): [`Usage`](../types.ts.md#Usage)
- used by: [`processResponsesStream`](openai-responses-shared.ts.md#processResponsesStream)

## Functions
- `convertResponsesMessages(model: Model<TApi>, context: Context, allowedToolCallProviders: ReadonlySet<string>, options?: ConvertResponsesMessagesOptions | undefined)` — [`L91`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses-shared.ts#L91)
- `convertResponsesTools(tools: Tool<TSchema>[], options?: ConvertResponsesToolsOptions | undefined)` — [`L269`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses-shared.ts#L269)
- `encodeTextSignatureV1(id: string, phase?: "commentary" | "final_answer" | undefined)` — [`L41`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses-shared.ts#L41)
- `mapStopReason(status: ResponseStatus | undefined)` — [`L543`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses-shared.ts#L543)
- `parseTextSignature(signature: string | undefined)` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses-shared.ts#L47)
- `processResponsesStream(openaiStream: AsyncIterable<ResponseStreamEvent>, output: AssistantMessage, stream: AssistantMessageEventStream, model: Model<...>, options?: OpenAIResponsesStreamOptions | undefined)` — [`L284`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses-shared.ts#L284)


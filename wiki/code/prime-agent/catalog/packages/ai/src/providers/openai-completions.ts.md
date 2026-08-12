---
title: 'Module: packages/ai/src/providers/openai-completions.ts'
type: catalog
provenance: extracted
module: packages/ai/src/providers/openai-completions.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/providers/`openai-completions.ts`/
symbols:
  streamOpenAICompletions: streamOpenAICompletions.
  convertMessages: convertMessages().
  buildParams: buildParams().
  getCompat: getCompat().
  parseChunkUsage.rawUsage-typeLiteral506.prompt_tokens_details.typeLiteral507.cache_write_tokens: parseChunkUsage().(rawUsage)typeLiteral506:prompt_tokens_details.typeLiteral507:cache_write_tokens.
  detectCompat: detectCompat().
  createClient: createClient().
  streamSimpleOpenAICompletions: streamSimpleOpenAICompletions.
  hasToolHistory: hasToolHistory().
  convertTools: convertTools().
  OpenAICompletionsOptions.reasoningEffort: OpenAICompletionsOptions#reasoningEffort.
  OpenAICompletionsOptions: OpenAICompletionsOptions#
  ResolvedOpenAICompletionsCompat: ResolvedOpenAICompletionsCompat#
  getCompatCacheControl: getCompatCacheControl().
  OpenAICompatCacheControl: OpenAICompatCacheControl#
  applyAnthropicCacheControl: applyAnthropicCacheControl().
  mapStopReason.typeLiteral168.stopReason: mapStopReason().typeLiteral168:stopReason.
  addCacheControlToTextContent: addCacheControlToTextContent().
  addCacheControlToInstructionMessage: addCacheControlToInstructionMessage().
  isTextContentBlock: isTextContentBlock().
  isThinkingContentBlock: isThinkingContentBlock().
  isToolCallBlock: isToolCallBlock().
  isImageContentBlock: isImageContentBlock().
  addCacheControlToSystemPrompt: addCacheControlToSystemPrompt().
  addCacheControlToLastConversationMessage: addCacheControlToLastConversationMessage().
  addCacheControlToLastTool: addCacheControlToLastTool().
  addCacheControlToMessage: addCacheControlToMessage().
  mapStopReason: mapStopReason().
  mapStopReason.typeLiteral168.errorMessage: mapStopReason().typeLiteral168:errorMessage.
  ChatCompletionTextPartWithCacheControl: ChatCompletionTextPartWithCacheControl#
  resolveCacheRetention: resolveCacheRetention().
  OpenAICompletionsOptions.toolChoice: OpenAICompletionsOptions#toolChoice.
  ChatCompletionToolWithCacheControl: ChatCompletionToolWithCacheControl#
  ChatCompletionInstructionMessageParam: ChatCompletionInstructionMessageParam#
  parseChunkUsage: parseChunkUsage().
  parseChunkUsage.rawUsage-typeLiteral506.prompt_tokens_details: parseChunkUsage().(rawUsage)typeLiteral506:prompt_tokens_details.
  isTextContentBlock.block-typeLiteral7.type: isTextContentBlock().(block)typeLiteral7:type.
  isThinkingContentBlock.block-typeLiteral8.type: isThinkingContentBlock().(block)typeLiteral8:type.
  isToolCallBlock.block-typeLiteral9.type: isToolCallBlock().(block)typeLiteral9:type.
  isImageContentBlock.block-typeLiteral10.type: isImageContentBlock().(block)typeLiteral10:type.
  OpenAICompatCacheControl.ttl: OpenAICompatCacheControl#ttl.
  parseChunkUsage.rawUsage-typeLiteral506.prompt_tokens: parseChunkUsage().(rawUsage)typeLiteral506:prompt_tokens.
  parseChunkUsage.rawUsage-typeLiteral506.completion_tokens: parseChunkUsage().(rawUsage)typeLiteral506:completion_tokens.
  parseChunkUsage.rawUsage-typeLiteral506.prompt_cache_hit_tokens: parseChunkUsage().(rawUsage)typeLiteral506:prompt_cache_hit_tokens.
  parseChunkUsage.rawUsage-typeLiteral506.prompt_tokens_details.typeLiteral507.cached_tokens: parseChunkUsage().(rawUsage)typeLiteral506:prompt_tokens_details.typeLiteral507:cached_tokens.
  OpenAICompatCacheControl.type: OpenAICompatCacheControl#type.
---
# Module: [`packages/ai/src/providers/openai-completions.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts)

## Classes
### `ChatCompletionInstructionMessageParam`
- def: [`packages/ai/src/providers/openai-completions.ts:92`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L92)
- signature: `type ChatCompletionInstructionMessageParam`
- used by: [`addCacheControlToTextContent`](openai-completions.ts.md#addCacheControlToTextContent), [`addCacheControlToInstructionMessage`](openai-completions.ts.md#addCacheControlToInstructionMessage)

### `ChatCompletionTextPartWithCacheControl`
- def: [`packages/ai/src/providers/openai-completions.ts:94`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L94)
- signature: `type ChatCompletionTextPartWithCacheControl`
- uses (calls/refs, reference-scoped): [`OpenAICompatCacheControl`](openai-completions.ts.md#OpenAICompatCacheControl)
- used by: [`addCacheControlToTextContent`](openai-completions.ts.md#addCacheControlToTextContent)

### `ChatCompletionToolWithCacheControl`
- def: [`packages/ai/src/providers/openai-completions.ts:98`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L98)
- signature: `type ChatCompletionToolWithCacheControl`
- uses (calls/refs, reference-scoped): [`OpenAICompatCacheControl`](openai-completions.ts.md#OpenAICompatCacheControl)
- used by: [`addCacheControlToLastTool`](openai-completions.ts.md#addCacheControlToLastTool)

### `OpenAICompatCacheControl`
- def: [`packages/ai/src/providers/openai-completions.ts:83`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L83)
- signature: `interface OpenAICompatCacheControl`
- members:
  - `ttl` — [`L85`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L85)
  - `type` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L84)
- used by: [`streamOpenAICompletions`](openai-completions.ts.md#streamOpenAICompletions), [`buildParams`](openai-completions.ts.md#buildParams), [`getCompatCacheControl`](openai-completions.ts.md#getCompatCacheControl), [`applyAnthropicCacheControl`](openai-completions.ts.md#applyAnthropicCacheControl), [`addCacheControlToTextContent`](openai-completions.ts.md#addCacheControlToTextContent), [`addCacheControlToInstructionMessage`](openai-completions.ts.md#addCacheControlToInstructionMessage), [`addCacheControlToLastConversationMessage`](openai-completions.ts.md#addCacheControlToLastConversationMessage), [`addCacheControlToLastTool`](openai-completions.ts.md#addCacheControlToLastTool), [`addCacheControlToMessage`](openai-completions.ts.md#addCacheControlToMessage), [`addCacheControlToSystemPrompt`](openai-completions.ts.md#addCacheControlToSystemPrompt), [`ChatCompletionTextPartWithCacheControl`](openai-completions.ts.md#ChatCompletionTextPartWithCacheControl), [`ChatCompletionToolWithCacheControl`](openai-completions.ts.md#ChatCompletionToolWithCacheControl)

### `OpenAICompletionsOptions`
- def: [`packages/ai/src/providers/openai-completions.ts:78`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L78)
- signature: `interface OpenAICompletionsOptions`
- members:
  - `reasoningEffort` — [`L80`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L80)
  - `toolChoice` — [`L79`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L79)
- uses (calls/refs, reference-scoped): [`StreamOptions`](../types.ts.md#StreamOptions)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`streamOpenAICompletions`](openai-completions.ts.md#streamOpenAICompletions), [`openai-completions.ts`](openai-completions.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-openai-completions.ts), [`buildParams`](openai-completions.ts.md#buildParams), [`register-builtins.ts`](register-builtins.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-register-builtins.ts), [`streamSimpleOpenAICompletions`](openai-completions.ts.md#streamSimpleOpenAICompletions), [`loadOpenAICompletionsProviderModule`](register-builtins.ts.md#loadOpenAICompletionsProviderModule), [`openAICompletionsProviderModulePromise`](register-builtins.ts.md#openAICompletionsProviderModulePromise), [`streamOpenAICompletions`](register-builtins.ts.md#OpenAICompletionsProviderModule.streamOpenAICompletions)

### `ResolvedOpenAICompletionsCompat`
- def: [`packages/ai/src/providers/openai-completions.ts:88`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L88)
- signature: `type ResolvedOpenAICompletionsCompat`
- uses (calls/refs, reference-scoped): [`OpenAICompletionsCompat`](../types.ts.md#OpenAICompletionsCompat), [`cacheControlFormat`](../types.ts.md#OpenAICompletionsCompat.cacheControlFormat)
- used by: [`convertMessages`](openai-completions.ts.md#convertMessages), [`buildParams`](openai-completions.ts.md#buildParams), [`getCompat`](openai-completions.ts.md#getCompat), [`detectCompat`](openai-completions.ts.md#detectCompat), [`createClient`](openai-completions.ts.md#createClient), [`convertTools`](openai-completions.ts.md#convertTools), [`getCompatCacheControl`](openai-completions.ts.md#getCompatCacheControl)

## Functions
- `addCacheControlToInstructionMessage(message: ChatCompletionInstructionMessageParam, cacheControl: OpenAICompatCacheControl)` — [`L678`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L678)
- `addCacheControlToLastConversationMessage(messages: ChatCompletionMessageParam[], cacheControl: OpenAICompatCacheControl)` — [`L652`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L652)
- `addCacheControlToLastTool(tools: ChatCompletionTool[] | undefined, cacheControl: OpenAICompatCacheControl)` — [`L666`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L666)
- `addCacheControlToMessage(message: ChatCompletionMessageParam, cacheControl: OpenAICompatCacheControl)` — [`L685`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L685)
- `addCacheControlToSystemPrompt(messages: ChatCompletionMessageParam[], cacheControl: OpenAICompatCacheControl)` — [`L640`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L640)
- `addCacheControlToTextContent(message: ChatCompletionUserMessageParam | ChatCompletionAssistantMessageParam | ChatCompletionInstructionMessageParam, cacheControl: OpenAICompatCacheControl)` — [`L695`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L695)
- `applyAnthropicCacheControl(messages: ChatCompletionMessageParam[], tools: ChatCompletionTool[] | undefined, cacheControl: OpenAICompatCacheControl)` — [`L630`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L630)
- `buildParams(model: Model<"openai-completions">, context: Context, options?: OpenAICompletionsOptions | undefined, compat?: ResolvedOpenAICompletionsCompat, cacheRetention?: CacheRetention, cacheControl?: OpenAICompatCacheControl | undefined)` — [`L504`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L504)
- `convertMessages(model: Model<"openai-completions">, context: Context, compat: ResolvedOpenAICompletionsCompat)` — [`L733`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L733)
- `convertTools(tools: Tool<TSchema>[], compat: ResolvedOpenAICompletionsCompat)` — [`L989`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L989)
- `createClient(model: Model<"openai-completions">, context: Context, apiKey?: string | undefined, optionsHeaders?: Record<string, string> | undefined, sessionId?: string | undefined, compat?: ResolvedOpenAICompletionsCompat)` — [`L444`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L444)
- `detectCompat(model: Model<"openai-completions">)` — [`L1073`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L1073) — Detect compatibility settings from provider and baseUrl for known providers.
- `getCompat(model: Model<"openai-completions">)` — [`L1137`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L1137) — Get resolved compatibility settings for a model.
- `getCompatCacheControl(compat: ResolvedOpenAICompletionsCompat, cacheRetention: CacheRetention)` — [`L618`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L618)
- `hasToolHistory(messages: Message[])` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L48) — Check if conversation messages contain tool calls or tool results.
- `isImageContentBlock(block: { type: string; })` — [`L74`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L74)
- `isTextContentBlock(block: { type: string; })` — [`L62`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L62)
- `isThinkingContentBlock(block: { type: string; })` — [`L66`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L66)
- `isToolCallBlock(block: { type: string; })` — [`L70`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L70)
- `mapStopReason(reason: string | null)` — [`L1042`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L1042)
- `parseChunkUsage(rawUsage: { prompt_tokens?: number | undefined; completion_tokens?: number | undefined; prompt_cache_hit_tokens?: number | undefined; prompt_tokens_details?: { cached_tokens?: number | undefined; cache_write_tokens?: number | undefined; } | undefined; }, model: Model<...>, cacheWriteCost?: number | undefined)` — [`L1005`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L1005)
- `resolveCacheRetention(cacheRetention?: CacheRetention | undefined)` — [`L102`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L102)

## Module values
- `cache_write_tokens` — [`L1010`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L1010)
- `cached_tokens` — [`L1010`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L1010)
- `completion_tokens` — [`L1008`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L1008)
- `errorMessage` — [`L1044`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L1044)
- `prompt_cache_hit_tokens` — [`L1009`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L1009)
- `prompt_tokens` — [`L1007`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L1007)
- `prompt_tokens_details` — [`L1010`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L1010)
- `stopReason` — [`L1043`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L1043)
- `streamOpenAICompletions` — [`L112`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L112)
- `streamSimpleOpenAICompletions` — [`L422`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L422)
- `type` — [`L62`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L62)
- `type` — [`L66`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L66)
- `type` — [`L70`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L70)
- `type` — [`L74`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-completions.ts#L74)


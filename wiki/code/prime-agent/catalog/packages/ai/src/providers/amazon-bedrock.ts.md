---
title: 'Module: packages/ai/src/providers/amazon-bedrock.ts'
type: catalog
provenance: extracted
module: packages/ai/src/providers/amazon-bedrock.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/providers/`amazon-bedrock.ts`/
symbols:
  streamBedrock: streamBedrock.
  convertMessages: convertMessages().
  streamSimpleBedrock: streamSimpleBedrock.
  buildAdditionalModelRequestFields: buildAdditionalModelRequestFields().
  handleContentBlockDelta: handleContentBlockDelta().
  handleContentBlockStop: handleContentBlockStop().
  handleMetadata: handleMetadata().
  handleContentBlockStart: handleContentBlockStart().
  BedrockOptions: BedrockOptions#
  Block: Block#
  convertToolConfig: convertToolConfig().
  BedrockOptions.reasoning: BedrockOptions#reasoning.
  mapThinkingLevelToEffort: mapThinkingLevelToEffort().
  supportsPromptCaching: supportsPromptCaching().
  buildSystemPrompt: buildSystemPrompt().
  isGovCloudBedrockTarget: isGovCloudBedrockTarget().
  isAnthropicClaudeModel: isAnthropicClaudeModel().
  getConfiguredBedrockRegion: getConfiguredBedrockRegion().
  BedrockOptions.thinkingBudgets: BedrockOptions#thinkingBudgets.
  supportsThinkingSignature: supportsThinkingSignature().
  supportsAdaptiveThinking: supportsAdaptiveThinking().
  BedrockOptions.thinkingDisplay: BedrockOptions#thinkingDisplay.
  formatBedrockError: formatBedrockError().
  supportsAlwaysOnAdaptiveThinking: supportsAlwaysOnAdaptiveThinking().
  resolveCacheRetention: resolveCacheRetention().
  mapStopReason: mapStopReason().
  shouldUseExplicitBedrockEndpoint: shouldUseExplicitBedrockEndpoint().
  getModelMatchCandidates: getModelMatchCandidates().
  createImageBlock: createImageBlock().
  BedrockThinkingDisplay: BedrockThinkingDisplay#
  BedrockOptions.region: BedrockOptions#region.
  BedrockOptions.toolChoice: BedrockOptions#toolChoice.
  BedrockOptions.requestMetadata: BedrockOptions#requestMetadata.
  getStandardBedrockEndpointRegion: getStandardBedrockEndpointRegion().
  BedrockOptions.profile: BedrockOptions#profile.
  BedrockOptions.interleavedThinking: BedrockOptions#interleavedThinking.
  BedrockOptions.bearerToken: BedrockOptions#bearerToken.
  BEDROCK_ERROR_PREFIXES: BEDROCK_ERROR_PREFIXES.
  normalizeToolCallId: normalizeToolCallId().
  hasConfiguredBedrockProfile: hasConfiguredBedrockProfile().
---
# Module: [`packages/ai/src/providers/amazon-bedrock.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts)

## Classes
### `BedrockOptions`
- def: [`packages/ai/src/providers/amazon-bedrock.ts:52`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L52)
- signature: `interface BedrockOptions`
- members:
  - `bearerToken` — [`L83`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L83) — Bearer token for Bedrock API key authentication.
  - `interleavedThinking` — [`L61`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L61)
  - `profile` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L54)
  - `reasoning` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L57)
  - `region` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L53)
  - `requestMetadata` — [`L77`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L77) — Key-value pairs attached to the inference request for cost allocation tagging.
  - `thinkingBudgets` — [`L59`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L59)
  - `thinkingDisplay` — [`L72`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L72) — Controls how Claude's thinking content is returned in responses.
  - `toolChoice` — [`L55`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L55)
- uses (calls/refs, reference-scoped): [`StreamOptions`](../types.ts.md#StreamOptions), [`ThinkingLevel`](../types.ts.md#ThinkingLevel), [`ThinkingBudgets`](../types.ts.md#ThinkingBudgets), [`BedrockThinkingDisplay`](amazon-bedrock.ts.md#BedrockThinkingDisplay)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`streamBedrock`](amazon-bedrock.ts.md#streamBedrock), [`amazon-bedrock.ts`](amazon-bedrock.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-amazon-bedrock.ts), [`register-builtins.ts`](register-builtins.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-register-builtins.ts), [`streamSimpleBedrock`](amazon-bedrock.ts.md#streamSimpleBedrock), [`buildAdditionalModelRequestFields`](amazon-bedrock.ts.md#buildAdditionalModelRequestFields), [`loadBedrockProviderModule`](register-builtins.ts.md#loadBedrockProviderModule), [`convertToolConfig`](amazon-bedrock.ts.md#convertToolConfig), [`streamBedrock`](register-builtins.ts.md#BedrockProviderModule.streamBedrock), [`isGovCloudBedrockTarget`](amazon-bedrock.ts.md#isGovCloudBedrockTarget), [`bedrockProviderModuleOverride`](register-builtins.ts.md#bedrockProviderModuleOverride), [`bedrockProviderModulePromise`](register-builtins.ts.md#bedrockProviderModulePromise), [`getConfiguredBedrockRegion`](amazon-bedrock.ts.md#getConfiguredBedrockRegion)  (2 test-only)

### `BedrockThinkingDisplay`
- def: [`packages/ai/src/providers/amazon-bedrock.ts:50`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L50)
- signature: `type BedrockThinkingDisplay`
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`thinkingDisplay`](amazon-bedrock.ts.md#BedrockOptions.thinkingDisplay)

### `Block`
- def: [`packages/ai/src/providers/amazon-bedrock.ts:86`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L86)
- signature: `type Block`
- uses (calls/refs, reference-scoped): [`TextContent`](../types.ts.md#TextContent), [`ToolCall`](../types.ts.md#ToolCall), [`ThinkingContent`](../types.ts.md#ThinkingContent)
- used by: [`streamBedrock`](amazon-bedrock.ts.md#streamBedrock), [`handleContentBlockDelta`](amazon-bedrock.ts.md#handleContentBlockDelta), [`handleContentBlockStop`](amazon-bedrock.ts.md#handleContentBlockStop), [`handleContentBlockStart`](amazon-bedrock.ts.md#handleContentBlockStart)

## Functions
- `buildAdditionalModelRequestFields(model: Model<"bedrock-converse-stream">, options: BedrockOptions)` — [`L907`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L907)
- `buildSystemPrompt(systemPrompt: string | undefined, model: Model<"bedrock-converse-stream">, cacheRetention: CacheRetention)` — [`L625`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L625)
- `convertMessages(context: Context, model: Model<"bedrock-converse-stream">, cacheRetention: CacheRetention)` — [`L649`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L649)
- `convertToolConfig(tools: Tool<TSchema>[] | undefined, toolChoice: "auto" | "none" | "any" | { type: "tool"; name: string; } | undefined)` — [`L808`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L808)
- `createImageBlock(mimeType: string, data: string)` — [`L957`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L957)
- `formatBedrockError(error: unknown)` — [`L309`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L309) — Format a Bedrock error with a human-readable prefix.
- `getConfiguredBedrockRegion(options: BedrockOptions)` — [`L854`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L854)
- `getModelMatchCandidates(modelId: string, modelName?: string | undefined)` — [`L491`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L491) — Check if the model supports adaptive thinking (Opus 4.6+, Sonnet 4.6).
- `getStandardBedrockEndpointRegion(baseUrl: string | undefined)` — [`L870`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L870)
- `handleContentBlockDelta(event: ContentBlockDeltaEvent, blocks: Block[], output: AssistantMessage, stream: AssistantMessageEventStream)` — [`L385`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L385)
- `handleContentBlockStart(event: ContentBlockStartEvent, blocks: Block[], output: AssistantMessage, stream: AssistantMessageEventStream)` — [`L362`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L362)
- `handleContentBlockStop(event: ContentBlockStopEvent, blocks: Block[], output: AssistantMessage, stream: AssistantMessageEventStream)` — [`L458`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L458)
- `handleMetadata(event: ConverseStreamMetadataEvent, model: Model<"bedrock-converse-stream">, output: AssistantMessage)` — [`L443`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L443)
- `hasConfiguredBedrockProfile()` — [`L862`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L862)
- `isAnthropicClaudeModel(model: Model<"bedrock-converse-stream">)` — [`L570`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L570) — Check if the model is an Anthropic Claude model on Bedrock.
- `isGovCloudBedrockTarget(model: Model<"bedrock-converse-stream">, options: BedrockOptions)` — [`L897`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L897)
- `mapStopReason(reason: string | undefined)` — [`L839`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L839)
- `mapThinkingLevelToEffort(model: Model<"bedrock-converse-stream">, level: ThinkingLevel | undefined)` — [`L523`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L523)
- `normalizeToolCallId(id: string)` — [`L644`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L644)
- `resolveCacheRetention(cacheRetention?: CacheRetention | undefined)` — [`L555`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L555) — Resolve cache retention preference.
- `shouldUseExplicitBedrockEndpoint(baseUrl: string, configuredRegion: string | undefined, hasConfiguredProfile: boolean)` — [`L884`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L884)
- `supportsAdaptiveThinking(modelId: string, modelName?: string | undefined)` — [`L499`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L499)
- `supportsAlwaysOnAdaptiveThinking(modelId: string, modelName?: string | undefined)` — [`L518`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L518) — Fable/Mythos models think every turn and reject sampling params with a 400.
- `supportsPromptCaching(model: Model<"bedrock-converse-stream">)` — [`L594`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L594) — Check if the model supports prompt caching.
- `supportsThinkingSignature(model: Model<"bedrock-converse-stream">)` — [`L621`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L621) — Check if the model supports thinking signatures in reasoningContent.

## Module values
- `BEDROCK_ERROR_PREFIXES` — [`L294`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L294) — Human-readable prefixes for Bedrock SDK exception names.
- `streamBedrock` — [`L88`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L88)
- `streamSimpleBedrock` — [`L318`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/amazon-bedrock.ts#L318)


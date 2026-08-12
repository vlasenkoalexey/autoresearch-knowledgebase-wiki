---
title: 'Module: packages/ai/src/providers/register-builtins.ts'
type: catalog
provenance: extracted
module: packages/ai/src/providers/register-builtins.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/providers/`register-builtins.ts`/
symbols:
  createLazyLoadErrorMessage: createLazyLoadErrorMessage().
  registerBuiltInApiProviders: registerBuiltInApiProviders().
  createLazyStream: createLazyStream().
  createLazySimpleStream: createLazySimpleStream().
  LazyProviderModule: LazyProviderModule#
  loadBedrockProviderModule: loadBedrockProviderModule().
  loadAnthropicProviderModule: loadAnthropicProviderModule().
  loadAzureOpenAIResponsesProviderModule: loadAzureOpenAIResponsesProviderModule().
  loadGoogleProviderModule: loadGoogleProviderModule().
  loadGoogleVertexProviderModule: loadGoogleVertexProviderModule().
  loadMistralProviderModule: loadMistralProviderModule().
  loadOpenAICodexResponsesProviderModule: loadOpenAICodexResponsesProviderModule().
  loadOpenAICompletionsProviderModule: loadOpenAICompletionsProviderModule().
  loadOpenAIResponsesProviderModule: loadOpenAIResponsesProviderModule().
  BedrockProviderModule.streamBedrock: BedrockProviderModule#streamBedrock.
  BedrockProviderModule.streamSimpleBedrock: BedrockProviderModule#streamSimpleBedrock.
  setBedrockProviderModule: setBedrockProviderModule().
  forwardStream: forwardStream().
  bedrockProviderModuleOverride: bedrockProviderModuleOverride.
  anthropicProviderModulePromise: anthropicProviderModulePromise.
  azureOpenAIResponsesProviderModulePromise: azureOpenAIResponsesProviderModulePromise.
  googleProviderModulePromise: googleProviderModulePromise.
  googleVertexProviderModulePromise: googleVertexProviderModulePromise.
  mistralProviderModulePromise: mistralProviderModulePromise.
  openAICodexResponsesProviderModulePromise: openAICodexResponsesProviderModulePromise.
  openAICompletionsProviderModulePromise: openAICompletionsProviderModulePromise.
  openAIResponsesProviderModulePromise: openAIResponsesProviderModulePromise.
  bedrockProviderModulePromise: bedrockProviderModulePromise.
  resetApiProviders: resetApiProviders().
  LazyProviderModule.stream: LazyProviderModule#stream.
  LazyProviderModule.streamSimple: LazyProviderModule#streamSimple.
  streamSimpleAnthropic: streamSimpleAnthropic.
  streamSimpleOpenAIResponses: streamSimpleOpenAIResponses.
  AnthropicProviderModule: AnthropicProviderModule#
  AnthropicProviderModule.streamAnthropic: AnthropicProviderModule#streamAnthropic.
  AzureOpenAIResponsesProviderModule: AzureOpenAIResponsesProviderModule#
  AzureOpenAIResponsesProviderModule.streamAzureOpenAIResponses: AzureOpenAIResponsesProviderModule#streamAzureOpenAIResponses.
  GoogleProviderModule: GoogleProviderModule#
  GoogleProviderModule.streamGoogle: GoogleProviderModule#streamGoogle.
  GoogleVertexProviderModule: GoogleVertexProviderModule#
  GoogleVertexProviderModule.streamGoogleVertex: GoogleVertexProviderModule#streamGoogleVertex.
  MistralProviderModule: MistralProviderModule#
  MistralProviderModule.streamMistral: MistralProviderModule#streamMistral.
  OpenAICodexResponsesProviderModule: OpenAICodexResponsesProviderModule#
  OpenAICodexResponsesProviderModule.streamOpenAICodexResponses: OpenAICodexResponsesProviderModule#streamOpenAICodexResponses.
  OpenAICompletionsProviderModule: OpenAICompletionsProviderModule#
  OpenAICompletionsProviderModule.streamOpenAICompletions: OpenAICompletionsProviderModule#streamOpenAICompletions.
  OpenAIResponsesProviderModule: OpenAIResponsesProviderModule#
  OpenAIResponsesProviderModule.streamOpenAIResponses: OpenAIResponsesProviderModule#streamOpenAIResponses.
  streamAnthropic: streamAnthropic.
  streamAzureOpenAIResponses: streamAzureOpenAIResponses.
  streamSimpleAzureOpenAIResponses: streamSimpleAzureOpenAIResponses.
  streamGoogle: streamGoogle.
  streamSimpleGoogle: streamSimpleGoogle.
  streamGoogleVertex: streamGoogleVertex.
  streamSimpleGoogleVertex: streamSimpleGoogleVertex.
  streamMistral: streamMistral.
  streamSimpleMistral: streamSimpleMistral.
  streamOpenAICodexResponses: streamOpenAICodexResponses.
  streamSimpleOpenAICodexResponses: streamSimpleOpenAICodexResponses.
  streamOpenAICompletions: streamOpenAICompletions.
  streamSimpleOpenAICompletions: streamSimpleOpenAICompletions.
  streamOpenAIResponses: streamOpenAIResponses.
  streamBedrockLazy: streamBedrockLazy.
  streamSimpleBedrockLazy: streamSimpleBedrockLazy.
  BedrockProviderModule: BedrockProviderModule#
  AnthropicProviderModule.streamSimpleAnthropic: AnthropicProviderModule#streamSimpleAnthropic.
  AzureOpenAIResponsesProviderModule.streamSimpleAzureOpenAIResponses: AzureOpenAIResponsesProviderModule#streamSimpleAzureOpenAIResponses.
  GoogleProviderModule.streamSimpleGoogle: GoogleProviderModule#streamSimpleGoogle.
  GoogleVertexProviderModule.streamSimpleGoogleVertex: GoogleVertexProviderModule#streamSimpleGoogleVertex.
  MistralProviderModule.streamSimpleMistral: MistralProviderModule#streamSimpleMistral.
  OpenAICodexResponsesProviderModule.streamSimpleOpenAICodexResponses: OpenAICodexResponsesProviderModule#streamSimpleOpenAICodexResponses.
  OpenAICompletionsProviderModule.streamSimpleOpenAICompletions: OpenAICompletionsProviderModule#streamSimpleOpenAICompletions.
  OpenAIResponsesProviderModule.streamSimpleOpenAIResponses: OpenAIResponsesProviderModule#streamSimpleOpenAIResponses.
  importNodeOnlyProvider: importNodeOnlyProvider.
---
# Module: [`packages/ai/src/providers/register-builtins.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts)

## Classes
### `AnthropicProviderModule`
- def: [`packages/ai/src/providers/register-builtins.ts:36`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L36)
- signature: `interface AnthropicProviderModule`
- members:
  - `streamAnthropic` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L37)
  - `streamSimpleAnthropic` — [`L38`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L38)
- uses (calls/refs, reference-scoped): [`SimpleStreamOptions`](../types.ts.md#SimpleStreamOptions), [`StreamFunction`](../types.ts.md#StreamFunction), [`AnthropicOptions`](anthropic.ts.md#AnthropicOptions)
- used by: [`loadAnthropicProviderModule`](register-builtins.ts.md#loadAnthropicProviderModule)

### `AzureOpenAIResponsesProviderModule`
- def: [`packages/ai/src/providers/register-builtins.ts:41`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L41)
- signature: `interface AzureOpenAIResponsesProviderModule`
- members:
  - `streamAzureOpenAIResponses` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L42)
  - `streamSimpleAzureOpenAIResponses` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L43)
- uses (calls/refs, reference-scoped): [`SimpleStreamOptions`](../types.ts.md#SimpleStreamOptions), [`StreamFunction`](../types.ts.md#StreamFunction), [`AzureOpenAIResponsesOptions`](azure-openai-responses.ts.md#AzureOpenAIResponsesOptions)
- used by: [`loadAzureOpenAIResponsesProviderModule`](register-builtins.ts.md#loadAzureOpenAIResponsesProviderModule)

### `BedrockProviderModule`
- def: [`packages/ai/src/providers/register-builtins.ts:76`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L76)
- signature: `interface BedrockProviderModule`
- members:
  - `streamBedrock` — [`L77`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L77)
  - `streamSimpleBedrock` — [`L82`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L82)
- uses (calls/refs, reference-scoped): [`Model`](../types.ts.md#Model), [`Context`](../types.ts.md#Context), [`SimpleStreamOptions`](../types.ts.md#SimpleStreamOptions), [`AssistantMessageEvent`](../types.ts.md#AssistantMessageEvent), [`BedrockOptions`](amazon-bedrock.ts.md#BedrockOptions)
- used by: [`loadBedrockProviderModule`](register-builtins.ts.md#loadBedrockProviderModule), [`setBedrockProviderModule`](register-builtins.ts.md#setBedrockProviderModule)

### `GoogleProviderModule`
- def: [`packages/ai/src/providers/register-builtins.ts:46`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L46)
- signature: `interface GoogleProviderModule`
- members:
  - `streamGoogle` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L47)
  - `streamSimpleGoogle` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L48)
- uses (calls/refs, reference-scoped): [`SimpleStreamOptions`](../types.ts.md#SimpleStreamOptions), [`StreamFunction`](../types.ts.md#StreamFunction), [`GoogleOptions`](google.ts.md#GoogleOptions)
- used by: [`loadGoogleProviderModule`](register-builtins.ts.md#loadGoogleProviderModule)

### `GoogleVertexProviderModule`
- def: [`packages/ai/src/providers/register-builtins.ts:51`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L51)
- signature: `interface GoogleVertexProviderModule`
- members:
  - `streamGoogleVertex` — [`L52`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L52)
  - `streamSimpleGoogleVertex` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L53)
- uses (calls/refs, reference-scoped): [`SimpleStreamOptions`](../types.ts.md#SimpleStreamOptions), [`StreamFunction`](../types.ts.md#StreamFunction), [`GoogleVertexOptions`](google-vertex.ts.md#GoogleVertexOptions)
- used by: [`loadGoogleVertexProviderModule`](register-builtins.ts.md#loadGoogleVertexProviderModule)

### `LazyProviderModule`
- def: [`packages/ai/src/providers/register-builtins.ts:23`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L23)
- signature: `interface LazyProviderModule`
- members:
  - `stream` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L28)
  - `streamSimple` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L29)
- uses (calls/refs, reference-scoped): [`Model`](../types.ts.md#Model), [`Api`](../types.ts.md#Api), [`Context`](../types.ts.md#Context), [`SimpleStreamOptions`](../types.ts.md#SimpleStreamOptions), [`StreamOptions`](../types.ts.md#StreamOptions), [`AssistantMessageEvent`](../types.ts.md#AssistantMessageEvent)
- used by: [`createLazySimpleStream`](register-builtins.ts.md#createLazySimpleStream), [`createLazyStream`](register-builtins.ts.md#createLazyStream), [`loadBedrockProviderModule`](register-builtins.ts.md#loadBedrockProviderModule), [`loadAnthropicProviderModule`](register-builtins.ts.md#loadAnthropicProviderModule), [`loadAzureOpenAIResponsesProviderModule`](register-builtins.ts.md#loadAzureOpenAIResponsesProviderModule), [`loadGoogleProviderModule`](register-builtins.ts.md#loadGoogleProviderModule), [`loadGoogleVertexProviderModule`](register-builtins.ts.md#loadGoogleVertexProviderModule), [`loadMistralProviderModule`](register-builtins.ts.md#loadMistralProviderModule), [`loadOpenAICodexResponsesProviderModule`](register-builtins.ts.md#loadOpenAICodexResponsesProviderModule), [`loadOpenAICompletionsProviderModule`](register-builtins.ts.md#loadOpenAICompletionsProviderModule), [`loadOpenAIResponsesProviderModule`](register-builtins.ts.md#loadOpenAIResponsesProviderModule), [`bedrockProviderModuleOverride`](register-builtins.ts.md#bedrockProviderModuleOverride), [`anthropicProviderModulePromise`](register-builtins.ts.md#anthropicProviderModulePromise), [`azureOpenAIResponsesProviderModulePromise`](register-builtins.ts.md#azureOpenAIResponsesProviderModulePromise), [`bedrockProviderModulePromise`](register-builtins.ts.md#bedrockProviderModulePromise), [`googleProviderModulePromise`](register-builtins.ts.md#googleProviderModulePromise), [`googleVertexProviderModulePromise`](register-builtins.ts.md#googleVertexProviderModulePromise), [`mistralProviderModulePromise`](register-builtins.ts.md#mistralProviderModulePromise), [`openAICodexResponsesProviderModulePromise`](register-builtins.ts.md#openAICodexResponsesProviderModulePromise), [`openAICompletionsProviderModulePromise`](register-builtins.ts.md#openAICompletionsProviderModulePromise), [`openAIResponsesProviderModulePromise`](register-builtins.ts.md#openAIResponsesProviderModulePromise)

### `MistralProviderModule`
- def: [`packages/ai/src/providers/register-builtins.ts:56`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L56)
- signature: `interface MistralProviderModule`
- members:
  - `streamMistral` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L57)
  - `streamSimpleMistral` — [`L58`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L58)
- uses (calls/refs, reference-scoped): [`SimpleStreamOptions`](../types.ts.md#SimpleStreamOptions), [`StreamFunction`](../types.ts.md#StreamFunction), [`MistralOptions`](mistral.ts.md#MistralOptions)
- used by: [`loadMistralProviderModule`](register-builtins.ts.md#loadMistralProviderModule)

### `OpenAICodexResponsesProviderModule`
- def: [`packages/ai/src/providers/register-builtins.ts:61`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L61)
- signature: `interface OpenAICodexResponsesProviderModule`
- members:
  - `streamOpenAICodexResponses` — [`L62`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L62)
  - `streamSimpleOpenAICodexResponses` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L63)
- uses (calls/refs, reference-scoped): [`SimpleStreamOptions`](../types.ts.md#SimpleStreamOptions), [`StreamFunction`](../types.ts.md#StreamFunction), [`OpenAICodexResponsesOptions`](openai-codex-responses.ts.md#OpenAICodexResponsesOptions)
- used by: [`loadOpenAICodexResponsesProviderModule`](register-builtins.ts.md#loadOpenAICodexResponsesProviderModule)

### `OpenAICompletionsProviderModule`
- def: [`packages/ai/src/providers/register-builtins.ts:66`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L66)
- signature: `interface OpenAICompletionsProviderModule`
- members:
  - `streamOpenAICompletions` — [`L67`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L67)
  - `streamSimpleOpenAICompletions` — [`L68`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L68)
- uses (calls/refs, reference-scoped): [`SimpleStreamOptions`](../types.ts.md#SimpleStreamOptions), [`StreamFunction`](../types.ts.md#StreamFunction), [`OpenAICompletionsOptions`](openai-completions.ts.md#OpenAICompletionsOptions)
- used by: [`loadOpenAICompletionsProviderModule`](register-builtins.ts.md#loadOpenAICompletionsProviderModule)

### `OpenAIResponsesProviderModule`
- def: [`packages/ai/src/providers/register-builtins.ts:71`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L71)
- signature: `interface OpenAIResponsesProviderModule`
- members:
  - `streamOpenAIResponses` — [`L72`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L72)
  - `streamSimpleOpenAIResponses` — [`L73`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L73)
- uses (calls/refs, reference-scoped): [`SimpleStreamOptions`](../types.ts.md#SimpleStreamOptions), [`StreamFunction`](../types.ts.md#StreamFunction), [`OpenAIResponsesOptions`](openai-responses.ts.md#OpenAIResponsesOptions)
- used by: [`loadOpenAIResponsesProviderModule`](register-builtins.ts.md#loadOpenAIResponsesProviderModule)

## Functions
- `createLazyLoadErrorMessage(model: Model<TApi>, error: unknown)` — [`L138`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L138)
- `createLazySimpleStream(loadModule: () => Promise<LazyProviderModule<TApi, TOptions, TSimpleOptions>>)` — [`L180`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L180)
- `createLazyStream(loadModule: () => Promise<LazyProviderModule<TApi, TOptions, TSimpleOptions>>)` — [`L159`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L159)
- `forwardStream(target: AssistantMessageEventStream, source: AsyncIterable<AssistantMessageEvent>)` — [`L129`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L129)
- `loadAnthropicProviderModule()` — [`L203`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L203)
- `loadAzureOpenAIResponsesProviderModule()` — [`L216`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L216)
- `loadBedrockProviderModule()` — [`L307`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L307)
- `loadGoogleProviderModule()` — [`L229`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L229)
- `loadGoogleVertexProviderModule()` — [`L242`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L242)
- `loadMistralProviderModule()` — [`L255`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L255)
- `loadOpenAICodexResponsesProviderModule()` — [`L268`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L268)
- `loadOpenAICompletionsProviderModule()` — [`L281`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L281)
- `loadOpenAIResponsesProviderModule()` — [`L294`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L294)
- `registerBuiltInApiProviders()` — [`L342`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L342)
- `resetApiProviders()` — [`L398`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L398)
- `setBedrockProviderModule(module: BedrockProviderModule)` — [`L122`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L122)

## Module values
- `anthropicProviderModulePromise` — [`L91`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L91)
- `azureOpenAIResponsesProviderModulePromise` — [`L94`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L94)
- `bedrockProviderModuleOverride` — [`L115`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L115)
- `bedrockProviderModulePromise` — [`L118`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L118)
- `googleProviderModulePromise` — [`L97`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L97)
- `googleVertexProviderModulePromise` — [`L100`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L100)
- `importNodeOnlyProvider` — [`L89`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L89)
- `mistralProviderModulePromise` — [`L103`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L103)
- `openAICodexResponsesProviderModulePromise` — [`L106`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L106)
- `openAICompletionsProviderModulePromise` — [`L109`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L109)
- `openAIResponsesProviderModulePromise` — [`L112`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L112)
- `streamAnthropic` — [`L323`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L323)
- `streamAzureOpenAIResponses` — [`L325`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L325)
- `streamBedrockLazy` — [`L339`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L339)
- `streamGoogle` — [`L327`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L327)
- `streamGoogleVertex` — [`L329`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L329)
- `streamMistral` — [`L331`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L331)
- `streamOpenAICodexResponses` — [`L333`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L333)
- `streamOpenAICompletions` — [`L335`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L335)
- `streamOpenAIResponses` — [`L337`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L337)
- `streamSimpleAnthropic` — [`L324`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L324)
- `streamSimpleAzureOpenAIResponses` — [`L326`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L326)
- `streamSimpleBedrockLazy` — [`L340`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L340)
- `streamSimpleGoogle` — [`L328`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L328)
- `streamSimpleGoogleVertex` — [`L330`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L330)
- `streamSimpleMistral` — [`L332`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L332)
- `streamSimpleOpenAICodexResponses` — [`L334`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L334)
- `streamSimpleOpenAICompletions` — [`L336`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L336)
- `streamSimpleOpenAIResponses` — [`L338`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/register-builtins.ts#L338)


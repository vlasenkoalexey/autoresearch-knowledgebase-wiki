---
title: 'Module: packages/ai/src/providers/faux.ts'
type: catalog
provenance: extracted
module: packages/ai/src/providers/faux.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/providers/`faux.ts`/
symbols:
  fauxAssistantMessage: fauxAssistantMessage().
  registerFauxProvider: registerFauxProvider().
  FauxModelDefinition.id: FauxModelDefinition#id.
  fauxToolCall: fauxToolCall().
  FauxProviderRegistration.getModel: FauxProviderRegistration#getModel().
  FauxModelDefinition.reasoning: FauxModelDefinition#reasoning.
  FauxModelDefinition.name: FauxModelDefinition#name.
  withUsageEstimate: withUsageEstimate().
  fauxAssistantMessage.options-typeLiteral2.timestamp: fauxAssistantMessage().(options)typeLiteral2:timestamp.
  streamWithDeltas: streamWithDeltas().
  FauxProviderRegistration.setResponses: FauxProviderRegistration#setResponses.
  DEFAULT_USAGE: DEFAULT_USAGE.
  createErrorMessage: createErrorMessage().
  assistantContentToText: assistantContentToText().
  messageToText: messageToText().
  FauxProviderRegistration.state: FauxProviderRegistration#state.
  FauxProviderRegistration.state.typeLiteral11.callCount: FauxProviderRegistration#state.typeLiteral11:callCount.
  serializeContext: serializeContext().
  FauxProviderRegistration.models: FauxProviderRegistration#models.
  contentToText: contentToText().
  cloneMessage: cloneMessage().
  FauxProviderRegistration.api: FauxProviderRegistration#api.
  fauxThinking: fauxThinking().
  fauxText: fauxText().
  createAbortedMessage: createAbortedMessage().
  FauxContentBlock: FauxContentBlock#
  FauxProviderRegistration.unregister: FauxProviderRegistration#unregister.
  FauxModelDefinition.contextWindow: FauxModelDefinition#contextWindow.
  FauxResponseFactory: FauxResponseFactory#
  FauxResponseStep: FauxResponseStep#
  toolResultToText: toolResultToText().
  FauxProviderRegistration: FauxProviderRegistration#
  FauxProviderRegistration.getPendingResponseCount: FauxProviderRegistration#getPendingResponseCount.
  normalizeFauxAssistantContent: normalizeFauxAssistantContent().
  fauxAssistantMessage.options-typeLiteral2.stopReason: fauxAssistantMessage().(options)typeLiteral2:stopReason.
  FauxProviderRegistration.appendResponses: FauxProviderRegistration#appendResponses.
  scheduleChunk: scheduleChunk().
  estimateTokens: estimateTokens().
  RegisterFauxProviderOptions.models: RegisterFauxProviderOptions#models.
  FauxModelDefinition: FauxModelDefinition#
  RegisterFauxProviderOptions.tokenSize: RegisterFauxProviderOptions#tokenSize.
  randomId: randomId().
  splitStringByTokenSize: splitStringByTokenSize().
  DEFAULT_API: DEFAULT_API.
  DEFAULT_PROVIDER: DEFAULT_PROVIDER.
  DEFAULT_MODEL_ID: DEFAULT_MODEL_ID.
  DEFAULT_MAX_TOKEN_SIZE: DEFAULT_MAX_TOKEN_SIZE.
  RegisterFauxProviderOptions.tokenSize.typeLiteral10.max: RegisterFauxProviderOptions#tokenSize.typeLiteral10:max.
  DEFAULT_MODEL_NAME: DEFAULT_MODEL_NAME.
  DEFAULT_BASE_URL: DEFAULT_BASE_URL.
  DEFAULT_MIN_TOKEN_SIZE: DEFAULT_MIN_TOKEN_SIZE.
  FauxModelDefinition.input: FauxModelDefinition#input.
  FauxModelDefinition.cost: FauxModelDefinition#cost.
  FauxModelDefinition.cost.typeLiteral0.input: FauxModelDefinition#cost.typeLiteral0:input.
  FauxModelDefinition.cost.typeLiteral0.output: FauxModelDefinition#cost.typeLiteral0:output.
  FauxModelDefinition.cost.typeLiteral0.cacheRead: FauxModelDefinition#cost.typeLiteral0:cacheRead.
  FauxModelDefinition.cost.typeLiteral0.cacheWrite: FauxModelDefinition#cost.typeLiteral0:cacheWrite.
  FauxModelDefinition.maxTokens: FauxModelDefinition#maxTokens.
  fauxToolCall.options-typeLiteral1.id: fauxToolCall().(options)typeLiteral1:id.
  fauxAssistantMessage.options-typeLiteral2.errorMessage: fauxAssistantMessage().(options)typeLiteral2:errorMessage.
  fauxAssistantMessage.options-typeLiteral2.responseId: fauxAssistantMessage().(options)typeLiteral2:responseId.
  RegisterFauxProviderOptions: RegisterFauxProviderOptions#
  RegisterFauxProviderOptions.api: RegisterFauxProviderOptions#api.
  RegisterFauxProviderOptions.provider: RegisterFauxProviderOptions#provider.
  RegisterFauxProviderOptions.tokensPerSecond: RegisterFauxProviderOptions#tokensPerSecond.
  RegisterFauxProviderOptions.tokenSize.typeLiteral10.min: RegisterFauxProviderOptions#tokenSize.typeLiteral10:min.
  commonPrefixLength: commonPrefixLength().
---
# Module: [`packages/ai/src/providers/faux.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts)

## Classes
### `FauxContentBlock`
- def: [`packages/ai/src/providers/faux.ts:47`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L47)
- signature: `type FauxContentBlock`
- uses (calls/refs, reference-scoped): [`TextContent`](../types.ts.md#TextContent), [`ToolCall`](../types.ts.md#ToolCall), [`ThinkingContent`](../types.ts.md#ThinkingContent)
- used by: [`fauxAssistantMessage`](faux.ts.md#fauxAssistantMessage), [`normalizeFauxAssistantContent`](faux.ts.md#normalizeFauxAssistantContent)

### `FauxModelDefinition`
- def: [`packages/ai/src/providers/faux.ts:37`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L37)
- signature: `interface FauxModelDefinition`
- members:
  - `cacheRead` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L42)
  - `cacheWrite` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L42)
  - `contextWindow` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L43)
  - `cost` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L42)
  - `id` — [`L38`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L38)
  - `input` — [`L41`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L41)
  - `input` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L42)
  - `maxTokens` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L44)
  - `name` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L39)
  - `output` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L42)
  - `reasoning` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L40)
- used by: [`registerFauxProvider`](faux.ts.md#registerFauxProvider), [`models`](faux.ts.md#RegisterFauxProviderOptions.models)  (23 test-only)

### `FauxProviderRegistration`
- def: [`packages/ai/src/providers/faux.ts:116`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L116)
- signature: `interface FauxProviderRegistration`
- members:
  - `getModel(method)` — [`L119`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L119)
  - `api` — [`L117`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L117)
  - `appendResponses` — [`L123`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L123)
  - `callCount` — [`L121`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L121)
  - `getPendingResponseCount` — [`L124`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L124)
  - `models` — [`L118`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L118)
  - `setResponses` — [`L122`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L122)
  - `state` — [`L121`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L121)
  - `unregister` — [`L125`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L125)
- uses (calls/refs, reference-scoped): [`Model`](../types.ts.md#Model), [`FauxResponseStep`](faux.ts.md#FauxResponseStep)
- used by: [`registerFauxProvider`](faux.ts.md#registerFauxProvider)  (21 test-only)

### `FauxResponseFactory`
- def: [`packages/ai/src/providers/faux.ts:96`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L96)
- signature: `type FauxResponseFactory`
- uses (calls/refs, reference-scoped): [`Model`](../types.ts.md#Model), [`AssistantMessage`](../types.ts.md#AssistantMessage), [`Context`](../types.ts.md#Context), [`StreamOptions`](../types.ts.md#StreamOptions)
- used by: [`FauxResponseStep`](faux.ts.md#FauxResponseStep)

### `FauxResponseStep`
- def: [`packages/ai/src/providers/faux.ts:103`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L103)
- signature: `type FauxResponseStep`
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../types.ts.md#AssistantMessage), [`FauxResponseFactory`](faux.ts.md#FauxResponseFactory)
- used by: [`registerFauxProvider`](faux.ts.md#registerFauxProvider), [`setResponses`](faux.ts.md#FauxProviderRegistration.setResponses), [`appendResponses`](faux.ts.md#FauxProviderRegistration.appendResponses)  (3 test-only)

### `RegisterFauxProviderOptions`
- def: [`packages/ai/src/providers/faux.ts:105`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L105)
- signature: `interface RegisterFauxProviderOptions`
- members:
  - `api` — [`L106`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L106)
  - `max` — [`L112`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L112)
  - `min` — [`L111`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L111)
  - `models` — [`L108`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L108)
  - `provider` — [`L107`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L107)
  - `tokenSize` — [`L110`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L110)
  - `tokensPerSecond` — [`L109`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L109)
- uses (calls/refs, reference-scoped): [`FauxModelDefinition`](faux.ts.md#FauxModelDefinition)
- used by: [`registerFauxProvider`](faux.ts.md#registerFauxProvider)

## Functions
- `assistantContentToText(content: (TextContent | ThinkingContent | ToolCall)[])` — [`L150`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L150)
- `cloneMessage(message: AssistantMessage, api: string, provider: string, modelId: string)` — [`L253`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L253)
- `commonPrefixLength(a: string, b: string)` — [`L192`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L192)
- `contentToText(content: string | (TextContent | ImageContent)[])` — [`L136`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L136)
- `createAbortedMessage(partial: AssistantMessage)` — [`L279`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L279)
- `createErrorMessage(error: unknown, api: string, provider: string, modelId: string)` — [`L265`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L265)
- `estimateTokens(text: string)` — [`L128`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L128)
- `fauxAssistantMessage(content: string | FauxContentBlock | FauxContentBlock[], options?: { stopReason?: StopReason | undefined; errorMessage?: string | undefined; responseId?: string | undefined; timestamp?: number | undefined; })` — [`L73`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L73)
- `fauxText(text: string)` — [`L49`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L49)
- `fauxThinking(thinking: string)` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L53)
- `fauxToolCall(name: string, arguments_: Record<string, any>, options?: { id?: string | undefined; })` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L57)
- `messageToText(message: Message)` — [`L168`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L168)
- `normalizeFauxAssistantContent(content: string | FauxContentBlock | FauxContentBlock[])` — [`L66`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L66)
- `randomId(prefix: string)` — [`L132`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L132)
- `registerFauxProvider(options?: RegisterFauxProviderOptions)` — [`L391`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L391)
- `scheduleChunk(chunk: string, tokensPerSecond: number | undefined)` — [`L288`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L288)
- `serializeContext(context: Context)` — [`L178`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L178)
- `splitStringByTokenSize(text: string, minTokenSize: number, maxTokenSize: number)` — [`L241`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L241)
- `streamWithDeltas(stream: AssistantMessageEventStream, message: AssistantMessage, minTokenSize: number, maxTokenSize: number, tokensPerSecond: number | undefined, signal: AbortSignal | undefined)` — [`L296`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L296)
- `toolResultToText(message: ToolResultMessage<any>)` — [`L164`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L164)
- `withUsageEstimate(message: AssistantMessage, context: Context, options: StreamOptions | undefined, promptCache: Map<string, string>)` — [`L201`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L201)

## Module values
- `DEFAULT_API` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L20)
- `DEFAULT_BASE_URL` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L24)
- `DEFAULT_MAX_TOKEN_SIZE` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L26)
- `DEFAULT_MIN_TOKEN_SIZE` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L25)
- `DEFAULT_MODEL_ID` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L22)
- `DEFAULT_MODEL_NAME` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L23)
- `DEFAULT_PROVIDER` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L21)
- `DEFAULT_USAGE` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L28)
- `errorMessage` — [`L77`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L77)
- `id` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L57)
- `responseId` — [`L78`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L78)
- `stopReason` — [`L76`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L76)
- `timestamp` — [`L79`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/faux.ts#L79)


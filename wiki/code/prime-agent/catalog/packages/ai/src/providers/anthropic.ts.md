---
title: 'Module: packages/ai/src/providers/anthropic.ts'
type: catalog
provenance: extracted
module: packages/ai/src/providers/anthropic.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/providers/`anthropic.ts`/
symbols:
  streamAnthropic: streamAnthropic.
  convertMessages: convertMessages().
  buildParams: buildParams().
  streamSimpleAnthropic: streamSimpleAnthropic.
  createClient.typeLiteral202.isOAuthToken: createClient().typeLiteral202:isOAuthToken.
  iterateAnthropicEvents: iterateAnthropicEvents().
  convertContentBlocks: convertContentBlocks().
  flushSseEvent: flushSseEvent().
  iterateSseMessages: iterateSseMessages().
  decodeSseLine: decodeSseLine().
  anthropicSseError: anthropicSseError().
  mapThinkingLevelToEffort: mapThinkingLevelToEffort().
  getAnthropicCompat: getAnthropicCompat().
  getCacheControl.typeLiteral0.cacheControl: getCacheControl().typeLiteral0:cacheControl.
  AnthropicOptions: AnthropicOptions#
  shouldUseFineGrainedToolStreamingBeta: shouldUseFineGrainedToolStreamingBeta().
  convertTools: convertTools().
  AnthropicOptions.effort: AnthropicOptions#effort.
  consumeLine: consumeLine().
  getCacheControl: getCacheControl().
  fromClaudeCodeName: fromClaudeCodeName.
  AnthropicOptions.thinkingEnabled: AnthropicOptions#thinkingEnabled.
  ServerSentEvent.data: ServerSentEvent#data.
  SseDecoderState.event: SseDecoderState#event.
  SseDecoderState.data: SseDecoderState#data.
  createClient.typeLiteral202.client: createClient().typeLiteral202:client.
  getCacheControl.typeLiteral0.retention: getCacheControl().typeLiteral0:retention.
  toClaudeCodeName: toClaudeCodeName.
  AnthropicEffort: AnthropicEffort#
  AnthropicOptions.toolChoice: AnthropicOptions#toolChoice.
  mergeHeaders: mergeHeaders().
  ServerSentEvent: ServerSentEvent#
  ServerSentEvent.event: ServerSentEvent#event.
  SseDecoderState.raw: SseDecoderState#raw.
  resolveCacheRetention: resolveCacheRetention().
  ccToolLookup: ccToolLookup.
  AnthropicOptions.thinkingDisplay: AnthropicOptions#thinkingDisplay.
  createClient: createClient().
  mapStopReason: mapStopReason().
  AnthropicThinkingDisplay: AnthropicThinkingDisplay#
  SseDecoderState: SseDecoderState#
  supportsAdaptiveThinking: supportsAdaptiveThinking().
  AnthropicOptions.thinkingBudgetTokens: AnthropicOptions#thinkingBudgetTokens.
  AnthropicOptions.client: AnthropicOptions#client.
  ServerSentEvent.raw: ServerSentEvent#raw.
  isAlwaysOnAdaptiveThinkingModel: isAlwaysOnAdaptiveThinkingModel().
  claudeCodeVersion: claudeCodeVersion.
  claudeCodeTools: claudeCodeTools.
  FINE_GRAINED_TOOL_STREAMING_BETA: FINE_GRAINED_TOOL_STREAMING_BETA.
  INTERLEAVED_THINKING_BETA: INTERLEAVED_THINKING_BETA.
  AnthropicOptions.interleavedThinking: AnthropicOptions#interleavedThinking.
  ANTHROPIC_MESSAGE_EVENTS: ANTHROPIC_MESSAGE_EVENTS.
  nextLineBreakIndex: nextLineBreakIndex().
  isOAuthToken: isOAuthToken().
  normalizeToolCallId: normalizeToolCallId().
---
# Module: [`packages/ai/src/providers/anthropic.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts)

## Classes
### `AnthropicEffort`
- def: [`packages/ai/src/providers/anthropic.ts:170`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L170)
- signature: `type AnthropicEffort`
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`mapThinkingLevelToEffort`](anthropic.ts.md#mapThinkingLevelToEffort), [`effort`](anthropic.ts.md#AnthropicOptions.effort)

### `AnthropicOptions`
- def: [`packages/ai/src/providers/anthropic.ts:184`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L184)
- signature: `interface AnthropicOptions`
- members:
  - `client` — [`L226`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L226) — Pre-built Anthropic client instance. When provided, skips internal client
  - `effort` — [`L206`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L206) — Effort level for adaptive thinking (Opus 4.6+, Sonnet 4.6, Fable/Mythos).
  - `interleavedThinking` — [`L219`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L219)
  - `thinkingBudgetTokens` — [`L195`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L195) — Token budget for extended thinking (older models only).
  - `thinkingDisplay` — [`L218`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L218) — Controls how thinking content is returned in API responses.
  - `thinkingEnabled` — [`L190`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L190) — Enable extended thinking.
  - `toolChoice` — [`L220`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L220)
- uses (calls/refs, reference-scoped): [`StreamOptions`](../types.ts.md#StreamOptions), [`AnthropicEffort`](anthropic.ts.md#AnthropicEffort), [`AnthropicThinkingDisplay`](anthropic.ts.md#AnthropicThinkingDisplay)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`streamAnthropic`](anthropic.ts.md#streamAnthropic), [`anthropic.ts`](anthropic.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-anthropic.ts), [`register-builtins.ts`](register-builtins.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-register-builtins.ts), [`buildParams`](anthropic.ts.md#buildParams), [`streamSimpleAnthropic`](anthropic.ts.md#streamSimpleAnthropic), [`loadAnthropicProviderModule`](register-builtins.ts.md#loadAnthropicProviderModule), [`anthropicProviderModulePromise`](register-builtins.ts.md#anthropicProviderModulePromise), [`streamAnthropic`](register-builtins.ts.md#AnthropicProviderModule.streamAnthropic)

### `AnthropicThinkingDisplay`
- def: [`packages/ai/src/providers/anthropic.ts:172`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L172)
- signature: `type AnthropicThinkingDisplay`
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`buildParams`](anthropic.ts.md#buildParams), [`thinkingDisplay`](anthropic.ts.md#AnthropicOptions.thinkingDisplay)

### `ServerSentEvent`
- def: [`packages/ai/src/providers/anthropic.ts:239`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L239)
- signature: `interface ServerSentEvent`
- members:
  - `data` — [`L241`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L241)
  - `event` — [`L240`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L240)
  - `raw` — [`L242`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L242)
- used by: [`iterateAnthropicEvents`](anthropic.ts.md#iterateAnthropicEvents), [`flushSseEvent`](anthropic.ts.md#flushSseEvent), [`iterateSseMessages`](anthropic.ts.md#iterateSseMessages), [`decodeSseLine`](anthropic.ts.md#decodeSseLine)

### `SseDecoderState`
- def: [`packages/ai/src/providers/anthropic.ts:245`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L245)
- signature: `interface SseDecoderState`
- members:
  - `data` — [`L247`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L247)
  - `event` — [`L246`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L246)
  - `raw` — [`L248`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L248)
- used by: [`flushSseEvent`](anthropic.ts.md#flushSseEvent), [`iterateSseMessages`](anthropic.ts.md#iterateSseMessages), [`decodeSseLine`](anthropic.ts.md#decodeSseLine)

## Functions
- `anthropicSseError(data: string, requestId?: string | undefined)` — [`L391`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L391) — Turn an in-stream `error` SSE event (how Anthropic delivers overloads etc.) into a classified failure.
- `buildParams(model: Model<"anthropic-messages">, context: Context, isOAuthToken: boolean, options?: AnthropicOptions | undefined, cacheControl?: CacheControlEphemeral | undefined)` — [`L955`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L955)
- `consumeLine(text: string)` — [`L314`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L314)
- `convertContentBlocks(content: (TextContent | ImageContent)[])` — [`L121`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L121) — Convert content blocks to Anthropic API format
- `convertMessages(messages: Message[], model: Model<"anthropic-messages">, isOAuthToken: boolean, cacheControl?: CacheControlEphemeral | undefined)` — [`L1066`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L1066)
- `convertTools(tools: Tool<TSchema>[], isOAuthToken: boolean, supportsEagerToolInputStreaming: boolean, cacheControl?: CacheControlEphemeral | undefined)` — [`L1234`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L1234)
- `createClient(model: Model<"anthropic-messages">, apiKey: string, interleavedThinking: boolean, useFineGrainedToolStreamingBeta: boolean, optionsHeaders?: Record<string, string> | undefined, dynamicHeaders?: Record<...> | undefined)` — [`L849`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L849)
- `decodeSseLine(line: string, state: SseDecoderState)` — [`L276`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L276)
- `flushSseEvent(state: SseDecoderState)` — [`L260`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L260)
- `getAnthropicCompat(model: Model<"anthropic-messages">)` — [`L177`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L177)
- `getCacheControl(model: Model<"anthropic-messages">, cacheRetention?: CacheRetention | undefined)` — [`L64`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L64)
- `isAlwaysOnAdaptiveThinkingModel(modelId: string)` — [`L745`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L745) — Fable/Mythos models think every turn and reject an explicit
- `isOAuthToken(apiKey: string)` — [`L845`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L845)
- `iterateAnthropicEvents(response: Response, signal?: AbortSignal | undefined, requestId?: string | undefined)` — [`L412`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L412)
- `iterateSseMessages(body: ReadableStream<Uint8Array<ArrayBufferLike>>, signal?: AbortSignal | undefined)` — [`L331`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L331)
- `mapStopReason(reason: string)` — [`L1259`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L1259)
- `mapThinkingLevelToEffort(model: Model<"anthropic-messages">, level: ThinkingLevel | undefined)` — [`L776`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L776) — Map ThinkingLevel to Anthropic effort levels for adaptive thinking. The effort is
- `mergeHeaders(...headerSources: (Record<string, string | null> | undefined)[])` — [`L229`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L229)
- `nextLineBreakIndex(text: string)` — [`L302`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L302)
- `normalizeToolCallId(id: string)` — [`L1062`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L1062)
- `resolveCacheRetention(cacheRetention?: CacheRetention | undefined)` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L54) — Resolve cache retention preference.
- `shouldUseFineGrainedToolStreamingBeta(model: Model<"anthropic-messages">, context: Context)` — [`L1230`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L1230)
- `supportsAdaptiveThinking(modelId: string)` — [`L752`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L752) — Check if a model supports adaptive thinking (Opus 4.6+, Sonnet 4.6)

## Module values
- `ANTHROPIC_MESSAGE_EVENTS` — [`L251`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L251)
- `FINE_GRAINED_TOOL_STREAMING_BETA` — [`L174`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L174)
- `INTERLEAVED_THINKING_BETA` — [`L175`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L175)
- `cacheControl` — [`L67`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L67)
- `ccToolLookup` — [`L105`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L105)
- `claudeCodeTools` — [`L85`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L85)
- `claudeCodeVersion` — [`L80`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L80)
- `client` — [`L856`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L856)
- `fromClaudeCodeName` — [`L109`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L109)
- `isOAuthToken` — [`L856`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L856)
- `retention` — [`L67`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L67)
- `streamAnthropic` — [`L458`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L458)
- `streamSimpleAnthropic` — [`L804`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L804)
- `toClaudeCodeName` — [`L108`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/anthropic.ts#L108)


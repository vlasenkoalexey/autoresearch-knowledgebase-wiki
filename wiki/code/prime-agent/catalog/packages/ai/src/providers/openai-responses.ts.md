---
title: 'Module: packages/ai/src/providers/openai-responses.ts'
type: catalog
provenance: extracted
module: packages/ai/src/providers/openai-responses.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/providers/`openai-responses.ts`/
symbols:
  streamOpenAIResponses: streamOpenAIResponses.
  buildParams: buildParams().
  createClient: createClient().
  streamSimpleOpenAIResponses: streamSimpleOpenAIResponses.
  applyServiceTierPricing: applyServiceTierPricing().
  getCompat: getCompat().
  OpenAIResponsesOptions: OpenAIResponsesOptions#
  getPromptCacheRetention: getPromptCacheRetention().
  getServiceTierCostMultiplier: getServiceTierCostMultiplier().
  OpenAIResponsesOptions.reasoningEffort: OpenAIResponsesOptions#reasoningEffort.
  resolveCacheRetention: resolveCacheRetention().
  OpenAIResponsesOptions.serviceTier: OpenAIResponsesOptions#serviceTier.
  OpenAIResponsesOptions.reasoningSummary: OpenAIResponsesOptions#reasoningSummary.
  OPENAI_TOOL_CALL_PROVIDERS: OPENAI_TOOL_CALL_PROVIDERS.
---
# Module: [`packages/ai/src/providers/openai-responses.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses.ts)

## Classes
### `OpenAIResponsesOptions`
- def: [`packages/ai/src/providers/openai-responses.ts:60`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses.ts#L60)
- signature: `interface OpenAIResponsesOptions`
- members:
  - `reasoningEffort` — [`L61`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses.ts#L61)
  - `reasoningSummary` — [`L62`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses.ts#L62)
  - `serviceTier` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses.ts#L63)
- uses (calls/refs, reference-scoped): [`StreamOptions`](../types.ts.md#StreamOptions)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`streamOpenAIResponses`](openai-responses.ts.md#streamOpenAIResponses), [`openai-responses.ts`](openai-responses.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-openai-responses.ts), [`register-builtins.ts`](register-builtins.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-register-builtins.ts), [`buildParams`](openai-responses.ts.md#buildParams), [`streamSimpleOpenAIResponses`](openai-responses.ts.md#streamSimpleOpenAIResponses), [`loadOpenAIResponsesProviderModule`](register-builtins.ts.md#loadOpenAIResponsesProviderModule), [`openAIResponsesProviderModulePromise`](register-builtins.ts.md#openAIResponsesProviderModulePromise), [`streamOpenAIResponses`](register-builtins.ts.md#OpenAIResponsesProviderModule.streamOpenAIResponses)

## Functions
- `applyServiceTierPricing(usage: Usage, serviceTier: "auto" | "default" | "flex" | "scale" | "priority" | null | undefined, model: Pick<Model<"openai-responses">, "id">)` — [`L289`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses.ts#L289)
- `buildParams(model: Model<"openai-responses">, context: Context, options?: OpenAIResponsesOptions | undefined)` — [`L225`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses.ts#L225)
- `createClient(model: Model<"openai-responses">, context: Context, apiKey?: string | undefined, optionsHeaders?: Record<string, string> | undefined, sessionId?: string | undefined)` — [`L169`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses.ts#L169)
- `getCompat(model: Model<"openai-responses">)` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses.ts#L45)
- `getPromptCacheRetention(compat: Required<OpenAIResponsesCompat>, cacheRetention: CacheRetention)` — [`L52`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses.ts#L52)
- `getServiceTierCostMultiplier(model: Pick<Model<"openai-responses">, "id">, serviceTier: "auto" | "default" | "flex" | "scale" | "priority" | null | undefined)` — [`L275`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses.ts#L275)
- `resolveCacheRetention(cacheRetention?: CacheRetention | undefined)` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses.ts#L35) — Resolve cache retention preference.

## Module values
- `OPENAI_TOOL_CALL_PROVIDERS` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses.ts#L29)
- `streamOpenAIResponses` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses.ts#L69) — Generate function for OpenAI Responses API
- `streamSimpleOpenAIResponses` — [`L149`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/openai-responses.ts#L149)


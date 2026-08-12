---
title: 'Module: packages/ai/test/cross-provider-handoff.test.ts'
type: catalog
provenance: extracted
module: packages/ai/test/cross-provider-handoff.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 test/`cross-provider-handoff.test.ts`/
symbols:
  generateContext: generateContext().
  ProviderModelPair.label: ProviderModelPair#label.
  ProviderModelPair.provider: ProviderModelPair#provider.
  ProviderModelPair.model: ProviderModelPair#model.
  PROVIDER_MODEL_PAIRS: PROVIDER_MODEL_PAIRS.
  hasApiKey: hasApiKey().
  dumpFailurePayload: dumpFailurePayload().
  testTool: testTool.
  hasAnyApiKey: hasAnyApiKey().
  dumpFailurePayload.params-typeLiteral16.label: dumpFailurePayload().(params)typeLiteral16:label.
  ProviderModelPair.apiOverride: ProviderModelPair#apiOverride.
  getApiKey: getApiKey().
  getHeaders: getHeaders().
  dumpFailurePayload.params-typeLiteral16.error: dumpFailurePayload().(params)typeLiteral16:error.
  dumpFailurePayload.params-typeLiteral16.payload: dumpFailurePayload().(params)typeLiteral16:payload.
  dumpFailurePayload.params-typeLiteral16.messages: dumpFailurePayload().(params)typeLiteral16:messages.
  ProviderModelPair.upstreamApiKeyEnv: ProviderModelPair#upstreamApiKeyEnv.
  ProviderModelPair: ProviderModelPair#
  CachedContext.messages: CachedContext#messages.
  CachedContext.api: CachedContext#api.
  testToolSchema: testToolSchema.
  CachedContext: CachedContext#
  CachedContext.label: CachedContext#label.
  CachedContext.provider: CachedContext#provider.
  CachedContext.model: CachedContext#model.
  CachedContext.generatedAt: CachedContext#generatedAt.
---
# Module: [`packages/ai/test/cross-provider-handoff.test.ts`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts)

## Classes
### `CachedContext`
- def: [`packages/ai/test/cross-provider-handoff.test.ts:138`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L138)
- signature: `interface CachedContext`
- members:
  - `api` — [`L142`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L142)
  - `generatedAt` — [`L144`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L144)
  - `label` — [`L139`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L139)
  - `messages` — [`L143`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L143)
  - `model` — [`L141`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L141)
  - `provider` — [`L140`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L140)
- uses (calls/refs, reference-scoped): [`Api`](../src/types.ts.md#Api), [`Message`](../src/types.ts.md#Message)
- used by: (1 test-only callers)

### `ProviderModelPair`
- def: [`packages/ai/test/cross-provider-handoff.test.ts:48`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L48)
- signature: `interface ProviderModelPair`
- members:
  - `apiOverride` — [`L52`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L52)
  - `label` — [`L51`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L51)
  - `model` — [`L50`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L50)
  - `provider` — [`L49`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L49)
  - `upstreamApiKeyEnv` — [`L53`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L53)
- uses (calls/refs, reference-scoped): [`Api`](../src/types.ts.md#Api)
- used by: (5 test-only callers)

## Functions
- `dumpFailurePayload(params: { label: string; error: string; payload?: unknown; messages: Message[]; })` — [`L186`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L186)
- `generateContext(pair: ProviderModelPair, apiKey: string)` — [`L202`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L202) — Generate a context from a provider/model pair.
- `getApiKey(provider: string)` — [`L150`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L150) — Get API key for provider - checks OAuth storage first, then env vars
- `getHeaders(pair: ProviderModelPair)` — [`L173`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L173)
- `hasAnyApiKey()` — [`L182`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L182) — Check if any provider has API keys available (for skipIf at describe level)
- `hasApiKey(pair: ProviderModelPair)` — [`L159`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L159) — Synchronous check for API key availability (env vars only, for skipIf)

## Module values
- `PROVIDER_MODEL_PAIRS` — [`L56`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L56)
- `error` — [`L186`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L186)
- `label` — [`L186`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L186)
- `messages` — [`L186`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L186)
- `payload` — [`L186`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L186)
- `testTool` — [`L41`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L41)
- `testToolSchema` — [`L37`](../../../../../../../raw/code/prime-agent/packages/ai/test/cross-provider-handoff.test.ts#L37)


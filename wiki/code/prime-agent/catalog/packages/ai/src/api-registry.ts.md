---
title: 'Module: packages/ai/src/api-registry.ts'
type: catalog
provenance: extracted
module: packages/ai/src/api-registry.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/`api-registry.ts`/
symbols:
  registerApiProvider: registerApiProvider().
  getApiProvider: getApiProvider().
  ApiProvider.streamSimple: ApiProvider#streamSimple.
  ApiProvider.api: ApiProvider#api.
  wrapStream: wrapStream().
  wrapStreamSimple: wrapStreamSimple().
  ApiProvider.stream: ApiProvider#stream.
  ApiStreamFunction: ApiStreamFunction#
  ApiStreamSimpleFunction: ApiStreamSimpleFunction#
  ApiProviderInternal.streamSimple: ApiProviderInternal#streamSimple.
  apiProviderRegistry: apiProviderRegistry.
  getApiProviders: getApiProviders().
  unregisterApiProviders: unregisterApiProviders().
  ApiProvider: ApiProvider#
  RegisteredApiProvider.typeLiteral8.provider: RegisteredApiProvider#typeLiteral8:provider.
  ApiProviderInternal.stream: ApiProviderInternal#stream.
  clearApiProviders: clearApiProviders().
  ApiProviderInternal.api: ApiProviderInternal#api.
  ApiProviderInternal: ApiProviderInternal#
  RegisteredApiProvider.typeLiteral8.sourceId: RegisteredApiProvider#typeLiteral8:sourceId.
  RegisteredApiProvider: RegisteredApiProvider#
---
# Module: [`packages/ai/src/api-registry.ts`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts)

## Classes
### `ApiProvider`
- def: [`packages/ai/src/api-registry.ts:23`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L23)
- signature: `interface ApiProvider`
- members:
  - `api` — [`L24`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L24)
  - `stream` — [`L25`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L25)
  - `streamSimple` — [`L26`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L26)
- uses (calls/refs, reference-scoped): [`Api`](types.ts.md#Api), [`SimpleStreamOptions`](types.ts.md#SimpleStreamOptions), [`StreamFunction`](types.ts.md#StreamFunction), [`StreamOptions`](types.ts.md#StreamOptions)
- used by: [`registerFauxProvider`](providers/faux.ts.md#registerFauxProvider), [`applyProviderConfig`](../../coding-agent/src/core/model-registry.ts.md#ModelRegistry.applyProviderConfig), [`registerBuiltInApiProviders`](providers/register-builtins.ts.md#registerBuiltInApiProviders), [`registerApiProvider`](api-registry.ts.md#registerApiProvider)  (1 test-only)

### `ApiProviderInternal`
- def: [`packages/ai/src/api-registry.ts:29`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L29)
- signature: `interface ApiProviderInternal`
- members:
  - `api` — [`L30`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L30)
  - `stream` — [`L31`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L31)
  - `streamSimple` — [`L32`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L32)
- uses (calls/refs, reference-scoped): [`Api`](types.ts.md#Api), [`ApiStreamFunction`](api-registry.ts.md#ApiStreamFunction), [`ApiStreamSimpleFunction`](api-registry.ts.md#ApiStreamSimpleFunction)
- used by: [`streamSimple`](stream.ts.md#streamSimple), [`stream`](stream.ts.md#stream), [`registerApiProvider`](api-registry.ts.md#registerApiProvider), [`getApiProvider`](api-registry.ts.md#getApiProvider), [`getApiProviders`](api-registry.ts.md#getApiProviders), [`provider`](api-registry.ts.md#RegisteredApiProvider.typeLiteral8.provider)  (4 test-only)

### `ApiStreamFunction`
- def: [`packages/ai/src/api-registry.ts:11`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L11)
- signature: `type ApiStreamFunction`
- uses (calls/refs, reference-scoped): [`Model`](types.ts.md#Model), [`Api`](types.ts.md#Api), [`Context`](types.ts.md#Context), [`AssistantMessageEventStream`](utils/event-stream.ts.md#AssistantMessageEventStream), [`StreamOptions`](types.ts.md#StreamOptions)
- used by: [`wrapStream`](api-registry.ts.md#wrapStream), [`stream`](api-registry.ts.md#ApiProviderInternal.stream)

### `ApiStreamSimpleFunction`
- def: [`packages/ai/src/api-registry.ts:17`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L17)
- signature: `type ApiStreamSimpleFunction`
- uses (calls/refs, reference-scoped): [`Model`](types.ts.md#Model), [`Api`](types.ts.md#Api), [`Context`](types.ts.md#Context), [`SimpleStreamOptions`](types.ts.md#SimpleStreamOptions), [`AssistantMessageEventStream`](utils/event-stream.ts.md#AssistantMessageEventStream)
- used by: [`wrapStreamSimple`](api-registry.ts.md#wrapStreamSimple), [`streamSimple`](api-registry.ts.md#ApiProviderInternal.streamSimple)

### `RegisteredApiProvider`
- def: [`packages/ai/src/api-registry.ts:35`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L35)
- signature: `type RegisteredApiProvider`
- members:
  - `provider` — [`L36`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L36)
  - `sourceId` — [`L37`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L37)
- uses (calls/refs, reference-scoped): [`ApiProviderInternal`](api-registry.ts.md#ApiProviderInternal)
- used by: [`registerApiProvider`](api-registry.ts.md#registerApiProvider), [`getApiProvider`](api-registry.ts.md#getApiProvider), [`apiProviderRegistry`](api-registry.ts.md#apiProviderRegistry), [`getApiProviders`](api-registry.ts.md#getApiProviders), [`unregisterApiProviders`](api-registry.ts.md#unregisterApiProviders)

## Functions
- `clearApiProviders()` — [`L96`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L96)
- `getApiProvider(api: Api)` — [`L80`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L80)
- `getApiProviders()` — [`L84`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L84)
- `registerApiProvider(provider: ApiProvider<TApi, TOptions>, sourceId?: string | undefined)` — [`L66`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L66)
- `unregisterApiProviders(sourceId: string)` — [`L88`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L88)
- `wrapStream(api: TApi, stream: StreamFunction<TApi, TOptions>)` — [`L42`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L42)
- `wrapStreamSimple(api: TApi, streamSimple: StreamFunction<TApi, SimpleStreamOptions>)` — [`L54`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L54)

## Module values
- `apiProviderRegistry` — [`L40`](../../../../../../../raw/code/prime-agent/packages/ai/src/api-registry.ts#L40)


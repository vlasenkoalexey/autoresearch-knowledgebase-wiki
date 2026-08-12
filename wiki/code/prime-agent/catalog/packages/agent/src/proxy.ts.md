---
title: 'Module: packages/agent/src/proxy.ts'
type: catalog
provenance: extracted
module: packages/agent/src/proxy.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-agent-core 0.7.2 src/`proxy.ts`/
symbols:
  streamProxy: streamProxy().
  processProxyEvent: processProxyEvent().
  buildProxyRequestOptions: buildProxyRequestOptions().
  ProxyAssistantMessageEvent: ProxyAssistantMessageEvent#
  ProxyMessageEventStream: ProxyMessageEventStream#
  ProxyStreamOptions.signal: ProxyStreamOptions#signal.
  ProxySerializableStreamOptions: ProxySerializableStreamOptions#
  ProxyStreamOptions: ProxyStreamOptions#
  ProxyMessageEventStream.-constructor: ProxyMessageEventStream#`<constructor>`().
  ProxyStreamOptions.authToken: ProxyStreamOptions#authToken.
  ProxyStreamOptions.proxyUrl: ProxyStreamOptions#proxyUrl.
---
# Module: [`packages/agent/src/proxy.ts`](../../../../../../../raw/code/prime-agent/packages/agent/src/proxy.ts)

## Classes
### `ProxyAssistantMessageEvent`
- def: [`packages/agent/src/proxy.ts:36`](../../../../../../../raw/code/prime-agent/packages/agent/src/proxy.ts#L36)
- doc: Proxy event types - server sends these with partial field stripped to reduce bandwidth.
- signature: `type ProxyAssistantMessageEvent`
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../ai/src/types.ts.md#AssistantMessage), [`usage`](../../ai/src/types.ts.md#AssistantMessage.usage), [`StopReason`](../../ai/src/types.ts.md#StopReason)
- used by: [`streamProxy`](proxy.ts.md#streamProxy), [`processProxyEvent`](proxy.ts.md#processProxyEvent)

### `ProxyMessageEventStream`  ·  implements/extends AsyncIterable, EventStream
- def: [`packages/agent/src/proxy.ts:20`](../../../../../../../raw/code/prime-agent/packages/agent/src/proxy.ts#L20)
- signature: `class ProxyMessageEventStream`
- members:
  - `<constructor>()` — [`L21`](../../../../../../../raw/code/prime-agent/packages/agent/src/proxy.ts#L21)
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../ai/src/types.ts.md#AssistantMessage), [`AssistantMessageEvent`](../../ai/src/types.ts.md#AssistantMessageEvent), [`EventStream`](../../ai/src/utils/event-stream.ts.md#EventStream)
- used by: [`streamProxy`](proxy.ts.md#streamProxy), [`EventStream`](../../ai/src/utils/event-stream.ts.md#EventStream)

### `ProxySerializableStreamOptions`
- def: [`packages/agent/src/proxy.ts:59`](../../../../../../../raw/code/prime-agent/packages/agent/src/proxy.ts#L59)
- signature: `type ProxySerializableStreamOptions`
- uses (calls/refs, reference-scoped): [`SimpleStreamOptions`](../../ai/src/types.ts.md#SimpleStreamOptions)
- used by: [`buildProxyRequestOptions`](proxy.ts.md#buildProxyRequestOptions), [`ProxyStreamOptions`](proxy.ts.md#ProxyStreamOptions)

### `ProxyStreamOptions`
- def: [`packages/agent/src/proxy.ts:73`](../../../../../../../raw/code/prime-agent/packages/agent/src/proxy.ts#L73)
- signature: `interface ProxyStreamOptions`
- members:
  - `authToken` — [`L77`](../../../../../../../raw/code/prime-agent/packages/agent/src/proxy.ts#L77) — Auth token for the proxy server
  - `proxyUrl` — [`L79`](../../../../../../../raw/code/prime-agent/packages/agent/src/proxy.ts#L79) — Proxy server URL (e.g., "https://genai.example.com")
  - `signal` — [`L75`](../../../../../../../raw/code/prime-agent/packages/agent/src/proxy.ts#L75) — Local abort signal for the proxy request
- uses (calls/refs, reference-scoped): [`ProxySerializableStreamOptions`](proxy.ts.md#ProxySerializableStreamOptions)
- used by: [`streamProxy`](proxy.ts.md#streamProxy), [`buildProxyRequestOptions`](proxy.ts.md#buildProxyRequestOptions)

## Functions
- `buildProxyRequestOptions(options: ProxyStreamOptions)` — [`L101`](../../../../../../../raw/code/prime-agent/packages/agent/src/proxy.ts#L101) — Stream function that proxies through a server instead of calling LLM providers directly.
- `processProxyEvent(proxyEvent: ProxyAssistantMessageEvent, partial: AssistantMessage)` — [`L238`](../../../../../../../raw/code/prime-agent/packages/agent/src/proxy.ts#L238) — Process a proxy event and update the partial message.
- `streamProxy(model: Model<any>, context: Context, options: ProxyStreamOptions)` — [`L116`](../../../../../../../raw/code/prime-agent/packages/agent/src/proxy.ts#L116)


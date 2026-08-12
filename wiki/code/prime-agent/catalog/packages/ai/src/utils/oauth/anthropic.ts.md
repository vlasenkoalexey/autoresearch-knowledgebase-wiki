---
title: 'Module: packages/ai/src/utils/oauth/anthropic.ts'
type: catalog
provenance: extracted
module: packages/ai/src/utils/oauth/anthropic.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/utils/oauth/`anthropic.ts`/
symbols:
  loginAnthropic: loginAnthropic().
  startCallbackServer: startCallbackServer().
  refreshAnthropicToken: refreshAnthropicToken().
  exchangeAuthorizationCode: exchangeAuthorizationCode().
  parseAuthorizationInput.typeLiteral15.state: parseAuthorizationInput().typeLiteral15:state.
  REDIRECT_URI: REDIRECT_URI.
  getNodeApis: getNodeApis().
  parseAuthorizationInput: parseAuthorizationInput().
  formatErrorDetails: formatErrorDetails().
  parseAuthorizationInput.typeLiteral15.code: parseAuthorizationInput().typeLiteral15:code.
  nodeApis: nodeApis.
  TOKEN_URL: TOKEN_URL.
  nodeApisPromise: nodeApisPromise.
  CLIENT_ID: CLIENT_ID.
  loginAnthropic.options-typeLiteral136.onPrompt: loginAnthropic().(options)typeLiteral136:onPrompt.
  loginAnthropic.options-typeLiteral136.onManualCodeInput: loginAnthropic().(options)typeLiteral136:onManualCodeInput.
  NodeApis: NodeApis#
  loginAnthropic.options-typeLiteral136.onAuth: loginAnthropic().(options)typeLiteral136:onAuth.
  anthropicOAuthProvider: anthropicOAuthProvider.
  CallbackServerInfo.typeLiteral0.cancelWait: CallbackServerInfo#typeLiteral0:cancelWait.
  CallbackServerInfo.typeLiteral0.waitForCode: CallbackServerInfo#typeLiteral0:waitForCode.
  CALLBACK_PORT: CALLBACK_PORT.
  CALLBACK_PATH: CALLBACK_PATH.
  postJson: postJson().
  loginAnthropic.options-typeLiteral136.onProgress: loginAnthropic().(options)typeLiteral136:onProgress.
  CallbackServerInfo: CallbackServerInfo#
  CallbackServerInfo.typeLiteral0.server: CallbackServerInfo#typeLiteral0:server.
  NodeApis.typeLiteral7.createServer: NodeApis#typeLiteral7:createServer.
  decode: decode.
  AUTHORIZE_URL: AUTHORIZE_URL.
  CALLBACK_HOST: CALLBACK_HOST.
  SCOPES: SCOPES.
  CallbackServerInfo.typeLiteral0.redirectUri: CallbackServerInfo#typeLiteral0:redirectUri.
---
# Module: [`packages/ai/src/utils/oauth/anthropic.ts`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts)

## Classes
### `CallbackServerInfo`
- def: [`packages/ai/src/utils/oauth/anthropic.ts:13`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L13)
- signature: `type CallbackServerInfo`
- members:
  - `cancelWait` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L16)
  - `redirectUri` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L15)
  - `server` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L14)
  - `waitForCode` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L17)
- used by: [`loginAnthropic`](anthropic.ts.md#loginAnthropic), [`startCallbackServer`](anthropic.ts.md#startCallbackServer)

### `NodeApis`
- def: [`packages/ai/src/utils/oauth/anthropic.ts:20`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L20)
- signature: `type NodeApis`
- members:
  - `createServer` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L21)
- used by: [`startCallbackServer`](anthropic.ts.md#startCallbackServer), [`getNodeApis`](anthropic.ts.md#getNodeApis), [`nodeApis`](anthropic.ts.md#nodeApis), [`nodeApisPromise`](anthropic.ts.md#nodeApisPromise)

## Functions
- `exchangeAuthorizationCode(code: string, state: string, verifier: string, redirectUri: string)` — [`L189`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L189)
- `formatErrorDetails(error: unknown)` — [`L81`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L81)
- `getNodeApis()` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L37)
- `loginAnthropic(options: { onAuth: (info: { url: string; instructions?: string | undefined; }) => void; onPrompt: (prompt: OAuthPrompt) => Promise<string>; onProgress?: ((message: string) => void) | undefined; onManualCodeInput?: (() => Promise<...>) | undefined; })` — [`L230`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L230) — Login with Anthropic OAuth (authorization code + PKCE)
- `parseAuthorizationInput(input: string)` — [`L51`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L51)
- `postJson(url: string, body: Record<string, string | number>)` — [`L169`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L169)
- `refreshAnthropicToken(refreshToken: string)` — [`L348`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L348) — Refresh Anthropic OAuth token
- `startCallbackServer(expectedState: string)` — [`L98`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L98)

## Module values
- `AUTHORIZE_URL` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L29)
- `CALLBACK_HOST` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L31)
- `CALLBACK_PATH` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L33)
- `CALLBACK_PORT` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L32)
- `CLIENT_ID` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L28)
- `REDIRECT_URI` — [`L34`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L34)
- `SCOPES` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L35)
- `TOKEN_URL` — [`L30`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L30)
- `anthropicOAuthProvider` — [`L381`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L381)
- `code` — [`L51`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L51)
- `decode` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L27)
- `nodeApis` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L24)
- `nodeApisPromise` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L25)
- `onAuth` — [`L231`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L231)
- `onManualCodeInput` — [`L234`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L234)
- `onProgress` — [`L233`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L233)
- `onPrompt` — [`L232`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L232)
- `state` — [`L51`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/anthropic.ts#L51)


---
title: 'Module: packages/ai/src/utils/oauth/openai-codex.ts'
type: catalog
provenance: extracted
module: packages/ai/src/utils/oauth/openai-codex.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/utils/oauth/`openai-codex.ts`/
symbols:
  loginOpenAICodex: loginOpenAICodex().
  _http: _http.
  refreshOpenAICodexToken: refreshOpenAICodexToken().
  createAuthorizationFlow.Promise.typeLiteral70.url: createAuthorizationFlow().Promise:typeLiteral70:url.
  startLocalOAuthServer: startLocalOAuthServer().
  exchangeAuthorizationCode: exchangeAuthorizationCode().
  getAccountId: getAccountId().
  parseAuthorizationInput.typeLiteral14.state: parseAuthorizationInput().typeLiteral14:state.
  refreshAccessToken: refreshAccessToken().
  parseAuthorizationInput: parseAuthorizationInput().
  TokenResult: TokenResult#
  parseAuthorizationInput.typeLiteral14.code: parseAuthorizationInput().typeLiteral14:code.
  JwtPayload: JwtPayload#
  loginOpenAICodex.options-typeLiteral145.onPrompt: loginOpenAICodex().(options)typeLiteral145:onPrompt.
  TokenSuccess.typeLiteral8.access: TokenSuccess#typeLiteral8:access.
  createState: createState().
  decodeJwt: decodeJwt().
  _randomBytes: _randomBytes.
  CLIENT_ID: CLIENT_ID.
  loginOpenAICodex.options-typeLiteral145.onManualCodeInput: loginOpenAICodex().(options)typeLiteral145:onManualCodeInput.
  openaiCodexOAuthProvider: openaiCodexOAuthProvider.
  TOKEN_URL: TOKEN_URL.
  REDIRECT_URI: REDIRECT_URI.
  JWT_CLAIM_PATH: JWT_CLAIM_PATH.
  TokenSuccess.typeLiteral8.type: TokenSuccess#typeLiteral8:type.
  TokenSuccess.typeLiteral8.refresh: TokenSuccess#typeLiteral8:refresh.
  TokenSuccess.typeLiteral8.expires: TokenSuccess#typeLiteral8:expires.
  TokenFailure.typeLiteral9.type: TokenFailure#typeLiteral9:type.
  TokenFailure.typeLiteral9.message: TokenFailure#typeLiteral9:message.
  OAuthServerInfo.typeLiteral83.cancelWait: OAuthServerInfo#typeLiteral83:cancelWait.
  OAuthServerInfo.typeLiteral83.waitForCode: OAuthServerInfo#typeLiteral83:waitForCode.
  loginOpenAICodex.options-typeLiteral145.onAuth: loginOpenAICodex().(options)typeLiteral145:onAuth.
  CALLBACK_HOST: CALLBACK_HOST.
  AUTHORIZE_URL: AUTHORIZE_URL.
  SCOPE: SCOPE.
  TokenSuccess: TokenSuccess#
  TokenFailure: TokenFailure#
  JwtPayload.typeLiteral10.-JWT_CLAIM_PATH-.typeLiteral11.chatgpt_account_id: JwtPayload#typeLiteral10:`[JWT_CLAIM_PATH]`.typeLiteral11:chatgpt_account_id.
  createAuthorizationFlow: createAuthorizationFlow().
  createAuthorizationFlow.Promise.typeLiteral70.verifier: createAuthorizationFlow().Promise:typeLiteral70:verifier.
  createAuthorizationFlow.Promise.typeLiteral70.state: createAuthorizationFlow().Promise:typeLiteral70:state.
  OAuthServerInfo: OAuthServerInfo#
  OAuthServerInfo.typeLiteral83.close: OAuthServerInfo#typeLiteral83:close.
  loginOpenAICodex.options-typeLiteral145.onProgress: loginOpenAICodex().(options)typeLiteral145:onProgress.
  loginOpenAICodex.options-typeLiteral145.originator: loginOpenAICodex().(options)typeLiteral145:originator.
  TokenFailure.typeLiteral9.status: TokenFailure#typeLiteral9:status.
---
# Module: [`packages/ai/src/utils/oauth/openai-codex.ts`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts)

## Classes
### `JwtPayload`
- def: [`packages/ai/src/utils/oauth/openai-codex.ts:36`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L36)
- signature: `type JwtPayload`
- members:
  - `chatgpt_account_id` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L38)
- uses (calls/refs, reference-scoped): [`JWT_CLAIM_PATH`](openai-codex.ts.md#JWT_CLAIM_PATH)
- used by: [`getAccountId`](openai-codex.ts.md#getAccountId), [`decodeJwt`](openai-codex.ts.md#decodeJwt)

### `OAuthServerInfo`
- def: [`packages/ai/src/utils/oauth/openai-codex.ts:208`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L208)
- signature: `type OAuthServerInfo`
- members:
  - `cancelWait` — [`L210`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L210)
  - `close` — [`L209`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L209)
  - `waitForCode` — [`L211`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L211)
- used by: [`loginOpenAICodex`](openai-codex.ts.md#loginOpenAICodex), [`startLocalOAuthServer`](openai-codex.ts.md#startLocalOAuthServer)

### `TokenFailure`
- def: [`packages/ai/src/utils/oauth/openai-codex.ts:33`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L33)
- signature: `type TokenFailure`
- members:
  - `message` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L33)
  - `status` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L33)
  - `type` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L33)
- used by: [`loginOpenAICodex`](openai-codex.ts.md#loginOpenAICodex), [`refreshOpenAICodexToken`](openai-codex.ts.md#refreshOpenAICodexToken), [`TokenResult`](openai-codex.ts.md#TokenResult)

### `TokenResult`
- def: [`packages/ai/src/utils/oauth/openai-codex.ts:34`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L34)
- signature: `type TokenResult`
- uses (calls/refs, reference-scoped): [`TokenFailure`](openai-codex.ts.md#TokenFailure), [`TokenSuccess`](openai-codex.ts.md#TokenSuccess)
- used by: [`exchangeAuthorizationCode`](openai-codex.ts.md#exchangeAuthorizationCode), [`refreshAccessToken`](openai-codex.ts.md#refreshAccessToken)

### `TokenSuccess`
- def: [`packages/ai/src/utils/oauth/openai-codex.ts:32`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L32)
- signature: `type TokenSuccess`
- members:
  - `access` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L32)
  - `expires` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L32)
  - `refresh` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L32)
  - `type` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L32)
- used by: [`loginOpenAICodex`](openai-codex.ts.md#loginOpenAICodex), [`refreshOpenAICodexToken`](openai-codex.ts.md#refreshOpenAICodexToken), [`TokenResult`](openai-codex.ts.md#TokenResult)

## Functions
- `createAuthorizationFlow(originator?: string)` — [`L187`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L187)
- `createState()` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L43)
- `decodeJwt(token: string)` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L80)
- `exchangeAuthorizationCode(code: string, verifier: string, redirectUri?: string)` — [`L92`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L92)
- `getAccountId(accessToken: string)` — [`L290`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L290)
- `loginOpenAICodex(options: { onAuth: (info: { url: string; instructions?: string | undefined; }) => void; onPrompt: (prompt: OAuthPrompt) => Promise<string>; onProgress?: ((message: string) => void) | undefined; onManualCodeInput?: (() => Promise<...>) | undefined; originator?: string | undefined; })` — [`L308`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L308) — Login with OpenAI Codex OAuth
- `parseAuthorizationInput(input: string)` — [`L50`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L50)
- `refreshAccessToken(refreshToken: string)` — [`L139`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L139)
- `refreshOpenAICodexToken(refreshToken: string)` — [`L418`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L418) — Refresh OpenAI Codex OAuth token
- `startLocalOAuthServer(state: string)` — [`L214`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L214)

## Module values
- `AUTHORIZE_URL` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L26)
- `CALLBACK_HOST` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L24)
- `CLIENT_ID` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L25)
- `JWT_CLAIM_PATH` — [`L30`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L30)
- `REDIRECT_URI` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L28)
- `SCOPE` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L29)
- `TOKEN_URL` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L27)
- `_http` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L10)
- `_randomBytes` — [`L9`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L9) — OpenAI Codex (ChatGPT OAuth) flow
- `code` — [`L50`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L50)
- `onAuth` — [`L309`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L309)
- `onManualCodeInput` — [`L312`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L312)
- `onProgress` — [`L311`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L311)
- `onPrompt` — [`L310`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L310)
- `openaiCodexOAuthProvider` — [`L437`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L437)
- `originator` — [`L313`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L313)
- `state` — [`L50`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L50)
- `state` — [`L189`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L189)
- `url` — [`L189`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L189)
- `verifier` — [`L189`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/openai-codex.ts#L189)


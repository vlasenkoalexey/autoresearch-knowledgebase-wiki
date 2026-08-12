---
title: 'Module: packages/ai/src/utils/oauth/github-copilot.ts'
type: catalog
provenance: extracted
module: packages/ai/src/utils/oauth/github-copilot.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/utils/oauth/`github-copilot.ts`/
symbols:
  loginGitHubCopilot.options-typeLiteral135.signal: loginGitHubCopilot().(options)typeLiteral135:signal.
  pollForGitHubAccessToken: pollForGitHubAccessToken().
  refreshGitHubCopilotToken: refreshGitHubCopilotToken().
  startDeviceFlow: startDeviceFlow().
  getUrls: getUrls().
  enableAllGitHubCopilotModels: enableAllGitHubCopilotModels().
  enableGitHubCopilotModel: enableGitHubCopilotModel().
  getGitHubCopilotBaseUrl: getGitHubCopilotBaseUrl().
  loginGitHubCopilot: loginGitHubCopilot().
  CopilotCredentials: CopilotCredentials#
  CLIENT_ID: CLIENT_ID.
  loginGitHubCopilot.options-typeLiteral135.onAuth: loginGitHubCopilot().(options)typeLiteral135:onAuth.
  loginGitHubCopilot.options-typeLiteral135.onPrompt: loginGitHubCopilot().(options)typeLiteral135:onPrompt.
  normalizeDomain: normalizeDomain().
  fetchJson: fetchJson().
  loginGitHubCopilot.options-typeLiteral135.onProgress: loginGitHubCopilot().(options)typeLiteral135:onProgress.
  githubCopilotOAuthProvider: githubCopilotOAuthProvider.
  COPILOT_HEADERS: COPILOT_HEADERS.
  DeviceTokenSuccessResponse: DeviceTokenSuccessResponse#
  DeviceTokenSuccessResponse.typeLiteral6.access_token: DeviceTokenSuccessResponse#typeLiteral6:access_token.
  DeviceTokenErrorResponse: DeviceTokenErrorResponse#
  DeviceTokenErrorResponse.typeLiteral7.error: DeviceTokenErrorResponse#typeLiteral7:error.
  getUrls.typeLiteral14.deviceCodeUrl: getUrls().typeLiteral14:deviceCodeUrl.
  getUrls.typeLiteral14.accessTokenUrl: getUrls().typeLiteral14:accessTokenUrl.
  getUrls.typeLiteral14.copilotTokenUrl: getUrls().typeLiteral14:copilotTokenUrl.
  decode: decode.
  INITIAL_POLL_INTERVAL_MULTIPLIER: INITIAL_POLL_INTERVAL_MULTIPLIER.
  SLOW_DOWN_POLL_INTERVAL_MULTIPLIER: SLOW_DOWN_POLL_INTERVAL_MULTIPLIER.
  DeviceCodeResponse: DeviceCodeResponse#
  DeviceCodeResponse.typeLiteral5.device_code: DeviceCodeResponse#typeLiteral5:device_code.
  DeviceCodeResponse.typeLiteral5.user_code: DeviceCodeResponse#typeLiteral5:user_code.
  DeviceCodeResponse.typeLiteral5.verification_uri: DeviceCodeResponse#typeLiteral5:verification_uri.
  DeviceCodeResponse.typeLiteral5.interval: DeviceCodeResponse#typeLiteral5:interval.
  DeviceCodeResponse.typeLiteral5.expires_in: DeviceCodeResponse#typeLiteral5:expires_in.
  DeviceTokenErrorResponse.typeLiteral7.error_description: DeviceTokenErrorResponse#typeLiteral7:error_description.
  DeviceTokenErrorResponse.typeLiteral7.interval: DeviceTokenErrorResponse#typeLiteral7:interval.
  getBaseUrlFromToken: getBaseUrlFromToken().
  abortableSleep: abortableSleep().
  DeviceTokenSuccessResponse.typeLiteral6.token_type: DeviceTokenSuccessResponse#typeLiteral6:token_type.
  DeviceTokenSuccessResponse.typeLiteral6.scope: DeviceTokenSuccessResponse#typeLiteral6:scope.
---
# Module: [`packages/ai/src/utils/oauth/github-copilot.ts`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts)

## Classes
### `CopilotCredentials`
- def: [`packages/ai/src/utils/oauth/github-copilot.ts:9`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L9)
- signature: `type CopilotCredentials`
- uses (calls/refs, reference-scoped): [`OAuthCredentials`](types.ts.md#OAuthCredentials)
- used by: [`github-copilot.ts`](github-copilot.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-github-copilot.ts)

### `DeviceCodeResponse`
- def: [`packages/ai/src/utils/oauth/github-copilot.ts:26`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L26)
- signature: `type DeviceCodeResponse`
- members:
  - `device_code` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L27)
  - `expires_in` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L31)
  - `interval` — [`L30`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L30)
  - `user_code` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L28)
  - `verification_uri` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L29)
- used by: [`signal`](github-copilot.ts.md#loginGitHubCopilot.options-typeLiteral135.signal), [`startDeviceFlow`](github-copilot.ts.md#startDeviceFlow)

### `DeviceTokenErrorResponse`
- def: [`packages/ai/src/utils/oauth/github-copilot.ts:40`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L40)
- signature: `type DeviceTokenErrorResponse`
- members:
  - `error` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L41)
  - `error_description` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L42)
  - `interval` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L43)
- used by: [`pollForGitHubAccessToken`](github-copilot.ts.md#pollForGitHubAccessToken)

### `DeviceTokenSuccessResponse`
- def: [`packages/ai/src/utils/oauth/github-copilot.ts:34`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L34)
- signature: `type DeviceTokenSuccessResponse`
- members:
  - `access_token` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L35)
  - `scope` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L37)
  - `token_type` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L36)
- used by: [`pollForGitHubAccessToken`](github-copilot.ts.md#pollForGitHubAccessToken)

## Functions
- `abortableSleep(ms: number, signal?: AbortSignal | undefined)` — [`L150`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L150) — Sleep that can be interrupted by an AbortSignal
- `enableAllGitHubCopilotModels(token: string, enterpriseDomain?: string | undefined, onProgress?: ((model: string, success: boolean) => void) | undefined)` — [`L305`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L305) — Enable all known GitHub Copilot models that may require policy acceptance.
- `enableGitHubCopilotModel(token: string, modelId: string, enterpriseDomain?: string | undefined)` — [`L279`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L279) — Enable a model for the user's GitHub Copilot account.
- `fetchJson(url: string, init: RequestInit)` — [`L94`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L94)
- `getBaseUrlFromToken(token: string)` — [`L74`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L74) — Parse the proxy-ep from a Copilot token and convert to API base URL.
- `getGitHubCopilotBaseUrl(token?: string | undefined, enterpriseDomain?: string | undefined)` — [`L83`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L83)
- `getUrls(domain: string)` — [`L57`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L57)
- `loginGitHubCopilot(options: { onAuth: (url: string, instructions?: string | undefined) => void; onPrompt: (prompt: { message: string; placeholder?: string | undefined; allowEmpty?: boolean | undefined; }) => Promise<...>; onProgress?: ((message: string) => void) | undefined; signal?: AbortSignal | undefined; })` — [`L327`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L327) — Login with GitHub Copilot OAuth (device code flow)
- `normalizeDomain(input: string)` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L46)
- `pollForGitHubAccessToken(domain: string, deviceCode: string, intervalSeconds: number, expiresIn: number, signal?: AbortSignal | undefined)` — [`L170`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L170)
- `refreshGitHubCopilotToken(refreshToken: string, enterpriseDomain?: string | undefined)` — [`L241`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L241) — Refresh GitHub Copilot token
- `startDeviceFlow(domain: string)` — [`L103`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L103)

## Module values
- `CLIENT_ID` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L14)
- `COPILOT_HEADERS` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L16)
- `INITIAL_POLL_INTERVAL_MULTIPLIER` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L23)
- `SLOW_DOWN_POLL_INTERVAL_MULTIPLIER` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L24)
- `accessTokenUrl` — [`L59`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L59)
- `copilotTokenUrl` — [`L60`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L60)
- `decode` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L13)
- `deviceCodeUrl` — [`L58`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L58)
- `githubCopilotOAuthProvider` — [`L368`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L368)
- `onAuth` — [`L328`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L328)
- `onProgress` — [`L330`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L330)
- `onPrompt` — [`L329`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L329)
- `signal` — [`L331`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/github-copilot.ts#L331)


---
title: 'Module: packages/ai/src/utils/oauth/index.ts'
type: catalog
provenance: extracted
module: packages/ai/src/utils/oauth/index.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/utils/oauth/`index.ts`/
symbols:
  getOAuthProvider: getOAuthProvider().
  getOAuthApiKey: getOAuthApiKey().
  registerOAuthProvider: registerOAuthProvider().
  oauthProviderRegistry: oauthProviderRegistry.
  BUILT_IN_OAUTH_PROVIDERS: BUILT_IN_OAUTH_PROVIDERS.
  resetOAuthProviders: resetOAuthProviders().
  getOAuthProviders: getOAuthProviders().
  unregisterOAuthProvider: unregisterOAuthProvider().
  getOAuthProviderInfoList: getOAuthProviderInfoList().
  refreshOAuthToken: refreshOAuthToken().
---
# Module: [`packages/ai/src/utils/oauth/index.ts`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/index.ts)

## Functions
- `getOAuthApiKey(providerId: string, credentials: Record<string, OAuthCredentials>)` — [`L127`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/index.ts#L127) — Get API key for a provider from OAuth credentials.
- `getOAuthProvider(id: string)` — [`L47`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/index.ts#L47) — Get an OAuth provider by ID
- `getOAuthProviderInfoList()` — [`L93`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/index.ts#L93)
- `getOAuthProviders()` — [`L86`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/index.ts#L86) — Get all registered OAuth providers
- `refreshOAuthToken(providerId: string, credentials: OAuthCredentials)` — [`L109`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/index.ts#L109) — Refresh token for any OAuth provider.
- `registerOAuthProvider(provider: OAuthProviderInterface)` — [`L54`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/index.ts#L54) — Register a custom OAuth provider
- `resetOAuthProviders()` — [`L76`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/index.ts#L76) — Reset OAuth providers to built-ins.
- `unregisterOAuthProvider(id: string)` — [`L64`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/index.ts#L64) — Unregister an OAuth provider.

## Module values
- `BUILT_IN_OAUTH_PROVIDERS` — [`L34`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/index.ts#L34)
- `oauthProviderRegistry` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/index.ts#L40)


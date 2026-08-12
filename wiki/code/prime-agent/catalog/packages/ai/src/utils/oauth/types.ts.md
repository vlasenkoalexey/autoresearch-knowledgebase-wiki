---
title: 'Module: packages/ai/src/utils/oauth/types.ts'
type: catalog
provenance: extracted
module: packages/ai/src/utils/oauth/types.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/utils/oauth/`types.ts`/OAuth
symbols:
  OAuthCredentials: Credentials#
  OAuthProviderInterface.id: ProviderInterface#id.
  OAuthCredentials.typeLiteral0.access: Credentials#typeLiteral0:access.
  OAuthProviderInterface.name: ProviderInterface#name.
  OAuthLoginCallbacks: LoginCallbacks#
  OAuthProviderInterface: ProviderInterface#
  OAuthProviderId: ProviderId#
  OAuthProviderInterface.login: ProviderInterface#login().
  OAuthCredentials.typeLiteral0.refresh: Credentials#typeLiteral0:refresh.
  OAuthLoginCallbacks.onAuth: LoginCallbacks#onAuth.
  OAuthLoginCallbacks.onPrompt: LoginCallbacks#onPrompt.
  OAuthProviderInterface.getApiKey: ProviderInterface#getApiKey().
  OAuthProviderInterface.modifyModels: ProviderInterface#modifyModels().
  OAuthProviderInterface.refreshToken: ProviderInterface#refreshToken().
  OAuthAuthInfo.typeLiteral4.url: AuthInfo#typeLiteral4:url.
  OAuthLoginCallbacks.onProgress: LoginCallbacks#onProgress.
  OAuthProvider: Provider#
  OAuthSelectPrompt: SelectPrompt#
  OAuthCredentials.typeLiteral0.expires: Credentials#typeLiteral0:expires.
  OAuthAuthInfo.typeLiteral4.instructions: AuthInfo#typeLiteral4:instructions.
  OAuthLoginCallbacks.onManualCodeInput: LoginCallbacks#onManualCodeInput.
  OAuthPrompt: Prompt#
  OAuthPrompt.typeLiteral3.message: Prompt#typeLiteral3:message.
  OAuthProviderInterface.usesCallbackServer: ProviderInterface#usesCallbackServer.
  OAuthPrompt.typeLiteral3.placeholder: Prompt#typeLiteral3:placeholder.
  OAuthAuthInfo: AuthInfo#
  OAuthLoginCallbacks.onSelect: LoginCallbacks#onSelect.
  OAuthProviderInfo: ProviderInfo#
  OAuthProviderInfo.id: ProviderInfo#id.
  OAuthSelectOption: SelectOption#
  OAuthSelectOption.typeLiteral5.label: SelectOption#typeLiteral5:label.
  OAuthSelectPrompt.typeLiteral6.options: SelectPrompt#typeLiteral6:options.
  OAuthLoginCallbacks.signal: LoginCallbacks#signal.
  OAuthSelectOption.typeLiteral5.id: SelectOption#typeLiteral5:id.
  OAuthSelectPrompt.typeLiteral6.message: SelectPrompt#typeLiteral6:message.
  OAuthPrompt.typeLiteral3.allowEmpty: Prompt#typeLiteral3:allowEmpty.
  OAuthProviderInfo.name: ProviderInfo#name.
  OAuthProviderInfo.available: ProviderInfo#available.
---
# Module: [`packages/ai/src/utils/oauth/types.ts`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts)

## Classes
### `OAuthAuthInfo`
- def: [`packages/ai/src/utils/oauth/types.ts:21`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L21)
- signature: `type OAuthAuthInfo`
- members:
  - `instructions` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L23)
  - `url` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L22)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`createMcpOAuthProvider`](../../mcp/oauth.ts.md#createMcpOAuthProvider), [`github-copilot.ts`](github-copilot.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-github-copilot.ts), [`runPrimeInferenceLogin`](../../../../coding-agent/src/modes/interactive/auth-flows.ts.md#ProviderAuthFlows.runPrimeInferenceLogin), [`runPrimeAgentTracesLogin`](../../../../coding-agent/src/modes/interactive/auth-flows.ts.md#ProviderAuthFlows.runPrimeAgentTracesLogin), [`runPrimeBrowserLogin`](../../../../coding-agent/src/core/prime-inference-auth.ts.md#runPrimeBrowserLogin), [`login`](../../cli.ts.md#login), [`prime-inference-auth.ts`](../../../../coding-agent/src/core/prime-inference-auth.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-prime-inference-auth.ts), [`onAuth`](types.ts.md#OAuthLoginCallbacks.onAuth), [`onAuth`](../../../../coding-agent/src/core/prime-inference-auth.ts.md#PrimeInferenceLoginCallbacks.typeLiteral2.onAuth)  (3 test-only)

### `OAuthCredentials`
- def: [`packages/ai/src/utils/oauth/types.ts:3`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L3)
- signature: `type OAuthCredentials`
- members:
  - `access` — [`L5`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L5)
  - `expires` — [`L6`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L6)
  - `refresh` — [`L4`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L4)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`types.ts`](../../../../coding-agent/src/core/extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`createMcpOAuthProvider`](../../mcp/oauth.ts.md#createMcpOAuthProvider), [`auth-storage.ts`](../../../../coding-agent/src/core/auth-storage.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-auth-storage.ts), [`github-copilot.ts`](github-copilot.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-github-copilot.ts), [`anthropic.ts`](anthropic.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-anthropic.ts), [`includeFallback`](../../../../coding-agent/src/core/auth-storage.ts.md#AuthStorage.getApiKeyWithSourceToken.options-typeLiteral324.includeFallback), [`loginOpenAICodex`](openai-codex.ts.md#loginOpenAICodex), [`loginAnthropic`](anthropic.ts.md#loginAnthropic), [`openai-codex.ts`](openai-codex.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-openai-codex.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-index.ts), [`signal`](github-copilot.ts.md#loginGitHubCopilot.options-typeLiteral135.signal), [`_http`](openai-codex.ts.md#_http), [`refreshOAuthTokenWithLock`](../../../../coding-agent/src/core/auth-storage.ts.md#AuthStorage.refreshOAuthTokenWithLock), [`getStoredCredentialValueMaterial`](../../../../coding-agent/src/core/auth-storage.ts.md#AuthStorage.getStoredCredentialValueMaterial), [`toCredentials`](../../mcp/oauth.ts.md#toCredentials), [`oauth.ts`](../../mcp/oauth.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-mcp-oauth.ts), [`refreshOpenAICodexToken`](openai-codex.ts.md#refreshOpenAICodexToken), [`getOAuthApiKey`](index.ts.md#getOAuthApiKey), [`cli.ts`](../../cli.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-cli.ts), [`refreshAnthropicToken`](anthropic.ts.md#refreshAnthropicToken), [`login`](types.ts.md#OAuthProviderInterface.login), [`refreshGitHubCopilotToken`](github-copilot.ts.md#refreshGitHubCopilotToken), [`exchangeAuthorizationCode`](anthropic.ts.md#exchangeAuthorizationCode), [`getApiKey`](types.ts.md#OAuthProviderInterface.getApiKey), [`modifyModels`](types.ts.md#OAuthProviderInterface.modifyModels), [`refreshToken`](types.ts.md#OAuthProviderInterface.refreshToken), [`refreshOAuthToken`](index.ts.md#refreshOAuthToken), [`modifyModels`](../../../../coding-agent/src/core/extensions/types.ts.md#ProviderConfig.oauth.typeLiteral131.modifyModels), [`loadAuth`](../../cli.ts.md#loadAuth), [`saveAuth`](../../cli.ts.md#saveAuth), [`login`](../../../../coding-agent/src/core/extensions/types.ts.md#ProviderConfig.oauth.typeLiteral131.login), [`CopilotCredentials`](github-copilot.ts.md#CopilotCredentials), [`McpCredentials`](../../mcp/oauth.ts.md#McpCredentials), [`OAuthCredential`](../../../../coding-agent/src/core/auth-storage.ts.md#OAuthCredential), [`getApiKey`](../../../../coding-agent/src/core/extensions/types.ts.md#ProviderConfig.oauth.typeLiteral131.getApiKey), [`refreshToken`](../../../../coding-agent/src/core/extensions/types.ts.md#ProviderConfig.oauth.typeLiteral131.refreshToken)  (16 test-only)

### `OAuthLoginCallbacks`
- def: [`packages/ai/src/utils/oauth/types.ts:36`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L36)
- signature: `interface OAuthLoginCallbacks`
- members:
  - `onAuth` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L37)
  - `onManualCodeInput` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L40)
  - `onProgress` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L39)
  - `onPrompt` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L38)
  - `onSelect` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L42) — Show an interactive selector and return the selected option id, or undefined on cancel.
  - `signal` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L43)
- uses (calls/refs, reference-scoped): [`OAuthSelectPrompt`](types.ts.md#OAuthSelectPrompt), [`OAuthPrompt`](types.ts.md#OAuthPrompt), [`OAuthAuthInfo`](types.ts.md#OAuthAuthInfo)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`types.ts`](../../../../coding-agent/src/core/extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`createMcpOAuthProvider`](../../mcp/oauth.ts.md#createMcpOAuthProvider), [`auth-storage.ts`](../../../../coding-agent/src/core/auth-storage.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-auth-storage.ts), [`github-copilot.ts`](github-copilot.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-github-copilot.ts), [`anthropic.ts`](anthropic.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-anthropic.ts), [`showLoginDialog`](../../../../coding-agent/src/modes/interactive/auth-flows.ts.md#ProviderAuthFlows.showLoginDialog), [`openai-codex.ts`](openai-codex.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-openai-codex.ts), [`login`](../../cli.ts.md#login), [`_http`](openai-codex.ts.md#_http), [`oauth.ts`](../../mcp/oauth.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-mcp-oauth.ts), [`login`](types.ts.md#OAuthProviderInterface.login), [`login`](../../../../coding-agent/src/core/auth-storage.ts.md#AuthStorage.login), [`login`](../../../../coding-agent/src/core/extensions/types.ts.md#ProviderConfig.oauth.typeLiteral131.login)  (5 test-only)

### `OAuthPrompt`
- def: [`packages/ai/src/utils/oauth/types.ts:15`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L15)
- signature: `type OAuthPrompt`
- members:
  - `allowEmpty` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L18)
  - `message` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L16)
  - `placeholder` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L17)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`createMcpOAuthProvider`](../../mcp/oauth.ts.md#createMcpOAuthProvider), [`anthropic.ts`](anthropic.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-anthropic.ts), [`loginOpenAICodex`](openai-codex.ts.md#loginOpenAICodex), [`loginAnthropic`](anthropic.ts.md#loginAnthropic), [`login`](../../cli.ts.md#login), [`_http`](openai-codex.ts.md#_http), [`onPrompt`](types.ts.md#OAuthLoginCallbacks.onPrompt), [`onPrompt`](anthropic.ts.md#loginAnthropic.options-typeLiteral136.onPrompt), [`onPrompt`](openai-codex.ts.md#loginOpenAICodex.options-typeLiteral145.onPrompt)  (2 test-only)

### `OAuthProvider`
- def: [`packages/ai/src/utils/oauth/types.ts:13`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L13)
- signature: `type OAuthProvider`
- uses (calls/refs, reference-scoped): [`OAuthProviderId`](types.ts.md#OAuthProviderId)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts)  (4 test-only)

### `OAuthProviderId`
- def: [`packages/ai/src/utils/oauth/types.ts:10`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L10)
- signature: `type OAuthProviderId`
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`auth-flows.ts`](../../../../coding-agent/src/modes/interactive/auth-flows.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-auth-flows.ts), [`auth-storage.ts`](../../../../coding-agent/src/core/auth-storage.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-auth-storage.ts), [`showLoginDialog`](../../../../coding-agent/src/modes/interactive/auth-flows.ts.md#ProviderAuthFlows.showLoginDialog), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-index.ts), [`login`](../../cli.ts.md#login), [`getOAuthProvider`](index.ts.md#getOAuthProvider), [`refreshOAuthTokenWithLock`](../../../../coding-agent/src/core/auth-storage.ts.md#AuthStorage.refreshOAuthTokenWithLock), [`id`](types.ts.md#OAuthProviderInterface.id), [`getOAuthApiKey`](index.ts.md#getOAuthApiKey), [`cli.ts`](../../cli.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-cli.ts), [`login`](../../../../coding-agent/src/core/auth-storage.ts.md#AuthStorage.login), [`main`](../../cli.ts.md#main), [`refreshOAuthToken`](index.ts.md#refreshOAuthToken), [`OAuthProvider`](types.ts.md#OAuthProvider), [`id`](types.ts.md#OAuthProviderInfo.id)

### `OAuthProviderInfo`
- def: [`packages/ai/src/utils/oauth/types.ts:67`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L67)
- signature: `interface OAuthProviderInfo`
- members:
  - `available` — [`L70`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L70)
  - `id` — [`L68`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L68)
  - `name` — [`L69`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L69)
- uses (calls/refs, reference-scoped): [`OAuthProviderId`](types.ts.md#OAuthProviderId)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-index.ts), [`getOAuthProviderInfoList`](index.ts.md#getOAuthProviderInfoList)

### `OAuthProviderInterface`
- def: [`packages/ai/src/utils/oauth/types.ts:46`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L46)
- signature: `interface OAuthProviderInterface`
- members:
  - `getApiKey(method)` — [`L60`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L60) — Convert credentials to API key string for the provider
  - `login(method)` — [`L51`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L51) — Run the login flow, return credentials to persist
  - `modifyModels(method)` — [`L63`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L63) — Optional: modify models for this provider (e.g., update baseUrl)
  - `refreshToken(method)` — [`L57`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L57) — Refresh expired credentials, return updated credentials to persist
  - `id` — [`L47`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L47)
  - `name` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L48)
  - `usesCallbackServer` — [`L54`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L54) — Whether login uses a local callback server and supports manual code input.
- uses (calls/refs, reference-scoped): [`Model`](../../types.ts.md#Model), [`Api`](../../types.ts.md#Api), [`OAuthCredentials`](types.ts.md#OAuthCredentials), [`OAuthLoginCallbacks`](types.ts.md#OAuthLoginCallbacks), [`OAuthProviderId`](types.ts.md#OAuthProviderId)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`model-registry.ts`](../../../../coding-agent/src/core/model-registry.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-model-registry.ts), [`createMcpOAuthProvider`](../../mcp/oauth.ts.md#createMcpOAuthProvider), [`applyProviderConfig`](../../../../coding-agent/src/core/model-registry.ts.md#ModelRegistry.applyProviderConfig), [`github-copilot.ts`](github-copilot.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-github-copilot.ts), [`anthropic.ts`](anthropic.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-anthropic.ts), [`showLoginDialog`](../../../../coding-agent/src/modes/interactive/auth-flows.ts.md#ProviderAuthFlows.showLoginDialog), [`includeFallback`](../../../../coding-agent/src/core/auth-storage.ts.md#AuthStorage.getApiKeyWithSourceToken.options-typeLiteral324.includeFallback), [`<constructor>`](../../../../coding-agent/src/modes/interactive/components/login-dialog.ts.md#LoginDialogComponent.-constructor), [`openai-codex.ts`](openai-codex.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-openai-codex.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-utils-oauth-index.ts), [`loadModels`](../../../../coding-agent/src/core/model-registry.ts.md#ModelRegistry.loadModels), [`getLogoutProviderOptions`](../../../../coding-agent/src/modes/interactive/auth-flows.ts.md#ProviderAuthFlows.getLogoutProviderOptions), [`getLoginProviderOptions`](../../../../coding-agent/src/modes/interactive/auth-flows.ts.md#ProviderAuthFlows.getLoginProviderOptions), [`login`](../../cli.ts.md#login), [`_http`](openai-codex.ts.md#_http), [`getOAuthProvider`](index.ts.md#getOAuthProvider), [`refreshOAuthTokenWithLock`](../../../../coding-agent/src/core/auth-storage.ts.md#AuthStorage.refreshOAuthTokenWithLock), [`getStoredCredentialValueMaterial`](../../../../coding-agent/src/core/auth-storage.ts.md#AuthStorage.getStoredCredentialValueMaterial), [`oauth.ts`](../../mcp/oauth.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-mcp-oauth.ts), [`getProviderDisplayName`](../../../../coding-agent/src/core/model-registry.ts.md#ModelRegistry.getProviderDisplayName), [`getOAuthApiKey`](index.ts.md#getOAuthApiKey), [`runMcpLogin`](../../../../coding-agent/src/modes/interactive/auth-flows.ts.md#ProviderAuthFlows.runMcpLogin), [`registerOAuthProvider`](index.ts.md#registerOAuthProvider), [`login`](../../../../coding-agent/src/core/auth-storage.ts.md#AuthStorage.login), [`main`](../../cli.ts.md#main), [`oauthProviderRegistry`](index.ts.md#oauthProviderRegistry), [`BUILT_IN_OAUTH_PROVIDERS`](index.ts.md#BUILT_IN_OAUTH_PROVIDERS), [`resetOAuthProviders`](index.ts.md#resetOAuthProviders), [`getOAuthProviders`](index.ts.md#getOAuthProviders), [`oauth`](../../../../coding-agent/src/core/model-registry.ts.md#ProviderConfigInput.oauth), [`unregisterOAuthProvider`](index.ts.md#unregisterOAuthProvider), [`getOAuthProviderInfoList`](index.ts.md#getOAuthProviderInfoList), [`refreshOAuthToken`](index.ts.md#refreshOAuthToken)  (3 test-only)

### `OAuthSelectOption`
- def: [`packages/ai/src/utils/oauth/types.ts:26`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L26)
- signature: `type OAuthSelectOption`
- members:
  - `id` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L27)
  - `label` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L28)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`showOAuthLoginSelect`](../../../../coding-agent/src/modes/interactive/auth-flows.ts.md#ProviderAuthFlows.showOAuthLoginSelect), [`OAuthSelectPrompt`](types.ts.md#OAuthSelectPrompt)

### `OAuthSelectPrompt`
- def: [`packages/ai/src/utils/oauth/types.ts:31`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L31)
- signature: `type OAuthSelectPrompt`
- members:
  - `message` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L32)
  - `options` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/oauth/types.ts#L33)
- uses (calls/refs, reference-scoped): [`OAuthSelectOption`](types.ts.md#OAuthSelectOption)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`auth-flows.ts`](../../../../coding-agent/src/modes/interactive/auth-flows.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-auth-flows.ts), [`showLoginDialog`](../../../../coding-agent/src/modes/interactive/auth-flows.ts.md#ProviderAuthFlows.showLoginDialog), [`showOAuthLoginSelect`](../../../../coding-agent/src/modes/interactive/auth-flows.ts.md#ProviderAuthFlows.showOAuthLoginSelect), [`onSelect`](types.ts.md#OAuthLoginCallbacks.onSelect)


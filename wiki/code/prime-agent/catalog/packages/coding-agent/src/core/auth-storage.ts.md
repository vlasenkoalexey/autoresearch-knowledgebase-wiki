---
title: 'Module: packages/coding-agent/src/core/auth-storage.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/auth-storage.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`auth-storage.ts`/
symbols:
  AuthStorage: AuthStorage#
  AuthStorage.inMemory: AuthStorage#inMemory().
  AuthStorage.create: AuthStorage#create().
  ApiKeyCredential.typeLiteral1.type: ApiKeyCredential#typeLiteral1:type.
  AuthStorage.getApiKeyWithSourceToken.options-typeLiteral324.includeFallback: AuthStorage#getApiKeyWithSourceToken().(options)typeLiteral324:includeFallback.
  AuthStorage.getApiKey: AuthStorage#getApiKey().
  ApiKeyCredential.typeLiteral1.key: ApiKeyCredential#typeLiteral1:key.
  AuthStorage.getPrimeInferenceTeamSelection: AuthStorage#getPrimeInferenceTeamSelection().
  AuthStorage.setPrimeInferenceApiKey: AuthStorage#setPrimeInferenceApiKey().
  AuthStorage.setRuntimeApiKey: AuthStorage#setRuntimeApiKey().
  AuthStorage.createAuthSourceCandidate.options-typeLiteral120.resolveValueMaterial: AuthStorage#createAuthSourceCandidate().(options)typeLiteral120:resolveValueMaterial.
  AuthStorage.getStoredAuthCandidate.options-typeLiteral139.resolvedCommandValue: AuthStorage#getStoredAuthCandidate().(options)typeLiteral139:resolvedCommandValue.
  AuthStatus.typeLiteral5.source: AuthStatus#typeLiteral5:source.
  AuthStorage.toPrimeTeamCredential: AuthStorage#toPrimeTeamCredential().
  AuthStorage.getAuthStatus: AuthStorage#getAuthStatus().
  AuthStorage.refreshOAuthTokenWithLock: AuthStorage#refreshOAuthTokenWithLock().
  AuthStorage.setPrimeInferenceTeamSelection: AuthStorage#setPrimeInferenceTeamSelection().
  AuthStorage.getProviderHeaders: AuthStorage#getProviderHeaders().
  AuthStorage.getEnvironmentAuthCandidate: AuthStorage#getEnvironmentAuthCandidate().
  AuthStorage.getStoredCredentialValueMaterial: AuthStorage#getStoredCredentialValueMaterial().
  AuthStorage.set: AuthStorage#set().
  AuthStorage.getAuthSourceTokenForCandidate: AuthStorage#getAuthSourceTokenForCandidate().
  AuthStorage.reload: AuthStorage#reload().
  AuthStatus: AuthStatus#
  AuthSourceToken: AuthSourceToken#
  AuthStorage.getFallbackAuthCandidate: AuthStorage#getFallbackAuthCandidate().
  AuthStorage.persistProviderChange: AuthStorage#persistProviderChange().
  ApiKeyCredential.typeLiteral1.primeTeam: ApiKeyCredential#typeLiteral1:primeTeam.
  AuthStorage.getAuthSourceCandidates: AuthStorage#getAuthSourceCandidates().
  AuthStorage.toAuthStatus: AuthStorage#toAuthStatus().
  AuthStorage.getAuthStatusFromCandidates: AuthStorage#getAuthStatusFromCandidates().
  AuthStorage.hasAuth: AuthStorage#hasAuth().
  AuthStorage.getRuntimeAuthCandidate: AuthStorage#getRuntimeAuthCandidate().
  AuthStorage.isAuthSourceStale: AuthStorage#isAuthSourceStale().
  AuthStorage.logout: AuthStorage#logout().
  AuthStorage.get: AuthStorage#get().
  AuthStorage.data: AuthStorage#data.
  AuthStorage.getPrimeCliAuthCandidate: AuthStorage#getPrimeCliAuthCandidate().
  AuthStorage.getMatchingStaleAuthSources: AuthStorage#getMatchingStaleAuthSources().
  AuthStorage.markAuthStale: AuthStorage#markAuthStale().
  AuthStatus.typeLiteral5.configured: AuthStatus#typeLiteral5:configured.
  AuthStorage.markAuthSourceStale: AuthStorage#markAuthSourceStale().
  AuthSourceToken.typeLiteral8.source: AuthSourceToken#typeLiteral8:source.
  AuthStorage.login: AuthStorage#login().
  AuthStorage.getPrimeCliConfig: AuthStorage#getPrimeCliConfig().
  FileAuthStorageBackend.withLock: FileAuthStorageBackend#withLock().
  AuthCredential: AuthCredential#
  AuthStorage.clearStaleAuthSource: AuthStorage#clearStaleAuthSource().
  AuthStorage.getPrimeCliConfigPath: AuthStorage#getPrimeCliConfigPath().
  AuthSourceCandidate: AuthSourceCandidate#
  AuthStorage.getAvailableAuthCandidate.typeLiteral210.hasStaleCandidate: AuthStorage#getAvailableAuthCandidate().typeLiteral210:hasStaleCandidate.
  AuthStorageBackend: AuthStorageBackend#
  FileAuthStorageBackend.withLockAsync: FileAuthStorageBackend#withLockAsync().
  AuthStorage.getCurrentAuthSourceToken: AuthStorage#getCurrentAuthSourceToken().
  AuthStorage.createAuthSourceCandidate.options-typeLiteral120.source: AuthStorage#createAuthSourceCandidate().(options)typeLiteral120:source.
  AuthStorage.remove: AuthStorage#remove().
  AuthStatus.typeLiteral5.label: AuthStatus#typeLiteral5:label.
  InMemoryAuthStorageBackend.withLock: InMemoryAuthStorageBackend#withLock().
  AuthStorage.isPrimeCliConfigEnabled: AuthStorage#isPrimeCliConfigEnabled().
  AuthStorage.errors: AuthStorage#errors.
  ActiveAuthStatusSource: ActiveAuthStatusSource#
  AuthSourceToken.typeLiteral8.identityFingerprint: AuthSourceToken#typeLiteral8:identityFingerprint.
  InMemoryAuthStorageBackend.withLockAsync: InMemoryAuthStorageBackend#withLockAsync().
  AuthStorageData: AuthStorageData#
  AuthStorageBackend.withLock: AuthStorageBackend#withLock().
  AuthStorage.has: AuthStorage#has().
  AuthSourceToken.typeLiteral8.valueFingerprint: AuthSourceToken#typeLiteral8:valueFingerprint.
  AuthStorage.staleAuthSources: AuthStorage#staleAuthSources.
  AuthStorage.fromStorage: AuthStorage#fromStorage().
  AuthStorage.recordError: AuthStorage#recordError().
  AuthStorage.getOAuthProviders: AuthStorage#getOAuthProviders().
  AuthSourceToken.typeLiteral8.provider: AuthSourceToken#typeLiteral8:provider.
  AuthStorage.createAuthSourceCandidate.options-typeLiteral120.identityMaterial: AuthStorage#createAuthSourceCandidate().(options)typeLiteral120:identityMaterial.
  LockResult.typeLiteral7.result: LockResult#typeLiteral7:result.
  AuthStorage.createAuthSourceCandidate.options-typeLiteral120.valueMaterial: AuthStorage#createAuthSourceCandidate().(options)typeLiteral120:valueMaterial.
  AuthStorage.getStoredAuthCandidate: AuthStorage#getStoredAuthCandidate().
  AuthStorage.getPrimeCliApiKey: AuthStorage#getPrimeCliApiKey().
  AuthSourceCandidate.typeLiteral9.source: AuthSourceCandidate#typeLiteral9:source.
  AuthStorage.getAvailableAuthCandidate.typeLiteral210.candidate: AuthStorage#getAvailableAuthCandidate().typeLiteral210:candidate.
  LockResult: LockResult#
  LockResult.typeLiteral7.next: LockResult#typeLiteral7:next.
  AuthStorageBackend.withLockAsync: AuthStorageBackend#withLockAsync().
  AuthStorage.removeRuntimeApiKey: AuthStorage#removeRuntimeApiKey().
  AuthStorage.createAuthSourceCandidate.options-typeLiteral120.configured: AuthStorage#createAuthSourceCandidate().(options)typeLiteral120:configured.
  AuthStorage.fingerprintAuthSource: AuthStorage#fingerprintAuthSource().
  AuthStorage.parseStorageData: AuthStorage#parseStorageData().
  AuthStorage.drainErrors: AuthStorage#drainErrors().
  AuthStorage.getEnabledPrimeCliConfigPath: AuthStorage#getEnabledPrimeCliConfigPath().
  AuthStorage.loadError: AuthStorage#loadError.
  AuthStorage.createAuthSourceCandidate: AuthStorage#createAuthSourceCandidate().
  AuthStorage.getAll: AuthStorage#getAll().
  OAuthCredential: OAuthCredential#
  InMemoryAuthStorageBackend: InMemoryAuthStorageBackend#
  PrimeTeamCredential: PrimeTeamCredential#
  AuthStorageOptions: AuthStorageOptions#
  AuthApiKeyResult.typeLiteral10.apiKey: AuthApiKeyResult#typeLiteral10:apiKey.
  InMemoryAuthStorageBackend.value: InMemoryAuthStorageBackend#value.
  AuthStorage.runtimeOverrides: AuthStorage#runtimeOverrides.
  AuthStorage.createAuthSourceCandidate.options-typeLiteral120.label: AuthStorage#createAuthSourceCandidate().(options)typeLiteral120:label.
  AuthApiKeyResult: AuthApiKeyResult#
  FileAuthStorageBackend: FileAuthStorageBackend#
  FileAuthStorageBackend.-constructor: FileAuthStorageBackend#`<constructor>`().
  AuthStorage.list: AuthStorage#list().
  PrimeTeamCredential.typeLiteral0.teamId: PrimeTeamCredential#typeLiteral0:teamId.
  AuthStorageOptions.typeLiteral6.primeCliConfigPath: AuthStorageOptions#typeLiteral6:primeCliConfigPath.
  AuthSourceCandidate.typeLiteral9.label: AuthSourceCandidate#typeLiteral9:label.
  AuthSourceCandidate.typeLiteral9.identityFingerprint: AuthSourceCandidate#typeLiteral9:identityFingerprint.
  AuthSourceCandidate.typeLiteral9.valueFingerprint: AuthSourceCandidate#typeLiteral9:valueFingerprint.
  AuthSourceCandidate.typeLiteral9.resolveValueFingerprint: AuthSourceCandidate#typeLiteral9:resolveValueFingerprint.
  AuthStorage.fallbackResolver: AuthStorage#fallbackResolver.
  AuthStorage.getAvailableAuthCandidate: AuthStorage#getAvailableAuthCandidate().
  AuthStorage.getApiKeyWithSourceToken: AuthStorage#getApiKeyWithSourceToken().
  AuthStorage.setFallbackResolver: AuthStorage#setFallbackResolver().
  PrimeTeamCredential.typeLiteral0.name: PrimeTeamCredential#typeLiteral0:name.
  ApiKeyCredential: ApiKeyCredential#
  AuthSourceCandidate.typeLiteral9.configured: AuthSourceCandidate#typeLiteral9:configured.
  AuthApiKeyResult.typeLiteral10.sourceToken: AuthApiKeyResult#typeLiteral10:sourceToken.
  FileAuthStorageBackend.ensureParentDir: FileAuthStorageBackend#ensureParentDir().
  FileAuthStorageBackend.ensureFileExists: FileAuthStorageBackend#ensureFileExists().
  PrimeTeamCredential.typeLiteral0.slug: PrimeTeamCredential#typeLiteral0:slug.
  PrimeTeamCredential.typeLiteral0.role: PrimeTeamCredential#typeLiteral0:role.
  PrimeTeamCredential.typeLiteral0.createdAt: PrimeTeamCredential#typeLiteral0:createdAt.
  AuthStorageOptions.typeLiteral6.usePrimeCliConfig: AuthStorageOptions#typeLiteral6:usePrimeCliConfig.
  FileAuthStorageBackend.acquireLockSyncWithRetry: FileAuthStorageBackend#acquireLockSyncWithRetry().
  AuthStorage.getStoredAuthCandidate.options-typeLiteral139.resolveCommandValue: AuthStorage#getStoredAuthCandidate().(options)typeLiteral139:resolveCommandValue.
  AuthStorage.getAmbientEnvironmentIdentityMaterial: AuthStorage#getAmbientEnvironmentIdentityMaterial().
  AuthStorage.getAuthSourceCandidates.options-typeLiteral179.includeFallback: AuthStorage#getAuthSourceCandidates().(options)typeLiteral179:includeFallback.
  AuthStorage.getAvailableAuthCandidate.options-typeLiteral209.includeFallback: AuthStorage#getAvailableAuthCandidate().(options)typeLiteral209:includeFallback.
  AuthStorage.getApiKey.options-typeLiteral385.includeFallback: AuthStorage#getApiKey().(options)typeLiteral385:includeFallback.
---
# Module: [`packages/coding-agent/src/core/auth-storage.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts)

## Classes
### `ActiveAuthStatusSource`
- def: [`packages/coding-agent/src/core/auth-storage.ts:80`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L80)
- signature: `type ActiveAuthStatusSource`
- uses (calls/refs, reference-scoped): [`source`](auth-storage.ts.md#AuthStatus.typeLiteral5.source), [`AuthStatus`](auth-storage.ts.md#AuthStatus)
- used by: [`source`](auth-storage.ts.md#AuthSourceToken.typeLiteral8.source), [`clearStaleAuthSource`](auth-storage.ts.md#AuthStorage.clearStaleAuthSource), [`source`](auth-storage.ts.md#AuthStorage.createAuthSourceCandidate.options-typeLiteral120.source), [`source`](auth-storage.ts.md#AuthSourceCandidate.typeLiteral9.source), [`fingerprintAuthSource`](auth-storage.ts.md#AuthStorage.fingerprintAuthSource)

### `ApiKeyCredential`
- def: [`packages/coding-agent/src/core/auth-storage.ts:42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L42)
- signature: `type ApiKeyCredential`
- members:
  - `key` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L44)
  - `primeTeam` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L45)
  - `type` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L43) — documented in [packages-coding-agent-src-core-auth-storage.ts](../../../../../concepts/packages-coding-agent-src-core-auth-storage.ts.md)
- uses (calls/refs, reference-scoped): [`PrimeTeamCredential`](auth-storage.ts.md#PrimeTeamCredential)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`applyProviderConfig`](model-registry.ts.md#ModelRegistry.applyProviderConfig), [`includeFallback`](auth-storage.ts.md#AuthStorage.getApiKeyWithSourceToken.options-typeLiteral324.includeFallback), [`runStartupOnboarding`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.runStartupOnboarding), [`getPrimeInferenceTeamSelection`](auth-storage.ts.md#AuthStorage.getPrimeInferenceTeamSelection), [`setPrimeInferenceApiKey`](auth-storage.ts.md#AuthStorage.setPrimeInferenceApiKey), [`loadModels`](model-registry.ts.md#ModelRegistry.loadModels), [`getLogoutProviderOptions`](../modes/interactive/auth-flows.ts.md#ProviderAuthFlows.getLogoutProviderOptions), [`resolvedCommandValue`](auth-storage.ts.md#AuthStorage.getStoredAuthCandidate.options-typeLiteral139.resolvedCommandValue), [`_addWebsearchKeyEnv`](agent-session.ts.md#AgentSession._addWebsearchKeyEnv), [`formatStatusIndicator`](../modes/interactive/components/oauth-selector.ts.md#OAuthSelectorComponent.formatStatusIndicator), [`showApiKeyLoginDialog`](../modes/interactive/auth-flows.ts.md#ProviderAuthFlows.showApiKeyLoginDialog), [`refreshOAuthTokenWithLock`](auth-storage.ts.md#AuthStorage.refreshOAuthTokenWithLock), [`setPrimeInferenceTeamSelection`](auth-storage.ts.md#AuthStorage.setPrimeInferenceTeamSelection), [`getStoredCredentialValueMaterial`](auth-storage.ts.md#AuthStorage.getStoredCredentialValueMaterial), [`isProviderStale`](../modes/interactive/components/oauth-selector.ts.md#OAuthSelectorComponent.isProviderStale), [`completePrimeAgentTracesLogin`](../modes/interactive/auth-flows.ts.md#ProviderAuthFlows.completePrimeAgentTracesLogin), [`getAnthropicSubscriptionAuthWarning`](../modes/interactive/auth-flows.ts.md#getAnthropicSubscriptionAuthWarning), [`login`](auth-storage.ts.md#AuthStorage.login), [`telemetryAuthCategory`](telemetry.ts.md#telemetryAuthCategory), [`isUsingOAuth`](model-registry.ts.md#ModelRegistry.isUsingOAuth), [`AuthCredential`](auth-storage.ts.md#AuthCredential), [`storedCredentialType`](telemetry.ts.md#CaptureOnboardingCompletedOptions.storedCredentialType)  (9 test-only)

### `AuthApiKeyResult`
- def: [`packages/coding-agent/src/core/auth-storage.ts:98`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L98)
- signature: `type AuthApiKeyResult`
- members:
  - `apiKey` — [`L99`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L99)
  - `sourceToken` — [`L100`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L100)
- uses (calls/refs, reference-scoped): [`AuthSourceToken`](auth-storage.ts.md#AuthSourceToken)
- used by: [`getApiKeyAndHeaders`](model-registry.ts.md#ModelRegistry.getApiKeyAndHeaders), [`includeFallback`](auth-storage.ts.md#AuthStorage.getApiKeyWithSourceToken.options-typeLiteral324.includeFallback), [`getApiKey`](auth-storage.ts.md#AuthStorage.getApiKey), [`getApiKeyForProvider`](model-registry.ts.md#ModelRegistry.getApiKeyForProvider)

### `AuthCredential`
- def: [`packages/coding-agent/src/core/auth-storage.ts:52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L52)
- signature: `type AuthCredential`
- uses (calls/refs, reference-scoped): [`OAuthCredential`](auth-storage.ts.md#OAuthCredential), [`ApiKeyCredential`](auth-storage.ts.md#ApiKeyCredential)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`telemetry.ts`](telemetry.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-telemetry.ts), [`getStoredCredentialValueMaterial`](auth-storage.ts.md#AuthStorage.getStoredCredentialValueMaterial), [`set`](auth-storage.ts.md#AuthStorage.set), [`persistProviderChange`](auth-storage.ts.md#AuthStorage.persistProviderChange), [`get`](auth-storage.ts.md#AuthStorage.get), [`telemetryAuthCategory`](telemetry.ts.md#telemetryAuthCategory), [`AuthStorageData`](auth-storage.ts.md#AuthStorageData), [`storedCredentialType`](telemetry.ts.md#CaptureOnboardingCompletedOptions.storedCredentialType)

### `AuthSourceCandidate`
- def: [`packages/coding-agent/src/core/auth-storage.ts:89`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L89)
- signature: `type AuthSourceCandidate`
- members:
  - `configured` — [`L91`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L91)
  - `identityFingerprint` — [`L93`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L93)
  - `label` — [`L92`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L92)
  - `resolveValueFingerprint` — [`L95`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L95)
  - `source` — [`L90`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L90)
  - `valueFingerprint` — [`L94`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L94)
- uses (calls/refs, reference-scoped): [`ActiveAuthStatusSource`](auth-storage.ts.md#ActiveAuthStatusSource)
- used by: [`resolveValueMaterial`](auth-storage.ts.md#AuthStorage.createAuthSourceCandidate.options-typeLiteral120.resolveValueMaterial), [`resolvedCommandValue`](auth-storage.ts.md#AuthStorage.getStoredAuthCandidate.options-typeLiteral139.resolvedCommandValue), [`getEnvironmentAuthCandidate`](auth-storage.ts.md#AuthStorage.getEnvironmentAuthCandidate), [`getAuthSourceTokenForCandidate`](auth-storage.ts.md#AuthStorage.getAuthSourceTokenForCandidate), [`getFallbackAuthCandidate`](auth-storage.ts.md#AuthStorage.getFallbackAuthCandidate), [`getAuthSourceCandidates`](auth-storage.ts.md#AuthStorage.getAuthSourceCandidates), [`toAuthStatus`](auth-storage.ts.md#AuthStorage.toAuthStatus), [`getRuntimeAuthCandidate`](auth-storage.ts.md#AuthStorage.getRuntimeAuthCandidate), [`isAuthSourceStale`](auth-storage.ts.md#AuthStorage.isAuthSourceStale), [`getMatchingStaleAuthSources`](auth-storage.ts.md#AuthStorage.getMatchingStaleAuthSources), [`getPrimeCliAuthCandidate`](auth-storage.ts.md#AuthStorage.getPrimeCliAuthCandidate), [`candidate`](auth-storage.ts.md#AuthStorage.getAvailableAuthCandidate.typeLiteral210.candidate)

### `AuthSourceToken`
- def: [`packages/coding-agent/src/core/auth-storage.ts:82`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L82)
- signature: `type AuthSourceToken`
- members:
  - `identityFingerprint` — [`L85`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L85)
  - `provider` — [`L83`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L83)
  - `source` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L84)
  - `valueFingerprint` — [`L86`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L86)
- uses (calls/refs, reference-scoped): [`ActiveAuthStatusSource`](auth-storage.ts.md#ActiveAuthStatusSource)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`model-registry.ts`](model-registry.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-model-registry.ts), [`AgentConnectionSessionEvent`](../modes/agent-connection/types.ts.md#AgentConnectionSessionEvent), [`_handleRetryableError`](agent-session.ts.md#AgentSession._handleRetryableError), [`AgentSessionEvent`](agent-session.ts.md#AgentSessionEvent), [`getCurrentProviderAuthSourceToken`](model-registry.ts.md#ModelRegistry.getCurrentProviderAuthSourceToken), [`markProviderAuthSourceStale`](model-registry.ts.md#ModelRegistry.markProviderAuthSourceStale), [`_captureRetryAuthFailureSource`](agent-session.ts.md#AgentSession._captureRetryAuthFailureSource), [`getAuthSourceTokenForCandidate`](auth-storage.ts.md#AuthStorage.getAuthSourceTokenForCandidate), [`isAuthSourceStale`](auth-storage.ts.md#AuthStorage.isAuthSourceStale), [`getMatchingStaleAuthSources`](auth-storage.ts.md#AuthStorage.getMatchingStaleAuthSources), [`getMatchingStaleProviderRequestAuthSources`](model-registry.ts.md#ModelRegistry.getMatchingStaleProviderRequestAuthSources), [`_markProviderAuthStale`](agent-session.ts.md#AgentSession._markProviderAuthStale), [`authSourceTokens`](agent-session.ts.md#AgentSession._markProviderAuthStaleForRetryFailure.options-typeLiteral4097.authSourceTokens), [`clearStaleProviderRequestAuthSource`](model-registry.ts.md#ModelRegistry.clearStaleProviderRequestAuthSource), [`getProviderRequestAuthSourceToken`](model-registry.ts.md#ModelRegistry.getProviderRequestAuthSourceToken), [`markAuthSourceStale`](auth-storage.ts.md#AuthStorage.markAuthSourceStale), [`isProviderRequestAuthStale`](model-registry.ts.md#ModelRegistry.isProviderRequestAuthStale), [`isProviderRequestAuthStaleForStatus`](model-registry.ts.md#ModelRegistry.isProviderRequestAuthStaleForStatus), [`_retryAuthFailureSources`](agent-session.ts.md#AgentSession._retryAuthFailureSources), [`clearStaleAuthSource`](auth-storage.ts.md#AuthStorage.clearStaleAuthSource), [`getCurrentAuthSourceToken`](auth-storage.ts.md#AuthStorage.getCurrentAuthSourceToken), [`setLastProviderAuthSourceToken`](model-registry.ts.md#ModelRegistry.setLastProviderAuthSourceToken), [`staleAuthSources`](auth-storage.ts.md#AuthStorage.staleAuthSources), [`staleProviderRequestAuthSources`](model-registry.ts.md#ModelRegistry.staleProviderRequestAuthSources), [`lastProviderAuthSourceTokens`](model-registry.ts.md#ModelRegistry.lastProviderAuthSourceTokens), [`AuthApiKeyResult`](auth-storage.ts.md#AuthApiKeyResult)  (1 test-only)

### `AuthStatus`
- def: [`packages/coding-agent/src/core/auth-storage.ts:56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L56)
- signature: `type AuthStatus`
- members:
  - `configured` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L57)
  - `label` — [`L67`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L67)
  - `source` — [`L58`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L58)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`model-registry.ts`](model-registry.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-model-registry.ts), [`<constructor>`](../modes/interactive/components/oauth-selector.ts.md#OAuthSelectorComponent.-constructor), [`oauth-selector.ts`](../modes/interactive/components/oauth-selector.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-oauth-selector.ts), [`runStartupOnboarding`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.runStartupOnboarding), [`getPrimeInferenceTeamSelection`](auth-storage.ts.md#AuthStorage.getPrimeInferenceTeamSelection), [`telemetry.ts`](telemetry.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-telemetry.ts), [`getLogoutProviderOptions`](../modes/interactive/auth-flows.ts.md#ProviderAuthFlows.getLogoutProviderOptions), [`getProviderAuthStatus`](model-registry.ts.md#ModelRegistry.getProviderAuthStatus), [`formatStatusIndicator`](../modes/interactive/components/oauth-selector.ts.md#OAuthSelectorComponent.formatStatusIndicator), [`getAuthStatus`](auth-storage.ts.md#AuthStorage.getAuthStatus), [`shouldRunPrimeCliOnboardingSplash`](../modes/interactive/onboarding.ts.md#shouldRunPrimeCliOnboardingSplash), [`isProviderStale`](../modes/interactive/components/oauth-selector.ts.md#OAuthSelectorComponent.isProviderStale), [`_authenticatedRlmModels`](agent-session.ts.md#AgentSession._authenticatedRlmModels), [`onboarding.ts`](../modes/interactive/onboarding.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-onboarding.ts), [`getAuthStatusFromCandidates`](auth-storage.ts.md#AuthStorage.getAuthStatusFromCandidates), [`isProviderConfigured`](../modes/interactive/components/oauth-selector.ts.md#OAuthSelectorComponent.isProviderConfigured), [`toAuthStatus`](auth-storage.ts.md#AuthStorage.toAuthStatus), [`telemetryAuthCategory`](telemetry.ts.md#telemetryAuthCategory), [`formatApiKeyStatusIndicator`](../modes/interactive/components/oauth-selector.ts.md#OAuthSelectorComponent.formatApiKeyStatusIndicator), [`ActiveAuthStatusSource`](auth-storage.ts.md#ActiveAuthStatusSource), [`authSource`](telemetry.ts.md#CaptureOnboardingCompletedOptions.authSource), [`getAuthStatus`](../modes/interactive/components/oauth-selector.ts.md#OAuthSelectorComponent.getAuthStatus), [`getProviderAuthStatus`](../modes/interactive/onboarding.ts.md#OnboardingModelRegistryReader.getProviderAuthStatus)  (4 test-only)

### `AuthStorage`
- def: [`packages/coding-agent/src/core/auth-storage.ts:247`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L247) — documented in [packages-coding-agent-src-core-auth-storage.ts](../../../../../concepts/packages-coding-agent-src-core-auth-storage.ts.md)
- doc: Credential storage backed by a JSON file.
- signature: `class AuthStorage`
- members:
  - `clearStaleAuthSource(method)` — [`L605`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L605)
  - `create(method)` — [`L262`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L262) — documented in [packages-coding-agent-src-core-auth-storage.ts](../../../../../concepts/packages-coding-agent-src-core-auth-storage.ts.md)
  - `createAuthSourceCandidate(method)` — [`L312`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L312)
  - `drainErrors(method)` — [`L725`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L725)
  - `fingerprintAuthSource(method)` — [`L307`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L307)
  - `fromStorage(method)` — [`L267`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L267)
  - `get(method)` — [`L667`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L667) — Get credential for a provider.
  - `getAll(method)` — [`L721`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L721) — Get all credentials (for passing to getOAuthApiKey).
  - `getAmbientEnvironmentIdentityMaterial(method)` — [`L441`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L441)
  - `getApiKey(method)` — [`L964`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L964)
  - `getApiKeyWithSourceToken(method)` — [`L818`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L818) — Get API key for a provider.
  - `getAuthSourceCandidates(method)` — [`L483`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L483)
  - `getAuthSourceTokenForCandidate(method)` — [`L562`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L562)
  - `getAuthStatus(method)` — [`L714`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L714) — Return auth status without exposing credential values or refreshing tokens.
  - `getAuthStatusFromCandidates(method)` — [`L546`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L546)
  - `getAvailableAuthCandidate(method)` — [`L523`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L523)
  - `getCurrentAuthSourceToken(method)` — [`L578`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L578)
  - `getEnabledPrimeCliConfigPath(method)` — [`L1124`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L1124)
  - `getEnvironmentAuthCandidate(method)` — [`L423`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L423)
  - `getFallbackAuthCandidate(method)` — [`L469`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L469)
  - `getMatchingStaleAuthSources(method)` — [`L513`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L513)
  - `getOAuthProviders(method)` — [`L972`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L972) — Get all registered OAuth providers
  - `getPrimeCliApiKey(method)` — [`L1120`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L1120)
  - `getPrimeCliAuthCandidate(method)` — [`L378`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L378)
  - `getPrimeCliConfig(method)` — [`L1110`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L1110)
  - `getPrimeCliConfigPath(method)` — [`L1086`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L1086)
  - `getPrimeInferenceTeamSelection(method)` — [`L1029`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L1029)
  - `getProviderHeaders(method)` — [`L1072`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L1072)
  - `getRuntimeAuthCandidate(method)` — [`L362`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L362)
  - `getStoredAuthCandidate(method)` — [`L394`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L394)
  - `getStoredCredentialValueMaterial(method)` — [`L349`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L349)
  - `has(method)` — [`L699`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L699) — Check if credentials exist for a provider in auth.json.
  - `hasAuth(method)` — [`L707`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L707) — Check if any form of auth is configured for a provider.
  - `inMemory(method)` — [`L271`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L271) — documented in [packages-coding-agent-src-core-auth-storage.ts](../../../../../concepts/packages-coding-agent-src-core-auth-storage.ts.md)
  - `isAuthSourceStale(method)` — [`L504`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L504)
  - `isPrimeCliConfigEnabled(method)` — [`L1132`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L1132)
  - `list(method)` — [`L692`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L692) — List all providers with credentials.
  - `login(method)` — [`L734`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L734) — Login to an OAuth provider.
  - `logout(method)` — [`L747`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L747) — Logout from a provider.
  - `markAuthSourceStale(method)` — [`L586`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L586)
  - `markAuthStale(method)` — [`L557`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L557)
  - `parseStorageData(method)` — [`L618`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L618)
  - `persistProviderChange(method)` — [`L643`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L643)
  - `recordError(method)` — [`L302`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L302)
  - `refreshOAuthTokenWithLock(method)` — [`L764`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L764) — Refresh OAuth token with backend locking to prevent race conditions.
  - `reload(method)` — [`L628`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L628) — Reload credentials from storage.
  - `remove(method)` — [`L683`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L683) — Remove credential for a provider.
  - `removeRuntimeApiKey(method)` — [`L289`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L289) — Remove a runtime API key override.
  - `set(method)` — [`L674`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L674) — Set credential for a provider.
  - `setFallbackResolver(method)` — [`L298`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L298) — Set a fallback resolver for API keys not found in auth.json or env vars.
  - `setPrimeInferenceApiKey(method)` — [`L997`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L997)
  - `setPrimeInferenceTeamSelection(method)` — [`L976`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L976)
  - `setRuntimeApiKey(method)` — [`L281`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L281) — Set a runtime API key override (not persisted to disk).
  - `toAuthStatus(method)` — [`L538`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L538)
  - `toPrimeTeamCredential(method)` — [`L1093`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L1093)
  - `candidate` — [`L526`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L526)
  - `configured` — [`L314`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L314)
  - `data` — [`L248`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L248)
  - `errors` — [`L253`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L253)
  - `fallbackResolver` — [`L251`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L251)
  - `hasStaleCandidate` — [`L526`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L526)
  - `identityMaterial` — [`L315`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L315)
  - `includeFallback` — [`L483`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L483)
  - `includeFallback` — [`L525`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L525)
  - `includeFallback` — [`L820`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L820)
  - `includeFallback` — [`L964`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L964)
  - `label` — [`L317`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L317)
  - `loadError` — [`L252`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L252)
  - `resolveCommandValue` — [`L396`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L396)
  - `resolveValueMaterial` — [`L318`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L318)
  - `resolvedCommandValue` — [`L396`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L396)
  - `runtimeOverrides` — [`L249`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L249)
  - `source` — [`L313`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L313)
  - `staleAuthSources` — [`L250`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L250)
  - `valueMaterial` — [`L316`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L316)
- uses (calls/refs, reference-scoped): [`getAgentDir`](../config.ts.md#getAgentDir), [`type`](auth-storage.ts.md#ApiKeyCredential.typeLiteral1.type), [`PRIME_INFERENCE_PROVIDER_ID`](prime-inference-auth.ts.md#PRIME_INFERENCE_PROVIDER_ID), [`OAuthCredentials`](../../../ai/src/utils/oauth/types.ts.md#OAuthCredentials), [`loadPrimeCliConfig`](prime-inference-auth.ts.md#loadPrimeCliConfig), [`key`](auth-storage.ts.md#ApiKeyCredential.typeLiteral1.key), [`getEnvApiKey`](../../../ai/src/env-api-keys.ts.md#getEnvApiKey), [`source`](auth-storage.ts.md#AuthStatus.typeLiteral5.source), [`getOAuthProvider`](../../../ai/src/utils/oauth/index.ts.md#getOAuthProvider), [`savePrimeCliTeamSelection`](prime-inference-auth.ts.md#savePrimeCliTeamSelection), [`AuthSourceToken`](auth-storage.ts.md#AuthSourceToken), [`AuthStatus`](auth-storage.ts.md#AuthStatus), [`primeTeam`](auth-storage.ts.md#ApiKeyCredential.typeLiteral1.primeTeam), [`getOAuthApiKey`](../../../ai/src/utils/oauth/index.ts.md#getOAuthApiKey), [`access`](../../../ai/src/utils/oauth/types.ts.md#OAuthCredentials.typeLiteral0.access), [`OAuthLoginCallbacks`](../../../ai/src/utils/oauth/types.ts.md#OAuthLoginCallbacks), [`clearPrimeCliCredentials`](prime-inference-auth.ts.md#clearPrimeCliCredentials), [`configured`](auth-storage.ts.md#AuthStatus.typeLiteral5.configured), [`savePrimeCliApiKey`](prime-inference-auth.ts.md#savePrimeCliApiKey), [`source`](auth-storage.ts.md#AuthSourceToken.typeLiteral8.source), [`OAuthProviderId`](../../../ai/src/utils/oauth/types.ts.md#OAuthProviderId), [`login`](../../../ai/src/utils/oauth/types.ts.md#OAuthProviderInterface.login), [`findEnvKeys`](../../../ai/src/env-api-keys.ts.md#findEnvKeys), [`PrimeTeam`](prime-inference-auth.ts.md#PrimeTeam), [`AuthCredential`](auth-storage.ts.md#AuthCredential), [`refresh`](../../../ai/src/utils/oauth/types.ts.md#OAuthCredentials.typeLiteral0.refresh), [`teamId`](prime-inference-auth.ts.md#PrimeTeam.typeLiteral17.teamId), [`getApiKey`](../../../ai/src/utils/oauth/types.ts.md#OAuthProviderInterface.getApiKey), [`AuthSourceCandidate`](auth-storage.ts.md#AuthSourceCandidate), [`name`](prime-inference-auth.ts.md#PrimeTeam.typeLiteral17.name), [`role`](prime-inference-auth.ts.md#PrimeTeam.typeLiteral17.role), [`AuthStorageBackend`](auth-storage.ts.md#AuthStorageBackend), [`getOAuthProviders`](../../../ai/src/utils/oauth/index.ts.md#getOAuthProviders), [`apiKey`](prime-inference-auth.ts.md#PrimeCliConfig.typeLiteral1.apiKey), [`label`](auth-storage.ts.md#AuthStatus.typeLiteral5.label), [`withLock`](auth-storage.ts.md#InMemoryAuthStorageBackend.withLock), [`resolveConfigValueUncached`](resolve-config-value.ts.md#resolveConfigValueUncached), [`ActiveAuthStatusSource`](auth-storage.ts.md#ActiveAuthStatusSource), [`identityFingerprint`](auth-storage.ts.md#AuthSourceToken.typeLiteral8.identityFingerprint), [`teamId`](prime-inference-auth.ts.md#PrimeCliConfig.typeLiteral1.teamId)  (+35 more)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`createAgentSession`](sdk.ts.md#createAgentSession), [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`createAgentSessionServices`](agent-session-services.ts.md#createAgentSessionServices), [`sdk.ts`](sdk.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-sdk.ts), [`sessionOptionsOverride`](../main.ts.md#prepareRuntimeServices.options-typeLiteral166.sessionOptionsOverride), [`model-registry.ts`](model-registry.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-model-registry.ts), [`agent-session-services.ts`](agent-session-services.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-services.ts), [`<constructor>`](../modes/interactive/components/oauth-selector.ts.md#OAuthSelectorComponent.-constructor), [`applyProviderConfig`](model-registry.ts.md#ModelRegistry.applyProviderConfig), [`create`](model-registry.ts.md#ModelRegistry.create), [`getApiKeyAndHeaders`](model-registry.ts.md#ModelRegistry.getApiKeyAndHeaders), [`runPrimeInferenceLogin`](../modes/interactive/auth-flows.ts.md#ProviderAuthFlows.runPrimeInferenceLogin), [`configuration-menu.ts`](../modes/interactive/components/configuration-menu.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-configuration-menu.ts), [`showLoginDialog`](../modes/interactive/auth-flows.ts.md#ProviderAuthFlows.showLoginDialog), [`reload`](agent-session.ts.md#AgentSession.reload), [`oauth-selector.ts`](../modes/interactive/components/oauth-selector.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-oauth-selector.ts), [`runStartupOnboarding`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.runStartupOnboarding), [`refresh`](model-registry.ts.md#ModelRegistry.refresh), [`getApiKeyForProvider`](model-registry.ts.md#ModelRegistry.getApiKeyForProvider), [`agent-traces.ts`](agent-traces.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-traces.ts), [`loadModels`](model-registry.ts.md#ModelRegistry.loadModels), [`runLogout`](../modes/interactive/auth-flows.ts.md#ProviderAuthFlows.runLogout), [`getLogoutProviderOptions`](../modes/interactive/auth-flows.ts.md#ProviderAuthFlows.getLogoutProviderOptions), [`selectPrimeInferenceTeam`](../modes/interactive/auth-flows.ts.md#ProviderAuthFlows.selectPrimeInferenceTeam), [`getLoginProviderOptions`](../modes/interactive/auth-flows.ts.md#ProviderAuthFlows.getLoginProviderOptions), [`refreshPrivatePrimeInferenceAuthorization`](model-registry.ts.md#ModelRegistry.refreshPrivatePrimeInferenceAuthorization), [`handleMcpCommand`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleMcpCommand), [`getProviderAuthStatus`](model-registry.ts.md#ModelRegistry.getProviderAuthStatus), [`mcp-manager.ts`](mcp/mcp-manager.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-mcp-mcp-manager.ts), [`_addWebsearchKeyEnv`](agent-session.ts.md#AgentSession._addWebsearchKeyEnv), [`formatStatusIndicator`](../modes/interactive/components/oauth-selector.ts.md#OAuthSelectorComponent.formatStatusIndicator), [`showApiKeyLoginDialog`](../modes/interactive/auth-flows.ts.md#ProviderAuthFlows.showApiKeyLoginDialog), [`getCurrentProviderAuthSourceToken`](model-registry.ts.md#ModelRegistry.getCurrentProviderAuthSourceToken), [`authStorage`](agent-traces.ts.md#AgentTraceUploadOptions.authStorage), [`markProviderAuthSourceStale`](model-registry.ts.md#ModelRegistry.markProviderAuthSourceStale), [`configPath`](agent-traces.ts.md#getPrimeAgentTraceCredential.options-typeLiteral365.configPath), [`completePrimeInferenceLogin`](../modes/interactive/auth-flows.ts.md#ProviderAuthFlows.completePrimeInferenceLogin), [`isProviderStale`](../modes/interactive/components/oauth-selector.ts.md#OAuthSelectorComponent.isProviderStale), [`getProviderDisplayName`](model-registry.ts.md#ModelRegistry.getProviderDisplayName)  (+22 more; 55 test-only)

### `AuthStorageBackend`
- def: [`packages/coding-agent/src/core/auth-storage.ts:103`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L103)
- signature: `interface AuthStorageBackend`
- members:
  - `withLock(method)` — [`L104`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L104)
  - `withLockAsync(method)` — [`L105`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L105)
- uses (calls/refs, reference-scoped): [`withLock`](auth-storage.ts.md#FileAuthStorageBackend.withLock), [`withLockAsync`](auth-storage.ts.md#FileAuthStorageBackend.withLockAsync), [`withLock`](auth-storage.ts.md#InMemoryAuthStorageBackend.withLock), [`withLockAsync`](auth-storage.ts.md#InMemoryAuthStorageBackend.withLockAsync), [`LockResult`](auth-storage.ts.md#LockResult), [`InMemoryAuthStorageBackend`](auth-storage.ts.md#InMemoryAuthStorageBackend), [`FileAuthStorageBackend`](auth-storage.ts.md#FileAuthStorageBackend)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`refreshOAuthTokenWithLock`](auth-storage.ts.md#AuthStorage.refreshOAuthTokenWithLock), [`reload`](auth-storage.ts.md#AuthStorage.reload), [`persistProviderChange`](auth-storage.ts.md#AuthStorage.persistProviderChange), [`errors`](auth-storage.ts.md#AuthStorage.errors), [`fromStorage`](auth-storage.ts.md#AuthStorage.fromStorage), [`InMemoryAuthStorageBackend`](auth-storage.ts.md#InMemoryAuthStorageBackend), [`FileAuthStorageBackend`](auth-storage.ts.md#FileAuthStorageBackend)

### `AuthStorageData`
- def: [`packages/coding-agent/src/core/auth-storage.ts:54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L54)
- signature: `type AuthStorageData`
- uses (calls/refs, reference-scoped): [`AuthCredential`](auth-storage.ts.md#AuthCredential)
- used by: [`inMemory`](auth-storage.ts.md#AuthStorage.inMemory), [`refreshOAuthTokenWithLock`](auth-storage.ts.md#AuthStorage.refreshOAuthTokenWithLock), [`persistProviderChange`](auth-storage.ts.md#AuthStorage.persistProviderChange), [`data`](auth-storage.ts.md#AuthStorage.data), [`parseStorageData`](auth-storage.ts.md#AuthStorage.parseStorageData), [`getAll`](auth-storage.ts.md#AuthStorage.getAll)

### `AuthStorageOptions`
- def: [`packages/coding-agent/src/core/auth-storage.ts:70`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L70)
- signature: `type AuthStorageOptions`
- members:
  - `primeCliConfigPath` — [`L71`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L71)
  - `usePrimeCliConfig` — [`L72`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L72)
- used by: [`inMemory`](auth-storage.ts.md#AuthStorage.inMemory), [`create`](auth-storage.ts.md#AuthStorage.create), [`getPrimeCliConfig`](auth-storage.ts.md#AuthStorage.getPrimeCliConfig), [`getPrimeCliConfigPath`](auth-storage.ts.md#AuthStorage.getPrimeCliConfigPath), [`isPrimeCliConfigEnabled`](auth-storage.ts.md#AuthStorage.isPrimeCliConfigEnabled), [`errors`](auth-storage.ts.md#AuthStorage.errors), [`fromStorage`](auth-storage.ts.md#AuthStorage.fromStorage)

### `FileAuthStorageBackend`  ·  implements/extends AuthStorageBackend
- def: [`packages/coding-agent/src/core/auth-storage.ts:108`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L108)
- signature: `class FileAuthStorageBackend`
- members:
  - `<constructor>(authPath?: string)` — [`L109`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L109)
  - `acquireLockSyncWithRetry(method)` — [`L125`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L125)
  - `ensureFileExists(method)` — [`L118`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L118)
  - `ensureParentDir(method)` — [`L111`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L111)
  - `withLock(method)` — [`L152`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L152)
  - `withLockAsync(method)` — [`L173`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L173)
- uses (calls/refs, reference-scoped): [`getAgentDir`](../config.ts.md#getAgentDir), [`AuthStorageBackend`](auth-storage.ts.md#AuthStorageBackend), [`result`](auth-storage.ts.md#LockResult.typeLiteral7.result), [`LockResult`](auth-storage.ts.md#LockResult), [`next`](auth-storage.ts.md#LockResult.typeLiteral7.next)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`create`](auth-storage.ts.md#AuthStorage.create), [`AuthStorageBackend`](auth-storage.ts.md#AuthStorageBackend), [`withLock`](auth-storage.ts.md#AuthStorageBackend.withLock), [`withLockAsync`](auth-storage.ts.md#AuthStorageBackend.withLockAsync)

### `InMemoryAuthStorageBackend`  ·  implements/extends AuthStorageBackend
- def: [`packages/coding-agent/src/core/auth-storage.ts:224`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L224)
- signature: `class InMemoryAuthStorageBackend`
- members:
  - `withLock(method)` — [`L227`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L227)
  - `withLockAsync(method)` — [`L235`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L235)
  - `value` — [`L225`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L225)
- uses (calls/refs, reference-scoped): [`AuthStorageBackend`](auth-storage.ts.md#AuthStorageBackend), [`result`](auth-storage.ts.md#LockResult.typeLiteral7.result), [`LockResult`](auth-storage.ts.md#LockResult), [`next`](auth-storage.ts.md#LockResult.typeLiteral7.next)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`inMemory`](auth-storage.ts.md#AuthStorage.inMemory), [`AuthStorageBackend`](auth-storage.ts.md#AuthStorageBackend), [`withLock`](auth-storage.ts.md#AuthStorageBackend.withLock), [`withLockAsync`](auth-storage.ts.md#AuthStorageBackend.withLockAsync)

### `LockResult`
- def: [`packages/coding-agent/src/core/auth-storage.ts:75`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L75)
- signature: `type LockResult`
- members:
  - `next` — [`L77`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L77)
  - `result` — [`L76`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L76)
- used by: [`inMemory`](auth-storage.ts.md#AuthStorage.inMemory), [`reload`](auth-storage.ts.md#AuthStorage.reload), [`persistProviderChange`](auth-storage.ts.md#AuthStorage.persistProviderChange), [`withLock`](auth-storage.ts.md#FileAuthStorageBackend.withLock), [`AuthStorageBackend`](auth-storage.ts.md#AuthStorageBackend), [`withLockAsync`](auth-storage.ts.md#FileAuthStorageBackend.withLockAsync), [`withLock`](auth-storage.ts.md#InMemoryAuthStorageBackend.withLock), [`withLockAsync`](auth-storage.ts.md#InMemoryAuthStorageBackend.withLockAsync), [`withLock`](auth-storage.ts.md#AuthStorageBackend.withLock)

### `OAuthCredential`
- def: [`packages/coding-agent/src/core/auth-storage.ts:48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L48)
- signature: `type OAuthCredential`
- uses (calls/refs, reference-scoped): [`OAuthCredentials`](../../../ai/src/utils/oauth/types.ts.md#OAuthCredentials)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`AuthCredential`](auth-storage.ts.md#AuthCredential)

### `PrimeTeamCredential`
- def: [`packages/coding-agent/src/core/auth-storage.ts:34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L34)
- signature: `type PrimeTeamCredential`
- members:
  - `createdAt` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L39)
  - `name` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L36)
  - `role` — [`L38`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L38)
  - `slug` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L37)
  - `teamId` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-storage.ts#L35)
- used by: [`getPrimeInferenceTeamSelection`](auth-storage.ts.md#AuthStorage.getPrimeInferenceTeamSelection), [`selectPrimeInferenceTeam`](../modes/interactive/auth-flows.ts.md#ProviderAuthFlows.selectPrimeInferenceTeam), [`toPrimeTeamCredential`](auth-storage.ts.md#AuthStorage.toPrimeTeamCredential), [`getProviderHeaders`](auth-storage.ts.md#AuthStorage.getProviderHeaders), [`getPrimeInferenceDefaultTeamStatus`](../modes/interactive/auth-flows.ts.md#ProviderAuthFlows.getPrimeInferenceDefaultTeamStatus), [`primeTeam`](auth-storage.ts.md#ApiKeyCredential.typeLiteral1.primeTeam)


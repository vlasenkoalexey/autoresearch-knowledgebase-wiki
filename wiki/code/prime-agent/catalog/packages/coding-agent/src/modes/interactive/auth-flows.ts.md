---
title: 'Module: packages/coding-agent/src/modes/interactive/auth-flows.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/auth-flows.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/`auth-flows.ts`/
symbols:
  ProviderAuthFlows.runPrimeInferenceLogin: ProviderAuthFlows#runPrimeInferenceLogin().
  ProviderAuthFlows.showLoginDialog: ProviderAuthFlows#showLoginDialog().
  ProviderAuthFlows.runPrimeAgentTracesLogin: ProviderAuthFlows#runPrimeAgentTracesLogin().
  ProviderAuthFlows.runLogout: ProviderAuthFlows#runLogout().
  ProviderAuthFlows.getLogoutProviderOptions: ProviderAuthFlows#getLogoutProviderOptions().
  ProviderAuthFlows.runLogin: ProviderAuthFlows#runLogin().
  ProviderAuthFlows.selectPrimeInferenceTeam: ProviderAuthFlows#selectPrimeInferenceTeam().
  ProviderAuthFlows.getLoginProviderOptions: ProviderAuthFlows#getLoginProviderOptions().
  ProviderAuthFlows.showOAuthLoginSelect: ProviderAuthFlows#showOAuthLoginSelect().
  ProviderAuthFlows.showBedrockSetupDialog: ProviderAuthFlows#showBedrockSetupDialog().
  ProviderAuthFlowsHost.modelRegistry: ProviderAuthFlowsHost#modelRegistry.
  ProviderAuthFlows.showApiKeyLoginDialog: ProviderAuthFlows#showApiKeyLoginDialog().
  ProviderAuthFlows.loginProvider: ProviderAuthFlows#loginProvider().
  ProviderAuthFlowsHost.ui: ProviderAuthFlowsHost#ui.
  AuthenticationResult: AuthenticationResult#
  ProviderAuthFlows.completePrimeInferenceLogin: ProviderAuthFlows#completePrimeInferenceLogin().
  ProviderAuthFlows.showPrimeTeamSelector: ProviderAuthFlows#showPrimeTeamSelector().
  ProviderAuthFlows.getPrimeInferenceDefaultTeamStatus: ProviderAuthFlows#getPrimeInferenceDefaultTeamStatus().
  ProviderAuthFlows.completeProviderAuthentication: ProviderAuthFlows#completeProviderAuthentication().
  ProviderAuthFlows.completePrimeAgentTracesLogin: ProviderAuthFlows#completePrimeAgentTracesLogin().
  ProviderAuthFlows.runMcpLogin: ProviderAuthFlows#runMcpLogin().
  getAnthropicSubscriptionAuthWarning: getAnthropicSubscriptionAuthWarning().
  ProviderAuthFlows.completeExternalProviderSetup: ProviderAuthFlows#completeExternalProviderSetup().
  isApiKeyLoginProvider: isApiKeyLoginProvider().
  ProviderAuthFlowsHost.showError: ProviderAuthFlowsHost#showError().
  ProviderAuthFlowsHost.showStatus: ProviderAuthFlowsHost#showStatus().
  ProviderAuthFlows.-constructor: ProviderAuthFlows#`<constructor>`().
  ProviderAuthFlows.hasAvailableProviderModels: ProviderAuthFlows#hasAvailableProviderModels().
  ProviderAuthFlowsHost.onAuthChanged: ProviderAuthFlowsHost#onAuthChanged().
  ProviderAuthFlows: ProviderAuthFlows#
  BUILT_IN_MODEL_PROVIDERS: BUILT_IN_MODEL_PROVIDERS.
  ProviderLoginOptions: ProviderLoginOptions#
  ProviderAuthFlowsHost: ProviderAuthFlowsHost#
  ProviderAuthFlowsHost.getAvailableModels: ProviderAuthFlowsHost#getAvailableModels().
  ANTHROPIC_SUBSCRIPTION_AUTH_WARNING: ANTHROPIC_SUBSCRIPTION_AUTH_WARNING.
  ProviderAuthFlowsHost.onLoginCompleted: ProviderAuthFlowsHost#onLoginCompleted().
  BEDROCK_PROVIDER_ID: BEDROCK_PROVIDER_ID.
  isAnthropicSubscriptionAuthKey: isAnthropicSubscriptionAuthKey().
  ProviderAuthFlowsHost.getAvailableModels.Promise.ReadonlyArray.typeLiteral23.provider: ProviderAuthFlowsHost#getAvailableModels().Promise:ReadonlyArray:typeLiteral23:provider.
  ProviderLoginOptions.authType: ProviderLoginOptions#authType.
  ProviderLoginOptions.initialCategory: ProviderLoginOptions#initialCategory.
---
# Module: [`packages/coding-agent/src/modes/interactive/auth-flows.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts)

## Classes
### `AuthenticationResult`
- def: [`packages/coding-agent/src/modes/interactive/auth-flows.ts:43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L43)
- signature: `type AuthenticationResult`
- used by: [`interactive-mode.ts`](interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`runPrimeInferenceLogin`](auth-flows.ts.md#ProviderAuthFlows.runPrimeInferenceLogin), [`showLoginDialog`](auth-flows.ts.md#ProviderAuthFlows.showLoginDialog), [`runPrimeAgentTracesLogin`](auth-flows.ts.md#ProviderAuthFlows.runPrimeAgentTracesLogin), [`runLogin`](auth-flows.ts.md#ProviderAuthFlows.runLogin), [`prepareForModelSelectionAfterLogin`](interactive-mode.ts.md#InteractiveMode.prepareForModelSelectionAfterLogin), [`showBedrockSetupDialog`](auth-flows.ts.md#ProviderAuthFlows.showBedrockSetupDialog), [`showApiKeyLoginDialog`](auth-flows.ts.md#ProviderAuthFlows.showApiKeyLoginDialog), [`loginProvider`](auth-flows.ts.md#ProviderAuthFlows.loginProvider), [`completePrimeInferenceLogin`](auth-flows.ts.md#ProviderAuthFlows.completePrimeInferenceLogin), [`completeProviderAuthentication`](auth-flows.ts.md#ProviderAuthFlows.completeProviderAuthentication), [`completePrimeAgentTracesLogin`](auth-flows.ts.md#ProviderAuthFlows.completePrimeAgentTracesLogin), [`runMcpLogin`](auth-flows.ts.md#ProviderAuthFlows.runMcpLogin), [`completeExternalProviderSetup`](auth-flows.ts.md#ProviderAuthFlows.completeExternalProviderSetup)  (7 test-only)

### `ProviderAuthFlows`
- def: [`packages/coding-agent/src/modes/interactive/auth-flows.ts:123`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L123)
- signature: `class ProviderAuthFlows`
- members:
  - `<constructor>(host: ProviderAuthFlowsHost)` — [`L124`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L124)
  - `completeExternalProviderSetup(method)` — [`L347`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L347)
  - `completePrimeAgentTracesLogin(method)` — [`L517`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L517)
  - `completePrimeInferenceLogin(method)` — [`L498`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L498)
  - `completeProviderAuthentication(method)` — [`L322`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L322)
  - `getLoginProviderOptions(method)` — [`L247`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L247)
  - `getLogoutProviderOptions(method)` — [`L283`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L283)
  - `getPrimeInferenceDefaultTeamStatus(method)` — [`L434`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L434)
  - `hasAvailableProviderModels(method)` — [`L362`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L362)
  - `loginProvider(method)` — [`L183`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L183)
  - `runLogin(method)` — [`L144`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L144)
  - `runLogout(method)` — [`L199`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L199) — Returns the provider id that was logged out, or null if nothing changed (cancelled / none).
  - `runMcpLogin(method)` — [`L134`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L134) — Run the OAuth login flow for an MCP integration server.
  - `runPrimeAgentTracesLogin(method)` — [`L650`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L650)
  - `runPrimeInferenceLogin(method)` — [`L531`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L531)
  - `selectPrimeInferenceTeam(method)` — [`L463`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L463)
  - `showApiKeyLoginDialog(method)` — [`L756`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L756)
  - `showBedrockSetupDialog(method)` — [`L367`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L367)
  - `showLoginDialog(method)` — [`L826`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L826)
  - `showOAuthLoginSelect(method)` — [`L798`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L798)
  - `showPrimeTeamSelector(method)` — [`L407`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L407)
- uses (calls/refs, reference-scoped): [`provider`](../../../../ai/src/types.ts.md#Model.provider), [`fg`](theme/theme.ts.md#Theme.fg), [`theme`](theme/theme.ts.md#theme), [`requestRender`](../../../../tui/src/tui.ts.md#TUI.requestRender), [`<constructor>`](components/oauth-selector.ts.md#OAuthSelectorComponent.-constructor), [`<constructor>`](components/extension-selector.ts.md#ExtensionSelectorComponent.-constructor), [`type`](../../core/auth-storage.ts.md#ApiKeyCredential.typeLiteral1.type), [`terminal`](../../../../tui/src/tui.ts.md#TUI.terminal), [`PRIME_INFERENCE_PROVIDER_ID`](../../core/prime-inference-auth.ts.md#PRIME_INFERENCE_PROVIDER_ID), [`id`](components/oauth-selector.ts.md#AuthSelectorProvider.typeLiteral0.id), [`loadPrimeCliConfig`](../../core/prime-inference-auth.ts.md#loadPrimeCliConfig), [`<constructor>`](components/login-dialog.ts.md#LoginDialogComponent.-constructor), [`refresh`](../../core/model-registry.ts.md#ModelRegistry.refresh), [`showFullPaneOverlay`](components/centered-overlay.ts.md#showFullPaneOverlay), [`key`](../../core/auth-storage.ts.md#ApiKeyCredential.typeLiteral1.key), [`showAuth`](components/login-dialog.ts.md#LoginDialogComponent.showAuth), [`<constructor>`](components/prime-team-selector.ts.md#PrimeTeamSelectorComponent.-constructor), [`authType`](components/oauth-selector.ts.md#AuthSelectorProvider.typeLiteral0.authType), [`getPrimeInferenceTeamSelection`](../../core/auth-storage.ts.md#AuthStorage.getPrimeInferenceTeamSelection), [`loginPrimeAgentTraces`](../../core/prime-inference-auth.ts.md#loginPrimeAgentTraces), [`setPrimeInferenceApiKey`](../../core/auth-storage.ts.md#AuthStorage.setPrimeInferenceApiKey), [`loginPrimeInference`](../../core/prime-inference-auth.ts.md#loginPrimeInference), [`name`](components/oauth-selector.ts.md#AuthSelectorProvider.typeLiteral0.name), [`showManualInput`](components/login-dialog.ts.md#LoginDialogComponent.showManualInput), [`showPrompt`](components/login-dialog.ts.md#LoginDialogComponent.showPrompt), [`AuthSelectorProvider`](components/oauth-selector.ts.md#AuthSelectorProvider), [`getProviderAuthStatus`](../../core/model-registry.ts.md#ModelRegistry.getProviderAuthStatus), [`PRIME_AGENT_TRACES_PROVIDER_ID`](../../core/prime-inference-auth.ts.md#PRIME_AGENT_TRACES_PROVIDER_ID), [`OverlayHandle`](../../../../tui/src/tui.ts.md#OverlayHandle), [`showProgress`](components/login-dialog.ts.md#LoginDialogComponent.showProgress), [`modelRegistry`](auth-flows.ts.md#ProviderAuthFlowsHost.modelRegistry), [`hide`](../../../../tui/src/tui.ts.md#OverlayHandle.hide), [`source`](../../core/auth-storage.ts.md#AuthStatus.typeLiteral5.source), [`ui`](auth-flows.ts.md#ProviderAuthFlowsHost.ui), [`getAuthStatus`](../../core/auth-storage.ts.md#AuthStorage.getAuthStatus), [`showContinueInfo`](components/login-dialog.ts.md#LoginDialogComponent.showContinueInfo), [`setPrimeInferenceTeamSelection`](../../core/auth-storage.ts.md#AuthStorage.setPrimeInferenceTeamSelection), [`AuthenticationResult`](auth-flows.ts.md#AuthenticationResult), [`id`](../../../../ai/src/utils/oauth/types.ts.md#OAuthProviderInterface.id), [`focus`](../../../../tui/src/tui.ts.md#OverlayHandle.focus)  (+69 more)
- used by: [`interactive-mode.ts`](interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`showConfigurationMenu`](interactive-mode.ts.md#InteractiveMode.showConfigurationMenu), [`handleTracesCommand`](interactive-mode.ts.md#InteractiveMode.handleTracesCommand), [`createAuthFlows`](interactive-mode.ts.md#InteractiveMode.createAuthFlows), [`handleMcpCommand`](interactive-mode.ts.md#InteractiveMode.handleMcpCommand), [`runOnboardingFlow`](interactive-mode.ts.md#InteractiveMode.runOnboardingFlow), [`ensureModelProviderConfigured`](interactive-mode.ts.md#InteractiveMode.ensureModelProviderConfigured), [`handleModelCommand`](interactive-mode.ts.md#InteractiveMode.handleModelCommand), [`showLogoutSelector`](interactive-mode.ts.md#InteractiveMode.showLogoutSelector)  (1 test-only)

### `ProviderAuthFlowsHost`
- def: [`packages/coding-agent/src/modes/interactive/auth-flows.ts:105`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L105)
- signature: `interface ProviderAuthFlowsHost`
- members:
  - `getAvailableModels(method)` — [`L111`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L111) — Models currently visible to the host; used to detect providers configured via external credentials.
  - `onAuthChanged(method)` — [`L113`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L113) — Invoked after stored credentials change so the host can refresh dependent UI.
  - `onLoginCompleted(method)` — [`L115`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L115) — Invoked after a successful login (e.g. to surface billing warnings).
  - `showError(method)` — [`L109`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L109)
  - `showStatus(method)` — [`L108`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L108)
  - `modelRegistry` — [`L107`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L107)
  - `provider` — [`L111`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L111)
  - `ui` — [`L106`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L106)
- uses (calls/refs, reference-scoped): [`ModelRegistry`](../../core/model-registry.ts.md#ModelRegistry), [`TUI`](../../../../tui/src/tui.ts.md#TUI)
- used by: [`runPrimeInferenceLogin`](auth-flows.ts.md#ProviderAuthFlows.runPrimeInferenceLogin), [`showLoginDialog`](auth-flows.ts.md#ProviderAuthFlows.showLoginDialog), [`runPrimeAgentTracesLogin`](auth-flows.ts.md#ProviderAuthFlows.runPrimeAgentTracesLogin), [`createAuthFlows`](interactive-mode.ts.md#InteractiveMode.createAuthFlows), [`runLogout`](auth-flows.ts.md#ProviderAuthFlows.runLogout), [`getLogoutProviderOptions`](auth-flows.ts.md#ProviderAuthFlows.getLogoutProviderOptions), [`runLogin`](auth-flows.ts.md#ProviderAuthFlows.runLogin), [`selectPrimeInferenceTeam`](auth-flows.ts.md#ProviderAuthFlows.selectPrimeInferenceTeam), [`getLoginProviderOptions`](auth-flows.ts.md#ProviderAuthFlows.getLoginProviderOptions), [`showOAuthLoginSelect`](auth-flows.ts.md#ProviderAuthFlows.showOAuthLoginSelect), [`showBedrockSetupDialog`](auth-flows.ts.md#ProviderAuthFlows.showBedrockSetupDialog), [`showApiKeyLoginDialog`](auth-flows.ts.md#ProviderAuthFlows.showApiKeyLoginDialog), [`completePrimeInferenceLogin`](auth-flows.ts.md#ProviderAuthFlows.completePrimeInferenceLogin), [`showPrimeTeamSelector`](auth-flows.ts.md#ProviderAuthFlows.showPrimeTeamSelector), [`getPrimeInferenceDefaultTeamStatus`](auth-flows.ts.md#ProviderAuthFlows.getPrimeInferenceDefaultTeamStatus), [`completeProviderAuthentication`](auth-flows.ts.md#ProviderAuthFlows.completeProviderAuthentication), [`completePrimeAgentTracesLogin`](auth-flows.ts.md#ProviderAuthFlows.completePrimeAgentTracesLogin), [`runMcpLogin`](auth-flows.ts.md#ProviderAuthFlows.runMcpLogin), [`completeExternalProviderSetup`](auth-flows.ts.md#ProviderAuthFlows.completeExternalProviderSetup), [`<constructor>`](auth-flows.ts.md#ProviderAuthFlows.-constructor), [`hasAvailableProviderModels`](auth-flows.ts.md#ProviderAuthFlows.hasAvailableProviderModels)  (3 test-only)

### `ProviderLoginOptions`
- def: [`packages/coding-agent/src/modes/interactive/auth-flows.ts:118`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L118)
- signature: `interface ProviderLoginOptions`
- members:
  - `authType` — [`L119`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L119)
  - `initialCategory` — [`L120`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L120)
- uses (calls/refs, reference-scoped): [`AuthSelectorCategory`](components/oauth-selector.ts.md#AuthSelectorCategory)
- used by: [`runLogin`](auth-flows.ts.md#ProviderAuthFlows.runLogin)

## Functions
- `getAnthropicSubscriptionAuthWarning(modelRegistry: ModelRegistry, model: { provider: string; } | undefined)` — [`L65`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L65) — Returns the extra-usage warning when the given model would run on Anthropic subscription auth.
- `isAnthropicSubscriptionAuthKey(apiKey: string | undefined)` — [`L60`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L60)
- `isApiKeyLoginProvider(providerId: string, oauthProviderIds: ReadonlySet<string>, builtInProviderIds?: ReadonlySet<string>)` — [`L91`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L91)

## Module values
- `ANTHROPIC_SUBSCRIPTION_AUTH_WARNING` — [`L57`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L57)
- `BEDROCK_PROVIDER_ID` — [`L55`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L55)
- `BUILT_IN_MODEL_PROVIDERS` — [`L89`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/auth-flows.ts#L89)


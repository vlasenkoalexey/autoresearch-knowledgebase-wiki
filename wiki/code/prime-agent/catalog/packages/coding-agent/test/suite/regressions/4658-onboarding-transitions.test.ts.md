---
title: 'Module: packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/regressions/`4658-onboarding-transitions.test.ts`/
symbols:
  deferred: deferred().
  ConfigurationHarness.uiServices.typeLiteral2.settingsManager: ConfigurationHarness#uiServices.typeLiteral2:settingsManager.
  ConfigurationHarness.showFullPaneOverlay: ConfigurationHarness#showFullPaneOverlay().
  InteractiveOnboardingHarness.showOnboardingSplash: InteractiveOnboardingHarness#showOnboardingSplash().
  InteractiveOnboardingHarness.uiServices.typeLiteral0.modelRegistry: InteractiveOnboardingHarness#uiServices.typeLiteral0:modelRegistry.
  InteractiveOnboardingHarness.getModelCandidates: InteractiveOnboardingHarness#getModelCandidates().
  InteractiveOnboardingHarness.prepareForModelSelectionAfterLogin: InteractiveOnboardingHarness#prepareForModelSelectionAfterLogin().
  ConfigurationHarness.ui: ConfigurationHarness#ui.
  ConfigurationHarness.uiServices.typeLiteral2.modelRegistry: ConfigurationHarness#uiServices.typeLiteral2:modelRegistry.
  ConfigurationHarness.getCachedModelCandidates: ConfigurationHarness#getCachedModelCandidates().
  ConfigurationHarness.getCurrentModel: ConfigurationHarness#getCurrentModel().
  ConfigurationHarness.createAuthFlows.typeLiteral3.loginProvider: ConfigurationHarness#createAuthFlows().typeLiteral3:loginProvider().
  deferred.typeLiteral5.promise: deferred().typeLiteral5:promise.
  deferred.typeLiteral5.resolve: deferred().typeLiteral5:resolve().
  InteractiveOnboardingHarness.createAuthFlows.typeLiteral1.runPrimeInferenceLogin: InteractiveOnboardingHarness#createAuthFlows().typeLiteral1:runPrimeInferenceLogin().
  OnboardingSplashHandle: OnboardingSplashHandle#
  InteractiveOnboardingHarness.showConfigurationMenu: InteractiveOnboardingHarness#showConfigurationMenu().
  OnboardingSplashHandle.showProgress: OnboardingSplashHandle#showProgress().
  OnboardingSplashHandle.dismiss: OnboardingSplashHandle#dismiss().
  InteractiveOnboardingHarness: InteractiveOnboardingHarness#
  InteractiveOnboardingHarness.runOnboardingFlow: InteractiveOnboardingHarness#runOnboardingFlow().
  InteractiveOnboardingHarness.uiServices: InteractiveOnboardingHarness#uiServices.
  InteractiveOnboardingHarness.createAuthFlows: InteractiveOnboardingHarness#createAuthFlows().
  ConfigurationHarness: ConfigurationHarness#
  ConfigurationHarness.showConfigurationMenu: ConfigurationHarness#showConfigurationMenu().
  ConfigurationHarness.uiServices: ConfigurationHarness#uiServices.
  ConfigurationHarness.getScopedModelState: ConfigurationHarness#getScopedModelState().
  ConfigurationHarness.getModelSelectorRefreshPromise: ConfigurationHarness#getModelSelectorRefreshPromise().
  ConfigurationHarness.createAuthFlows: ConfigurationHarness#createAuthFlows().
  ConfigurationHarness.createAuthFlows.typeLiteral3.getLoginProviderOptions: ConfigurationHarness#createAuthFlows().typeLiteral3:getLoginProviderOptions().
  ConfigurationHarness.createAuthFlows.typeLiteral3.getLoginProviderOptions.Array.typeLiteral4.id: ConfigurationHarness#createAuthFlows().typeLiteral3:getLoginProviderOptions().Array:typeLiteral4:id.
  ConfigurationHarness.createAuthFlows.typeLiteral3.getLoginProviderOptions.Array.typeLiteral4.name: ConfigurationHarness#createAuthFlows().typeLiteral3:getLoginProviderOptions().Array:typeLiteral4:name.
  ConfigurationHarness.createAuthFlows.typeLiteral3.getLoginProviderOptions.Array.typeLiteral4.authType: ConfigurationHarness#createAuthFlows().typeLiteral3:getLoginProviderOptions().Array:typeLiteral4:authType.
  ConfigurationHarness.showError: ConfigurationHarness#showError().
  ConfigurationHarness.showStatus: ConfigurationHarness#showStatus().
---
# Module: [`packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts)

## Classes
### `ConfigurationHarness`
- def: [`packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts:31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L31)
- signature: `interface ConfigurationHarness`
- members:
  - `createAuthFlows(method)` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L42)
  - `getCachedModelCandidates(method)` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L38)
  - `getCurrentModel(method)` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L40)
  - `getLoginProviderOptions(method)` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L43)
  - `getModelSelectorRefreshPromise(method)` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L41)
  - `getScopedModelState(method)` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L39)
  - `loginProvider(method)` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L44)
  - `showConfigurationMenu(method)` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L32)
  - `showError(method)` — [`L47`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L47)
  - `showFullPaneOverlay(method)` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L46)
  - `showStatus(method)` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L48)
  - `authType` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L43)
  - `id` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L43)
  - `modelRegistry` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L35)
  - `name` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L43)
  - `settingsManager` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L36)
  - `ui` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L33)
  - `uiServices` — [`L34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L34)
- uses (calls/refs, reference-scoped): [`Component`](../../../../tui/src/tui.ts.md#Component), [`ModelRegistry`](../../../src/core/model-registry.ts.md#ModelRegistry), [`TUI`](../../../../tui/src/tui.ts.md#TUI), [`AgentConnectionModel`](../../../src/modes/agent-connection/types.ts.md#AgentConnectionModel), [`OverlayHandle`](../../../../tui/src/tui.ts.md#OverlayHandle), [`AuthenticationResult`](../../../src/modes/interactive/auth-flows.ts.md#AuthenticationResult)  (2 test-only)
- used by: (1 test-only callers)

### `InteractiveOnboardingHarness`
- def: [`packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts:17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L17)
- signature: `interface InteractiveOnboardingHarness`
- members:
  - `createAuthFlows(method)` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L24)
  - `getModelCandidates(method)` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L22)
  - `prepareForModelSelectionAfterLogin(method)` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L27)
  - `runOnboardingFlow(method)` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L18)
  - `runPrimeInferenceLogin(method)` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L25)
  - `showConfigurationMenu(method)` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L28)
  - `showOnboardingSplash(method)` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L23)
  - `modelRegistry` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L20)
  - `uiServices` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L19)
- uses (calls/refs, reference-scoped): [`ModelRegistry`](../../../src/core/model-registry.ts.md#ModelRegistry), [`AgentConnectionModel`](../../../src/modes/agent-connection/types.ts.md#AgentConnectionModel), [`AuthenticationResult`](../../../src/modes/interactive/auth-flows.ts.md#AuthenticationResult)  (1 test-only)
- used by: (1 test-only callers)

### `OnboardingSplashHandle`
- def: [`packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts:12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L12)
- signature: `interface OnboardingSplashHandle`
- members:
  - `dismiss(method)` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L14)
  - `showProgress(method)` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L13)
- used by: (2 test-only callers)

## Functions
- `deferred()` — [`L51`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L51)
- `resolve(method)` — [`L51`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L51)

## Module values
- `promise` — [`L51`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4658-onboarding-transitions.test.ts#L51)


---
title: 'Module: packages/coding-agent/src/modes/interactive/onboarding.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/onboarding.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/`onboarding.ts`/
symbols:
  shouldRunOnboarding: shouldRunOnboarding().
  shouldRunPrimeCliOnboardingSplash: shouldRunPrimeCliOnboardingSplash().
  OnboardingStartupState.model: OnboardingStartupState#model.
  isOnboardingModelReady: isOnboardingModelReady().
  OnboardingStartupState.modelRegistry: OnboardingStartupState#modelRegistry.
  OnboardingStartupState.settingsManager: OnboardingStartupState#settingsManager.
  OnboardingModelRegistryReader.hasConfiguredAuth: OnboardingModelRegistryReader#hasConfiguredAuth().
  OnboardingStartupState: OnboardingStartupState#
  OnboardingModelRegistryReader.getProviderAuthStatus: OnboardingModelRegistryReader#getProviderAuthStatus().
  OnboardingSettingsReader.getOnboardingShown: OnboardingSettingsReader#getOnboardingShown().
  OnboardingModelRegistryReader.refresh: OnboardingModelRegistryReader#refresh().
  OnboardingSettingsReader: OnboardingSettingsReader#
  OnboardingModelRegistryReader: OnboardingModelRegistryReader#
---
# Module: [`packages/coding-agent/src/modes/interactive/onboarding.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/onboarding.ts)

## Classes
### `OnboardingModelRegistryReader`
- def: [`packages/coding-agent/src/modes/interactive/onboarding.ts:9`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/onboarding.ts#L9)
- signature: `interface OnboardingModelRegistryReader`
- members:
  - `getProviderAuthStatus(method)` — [`L12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/onboarding.ts#L12)
  - `hasConfiguredAuth(method)` — [`L11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/onboarding.ts#L11)
  - `refresh(method)` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/onboarding.ts#L10)
- uses (calls/refs, reference-scoped): [`Model`](../../../../ai/src/types.ts.md#Model), [`Api`](../../../../ai/src/types.ts.md#Api), [`AuthStatus`](../../core/auth-storage.ts.md#AuthStatus)
- used by: [`shouldRunOnboarding`](onboarding.ts.md#shouldRunOnboarding), [`shouldRunPrimeCliOnboardingSplash`](onboarding.ts.md#shouldRunPrimeCliOnboardingSplash), [`isOnboardingModelReady`](onboarding.ts.md#isOnboardingModelReady), [`modelRegistry`](onboarding.ts.md#OnboardingStartupState.modelRegistry)  (1 test-only)

### `OnboardingSettingsReader`
- def: [`packages/coding-agent/src/modes/interactive/onboarding.ts:5`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/onboarding.ts#L5)
- signature: `interface OnboardingSettingsReader`
- members:
  - `getOnboardingShown(method)` — [`L6`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/onboarding.ts#L6)
- used by: [`shouldRunOnboarding`](onboarding.ts.md#shouldRunOnboarding), [`shouldRunPrimeCliOnboardingSplash`](onboarding.ts.md#shouldRunPrimeCliOnboardingSplash), [`settingsManager`](onboarding.ts.md#OnboardingStartupState.settingsManager)  (1 test-only)

### `OnboardingStartupState`
- def: [`packages/coding-agent/src/modes/interactive/onboarding.ts:15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/onboarding.ts#L15)
- signature: `interface OnboardingStartupState`
- members:
  - `model` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/onboarding.ts#L18)
  - `modelRegistry` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/onboarding.ts#L17)
  - `settingsManager` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/onboarding.ts#L16)
- uses (calls/refs, reference-scoped): [`Model`](../../../../ai/src/types.ts.md#Model), [`Api`](../../../../ai/src/types.ts.md#Api), [`OnboardingModelRegistryReader`](onboarding.ts.md#OnboardingModelRegistryReader), [`OnboardingSettingsReader`](onboarding.ts.md#OnboardingSettingsReader)
- used by: [`interactive-mode.ts`](interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`main`](../../main.ts.md#main), [`shouldRunOnboarding`](onboarding.ts.md#shouldRunOnboarding), [`shouldRunPrimeCliOnboardingSplash`](onboarding.ts.md#shouldRunPrimeCliOnboardingSplash), [`getOnboardingState`](interactive-mode.ts.md#InteractiveMode.getOnboardingState), [`isOnboardingModelReady`](onboarding.ts.md#isOnboardingModelReady)  (3 test-only)

## Functions
- `isOnboardingModelReady(state: OnboardingStartupState)` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/onboarding.ts#L32)
- `shouldRunOnboarding(state: OnboardingStartupState)` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/onboarding.ts#L36)
- `shouldRunPrimeCliOnboardingSplash(state: OnboardingStartupState)` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/onboarding.ts#L21)


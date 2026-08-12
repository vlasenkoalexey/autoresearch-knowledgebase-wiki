---
title: 'Module: packages/coding-agent/src/modes/interactive/components/login-dialog.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/login-dialog.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`login-dialog.ts`/
symbols:
  LoginDialogComponent.-constructor: LoginDialogComponent#`<constructor>`().
  LoginDialogComponent.showAuth: LoginDialogComponent#showAuth().
  LoginDialogComponent.showManualInput: LoginDialogComponent#showManualInput().
  LoginDialogComponent.showPrompt: LoginDialogComponent#showPrompt().
  LoginDialogComponent.handleInput: LoginDialogComponent#handleInput().
  LoginDialogComponent.contentContainer: LoginDialogComponent#contentContainer.
  LoginDialogComponent.showProgress: LoginDialogComponent#showProgress().
  LoginDialogComponent.showContinueInfo: LoginDialogComponent#showContinueInfo().
  LoginDialogComponent.startContent: LoginDialogComponent#startContent().
  LoginDialogComponent.showInfo: LoginDialogComponent#showInfo().
  LoginDialogComponent.getAuthActionsText: LoginDialogComponent#getAuthActionsText().
  LoginDialogComponent.showWaiting: LoginDialogComponent#showWaiting().
  PrimeLoginHeader.render: PrimeLoginHeader#render().
  LoginDialogComponent.-get-signal: LoginDialogComponent#`<get>signal`().
  LoginDialogComponent.addSectionTitle: LoginDialogComponent#addSectionTitle().
  LoginDialogComponent.addInstructions: LoginDialogComponent#addInstructions().
  LoginDialogComponent.copyAuthUrl: LoginDialogComponent#copyAuthUrl().
  LoginDialogComponent.addSectionSpacer: LoginDialogComponent#addSectionSpacer().
  LoginDialogComponent.addLabel: LoginDialogComponent#addLabel().
  LoginDialogComponent.addMutedText: LoginDialogComponent#addMutedText().
  LoginDialogComponent.cancel: LoginDialogComponent#cancel().
  LoginDialogComponent.tui: LoginDialogComponent#tui.
  LoginDialogComponent.input: LoginDialogComponent#input.
  LoginDialogComponent: LoginDialogComponent#
  LoginDialogComponent.authActions: LoginDialogComponent#authActions.
  LoginDialogComponent.-set-focused: LoginDialogComponent#`<set>focused`().
  LoginDialogComponent.waitForInput: LoginDialogComponent#waitForInput().
  centeredLine: centeredLine().
  PRIME_LOGO_WIDTH: PRIME_LOGO_WIDTH.
  LoginDialogComponent.inputVisible: LoginDialogComponent#inputVisible.
  LoginDialogComponent.authUrl: LoginDialogComponent#authUrl.
  LoginDialogComponent.inputResolver: LoginDialogComponent#inputResolver.
  LoginDialogComponent.inputRejecter: LoginDialogComponent#inputRejecter.
  LoginDialogComponent.continueResolver: LoginDialogComponent#continueResolver.
  LoginDialogComponent.continueRejecter: LoginDialogComponent#continueRejecter.
  PRIME_LOGO_LINES: PRIME_LOGO_LINES.
  LoginDialogComponent.isPrimeInference: LoginDialogComponent#isPrimeInference.
  PrimeLoginHeader: PrimeLoginHeader#
  LoginDialogComponent.-get-focused: LoginDialogComponent#`<get>focused`().
  LoginDialogComponent.abortController: LoginDialogComponent#abortController.
  LoginDialogComponent._focused: LoginDialogComponent#_focused.
  PRIME_INFERENCE_PROVIDER_ID: PRIME_INFERENCE_PROVIDER_ID.
  isTextEntryKeybinding: isTextEntryKeybinding().
  isPrintableInput: isPrintableInput().
  PrimeLoginHeader.invalidate: PrimeLoginHeader#invalidate().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/login-dialog.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts)

## Classes
### `LoginDialogComponent`  ·  implements/extends Component, Container, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/login-dialog.ts:72`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L72)
- doc: Login dialog component - replaces editor during OAuth login flow
- signature: `class LoginDialogComponent`
- members:
  - `<constructor>(tui: TUI, providerId: string, onComplete: (success: boolean, message?: string | undefined) => void, providerNameOverride?: string | undefined, titleOverride?: string | undefined)` — [`L99`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L99) — Login dialog component - replaces editor during OAuth login flow
  - `<get>focused` — [`L91`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L91) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `<get>signal` — [`L135`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L135)
  - `<set>focused` — [`L94`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L94) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `addInstructions(method)` — [`L323`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L323)
  - `addLabel(method)` — [`L338`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L338)
  - `addMutedText(method)` — [`L342`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L342)
  - `addSectionSpacer(method)` — [`L315`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L315)
  - `addSectionTitle(method)` — [`L334`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L334)
  - `cancel(method)` — [`L139`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L139)
  - `copyAuthUrl(method)` — [`L367`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L367)
  - `getAuthActionsText(method)` — [`L346`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L346)
  - `handleInput(method)` — [`L386`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L386)
  - `showAuth(method)` — [`L157`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L157) — Called by onAuth callback - show URL and optional instructions
  - `showContinueInfo(method)` — [`L255`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L255)
  - `showInfo(method)` — [`L245`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L245) — Show informational text without prompting for input.
  - `showManualInput(method)` — [`L193`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L193) — Show input for manual code/URL entry (for callback server providers)
  - `showProgress(method)` — [`L292`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L292) — Called by onProgress callback
  - `showPrompt(method)` — [`L220`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L220) — Called by onPrompt callback - show prompt and wait for input
  - `showWaiting(method)` — [`L282`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L282) — Show waiting message (for polling flows like GitHub Copilot)
  - `startContent(method)` — [`L301`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L301)
  - `waitForInput(method)` — [`L209`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L209) — Wait for the next submission of the already-visible input.
  - `abortController` — [`L77`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L77)
  - `authActions` — [`L87`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L87)
  - `authUrl` — [`L86`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L86)
  - `contentContainer` — [`L73`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L73)
  - `continueRejecter` — [`L85`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L85)
  - `continueResolver` — [`L84`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L84)
  - `input` — [`L74`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L74)
  - `inputRejecter` — [`L79`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L79)
  - `inputResolver` — [`L78`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L78)
  - `inputVisible` — [`L83`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L83)
  - `isPrimeInference` — [`L76`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L76)
  - `tui` — [`L75`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L75)
- protocol/private: `_focused`[`L90`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L90)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`requestRender`](../../../../../tui/src/tui.ts.md#TUI.requestRender), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`TUI`](../../../../../tui/src/tui.ts.md#TUI), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`children`](../../../../../tui/src/tui.ts.md#Container.children), [`bold`](../theme/theme.ts.md#Theme.bold), [`Text`](../../../../../tui/src/components/text.ts.md#Text), [`clear`](../../../../../tui/src/tui.ts.md#Container.clear), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`keyHint`](keybinding-hints.ts.md#keyHint), [`hyperlinks`](../../../../../tui/src/terminal-image.ts.md#TerminalCapabilities.hyperlinks), [`copyToClipboard`](../../../utils/clipboard.ts.md#copyToClipboard), [`id`](../../../../../ai/src/utils/oauth/types.ts.md#OAuthProviderInterface.id), [`getKeys`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.getKeys), [`setText`](../../../../../tui/src/components/text.ts.md#Text.setText), [`formatKeyText`](keybinding-hints.ts.md#formatKeyText), [`getCapabilities`](../../../../../tui/src/terminal-image.ts.md#getCapabilities), [`name`](../../../../../ai/src/utils/oauth/types.ts.md#OAuthProviderInterface.name), [`MenuSearchInput`](menu-panel.ts.md#MenuSearchInput), [`<constructor>`](menu-panel.ts.md#MenuPanel.-constructor), [`getValue`](menu-panel.ts.md#MenuSearchInput.getValue), [`shouldTreatAsBack`](modal-back.ts.md#shouldTreatAsBack), [`getOAuthProviders`](../../../../../ai/src/utils/oauth/index.ts.md#getOAuthProviders), [`title`](menu-panel.ts.md#MenuPanelOptions.title), [`<get>focused`](menu-panel.ts.md#MenuSearchInput.-get-focused), [`<set>focused`](menu-panel.ts.md#MenuSearchInput.-set-focused), [`handleInput`](menu-panel.ts.md#MenuSearchInput.handleInput), [`subtitle`](menu-panel.ts.md#MenuPanelOptions.subtitle), [`<set>onSubmit`](menu-panel.ts.md#MenuSearchInput.-set-onSubmit), [`setValue`](menu-panel.ts.md#MenuSearchInput.setValue), [`<constructor>`](menu-panel.ts.md#MenuSearchInput.-constructor), [`PrimeLoginHeader`](login-dialog.ts.md#PrimeLoginHeader), [`PRIME_INFERENCE_PROVIDER_ID`](login-dialog.ts.md#PRIME_INFERENCE_PROVIDER_ID), [`isPrintableInput`](login-dialog.ts.md#isPrintableInput)  (+1 more)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`auth-flows.ts`](../auth-flows.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-auth-flows.ts), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`runPrimeInferenceLogin`](../auth-flows.ts.md#ProviderAuthFlows.runPrimeInferenceLogin), [`showLoginDialog`](../auth-flows.ts.md#ProviderAuthFlows.showLoginDialog), [`runPrimeAgentTracesLogin`](../auth-flows.ts.md#ProviderAuthFlows.runPrimeAgentTracesLogin), [`selectPrimeInferenceTeam`](../auth-flows.ts.md#ProviderAuthFlows.selectPrimeInferenceTeam), [`showBedrockSetupDialog`](../auth-flows.ts.md#ProviderAuthFlows.showBedrockSetupDialog), [`showApiKeyLoginDialog`](../auth-flows.ts.md#ProviderAuthFlows.showApiKeyLoginDialog), [`completePrimeInferenceLogin`](../auth-flows.ts.md#ProviderAuthFlows.completePrimeInferenceLogin)  (1 test-only)

### `PrimeLoginHeader`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/login-dialog.ts:45`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L45)
- signature: `class PrimeLoginHeader`
- members:
  - `invalidate(method)` — [`L46`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L46) — Invalidate any cached rendering state.
  - `render(method)` — [`L50`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L50) — Render the component to lines for the given viewport width
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`bold`](../theme/theme.ts.md#Theme.bold), [`centeredLine`](login-dialog.ts.md#centeredLine), [`PRIME_LOGO_WIDTH`](login-dialog.ts.md#PRIME_LOGO_WIDTH), [`PRIME_LOGO_LINES`](login-dialog.ts.md#PRIME_LOGO_LINES)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`startContent`](login-dialog.ts.md#LoginDialogComponent.startContent)

## Functions
- `centeredLine(text: string, width: number)` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L27)
- `isPrintableInput(data: string)` — [`L41`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L41)
- `isTextEntryKeybinding(key: string)` — [`L35`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L35)

## Module values
- `PRIME_INFERENCE_PROVIDER_ID` — [`L23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L23)
- `PRIME_LOGO_LINES` — [`L24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L24)
- `PRIME_LOGO_WIDTH` — [`L25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/login-dialog.ts#L25)


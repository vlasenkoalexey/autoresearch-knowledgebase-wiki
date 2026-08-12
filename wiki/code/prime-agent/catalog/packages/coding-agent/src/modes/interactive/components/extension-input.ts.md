---
title: 'Module: packages/coding-agent/src/modes/interactive/components/extension-input.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/extension-input.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`extension-input.ts`/ExtensionInput
symbols:
  ExtensionInputComponent.-constructor: Component#`<constructor>`().
  ExtensionInputComponent.handleInput: Component#handleInput().
  ExtensionInputComponent: Component#
  ExtensionInputComponent.input: Component#input.
  ExtensionInputComponent.-set-focused: Component#`<set>focused`().
  ExtensionInputComponent.dispose: Component#dispose().
  ExtensionInputComponent.titleText: Component#titleText.
  ExtensionInputOptions.tui: Options#tui.
  ExtensionInputComponent.countdown: Component#countdown.
  ExtensionInputOptions.timeout: Options#timeout.
  ExtensionInputComponent.onCancelCallback: Component#onCancelCallback.
  ExtensionInputComponent.-get-focused: Component#`<get>focused`().
  ExtensionInputComponent.onSubmitCallback: Component#onSubmitCallback.
  ExtensionInputComponent.baseTitle: Component#baseTitle.
  ExtensionInputComponent._focused: Component#_focused.
  ExtensionInputOptions: Options#
---
# Module: [`packages/coding-agent/src/modes/interactive/components/extension-input.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts)

## Classes
### `ExtensionInputComponent`  ·  implements/extends Component, Container, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/extension-input.ts:16`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L16)
- signature: `class ExtensionInputComponent`
- members:
  - `<constructor>(title: string, _placeholder: string | undefined, onSubmit: (value: string) => void, onCancel: () => void, opts?: ExtensionInputOptions | undefined)` — [`L34`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L34)
  - `<get>focused` — [`L26`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L26) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `<set>focused` — [`L29`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L29) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `dispose(method)` — [`L84`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L84)
  - `handleInput(method)` — [`L73`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L73)
  - `baseTitle` — [`L21`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L21)
  - `countdown` — [`L22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L22)
  - `input` — [`L17`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L17)
  - `onCancelCallback` — [`L19`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L19)
  - `onSubmitCallback` — [`L18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L18)
  - `titleText` — [`L20`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L20)
- protocol/private: `_focused`[`L25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L25)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`handleInput`](../../../../../tui/src/components/input.ts.md#Input.handleInput), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`getValue`](../../../../../tui/src/components/input.ts.md#Input.getValue), [`Text`](../../../../../tui/src/components/text.ts.md#Text), [`Input`](../../../../../tui/src/components/input.ts.md#Input), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`keyHint`](keybinding-hints.ts.md#keyHint), [`<constructor>`](dynamic-border.ts.md#DynamicBorder.-constructor), [`setText`](../../../../../tui/src/components/text.ts.md#Text.setText), [`<constructor>`](countdown-timer.ts.md#CountdownTimer.-constructor), [`focused`](../../../../../tui/src/components/input.ts.md#Input.focused), [`dispose`](countdown-timer.ts.md#CountdownTimer.dispose), [`CountdownTimer`](countdown-timer.ts.md#CountdownTimer), [`tui`](extension-input.ts.md#ExtensionInputOptions.tui), [`timeout`](extension-input.ts.md#ExtensionInputOptions.timeout), [`ExtensionInputOptions`](extension-input.ts.md#ExtensionInputOptions)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`showExtensionInput`](../interactive-mode.ts.md#InteractiveMode.showExtensionInput), [`hideExtensionInput`](../interactive-mode.ts.md#InteractiveMode.hideExtensionInput), [`extensionInput`](../interactive-mode.ts.md#InteractiveMode.extensionInput)

### `ExtensionInputOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/extension-input.ts:11`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L11)
- signature: `interface ExtensionInputOptions`
- members:
  - `timeout` — [`L13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L13)
  - `tui` — [`L12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-input.ts#L12)
- uses (calls/refs, reference-scoped): [`TUI`](../../../../../tui/src/tui.ts.md#TUI)
- used by: [`<constructor>`](extension-input.ts.md#ExtensionInputComponent.-constructor)


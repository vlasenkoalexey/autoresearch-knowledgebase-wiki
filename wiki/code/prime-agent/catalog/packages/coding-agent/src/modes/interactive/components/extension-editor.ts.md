---
title: 'Module: packages/coding-agent/src/modes/interactive/components/extension-editor.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/extension-editor.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`extension-editor.ts`/ExtensionEditorComponent#
symbols:
  ExtensionEditorComponent.-constructor: '`<constructor>`().'
  ExtensionEditorComponent.openExternalEditor: openExternalEditor().
  ExtensionEditorComponent.handleInput: handleInput().
  ExtensionEditorComponent.editor: editor.
  ExtensionEditorComponent: ''
  ExtensionEditorComponent.-set-focused: '`<set>focused`().'
  ExtensionEditorComponent.tui: tui.
  ExtensionEditorComponent.keybindings: keybindings.
  ExtensionEditorComponent.-get-focused: '`<get>focused`().'
  ExtensionEditorComponent.onSubmitCallback: onSubmitCallback.
  ExtensionEditorComponent.onCancelCallback: onCancelCallback.
  ExtensionEditorComponent._focused: _focused.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/extension-editor.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-editor.ts)

## Classes
### `ExtensionEditorComponent`  ·  implements/extends Component, Container, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/extension-editor.ts:25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-editor.ts#L25)
- signature: `class ExtensionEditorComponent`
- members:
  - `<constructor>(tui: TUI, keybindings: KeybindingsManager, title: string, prefill: string | undefined, onSubmit: (value: string) => void, onCancel: () => void, options?: EditorOptions | undefined)` — [`L41`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-editor.ts#L41)
  - `<get>focused` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-editor.ts#L33) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `<set>focused` — [`L36`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-editor.ts#L36) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `handleInput(method)` — [`L95`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-editor.ts#L95)
  - `openExternalEditor(method)` — [`L113`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-editor.ts#L113)
  - `editor` — [`L26`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-editor.ts#L26)
  - `keybindings` — [`L30`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-editor.ts#L30)
  - `onCancelCallback` — [`L28`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-editor.ts#L28)
  - `onSubmitCallback` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-editor.ts#L27)
  - `tui` — [`L29`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-editor.ts#L29)
- protocol/private: `_focused`[`L32`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-editor.ts#L32)
- uses (calls/refs, reference-scoped): [`handleInput`](../../../../../tui/src/components/editor.ts.md#Editor.handleInput), [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`requestRender`](../../../../../tui/src/tui.ts.md#TUI.requestRender), [`getText`](../../../../../tui/src/components/editor.ts.md#Editor.getText), [`<constructor>`](../../../../../tui/src/components/editor.ts.md#Editor.-constructor), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`stop`](../../../../../tui/src/tui.ts.md#TUI.stop), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`TUI`](../../../../../tui/src/tui.ts.md#TUI), [`setText`](../../../../../tui/src/components/editor.ts.md#Editor.setText), [`start`](../../../../../tui/src/tui.ts.md#TUI.start), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`KeybindingsManager`](../../../core/keybindings.ts.md#KeybindingsManager), [`keyHint`](keybinding-hints.ts.md#keyHint), [`getEditorTheme`](../theme/theme.ts.md#getEditorTheme), [`<constructor>`](dynamic-border.ts.md#DynamicBorder.-constructor), [`Editor`](../../../../../tui/src/components/editor.ts.md#Editor), [`onSubmit`](../../../../../tui/src/components/editor.ts.md#Editor.onSubmit), [`focused`](../../../../../tui/src/components/editor.ts.md#Editor.focused), [`EditorOptions`](../../../../../tui/src/components/editor.ts.md#EditorOptions)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`showExtensionEditor`](../interactive-mode.ts.md#InteractiveMode.showExtensionEditor), [`extensionEditor`](../interactive-mode.ts.md#InteractiveMode.extensionEditor)


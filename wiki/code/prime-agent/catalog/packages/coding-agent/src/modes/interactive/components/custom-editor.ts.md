---
title: 'Module: packages/coding-agent/src/modes/interactive/components/custom-editor.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/custom-editor.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`custom-editor.ts`/CustomEditor
symbols:
  CustomEditor.handleInput: '#handleInput().'
  CustomEditor.-constructor: '#`<constructor>`().'
  CustomEditor.render: '#render().'
  CustomEditor.renderPlaceholderLine: '#renderPlaceholderLine().'
  CustomEditor.onAction: '#onAction().'
  CustomEditor: '#'
  CustomEditor.renderHeaderContentLine: '#renderHeaderContentLine().'
  CustomEditor.isCursorAtEnd: '#isCursorAtEnd().'
  CustomEditor.keybindings: '#keybindings.'
  CustomEditor.getPromptPrefix: '#getPromptPrefix().'
  CustomEditor.splitRepeatedKeybinding: '#splitRepeatedKeybinding().'
  CustomEditor.onEscape: '#onEscape.'
  CustomEditor.getHeaderLine: '#getHeaderLine.'
  CustomEditor.setPlaceholder: '#setPlaceholder().'
  CustomEditor.actionHandlers: '#actionHandlers.'
  CustomEditor.getEffectivePaddingX: '#getEffectivePaddingX().'
  CustomEditor.styleDisplayText: '#styleDisplayText().'
  CustomEditor.placeholder: '#placeholder.'
  CustomEditor.onCtrlD: '#onCtrlD.'
  CustomEditor.onAgentsBack: '#onAgentsBack.'
  CustomEditor.onExtensionShortcut: '#onExtensionShortcut.'
  CustomEditorOptions: Options#
  CustomEditor.formatPromptPrefix: '#formatPromptPrefix().'
  CustomEditor.onPasteImage: '#onPasteImage.'
  CustomEditor.onMoveBelowPrompt: '#onMoveBelowPrompt.'
  CustomEditor.getHiddenTextPrefixLength: '#getHiddenTextPrefixLength().'
  CustomEditor.defaultPromptPrefix: '#defaultPromptPrefix.'
  CustomEditor.configuredPaddingX: '#configuredPaddingX.'
  CustomEditor.placeholderColor: '#placeholderColor.'
  CustomEditor.isArgumentCommand: '#isArgumentCommand.'
  CustomEditor.getBashPromptInfo: '#getBashPromptInfo().'
  CustomEditorOptions.placeholder: Options#placeholder.
  CustomEditorOptions.placeholderColor: Options#placeholderColor.
  CustomEditorOptions.isArgumentCommand: Options#isArgumentCommand.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/custom-editor.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts)

## Classes
### `CustomEditor`  ·  implements/extends Component, Editor, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/custom-editor.ts:21`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L21)
- doc: Custom editor that handles app-level keybindings for coding-agent.
- signature: `class CustomEditor`
- members:
  - `<constructor>(tui: TUI, theme: EditorTheme, keybindings: KeybindingsManager, options?: CustomEditorOptions | undefined)` — [`L41`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L41) — Custom editor that handles app-level keybindings for coding-agent.
  - `formatPromptPrefix(method)` — [`L56`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L56)
  - `getBashPromptInfo(method)` — [`L100`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L100)
  - `getEffectivePaddingX(method)` — [`L260`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L260)
  - `getHiddenTextPrefixLength(method)` — [`L60`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L60)
  - `getPromptPrefix(method)` — [`L52`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L52)
  - `handleInput(method)` — [`L147`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L147) — Optional handler for keyboard input when component has focus
  - `isCursorAtEnd(method)` — [`L231`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L231)
  - `onAction(method)` — [`L121`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L121) — Register a handler for an app action.
  - `render(method)` — [`L125`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L125) — Render the component to lines for the given viewport width
  - `renderHeaderContentLine(method)` — [`L268`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L268)
  - `renderPlaceholderLine(method)` — [`L285`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L285)
  - `setPlaceholder(method)` — [`L142`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L142)
  - `splitRepeatedKeybinding(method)` — [`L237`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L237)
  - `styleDisplayText(method)` — [`L67`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L67)
  - `actionHandlers` — [`L28`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L28)
  - `configuredPaddingX` — [`L24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L24)
  - `defaultPromptPrefix` — [`L23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L23)
  - `getHeaderLine` — [`L37`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L37) — When set, the returned line is rendered inside the top of the editor box.
  - `isArgumentCommand` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L27)
  - `keybindings` — [`L22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L22)
  - `onAgentsBack` — [`L35`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L35)
  - `onCtrlD` — [`L32`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L32)
  - `onEscape` — [`L31`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L31)
  - `onExtensionShortcut` — [`L39`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L39) — Handler for extension-registered shortcuts. Returns true if handled.
  - `onMoveBelowPrompt` — [`L34`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L34)
  - `onPasteImage` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L33)
  - `placeholder` — [`L25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L25)
  - `placeholderColor` — [`L26`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L26)
- uses (calls/refs, reference-scoped): [`handleInput`](../../../../../tui/src/components/editor.ts.md#Editor.handleInput), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`getText`](../../../../../tui/src/components/editor.ts.md#Editor.getText), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`TUI`](../../../../../tui/src/tui.ts.md#TUI), [`getCursor`](../../../../../tui/src/components/editor.ts.md#Editor.getCursor), [`render`](../../../../../tui/src/components/editor.ts.md#Editor.render), [`KeybindingsManager`](../../../core/keybindings.ts.md#KeybindingsManager), [`isShowingAutocomplete`](../../../../../tui/src/components/editor.ts.md#Editor.isShowingAutocomplete), [`Editor`](../../../../../tui/src/components/editor.ts.md#Editor), [`CURSOR_MARKER`](../../../../../tui/src/tui.ts.md#CURSOR_MARKER), [`EditorTheme`](../../../../../tui/src/components/editor.ts.md#EditorTheme), [`cancelAutocomplete`](../../../../../tui/src/components/editor.ts.md#Editor.cancelAutocomplete), [`AppKeybinding`](../../../core/keybindings.ts.md#AppKeybinding), [`getLines`](../../../../../tui/src/components/editor.ts.md#Editor.getLines), [`backgroundColor`](../../../../../tui/src/components/editor.ts.md#Editor.backgroundColor), [`borderColor`](../../../../../tui/src/components/editor.ts.md#Editor.borderColor), [`focused`](../../../../../tui/src/components/editor.ts.md#Editor.focused), [`line`](../../../../../tui/src/components/editor.ts.md#Editor.getCursor.typeLiteral469.line), [`getAutocompleteAnchorMarker`](../../../../../tui/src/components/editor.ts.md#Editor.getAutocompleteAnchorMarker), [`col`](../../../../../tui/src/components/editor.ts.md#Editor.getCursor.typeLiteral469.col), [`CustomEditorOptions`](custom-editor.ts.md#CustomEditorOptions), [`isHistoryNavigationActive`](../../../../../tui/src/components/editor.ts.md#Editor.isHistoryNavigationActive), [`invalidate`](../../../../../tui/src/components/editor.ts.md#Editor.invalidate), [`commandColor`](../../../../../tui/src/components/editor.ts.md#Editor.commandColor), [`paddingX`](../../../../../tui/src/components/editor.ts.md#EditorOptions.paddingX), [`promptPrefix`](../../../../../tui/src/components/editor.ts.md#EditorOptions.promptPrefix), [`isArgumentCommand`](custom-editor.ts.md#CustomEditorOptions.isArgumentCommand), [`placeholder`](custom-editor.ts.md#CustomEditorOptions.placeholder), [`placeholderColor`](custom-editor.ts.md#CustomEditorOptions.placeholderColor)  (6 test-only)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`handleInput`](../../../../../tui/src/components/editor.ts.md#Editor.handleInput), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`agents-view-mode.ts`](../../agents-view/agents-view-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agents-view-agents-view-mode.ts), [`<constructor>`](../../agents-view/agents-view-mode.ts.md#AgentsViewMode.-constructor), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`<constructor>`](../interactive-mode.ts.md#InteractiveMode.-constructor), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`render`](../../../../../tui/src/components/editor.ts.md#Editor.render), [`setupExtensionShortcuts`](../interactive-mode.ts.md#InteractiveMode.setupExtensionShortcuts), [`setupKeyHandlers`](../interactive-mode.ts.md#InteractiveMode.setupKeyHandlers), [`setCustomEditorComponent`](../interactive-mode.ts.md#InteractiveMode.setCustomEditorComponent), [`resetExtensionUI`](../interactive-mode.ts.md#InteractiveMode.resetExtensionUI), [`setReplyTarget`](../../agents-view/agents-view-mode.ts.md#AgentsViewMode.setReplyTarget), [`defaultEditor`](../interactive-mode.ts.md#InteractiveMode.defaultEditor), [`handleInput`](../../agents-view/agents-view-mode.ts.md#AgentsViewMode.handleInput), [`enterRenameMode`](../../agents-view/agents-view-mode.ts.md#AgentsViewMode.enterRenameMode), [`editor`](../../agents-view/agents-view-mode.ts.md#AgentsViewMode.editor), [`Editor`](../../../../../tui/src/components/editor.ts.md#Editor), [`exitRenameMode`](../../agents-view/agents-view-mode.ts.md#AgentsViewMode.exitRenameMode), [`getPromptPrefix`](../../../../../tui/src/components/editor.ts.md#Editor.getPromptPrefix), [`getHiddenTextPrefixLength`](../../../../../tui/src/components/editor.ts.md#Editor.getHiddenTextPrefixLength), [`renderPrompt`](../../agents-view/agents-view-mode.ts.md#AgentsViewMode.renderPrompt), [`formatPromptPrefix`](../../../../../tui/src/components/editor.ts.md#Editor.formatPromptPrefix), [`styleDisplayText`](../../../../../tui/src/components/editor.ts.md#Editor.styleDisplayText)  (10 test-only)

### `CustomEditorOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/custom-editor.ts:12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L12)
- signature: `interface CustomEditorOptions`
- members:
  - `isArgumentCommand` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L15)
  - `placeholder` — [`L13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L13)
  - `placeholderColor` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-editor.ts#L14)
- uses (calls/refs, reference-scoped): [`EditorOptions`](../../../../../tui/src/components/editor.ts.md#EditorOptions)
- used by: [`<constructor>`](custom-editor.ts.md#CustomEditor.-constructor)


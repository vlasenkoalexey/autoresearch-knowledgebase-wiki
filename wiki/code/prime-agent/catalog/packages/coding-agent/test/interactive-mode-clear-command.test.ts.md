---
title: 'Module: packages/coding-agent/test/interactive-mode-clear-command.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/interactive-mode-clear-command.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`interactive-mode-clear-command.test.ts`/
symbols:
  renderAll: renderAll().
  interactiveModePrototype: interactiveModePrototype.
  ClearCommandContext.typeLiteral0.chatContainer: ClearCommandContext#typeLiteral0:chatContainer.
  InteractiveModePrototype.typeLiteral28.handleClearCommand: InteractiveModePrototype#typeLiteral28:handleClearCommand().
  ClearCommandContext: ClearCommandContext#
  ClearCommandContext.typeLiteral0.stopWorkingLoader: ClearCommandContext#typeLiteral0:stopWorkingLoader.
  ClearCommandContext.typeLiteral0.renderCurrentSessionState: ClearCommandContext#typeLiteral0:renderCurrentSessionState.
  ClearCommandContext.typeLiteral0.ui: ClearCommandContext#typeLiteral0:ui.
  ClearCommandContext.typeLiteral0.ui.typeLiteral24.requestRender: ClearCommandContext#typeLiteral0:ui.typeLiteral24:requestRender.
  ClearCommandContext.typeLiteral0.agentConnection: ClearCommandContext#typeLiteral0:agentConnection.
  ClearCommandContext.typeLiteral0.agentConnection.typeLiteral1.newSession: ClearCommandContext#typeLiteral0:agentConnection.typeLiteral1:newSession.
  ClearCommandContext.typeLiteral0.editor: ClearCommandContext#typeLiteral0:editor.
  ClearCommandContext.typeLiteral0.getPromptStashImages: ClearCommandContext#typeLiteral0:getPromptStashImages.
  ClearCommandContext.typeLiteral0.pastedImages: ClearCommandContext#typeLiteral0:pastedImages.
  ClearCommandContext.typeLiteral0.handleFatalRuntimeError: ClearCommandContext#typeLiteral0:handleFatalRuntimeError.
  ClearCommandContext.typeLiteral0.agentConnection.typeLiteral1.setSessionName: ClearCommandContext#typeLiteral0:agentConnection.typeLiteral1:setSessionName.
  ClearCommandContext.typeLiteral0.agentConnection.typeLiteral1.prompt: ClearCommandContext#typeLiteral0:agentConnection.typeLiteral1:prompt.
  ClearCommandContext.typeLiteral0.collectImagesFor: ClearCommandContext#typeLiteral0:collectImagesFor.
  InteractiveModePrototype: InteractiveModePrototype#
  ClearCommandContext.typeLiteral0.editor.typeLiteral13.setText: ClearCommandContext#typeLiteral0:editor.typeLiteral13:setText.
  ClearCommandContext.typeLiteral0.editor.typeLiteral13.addToHistory: ClearCommandContext#typeLiteral0:editor.typeLiteral13:addToHistory.
  ClearCommandContext.typeLiteral0.showError: ClearCommandContext#typeLiteral0:showError.
  InteractiveModePrototype.typeLiteral28.handleClearCommand.options-typeLiteral29.name: InteractiveModePrototype#typeLiteral28:handleClearCommand().(options)typeLiteral29:name.
  InteractiveModePrototype.typeLiteral28.handleClearCommand.options-typeLiteral29.prompt: InteractiveModePrototype#typeLiteral28:handleClearCommand().(options)typeLiteral29:prompt.
---
# Module: [`packages/coding-agent/test/interactive-mode-clear-command.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts)

## Classes
### `ClearCommandContext`
- def: [`packages/coding-agent/test/interactive-mode-clear-command.test.ts:6`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L6)
- signature: `type ClearCommandContext`
- members:
  - `addToHistory` — [`L13`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L13)
  - `agentConnection` — [`L8`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L8)
  - `chatContainer` — [`L19`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L19)
  - `collectImagesFor` — [`L14`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L14)
  - `editor` — [`L13`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L13)
  - `getPromptStashImages` — [`L15`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L15)
  - `handleFatalRuntimeError` — [`L21`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L21)
  - `newSession` — [`L9`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L9)
  - `pastedImages` — [`L16`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L16)
  - `prompt` — [`L11`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L11)
  - `renderCurrentSessionState` — [`L18`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L18)
  - `requestRender` — [`L20`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L20)
  - `setSessionName` — [`L10`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L10)
  - `setText` — [`L13`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L13)
  - `showError` — [`L17`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L17)
  - `stopWorkingLoader` — [`L7`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L7)
  - `ui` — [`L20`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L20)
- uses (calls/refs, reference-scoped): [`Container`](../../tui/src/tui.ts.md#Container)
- used by: (2 test-only callers)

### `InteractiveModePrototype`
- def: [`packages/coding-agent/test/interactive-mode-clear-command.test.ts:24`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L24)
- signature: `type InteractiveModePrototype`
- members:
  - `handleClearCommand(method)` — [`L25`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L25)
  - `name` — [`L25`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L25)
  - `prompt` — [`L25`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L25)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

## Functions
- `renderAll(container: Container, width?: number)` — [`L30`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L30)

## Module values
- `interactiveModePrototype` — [`L28`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-clear-command.test.ts#L28)


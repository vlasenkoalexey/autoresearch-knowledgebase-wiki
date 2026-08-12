---
title: 'Module: packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`interactive-mode-rlm-max-depth-command.test.ts`/
symbols:
  makeContext: makeContext().
  renderAll: renderAll().
  prototype: prototype.
  Context.typeLiteral0.chatContainer: Context#typeLiteral0:chatContainer.
  Prototype.typeLiteral34.handleRlmMaxDepthCommand: Prototype#typeLiteral34:handleRlmMaxDepthCommand().
  Context.typeLiteral0.agentConnection: Context#typeLiteral0:agentConnection.
  Prototype: Prototype#
  Context: Context#
  Context.typeLiteral0.agentConnection.typeLiteral1.setRlmMaxDepth: Context#typeLiteral0:agentConnection.typeLiteral1:setRlmMaxDepth.
  Context.typeLiteral0.agentConnection.typeLiteral1.getRlmMaxDepthStatus: Context#typeLiteral0:agentConnection.typeLiteral1:getRlmMaxDepthStatus.
  Context.typeLiteral0.showError: Context#typeLiteral0:showError.
  SubmitContext: SubmitContext#
  Context.typeLiteral0.ui: Context#typeLiteral0:ui.
  Context.typeLiteral0.ui.typeLiteral18.requestRender: Context#typeLiteral0:ui.typeLiteral18:requestRender.
  Context.typeLiteral0.showWarning: Context#typeLiteral0:showWarning.
  SubmitContext.typeLiteral23.defaultEditor: SubmitContext#typeLiteral23:defaultEditor.
  SubmitContext.typeLiteral23.defaultEditor.typeLiteral24.onSubmit: SubmitContext#typeLiteral23:defaultEditor.typeLiteral24:onSubmit.
  SubmitContext.typeLiteral23.handleRlmMaxDepthCommand: SubmitContext#typeLiteral23:handleRlmMaxDepthCommand.
  Prototype.typeLiteral34.setupEditorSubmitHandler: Prototype#typeLiteral34:setupEditorSubmitHandler().
  SubmitContext.typeLiteral23.editor: SubmitContext#typeLiteral23:editor.
  SubmitContext.typeLiteral23.editor.typeLiteral27.getText: SubmitContext#typeLiteral23:editor.typeLiteral27:getText.
  SubmitContext.typeLiteral23.editor.typeLiteral27.setText: SubmitContext#typeLiteral23:editor.typeLiteral27:setText.
---
# Module: [`packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts)

## Classes
### `Context`
- def: [`packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts:6`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L6)
- signature: `type Context`
- members:
  - `agentConnection` — [`L7`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L7)
  - `chatContainer` — [`L14`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L14)
  - `getRlmMaxDepthStatus` — [`L8`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L8)
  - `requestRender` — [`L15`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L15)
  - `setRlmMaxDepth` — [`L9`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L9)
  - `showError` — [`L17`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L17)
  - `showWarning` — [`L16`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L16)
  - `ui` — [`L15`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L15)
- uses (calls/refs, reference-scoped): [`Container`](../../tui/src/tui.ts.md#Container)
- used by: (3 test-only callers)

### `Prototype`
- def: [`packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts:27`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L27)
- signature: `type Prototype`
- members:
  - `handleRlmMaxDepthCommand(method)` — [`L28`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L28)
  - `setupEditorSubmitHandler(method)` — [`L29`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L29)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

### `SubmitContext`
- def: [`packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts:20`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L20)
- signature: `type SubmitContext`
- members:
  - `defaultEditor` — [`L21`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L21)
  - `editor` — [`L22`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L22)
  - `getText` — [`L22`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L22)
  - `handleRlmMaxDepthCommand` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L23)
  - `onSubmit` — [`L21`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L21)
  - `setText` — [`L22`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L22)
- used by: (2 test-only callers)

## Functions
- `makeContext(overrides?: Partial<{ getRlmMaxDepthStatus: () => Promise<{ maxDepth: number; source: "chat"; }>; setRlmMaxDepth: (maxDepth: number, options?: { global?: boolean | undefined; } | undefined) => Promise<...>; }>)` — [`L41`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L41)
- `renderAll(container: Container, width?: number)` — [`L34`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L34)

## Module values
- `prototype` — [`L32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-rlm-max-depth-command.test.ts#L32)


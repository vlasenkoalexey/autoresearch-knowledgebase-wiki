---
title: 'Module: packages/coding-agent/src/modes/interactive/components/bash-execution.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/bash-execution.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`bash-execution.ts`/
symbols:
  BashExecutionComponent.updateDisplay: BashExecutionComponent#updateDisplay().
  BashExecutionComponent.-constructor: BashExecutionComponent#`<constructor>`().
  BashExecutionComponent.setComplete: BashExecutionComponent#setComplete().
  BashExecutionComponent: BashExecutionComponent#
  BashExecutionComponent.setFailed: BashExecutionComponent#setFailed().
  BashExecutionComponent.contentContainer: BashExecutionComponent#contentContainer.
  BashExecutionComponent.appendOutput: BashExecutionComponent#appendOutput().
  BashExecutionComponent.loader: BashExecutionComponent#loader.
  BashExecutionComponent.outputLines: BashExecutionComponent#outputLines.
  BashExecutionComponent.getOutput: BashExecutionComponent#getOutput().
  BashExecutionComponent.status: BashExecutionComponent#status.
  BashExecutionComponent.setExpanded: BashExecutionComponent#setExpanded().
  BashExecutionComponent.invalidate: BashExecutionComponent#invalidate().
  BashExecutionComponent.truncationResult: BashExecutionComponent#truncationResult.
  BashExecutionComponent.command: BashExecutionComponent#command.
  BashExecutionComponent.errorMessage: BashExecutionComponent#errorMessage.
  BashExecutionComponent.fullOutputPath: BashExecutionComponent#fullOutputPath.
  BashExecutionComponent.expanded: BashExecutionComponent#expanded.
  BashExecutionComponent.getCommand: BashExecutionComponent#getCommand().
  PREVIEW_LINES: PREVIEW_LINES.
  BashExecutionComponent.exitCode: BashExecutionComponent#exitCode.
  BashExecutionComponent.-constructor-.options-typeLiteral0.suppressLeadingSpace: BashExecutionComponent#`<constructor>`().(options)typeLiteral0:suppressLeadingSpace.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/bash-execution.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts)

## Classes
### `BashExecutionComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/bash-execution.ts:21`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L21)
- signature: `class BashExecutionComponent`
- members:
  - `<constructor>(command: string, ui: TUI, excludeFromContext?: boolean, options?: { suppressLeadingSpace?: boolean | undefined; })` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L33)
  - `appendOutput(method)` — [`L81`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L81)
  - `getCommand(method)` — [`L229`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L229) — Get the command that was executed.
  - `getOutput(method)` — [`L222`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L222) — Get the raw output for creating BashExecutionMessage.
  - `invalidate(method)` — [`L76`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L76) — Invalidate any cached rendering state.
  - `setComplete(method)` — [`L99`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L99)
  - `setExpanded(method)` — [`L71`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L71) — Set whether the output is expanded (shows full output) or collapsed (preview only).
  - `setFailed(method)` — [`L121`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L121) — Mark the execution as failed before producing a result (e.g. spawn failure).
  - `updateDisplay(method)` — [`L128`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L128)
  - `command` — [`L22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L22)
  - `contentContainer` — [`L31`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L31)
  - `errorMessage` — [`L26`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L26)
  - `exitCode` — [`L25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L25)
  - `expanded` — [`L30`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L30)
  - `fullOutputPath` — [`L29`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L29)
  - `loader` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L27)
  - `outputLines` — [`L23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L23)
  - `status` — [`L24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L24)
  - `suppressLeadingSpace` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L33)
  - `truncationResult` — [`L28`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L28)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`TUI`](../../../../../tui/src/tui.ts.md#TUI), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`keyText`](keybinding-hints.ts.md#keyText), [`bold`](../theme/theme.ts.md#Theme.bold), [`clear`](../../../../../tui/src/tui.ts.md#Container.clear), [`truncateTail`](../../../core/tools/truncate.ts.md#truncateTail), [`<constructor>`](dynamic-border.ts.md#DynamicBorder.-constructor), [`expandCollapseHint`](keybinding-hints.ts.md#expandCollapseHint), [`invalidate`](../../../../../tui/src/tui.ts.md#Container.invalidate), [`truncated`](../../../core/tools/truncate.ts.md#TruncationResult.truncated), [`Loader`](../../../../../tui/src/components/loader.ts.md#Loader), [`truncateToVisualLines`](visual-truncate.ts.md#truncateToVisualLines), [`DEFAULT_MAX_BYTES`](../../../core/tools/truncate.ts.md#DEFAULT_MAX_BYTES), [`TruncationResult`](../../../core/tools/truncate.ts.md#TruncationResult), [`<constructor>`](../../../../../tui/src/components/loader.ts.md#Loader.-constructor), [`stop`](../../../../../tui/src/components/loader.ts.md#Loader.stop), [`DEFAULT_MAX_LINES`](../../../core/tools/truncate.ts.md#DEFAULT_MAX_LINES), [`content`](../../../core/tools/truncate.ts.md#TruncationResult.content), [`visualLines`](visual-truncate.ts.md#VisualTruncateResult.visualLines), [`PREVIEW_LINES`](bash-execution.ts.md#PREVIEW_LINES)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`handleEvent`](../interactive-mode.ts.md#InteractiveMode.handleEvent), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`addMessageToChat`](../interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`resetCurrentSessionRenderState`](../interactive-mode.ts.md#InteractiveMode.resetCurrentSessionRenderState), [`conversation-components.ts`](conversation-components.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-conversation-components.ts), [`renderResyncedSession`](../interactive-mode.ts.md#InteractiveMode.renderResyncedSession), [`invalidate`](../../../../../tui/src/tui.ts.md#Container.invalidate), [`isCompactAgentMessageNeighbor`](conversation-components.ts.md#isCompactAgentMessageNeighbor), [`activeBashComponent`](../interactive-mode.ts.md#InteractiveMode.activeBashComponent), [`sideQuestionBashComponent`](../interactive-mode.ts.md#InteractiveMode.sideQuestionBashComponent), [`pendingBashComponents`](../interactive-mode.ts.md#InteractiveMode.pendingBashComponents)  (3 test-only)

## Module values
- `PREVIEW_LINES` — [`L19`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bash-execution.ts#L19)


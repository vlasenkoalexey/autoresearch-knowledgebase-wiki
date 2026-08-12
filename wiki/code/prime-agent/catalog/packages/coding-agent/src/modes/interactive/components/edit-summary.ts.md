---
title: 'Module: packages/coding-agent/src/modes/interactive/components/edit-summary.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/edit-summary.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`edit-summary.ts`/
symbols:
  mergeTurnFileChanges: mergeTurnFileChanges().
  getToolFileChanges.result-typeLiteral16.isError: getToolFileChanges().(result)typeLiteral16:isError.
  formatTotalChangeSummary: formatTotalChangeSummary().
  mergeFileChange: mergeFileChange().
  FileChangeSummaryComponent.render: FileChangeSummaryComponent#render().
  counts: counts().
  FileChangeSummary: FileChangeSummary#
  FileChangeSummary.added: FileChangeSummary#added.
  FileChangeSummary.removed: FileChangeSummary#removed.
  FileChangeSummary.path: FileChangeSummary#path.
  formatFileChangePath: formatFileChangePath().
  getToolFileChanges: getToolFileChanges().
  countChangedLines: countChangedLines().
  getToolFileChanges.result-typeLiteral16.details: getToolFileChanges().(result)typeLiteral16:details.
  FileChangeSummaryComponent: FileChangeSummaryComponent#
  FileChangeSummaryComponent.-constructor: FileChangeSummaryComponent#`<constructor>`().
  countChangedLines.typeLiteral0.added: countChangedLines().typeLiteral0:added.
  countChangedLines.typeLiteral0.removed: countChangedLines().typeLiteral0:removed.
  FileChangeSummaryComponent.invalidate: FileChangeSummaryComponent#invalidate().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/edit-summary.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts)

## Classes
### `FileChangeSummary`
- def: [`packages/coding-agent/src/modes/interactive/components/edit-summary.ts:12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L12)
- signature: `interface FileChangeSummary`
- members:
  - `added` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L14)
  - `path` — [`L13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L13)
  - `removed` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L15)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`mergeTurnFileChanges`](edit-summary.ts.md#mergeTurnFileChanges), [`isError`](edit-summary.ts.md#getToolFileChanges.result-typeLiteral16.isError), [`formatTotalChangeSummary`](edit-summary.ts.md#formatTotalChangeSummary), [`mergeFileChange`](edit-summary.ts.md#mergeFileChange), [`render`](edit-summary.ts.md#FileChangeSummaryComponent.render), [`counts`](edit-summary.ts.md#counts), [`agentRunFileChanges`](../interactive-mode.ts.md#InteractiveMode.agentRunFileChanges), [`<constructor>`](edit-summary.ts.md#FileChangeSummaryComponent.-constructor)  (4 test-only)

### `FileChangeSummaryComponent`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/edit-summary.ts:93`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L93)
- signature: `class FileChangeSummaryComponent`
- members:
  - `<constructor>(changes: readonly FileChangeSummary[], cwd: string)` — [`L94`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L94)
  - `invalidate(method)` — [`L110`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L110) — Invalidate any cached rendering state.
  - `render(method)` — [`L99`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L99) — Render the component to lines for the given viewport width
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`counts`](edit-summary.ts.md#counts), [`FileChangeSummary`](edit-summary.ts.md#FileChangeSummary), [`path`](edit-summary.ts.md#FileChangeSummary.path), [`formatFileChangePath`](edit-summary.ts.md#formatFileChangePath)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`updateDisplay`](tool-execution.ts.md#ToolExecutionComponent.updateDisplay), [`tool-execution.ts`](tool-execution.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-tool-execution.ts)

## Functions
- `countChangedLines(diff: string)` — [`L18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L18)
- `counts(change: Pick<FileChangeSummary, "added" | "removed">)` — [`L82`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L82)
- `formatFileChangePath(path: string, cwd: string)` — [`L86`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L86)
- `formatTotalChangeSummary(changes: readonly FileChangeSummary[])` — [`L113`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L113)
- `getToolFileChanges(toolName: string, args: unknown, result: { details?: unknown; isError: boolean; }, cwd: string)` — [`L40`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L40)
- `mergeFileChange(target: Map<string, FileChangeSummary>, change: FileChangeSummary, cwd: string)` — [`L28`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L28)
- `mergeTurnFileChanges(target: Map<string, FileChangeSummary>, message: AgentMessage, toolResults: readonly ToolResultMessage<any>[], cwd: string)` — [`L63`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L63)

## Module values
- `added` — [`L18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L18)
- `details` — [`L43`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L43)
- `isError` — [`L43`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L43)
- `removed` — [`L18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/edit-summary.ts#L18)


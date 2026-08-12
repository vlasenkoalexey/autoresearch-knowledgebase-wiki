---
title: 'Module: packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`subagent-summary-line.ts`/
symbols:
  SubagentSummaryLine.render: SubagentSummaryLine#render().
  countDirectSubagentStatuses: countDirectSubagentStatuses().
  SubagentSummaryLine.counts: SubagentSummaryLine#counts.
  SubagentSummaryLine.handleInput: SubagentSummaryLine#handleInput().
  SubagentSummaryLine.isSelectable: SubagentSummaryLine#isSelectable().
  SubagentSummaryCounts.total: SubagentSummaryCounts#total.
  SubagentSummaryLine.setSubagentCounts: SubagentSummaryLine#setSubagentCounts().
  SubagentSummaryLine.renderInfoLine: SubagentSummaryLine#renderInfoLine().
  SubagentSummaryLine.invalidate: SubagentSummaryLine#invalidate().
  SubagentSummaryLine: SubagentSummaryLine#
  SubagentSummaryLine.-constructor: SubagentSummaryLine#`<constructor>`().
  SubagentSummaryCounts.running: SubagentSummaryCounts#running.
  SubagentSummaryCounts.idle: SubagentSummaryCounts#idle.
  SubagentSummaryCounts.inactive: SubagentSummaryCounts#inactive.
  SubagentSummaryLine.setOpenable: SubagentSummaryLine#setOpenable().
  SubagentSummaryLine.onOpen: SubagentSummaryLine#onOpen.
  SubagentSummaryCounts: SubagentSummaryCounts#
  SubagentSummaryLine.focused: SubagentSummaryLine#focused.
  SubagentSummaryLine.openable: SubagentSummaryLine#openable.
  SubagentSummaryLine.onCancel: SubagentSummaryLine#onCancel.
  SubagentSummaryLine.onChatAction: SubagentSummaryLine#onChatAction.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts)

## Classes
### `SubagentSummaryCounts`
- def: [`packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts:6`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L6)
- signature: `interface SubagentSummaryCounts`
- members:
  - `idle` — [`L9`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L9)
  - `inactive` — [`L10`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L10)
  - `running` — [`L8`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L8)
  - `total` — [`L7`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L7)
- used by: [`render`](subagent-summary-line.ts.md#SubagentSummaryLine.render), [`countDirectSubagentStatuses`](subagent-summary-line.ts.md#countDirectSubagentStatuses), [`counts`](subagent-summary-line.ts.md#SubagentSummaryLine.counts), [`isSelectable`](subagent-summary-line.ts.md#SubagentSummaryLine.isSelectable), [`setSubagentCounts`](subagent-summary-line.ts.md#SubagentSummaryLine.setSubagentCounts)  (1 test-only)

### `SubagentSummaryLine`  ·  implements/extends Component, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts:39`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L39)
- doc: One-line entry into the current session's scoped agents view.
- signature: `class SubagentSummaryLine`
- members:
  - `<constructor>(getLocationLabel?: () => string | undefined, getContextLabel?: () => string | undefined, getOverrideLabel?: () => string | undefined)` — [`L48`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L48) — One-line entry into the current session's scoped agents view.
  - `handleInput(method)` — [`L66`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L66) — Optional handler for keyboard input when component has focus
  - `invalidate(method)` — [`L113`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L113) — Invalidate any cached rendering state.
  - `isSelectable(method)` — [`L62`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L62)
  - `render(method)` — [`L83`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L83) — Render the component to lines for the given viewport width
  - `renderInfoLine(method)` — [`L96`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L96)
  - `setOpenable(method)` — [`L58`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L58)
  - `setSubagentCounts(method)` — [`L54`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L54)
  - `counts` — [`L41`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L41)
  - `focused` — [`L40`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L40) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `onCancel` — [`L45`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L45)
  - `onChatAction` — [`L46`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L46)
  - `onOpen` — [`L44`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L44)
  - `openable` — [`L42`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L42)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`keyText`](keybinding-hints.ts.md#keyText), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`bg`](../theme/theme.ts.md#Theme.bg), [`total`](subagent-summary-line.ts.md#SubagentSummaryCounts.total), [`idle`](subagent-summary-line.ts.md#SubagentSummaryCounts.idle), [`inactive`](subagent-summary-line.ts.md#SubagentSummaryCounts.inactive), [`running`](subagent-summary-line.ts.md#SubagentSummaryCounts.running), [`SubagentSummaryCounts`](subagent-summary-line.ts.md#SubagentSummaryCounts)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`handleEvent`](../interactive-mode.ts.md#InteractiveMode.handleEvent), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`<constructor>`](../interactive-mode.ts.md#InteractiveMode.-constructor), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`applySelectedModel`](../interactive-mode.ts.md#InteractiveMode.applySelectedModel), [`handleFastCommand`](../interactive-mode.ts.md#InteractiveMode.handleFastCommand), [`updateSubagentSummaryLine`](../interactive-mode.ts.md#InteractiveMode.updateSubagentSummaryLine), [`subagentSummaryLine`](../interactive-mode.ts.md#InteractiveMode.subagentSummaryLine), [`showCtrlCExitHint`](../interactive-mode.ts.md#InteractiveMode.showCtrlCExitHint), [`focused`](../../../../../tui/src/tui.ts.md#Focusable.focused), [`clearCtrlCExitHint`](../interactive-mode.ts.md#InteractiveMode.clearCtrlCExitHint), [`updateGoalTrayTimer`](../interactive-mode.ts.md#InteractiveMode.updateGoalTrayTimer), [`focusSubagentSummary`](../interactive-mode.ts.md#InteractiveMode.focusSubagentSummary), [`setSessionHasMessages`](../interactive-mode.ts.md#InteractiveMode.setSessionHasMessages), [`syncGoalTray`](../interactive-mode.ts.md#InteractiveMode.syncGoalTray)  (1 test-only)

## Functions
- `countDirectSubagentStatuses(children: Iterable<AgentConnectionRlmChildAgentSnapshot>, parentId: string | undefined, activeHeartbeatSessionIds: ReadonlySet<string>)` — [`L13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/subagent-summary-line.ts#L13)


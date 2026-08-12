---
title: 'Module: packages/coding-agent/src/modes/interactive/components/tool-panel.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/tool-panel.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`tool-panel.ts`/
symbols:
  ToolPanel.render: ToolPanel#render().
  toolPanelLine: toolPanelLine().
  ToolPanel.addChild: ToolPanel#addChild().
  ToolPanel: ToolPanel#
  ToolPanel.invalidate: ToolPanel#invalidate().
  ToolPanel.children: ToolPanel#children.
  ToolPanel.clear: ToolPanel#clear().
  toolPanelContentWidth: toolPanelContentWidth().
  ToolPanel.cache: ToolPanel#cache.
  ToolPanel.setHeader: ToolPanel#setHeader().
  ToolPanel.header: ToolPanel#header.
  TOOL_PANEL_PADDING_X: TOOL_PANEL_PADDING_X.
  ToolPanel.cache.typeLiteral12.childLines: ToolPanel#cache.typeLiteral12:childLines.
  ToolPanel.cache.typeLiteral12.width: ToolPanel#cache.typeLiteral12:width.
  ToolPanel.cache.typeLiteral12.header: ToolPanel#cache.typeLiteral12:header.
  ToolPanel.cache.typeLiteral12.bgSample: ToolPanel#cache.typeLiteral12:bgSample.
  ToolPanel.cache.typeLiteral12.lines: ToolPanel#cache.typeLiteral12:lines.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/tool-panel.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts)

## Classes
### `ToolPanel`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/tool-panel.ts:30`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L30)
- doc: Panel shell for tool executions: a status header line followed by the
- signature: `class ToolPanel`
- members:
  - `addChild(method)` — [`L45`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L45)
  - `clear(method)` — [`L50`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L50)
  - `invalidate(method)` — [`L55`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L55) — Invalidate any cached rendering state.
  - `render(method)` — [`L62`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L62) — Render the component to lines for the given viewport width
  - `setHeader(method)` — [`L41`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L41)
  - `bgSample` — [`L36`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L36)
  - `cache` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L33)
  - `childLines` — [`L37`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L37)
  - `children` — [`L31`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L31)
  - `header` — [`L32`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L32)
  - `header` — [`L35`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L35)
  - `lines` — [`L38`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L38)
  - `width` — [`L34`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L34)
- uses (calls/refs, reference-scoped): [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`bg`](../theme/theme.ts.md#Theme.bg), [`toolPanelLine`](tool-panel.ts.md#toolPanelLine), [`toolPanelContentWidth`](tool-panel.ts.md#toolPanelContentWidth)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`updateDisplay`](tool-execution.ts.md#ToolExecutionComponent.updateDisplay), [`tool-execution.ts`](tool-execution.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-tool-execution.ts), [`<constructor>`](tool-execution.ts.md#ToolExecutionComponent.-constructor), [`mountRenderers`](tool-execution.ts.md#ToolExecutionComponent.mountRenderers), [`render`](tool-execution.ts.md#ToolExecutionComponent.render), [`contentPanel`](tool-execution.ts.md#ToolExecutionComponent.contentPanel)

## Functions
- `toolPanelContentWidth(width: number)` — [`L6`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L6)
- `toolPanelLine(line: string, width: number)` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L15) — Format a single tool panel line: content indented by the panel padding and

## Module values
- `TOOL_PANEL_PADDING_X` — [`L4`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tool-panel.ts#L4)


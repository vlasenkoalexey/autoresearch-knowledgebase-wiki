---
title: 'Module: packages/coding-agent/src/modes/interactive/components/collapsible-error.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/collapsible-error.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`collapsible-error.ts`/
symbols:
  CollapsibleErrorComponent.render: CollapsibleErrorComponent#render().
  summarizeErrorDetails: summarizeErrorDetails().
  CollapsibleErrorComponent.renderText: CollapsibleErrorComponent#renderText().
  normalizeErrorDetails: normalizeErrorDetails().
  isStackContextLine: isStackContextLine().
  summarizeStackContext: summarizeStackContext().
  CollapsibleErrorComponent.-constructor: CollapsibleErrorComponent#`<constructor>`().
  ErrorDetailLine.trimmed: ErrorDetailLine#trimmed.
  startsStackContext: startsStackContext().
  shouldCollapseErrorDetails: shouldCollapseErrorDetails().
  errorDetailLines: errorDetailLines().
  ErrorDetailLine: ErrorDetailLine#
  CollapsibleErrorComponent: CollapsibleErrorComponent#
  CollapsibleErrorComponent.expanded: CollapsibleErrorComponent#expanded.
  CollapsibleErrorComponent.setExpanded: CollapsibleErrorComponent#setExpanded().
  CollapsibleErrorOptions.text: CollapsibleErrorOptions#text.
  CollapsibleErrorOptions.summary: CollapsibleErrorOptions#summary.
  CollapsibleErrorOptions.expanded: CollapsibleErrorOptions#expanded.
  ErrorDetailLine.raw: ErrorDetailLine#raw.
  CollapsibleErrorOptions: CollapsibleErrorOptions#
  CollapsibleErrorOptions.forceCollapse: CollapsibleErrorOptions#forceCollapse.
  CollapsibleErrorOptions.paddingX: CollapsibleErrorOptions#paddingX.
  CollapsibleErrorComponent.invalidate: CollapsibleErrorComponent#invalidate().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/collapsible-error.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts)

## Classes
### `CollapsibleErrorComponent`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/collapsible-error.ts:78`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L78)
- signature: `class CollapsibleErrorComponent`
- members:
  - `<constructor>(options: CollapsibleErrorOptions)` — [`L81`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L81)
  - `invalidate(method)` — [`L89`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L89) — Invalidate any cached rendering state.
  - `render(method)` — [`L93`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L93) — Render the component to lines for the given viewport width
  - `renderText(method)` — [`L109`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L109)
  - `setExpanded(method)` — [`L85`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L85)
  - `expanded` — [`L79`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L79)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`wrapTextWithAnsi`](../../../../../tui/src/utils.ts.md#wrapTextWithAnsi), [`expandCollapseHint`](keybinding-hints.ts.md#expandCollapseHint), [`summarizeErrorDetails`](collapsible-error.ts.md#summarizeErrorDetails), [`normalizeErrorDetails`](collapsible-error.ts.md#normalizeErrorDetails), [`shouldCollapseErrorDetails`](collapsible-error.ts.md#shouldCollapseErrorDetails), [`expanded`](collapsible-error.ts.md#CollapsibleErrorOptions.expanded), [`summary`](collapsible-error.ts.md#CollapsibleErrorOptions.summary), [`text`](collapsible-error.ts.md#CollapsibleErrorOptions.text), [`CollapsibleErrorOptions`](collapsible-error.ts.md#CollapsibleErrorOptions), [`forceCollapse`](collapsible-error.ts.md#CollapsibleErrorOptions.forceCollapse), [`paddingX`](collapsible-error.ts.md#CollapsibleErrorOptions.paddingX)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`assistant-message.ts`](assistant-message.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-assistant-message.ts), [`createErrorComponent`](assistant-message.ts.md#AssistantMessageComponent.createErrorComponent)

### `CollapsibleErrorOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/collapsible-error.ts:6`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L6)
- signature: `interface CollapsibleErrorOptions`
- members:
  - `expanded` — [`L9`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L9)
  - `forceCollapse` — [`L10`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L10)
  - `paddingX` — [`L11`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L11)
  - `summary` — [`L8`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L8)
  - `text` — [`L7`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L7)
- used by: [`createErrorComponent`](assistant-message.ts.md#AssistantMessageComponent.createErrorComponent), [`render`](collapsible-error.ts.md#CollapsibleErrorComponent.render), [`renderText`](collapsible-error.ts.md#CollapsibleErrorComponent.renderText), [`<constructor>`](collapsible-error.ts.md#CollapsibleErrorComponent.-constructor)

### `ErrorDetailLine`
- def: [`packages/coding-agent/src/modes/interactive/components/collapsible-error.ts:18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L18)
- signature: `interface ErrorDetailLine`
- members:
  - `raw` — [`L19`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L19)
  - `trimmed` — [`L20`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L20)
- used by: [`summarizeErrorDetails`](collapsible-error.ts.md#summarizeErrorDetails), [`isStackContextLine`](collapsible-error.ts.md#isStackContextLine), [`summarizeStackContext`](collapsible-error.ts.md#summarizeStackContext), [`startsStackContext`](collapsible-error.ts.md#startsStackContext), [`errorDetailLines`](collapsible-error.ts.md#errorDetailLines)

## Functions
- `errorDetailLines(text: string)` — [`L23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L23)
- `isStackContextLine(line: ErrorDetailLine)` — [`L46`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L46)
- `normalizeErrorDetails(text: string)` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L14)
- `shouldCollapseErrorDetails(text: string)` — [`L74`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L74)
- `startsStackContext(line: ErrorDetailLine)` — [`L30`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L30)
- `summarizeErrorDetails(text: string)` — [`L63`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L63)
- `summarizeStackContext(lines: readonly ErrorDetailLine[])` — [`L53`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/collapsible-error.ts#L53)


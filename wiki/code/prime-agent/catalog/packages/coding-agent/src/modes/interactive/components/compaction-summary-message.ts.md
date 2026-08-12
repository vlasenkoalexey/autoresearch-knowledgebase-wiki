---
title: 'Module: packages/coding-agent/src/modes/interactive/components/compaction-summary-message.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/compaction-summary-message.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`compaction-summary-message.ts`/CompactionSummaryMessageComponent#
symbols:
  CompactionSummaryMessageComponent.updateDisplay: updateDisplay().
  CompactionSummaryMessageComponent.-constructor: '`<constructor>`().'
  CompactionSummaryMessageComponent.message: message.
  CompactionSummaryMessageComponent.setExpanded: setExpanded().
  CompactionSummaryMessageComponent: ''
  CompactionSummaryMessageComponent.invalidate: invalidate().
  CompactionSummaryMessageComponent.markdownTheme: markdownTheme.
  CompactionSummaryMessageComponent.expanded: expanded.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/compaction-summary-message.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-summary-message.ts)

## Classes
### `CompactionSummaryMessageComponent`  ·  implements/extends Box, Component
- def: [`packages/coding-agent/src/modes/interactive/components/compaction-summary-message.ts:10`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-summary-message.ts#L10)
- doc: Component that renders a compaction message with collapsed/expanded state.
- signature: `class CompactionSummaryMessageComponent`
- members:
  - `<constructor>(message: CompactionSummaryMessage, markdownTheme?: MarkdownTheme)` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-summary-message.ts#L15) — Component that renders a compaction message with collapsed/expanded state.
  - `invalidate(method)` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-summary-message.ts#L27) — Invalidate any cached rendering state.
  - `setExpanded(method)` — [`L22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-summary-message.ts#L22)
  - `updateDisplay(method)` — [`L32`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-summary-message.ts#L32)
  - `expanded` — [`L11`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-summary-message.ts#L11)
  - `markdownTheme` — [`L13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-summary-message.ts#L13)
  - `message` — [`L12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-summary-message.ts#L12)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`<constructor>`](../../../../../tui/src/components/markdown.ts.md#Markdown.-constructor), [`getMarkdownTheme`](../theme/theme.ts.md#getMarkdownTheme), [`bg`](../theme/theme.ts.md#Theme.bg), [`MarkdownTheme`](../../../../../tui/src/components/markdown.ts.md#MarkdownTheme), [`expandCollapseHint`](keybinding-hints.ts.md#expandCollapseHint), [`addChild`](../../../../../tui/src/components/box.ts.md#Box.addChild), [`Box`](../../../../../tui/src/components/box.ts.md#Box), [`invalidate`](../../../../../tui/src/components/box.ts.md#Box.invalidate), [`clear`](../../../../../tui/src/components/box.ts.md#Box.clear), [`summary`](../../../core/messages.ts.md#CompactionSummaryMessage.summary), [`CompactionSummaryMessage`](../../../core/messages.ts.md#CompactionSummaryMessage), [`customInstructions`](../../../core/messages.ts.md#CompactionSummaryMessage.customInstructions), [`tokensBefore`](../../../core/messages.ts.md#CompactionSummaryMessage.tokensBefore)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`addMessageToChat`](../interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`Box`](../../../../../tui/src/components/box.ts.md#Box), [`invalidate`](../../../../../tui/src/components/box.ts.md#Box.invalidate)


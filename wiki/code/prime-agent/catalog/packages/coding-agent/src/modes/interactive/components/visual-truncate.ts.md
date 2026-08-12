---
title: 'Module: packages/coding-agent/src/modes/interactive/components/visual-truncate.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/visual-truncate.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`visual-truncate.ts`/
symbols:
  truncateToVisualLines: truncateToVisualLines().
  VisualTruncateResult.visualLines: VisualTruncateResult#visualLines.
  VisualTruncateResult.skippedCount: VisualTruncateResult#skippedCount.
  VisualTruncateResult: VisualTruncateResult#
---
# Module: [`packages/coding-agent/src/modes/interactive/components/visual-truncate.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/visual-truncate.ts)

## Classes
### `VisualTruncateResult`
- def: [`packages/coding-agent/src/modes/interactive/components/visual-truncate.ts:8`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/visual-truncate.ts#L8)
- signature: `interface VisualTruncateResult`
- members:
  - `skippedCount` — [`L12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/visual-truncate.ts#L12) — Number of visual lines that were skipped (hidden)
  - `visualLines` — [`L10`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/visual-truncate.ts#L10) — The visual lines to display
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`details`](../../../core/tools/bash.ts.md#rebuildBashResultRenderComponent.result-typeLiteral96.details), [`updateDisplay`](bash-execution.ts.md#BashExecutionComponent.updateDisplay), [`truncateToVisualLines`](visual-truncate.ts.md#truncateToVisualLines)

## Functions
- `truncateToVisualLines(text: string, maxVisualLines: number, width: number, paddingX?: number)` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/visual-truncate.ts#L27) — Truncate text to a maximum number of visual lines (from the end).


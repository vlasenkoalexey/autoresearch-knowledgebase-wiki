---
title: 'Module: packages/coding-agent/src/modes/interactive/components/diff.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/diff.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`diff.ts`/
symbols:
  renderRichDiff: renderRichDiff().
  buildRichDiffLine: buildRichDiffLine().
  renderDiff: renderDiff().
  renderDiffSeparator: renderDiffSeparator().
  renderIntraLineDiff: renderIntraLineDiff().
  highlightContent: highlightContent().
  replaceTabs: replaceTabs().
  DiffLineSpec.bg: DiffLineSpec#bg.
  DiffLineSpec.gutterFg: DiffLineSpec#gutterFg.
  ThemeColor: ThemeColor#
  DiffLineSpec.contentFg: DiffLineSpec#contentFg.
  ThemeBg: ThemeBg#
  DiffLineSpec.gutter: DiffLineSpec#gutter.
  DiffLineSpec.content: DiffLineSpec#content.
  DiffLineSpec.width: DiffLineSpec#width.
  padToWidth: padToWidth().
  DiffLineSpec.language: DiffLineSpec#language.
  parseDiffLine: parseDiffLine().
  keepBackground: keepBackground().
  RenderDiffOptions: RenderDiffOptions#
  renderIntraLineDiff.typeLiteral8.removedLine: renderIntraLineDiff().typeLiteral8:removedLine.
  renderIntraLineDiff.typeLiteral8.addedLine: renderIntraLineDiff().typeLiteral8:addedLine.
  BG_CLEARING_RESET: BG_CLEARING_RESET.
  DiffLineSpec: DiffLineSpec#
  RichDiffOptions: RichDiffOptions#
  RichDiffOptions.language: RichDiffOptions#language.
  RenderDiffOptions.filePath: RenderDiffOptions#filePath.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/diff.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts)

## Classes
### `DiffLineSpec`
- def: [`packages/coding-agent/src/modes/interactive/components/diff.ts:171`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L171)
- signature: `interface DiffLineSpec`
- members:
  - `bg` — [`L172`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L172)
  - `content` — [`L175`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L175)
  - `contentFg` — [`L179`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L179) — Flat content color instead of syntax highlighting (256-color fallback).
  - `gutter` — [`L173`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L173)
  - `gutterFg` — [`L174`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L174)
  - `language` — [`L176`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L176)
  - `width` — [`L177`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L177)
- uses (calls/refs, reference-scoped): [`ThemeColor`](diff.ts.md#ThemeColor), [`ThemeBg`](diff.ts.md#ThemeBg)
- used by: [`renderRichDiff`](diff.ts.md#renderRichDiff), [`buildRichDiffLine`](diff.ts.md#buildRichDiffLine)

### `RenderDiffOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/diff.ts:69`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L69)
- signature: `interface RenderDiffOptions`
- members:
  - `filePath` — [`L71`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L71) — File path (unused, kept for API compatibility)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`renderDiff`](diff.ts.md#renderDiff)

### `RichDiffOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/diff.ts:214`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L214)
- signature: `interface RichDiffOptions`
- members:
  - `language` — [`L216`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L216) — Language id for syntax highlighting the diff content (e.g. "typescript").
- used by: [`renderRichDiff`](diff.ts.md#renderRichDiff)

### `ThemeBg`
- def: [`packages/coding-agent/src/modes/interactive/components/diff.ts:150`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L150)
- signature: `type ThemeBg`
- uses (calls/refs, reference-scoped): [`theme`](../theme/theme.ts.md#theme), [`bg`](../theme/theme.ts.md#Theme.bg)
- used by: [`bg`](diff.ts.md#DiffLineSpec.bg)

### `ThemeColor`
- def: [`packages/coding-agent/src/modes/interactive/components/diff.ts:151`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L151)
- signature: `type ThemeColor`
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme)
- used by: [`gutterFg`](diff.ts.md#DiffLineSpec.gutterFg), [`contentFg`](diff.ts.md#DiffLineSpec.contentFg)

## Functions
- `buildRichDiffLine(spec: DiffLineSpec)` — [`L194`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L194)
- `highlightContent(content: string, language: string | undefined)` — [`L161`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L161)
- `keepBackground(highlighted: string)` — [`L157`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L157)
- `padToWidth(inner: string, width: number)` — [`L182`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L182)
- `parseDiffLine(line: string)` — [`L9`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L9) — Parse diff line to extract prefix, line number, and content.
- `renderDiff(diffText: string, _options?: RenderDiffOptions)` — [`L80`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L80) — Render a diff string with colored lines and intra-line change highlighting.
- `renderDiffSeparator(contentWidth: number)` — [`L220`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L220) — A dim `⋮` row separating non-adjacent hunks of one file's diff.
- `renderIntraLineDiff(oldContent: string, newContent: string)` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L27) — Compute word-level diff and render with inverse on changed parts.
- `renderRichDiff(diffText: string, contentWidth: number, options?: RichDiffOptions)` — [`L228`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L228) — Render a unified diff as full-width rows: green/red blocks, syntax-highlighted.
- `replaceTabs(text: string)` — [`L18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L18) — Replace tabs with spaces for consistent rendering.

## Module values
- `BG_CLEARING_RESET` — [`L155`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L155)
- `addedLine` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L27)
- `removedLine` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/diff.ts#L27)


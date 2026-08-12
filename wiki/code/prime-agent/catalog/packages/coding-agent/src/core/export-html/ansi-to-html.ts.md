---
title: 'Module: packages/coding-agent/src/core/export-html/ansi-to-html.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/export-html/ansi-to-html.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/export-html/`ansi-to-html.ts`/
symbols:
  applySgrCode: applySgrCode().
  createEmptyStyle: createEmptyStyle().
  styleToInlineCSS: styleToInlineCSS().
  hasStyle: hasStyle().
  ansiToHtml: ansiToHtml().
  TextStyle.fg: TextStyle#fg.
  TextStyle.bg: TextStyle#bg.
  ansiLinesToHtml: ansiLinesToHtml().
  TextStyle.bold: TextStyle#bold.
  TextStyle.dim: TextStyle#dim.
  TextStyle.italic: TextStyle#italic.
  TextStyle.underline: TextStyle#underline.
  ANSI_COLORS: ANSI_COLORS.
  color256ToHex: color256ToHex().
  TextStyle: TextStyle#
  ANSI_REGEX: ANSI_REGEX.
  escapeHtml: escapeHtml().
---
# Module: [`packages/coding-agent/src/core/export-html/ansi-to-html.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts)

## Classes
### `TextStyle`
- def: [`packages/coding-agent/src/core/export-html/ansi-to-html.ts:72`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L72)
- signature: `interface TextStyle`
- members:
  - `bg` — [`L74`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L74)
  - `bold` — [`L75`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L75)
  - `dim` — [`L76`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L76)
  - `fg` — [`L73`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L73)
  - `italic` — [`L77`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L77)
  - `underline` — [`L78`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L78)
- used by: [`applySgrCode`](ansi-to-html.ts.md#applySgrCode), [`createEmptyStyle`](ansi-to-html.ts.md#createEmptyStyle), [`hasStyle`](ansi-to-html.ts.md#hasStyle), [`styleToInlineCSS`](ansi-to-html.ts.md#styleToInlineCSS)

## Functions
- `ansiLinesToHtml(lines: string[])` — [`L256`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L256) — Convert array of ANSI-escaped lines to HTML.
- `ansiToHtml(text: string)` — [`L198`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L198) — Convert ANSI-escaped text to HTML with inline styles.
- `applySgrCode(params: number[], style: TextStyle)` — [`L110`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L110) — Parse ANSI SGR (Select Graphic Rendition) codes and update style.
- `color256ToHex(index: number)` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L37) — Convert 256-color index to hex.
- `createEmptyStyle()` — [`L81`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L81)
- `escapeHtml(text: string)` — [`L63`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L63) — Escape HTML special characters.
- `hasStyle(style: TextStyle)` — [`L103`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L103)
- `styleToInlineCSS(style: TextStyle)` — [`L92`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L92)

## Module values
- `ANSI_COLORS` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L15) — ANSI escape code to HTML converter.
- `ANSI_REGEX` — [`L193`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/ansi-to-html.ts#L193)


---
title: 'Module: packages/coding-agent/src/core/tools/ipython-cell-code.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/tools/ipython-cell-code.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/tools/`ipython-cell-code.ts`/
symbols:
  parseIpythonBashCell: parseIpythonBashCell().
  ParsedIpythonBashCell.body: ParsedIpythonBashCell#body.
  ParsedIpythonBashCell.indent: ParsedIpythonBashCell#indent.
  ParsedIpythonBashCell.magicArguments: ParsedIpythonBashCell#magicArguments.
  BASH_CELL_MAGIC_PATTERN: BASH_CELL_MAGIC_PATTERN.
  ParsedIpythonBashCell: ParsedIpythonBashCell#
  ParsedIpythonBashCell.leadingWhitespace: ParsedIpythonBashCell#leadingWhitespace.
  ParsedIpythonBashCell.lineBreak: ParsedIpythonBashCell#lineBreak.
---
# Module: [`packages/coding-agent/src/core/tools/ipython-cell-code.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython-cell-code.ts)

## Classes
### `ParsedIpythonBashCell`
- def: [`packages/coding-agent/src/core/tools/ipython-cell-code.ts:3`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython-cell-code.ts#L3)
- signature: `interface ParsedIpythonBashCell`
- members:
  - `body` — [`L8`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython-cell-code.ts#L8)
  - `indent` — [`L5`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython-cell-code.ts#L5)
  - `leadingWhitespace` — [`L4`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython-cell-code.ts#L4)
  - `lineBreak` — [`L7`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython-cell-code.ts#L7)
  - `magicArguments` — [`L6`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython-cell-code.ts#L6)
- used by: [`lineCounts`](../../modes/interactive/components/ipython-cell.ts.md#IPythonCellComponent.lineCounts), [`applyShellSettingsToBashMagicCell`](ipython.ts.md#applyShellSettingsToBashMagicCell), [`parseIpythonBashCell`](ipython-cell-code.ts.md#parseIpythonBashCell), [`previewIpythonCode`](code-preview.ts.md#previewIpythonCode)

## Functions
- `parseIpythonBashCell(code: string)` — [`L11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython-cell-code.ts#L11)

## Module values
- `BASH_CELL_MAGIC_PATTERN` — [`L1`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython-cell-code.ts#L1)


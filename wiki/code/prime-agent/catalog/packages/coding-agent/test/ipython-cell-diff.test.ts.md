---
title: 'Module: packages/coding-agent/test/ipython-cell-diff.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/ipython-cell-diff.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`ipython-cell-diff.test.ts`/
symbols:
  renderCell: renderCell().
  fgAnsi: fgAnsi().
  bgAnsi: bgAnsi().
  stripAnsi: stripAnsi().
  changedRow: changedRow().
  ThemeFg: ThemeFg#
  ThemeBg: ThemeBg#
  hasBackground: hasBackground().
---
# Module: [`packages/coding-agent/test/ipython-cell-diff.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/ipython-cell-diff.test.ts)

## Classes
### `ThemeBg`
- def: [`packages/coding-agent/test/ipython-cell-diff.test.ts:16`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/ipython-cell-diff.test.ts#L16)
- signature: `type ThemeBg`
- uses (calls/refs, reference-scoped): [`theme`](../src/modes/interactive/theme/theme.ts.md#theme), [`bg`](../src/modes/interactive/theme/theme.ts.md#Theme.bg)
- used by: (1 test-only callers)

### `ThemeFg`
- def: [`packages/coding-agent/test/ipython-cell-diff.test.ts:15`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/ipython-cell-diff.test.ts#L15)
- signature: `type ThemeFg`
- uses (calls/refs, reference-scoped): [`fg`](../src/modes/interactive/theme/theme.ts.md#Theme.fg), [`theme`](../src/modes/interactive/theme/theme.ts.md#theme)
- used by: (1 test-only callers)

## Functions
- `bgAnsi(color: ThemeBg)` — [`L22`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/ipython-cell-diff.test.ts#L22)
- `changedRow(rows: readonly string[], prefix: "-" | "+")` — [`L26`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/ipython-cell-diff.test.ts#L26)
- `fgAnsi(color: ThemeColor)` — [`L18`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/ipython-cell-diff.test.ts#L18)
- `hasBackground(line: string)` — [`L11`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/ipython-cell-diff.test.ts#L11)
- `renderCell(state: IPythonCellState)` — [`L32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/ipython-cell-diff.test.ts#L32)
- `stripAnsi(text: string)` — [`L7`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/ipython-cell-diff.test.ts#L7)


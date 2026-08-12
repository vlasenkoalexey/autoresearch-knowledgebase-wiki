---
title: 'Module: packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`keybinding-hints.ts`/
symbols:
  keyText: keyText().
  keyHint: keyHint().
  expandCollapseHint: expandCollapseHint().
  formatKeyText: formatKeyText().
  rawKeyHint: rawKeyHint().
  formatKeys: formatKeys().
  formatKeyPart: formatKeyPart().
  KeyTextOptions: KeyTextOptions#
  KeyTextOptions.primaryOnly: KeyTextOptions#primaryOnly.
  normalizeKeyPart: normalizeKeyPart().
  formatArrowKey: formatArrowKey().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts)

## Classes
### `KeyTextOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts:8`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts#L8)
- signature: `interface KeyTextOptions`
- members:
  - `primaryOnly` — [`L9`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts#L9)
- used by: [`keyText`](keybinding-hints.ts.md#keyText), [`keyHint`](keybinding-hints.ts.md#keyHint), [`formatKeys`](keybinding-hints.ts.md#formatKeys)

## Functions
- `expandCollapseHint(keybinding: keyof Keybindings, expanded: boolean)` — [`L70`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts#L70) — Canonical bracketed expand/collapse hint, e.g. `(Ctrl+O to expand)`, fully dim.
- `formatArrowKey(part: string)` — [`L16`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts#L16)
- `formatKeyPart(part: string, platform: Platform)` — [`L31`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts#L31)
- `formatKeyText(key: string, platform?: Platform)` — [`L42`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts#L42)
- `formatKeys(keys: KeyId[], options?: KeyTextOptions)` — [`L54`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts#L54)
- `keyHint(keybinding: keyof Keybindings, description: string, options?: KeyTextOptions)` — [`L65`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts#L65)
- `keyText(keybinding: keyof Keybindings, options?: KeyTextOptions)` — [`L61`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts#L61)
- `normalizeKeyPart(part: string)` — [`L12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts#L12)
- `rawKeyHint(key: string, description: string)` — [`L74`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/keybinding-hints.ts#L74)


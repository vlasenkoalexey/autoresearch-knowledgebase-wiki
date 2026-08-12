---
title: 'Module: packages/coding-agent/src/modes/interactive/components/show-images-selector.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/show-images-selector.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`show-images-selector.ts`/S
symbols:
  ShowImagesSelectorComponent.-constructor: howImagesSelectorComponent#`<constructor>`().
  SHOW_IMAGES_SELECT_LIST_LAYOUT: HOW_IMAGES_SELECT_LIST_LAYOUT.
  ShowImagesSelectorComponent.selectList: howImagesSelectorComponent#selectList.
  ShowImagesSelectorComponent.getSelectList: howImagesSelectorComponent#getSelectList().
  ShowImagesSelectorComponent: howImagesSelectorComponent#
---
# Module: [`packages/coding-agent/src/modes/interactive/components/show-images-selector.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/show-images-selector.ts)

## Classes
### `ShowImagesSelectorComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/show-images-selector.ts:13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/show-images-selector.ts#L13)
- doc: Component that renders a show images selector with borders
- signature: `class ShowImagesSelectorComponent`
- members:
  - `<constructor>(currentValue: boolean, onSelect: (show: boolean) => void, onCancel: () => void)` — [`L16`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/show-images-selector.ts#L16) — Component that renders a show images selector with borders
  - `getSelectList(method)` — [`L47`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/show-images-selector.ts#L47)
  - `selectList` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/show-images-selector.ts#L14)
- uses (calls/refs, reference-scoped): [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`<constructor>`](dynamic-border.ts.md#DynamicBorder.-constructor), [`<constructor>`](../../../../../tui/src/components/select-list.ts.md#SelectList.-constructor), [`getSelectListTheme`](../theme/theme.ts.md#getSelectListTheme), [`SelectItem`](../../../../../tui/src/components/select-list.ts.md#SelectItem), [`SelectList`](../../../../../tui/src/components/select-list.ts.md#SelectList), [`value`](../../../../../tui/src/components/select-list.ts.md#SelectItem.value), [`setSelectedIndex`](../../../../../tui/src/components/select-list.ts.md#SelectList.setSelectedIndex), [`onSelect`](../../../../../tui/src/components/select-list.ts.md#SelectList.onSelect), [`SHOW_IMAGES_SELECT_LIST_LAYOUT`](show-images-selector.ts.md#SHOW_IMAGES_SELECT_LIST_LAYOUT), [`onCancel`](../../../../../tui/src/components/select-list.ts.md#SelectList.onCancel), [`description`](../../../../../tui/src/components/select-list.ts.md#SelectItem.description), [`label`](../../../../../tui/src/components/select-list.ts.md#SelectItem.label)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts)

## Module values
- `SHOW_IMAGES_SELECT_LIST_LAYOUT` — [`L5`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/show-images-selector.ts#L5)


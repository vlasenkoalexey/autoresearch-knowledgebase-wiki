---
title: 'Module: packages/coding-agent/src/modes/interactive/components/theme-selector.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/theme-selector.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`theme-selector.ts`/T
symbols:
  ThemeSelectorComponent.-constructor: hemeSelectorComponent#`<constructor>`().
  ThemeSelectorComponent.selectList: hemeSelectorComponent#selectList.
  THEME_SELECT_LIST_LAYOUT: HEME_SELECT_LIST_LAYOUT.
  ThemeSelectorComponent.getSelectList: hemeSelectorComponent#getSelectList().
  ThemeSelectorComponent: hemeSelectorComponent#
  ThemeSelectorComponent.onPreview: hemeSelectorComponent#onPreview.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/theme-selector.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/theme-selector.ts)

## Classes
### `ThemeSelectorComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/theme-selector.ts:13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/theme-selector.ts#L13)
- doc: Component that renders a theme selector
- signature: `class ThemeSelectorComponent`
- members:
  - `<constructor>(currentTheme: string, onSelect: (themeName: string) => void, onCancel: () => void, onPreview: (themeName: string) => void)` — [`L17`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/theme-selector.ts#L17) — Component that renders a theme selector
  - `getSelectList(method)` — [`L64`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/theme-selector.ts#L64)
  - `onPreview` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/theme-selector.ts#L15)
  - `selectList` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/theme-selector.ts#L14)
- uses (calls/refs, reference-scoped): [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`<constructor>`](dynamic-border.ts.md#DynamicBorder.-constructor), [`<constructor>`](../../../../../tui/src/components/select-list.ts.md#SelectList.-constructor), [`getSelectListTheme`](../theme/theme.ts.md#getSelectListTheme), [`SelectItem`](../../../../../tui/src/components/select-list.ts.md#SelectItem), [`SelectList`](../../../../../tui/src/components/select-list.ts.md#SelectList), [`value`](../../../../../tui/src/components/select-list.ts.md#SelectItem.value), [`setSelectedIndex`](../../../../../tui/src/components/select-list.ts.md#SelectList.setSelectedIndex), [`getAvailableThemes`](../theme/theme.ts.md#getAvailableThemes), [`onSelect`](../../../../../tui/src/components/select-list.ts.md#SelectList.onSelect), [`THEME_SELECT_LIST_LAYOUT`](theme-selector.ts.md#THEME_SELECT_LIST_LAYOUT), [`onCancel`](../../../../../tui/src/components/select-list.ts.md#SelectList.onCancel), [`onSelectionChange`](../../../../../tui/src/components/select-list.ts.md#SelectList.onSelectionChange)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts)

## Module values
- `THEME_SELECT_LIST_LAYOUT` — [`L5`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/theme-selector.ts#L5)


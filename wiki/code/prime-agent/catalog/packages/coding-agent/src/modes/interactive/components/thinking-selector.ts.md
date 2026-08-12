---
title: 'Module: packages/coding-agent/src/modes/interactive/components/thinking-selector.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/thinking-selector.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`thinking-selector.ts`/
symbols:
  ThinkingSelectorComponent.-constructor: ThinkingSelectorComponent#`<constructor>`().
  ThinkingSelectorComponent.getSelectList: ThinkingSelectorComponent#getSelectList().
  ThinkingSelectorComponent: ThinkingSelectorComponent#
  THINKING_SELECT_LIST_LAYOUT: THINKING_SELECT_LIST_LAYOUT.
  ThinkingSelectorComponent.selectList: ThinkingSelectorComponent#selectList.
  LEVEL_DESCRIPTIONS: LEVEL_DESCRIPTIONS.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/thinking-selector.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/thinking-selector.ts)

## Classes
### `ThinkingSelectorComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/thinking-selector.ts:24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/thinking-selector.ts#L24)
- doc: Component that renders a thinking level selector with borders
- signature: `class ThinkingSelectorComponent`
- members:
  - `<constructor>(currentLevel: ThinkingLevel, availableLevels: ThinkingLevel[], onSelect: (level: ThinkingLevel) => void, onCancel: () => void)` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/thinking-selector.ts#L27) — Component that renders a thinking level selector with borders
  - `getSelectList(method)` — [`L72`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/thinking-selector.ts#L72)
  - `selectList` — [`L25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/thinking-selector.ts#L25)
- uses (calls/refs, reference-scoped): [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`ThinkingLevel`](../../../../../agent/src/types.ts.md#ThinkingLevel), [`<constructor>`](dynamic-border.ts.md#DynamicBorder.-constructor), [`<constructor>`](../../../../../tui/src/components/select-list.ts.md#SelectList.-constructor), [`getSelectListTheme`](../theme/theme.ts.md#getSelectListTheme), [`SelectItem`](../../../../../tui/src/components/select-list.ts.md#SelectItem), [`SelectList`](../../../../../tui/src/components/select-list.ts.md#SelectList), [`value`](../../../../../tui/src/components/select-list.ts.md#SelectItem.value), [`setSelectedIndex`](../../../../../tui/src/components/select-list.ts.md#SelectList.setSelectedIndex), [`onSelect`](../../../../../tui/src/components/select-list.ts.md#SelectList.onSelect), [`THINKING_SELECT_LIST_LAYOUT`](thinking-selector.ts.md#THINKING_SELECT_LIST_LAYOUT), [`onCancel`](../../../../../tui/src/components/select-list.ts.md#SelectList.onCancel), [`LEVEL_DESCRIPTIONS`](thinking-selector.ts.md#LEVEL_DESCRIPTIONS)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`showThinkingSelector`](../interactive-mode.ts.md#InteractiveMode.showThinkingSelector)  (1 test-only)

## Module values
- `LEVEL_DESCRIPTIONS` — [`L11`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/thinking-selector.ts#L11)
- `THINKING_SELECT_LIST_LAYOUT` — [`L6`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/thinking-selector.ts#L6)


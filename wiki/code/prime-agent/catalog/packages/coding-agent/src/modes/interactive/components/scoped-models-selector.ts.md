---
title: 'Module: packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`scoped-models-selector.ts`/
symbols:
  ScopedModelsSelectorComponent.handleInput: ScopedModelsSelectorComponent#handleInput().
  ScopedModelsSelectorComponent.-constructor: ScopedModelsSelectorComponent#`<constructor>`().
  ScopedModelsSelectorComponent.updateList: ScopedModelsSelectorComponent#updateList().
  ScopedModelsSelectorComponent.refresh: ScopedModelsSelectorComponent#refresh().
  ScopedModelsSelectorComponent.enabledIds: ScopedModelsSelectorComponent#enabledIds.
  ScopedModelsSelectorComponent.filteredItems: ScopedModelsSelectorComponent#filteredItems.
  ScopedModelsSelectorComponent.getFooterText: ScopedModelsSelectorComponent#getFooterText().
  ScopedModelsSelectorComponent.buildItems: ScopedModelsSelectorComponent#buildItems().
  ScopedModelsSelectorComponent.selectedIndex: ScopedModelsSelectorComponent#selectedIndex.
  ScopedModelsSelectorComponent.searchInput: ScopedModelsSelectorComponent#searchInput.
  ScopedModelsSelectorComponent.notifyChange: ScopedModelsSelectorComponent#notifyChange().
  EnabledIds: EnabledIds#
  ScopedModelsSelectorComponent.listContainer: ScopedModelsSelectorComponent#listContainer.
  ModelItem.model: ModelItem#model.
  ScopedModelsSelectorComponent: ScopedModelsSelectorComponent#
  ScopedModelsSelectorComponent.allIds: ScopedModelsSelectorComponent#allIds.
  ScopedModelsSelectorComponent.-set-focused: ScopedModelsSelectorComponent#`<set>focused`().
  ScopedModelsSelectorComponent.callbacks: ScopedModelsSelectorComponent#callbacks.
  ScopedModelsSelectorComponent.isDirty: ScopedModelsSelectorComponent#isDirty.
  ModelsConfig.allModels: ModelsConfig#allModels.
  ScopedModelsSelectorComponent.modelsById: ScopedModelsSelectorComponent#modelsById.
  ScopedModelsSelectorComponent.footerText: ScopedModelsSelectorComponent#footerText.
  ModelItem.fullId: ModelItem#fullId.
  isEnabled: isEnabled().
  ModelsConfig.enabledModelIds: ModelsConfig#enabledModelIds.
  ModelsCallbacks.onCancel: ModelsCallbacks#onCancel.
  ScopedModelsSelectorComponent.getSearchInput: ScopedModelsSelectorComponent#getSearchInput().
  enableAll: enableAll().
  clearAll: clearAll().
  ModelsCallbacks.onChange: ModelsCallbacks#onChange.
  ModelsCallbacks.onPersist: ModelsCallbacks#onPersist.
  toggle: toggle().
  move: move().
  getSortedIds: getSortedIds().
  ModelsCallbacks: ModelsCallbacks#
  ScopedModelsSelectorComponent.maxVisible: ScopedModelsSelectorComponent#maxVisible.
  ScopedModelsSelectorComponent.-get-focused: ScopedModelsSelectorComponent#`<get>focused`().
  ModelItem: ModelItem#
  ModelsConfig: ModelsConfig#
  ScopedModelsSelectorComponent.searchQuery: ScopedModelsSelectorComponent#searchQuery.
  ScopedModelsSelectorComponent._focused: ScopedModelsSelectorComponent#_focused.
  ModelItem.enabled: ModelItem#enabled.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts)

## Classes
### `EnabledIds`
- def: [`packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts:18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L18)
- signature: `type EnabledIds`
- used by: [`enabledIds`](scoped-models-selector.ts.md#ScopedModelsSelectorComponent.enabledIds), [`isEnabled`](scoped-models-selector.ts.md#isEnabled), [`clearAll`](scoped-models-selector.ts.md#clearAll), [`enableAll`](scoped-models-selector.ts.md#enableAll), [`getSortedIds`](scoped-models-selector.ts.md#getSortedIds), [`move`](scoped-models-selector.ts.md#move), [`toggle`](scoped-models-selector.ts.md#toggle)

### `ModelItem`
- def: [`packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts:67`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L67)
- signature: `interface ModelItem`
- members:
  - `enabled` — [`L70`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L70)
  - `fullId` — [`L68`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L68)
  - `model` — [`L69`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L69)
- uses (calls/refs, reference-scoped): [`Model`](../../../../../ai/src/types.ts.md#Model)
- used by: [`handleInput`](scoped-models-selector.ts.md#ScopedModelsSelectorComponent.handleInput), [`updateList`](scoped-models-selector.ts.md#ScopedModelsSelectorComponent.updateList), [`refresh`](scoped-models-selector.ts.md#ScopedModelsSelectorComponent.refresh), [`filteredItems`](scoped-models-selector.ts.md#ScopedModelsSelectorComponent.filteredItems), [`buildItems`](scoped-models-selector.ts.md#ScopedModelsSelectorComponent.buildItems)

### `ModelsCallbacks`
- def: [`packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts:78`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L78)
- signature: `interface ModelsCallbacks`
- members:
  - `onCancel` — [`L83`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L83)
  - `onChange` — [`L80`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L80) — Called whenever the enabled model set or order changes (session-only, no persist)
  - `onPersist` — [`L82`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L82) — Called when user wants to persist current selection to settings
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`handleInput`](scoped-models-selector.ts.md#ScopedModelsSelectorComponent.handleInput), [`showModelsSelector`](../interactive-mode.ts.md#InteractiveMode.showModelsSelector), [`<constructor>`](scoped-models-selector.ts.md#ScopedModelsSelectorComponent.-constructor), [`notifyChange`](scoped-models-selector.ts.md#ScopedModelsSelectorComponent.notifyChange), [`callbacks`](scoped-models-selector.ts.md#ScopedModelsSelectorComponent.callbacks)  (2 test-only)

### `ModelsConfig`
- def: [`packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts:73`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L73)
- signature: `interface ModelsConfig`
- members:
  - `allModels` — [`L74`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L74)
  - `enabledModelIds` — [`L75`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L75)
- uses (calls/refs, reference-scoped): [`Model`](../../../../../ai/src/types.ts.md#Model)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`showModelsSelector`](../interactive-mode.ts.md#InteractiveMode.showModelsSelector), [`<constructor>`](scoped-models-selector.ts.md#ScopedModelsSelectorComponent.-constructor)  (2 test-only)

### `ScopedModelsSelectorComponent`  ·  implements/extends Component, Container, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts:90`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L90)
- doc: Component for enabling/disabling models for Ctrl+P cycling.
- signature: `class ScopedModelsSelectorComponent`
- members:
  - `<constructor>(config: ModelsConfig, callbacks: ModelsCallbacks)` — [`L114`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L114) — Component for enabling/disabling models for Ctrl+P cycling.
  - `<get>focused` — [`L101`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L101) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `<set>focused` — [`L104`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L104) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `buildItems(method)` — [`L154`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L154)
  - `getFooterText(method)` — [`L165`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L165)
  - `getSearchInput(method)` — [`L355`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L355)
  - `handleInput(method)` — [`L237`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L237)
  - `notifyChange(method)` — [`L194`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L194)
  - `refresh(method)` — [`L183`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L183)
  - `updateList(method)` — [`L198`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L198)
  - `allIds` — [`L92`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L92)
  - `callbacks` — [`L110`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L110)
  - `enabledIds` — [`L93`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L93)
  - `filteredItems` — [`L94`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L94)
  - `footerText` — [`L109`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L109)
  - `isDirty` — [`L112`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L112)
  - `listContainer` — [`L108`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L108)
  - `maxVisible` — [`L111`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L111)
  - `modelsById` — [`L91`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L91)
  - `searchInput` — [`L97`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L97)
  - `searchQuery` — [`L96`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L96)
  - `selectedIndex` — [`L95`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L95)
- protocol/private: `_focused`[`L100`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L100)
- uses (calls/refs, reference-scoped): [`Model`](../../../../../ai/src/types.ts.md#Model), [`id`](../../../../../ai/src/types.ts.md#Model.id), [`provider`](../../../../../ai/src/types.ts.md#Model.provider), [`name`](../../../../../ai/src/types.ts.md#Model.name), [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`matchesKey`](../../../../../tui/src/keys.ts.md#matchesKey), [`handleInput`](../../../../../tui/src/components/input.ts.md#Input.handleInput), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`keyText`](keybinding-hints.ts.md#keyText), [`getValue`](../../../../../tui/src/components/input.ts.md#Input.getValue), [`bold`](../theme/theme.ts.md#Theme.bold), [`Text`](../../../../../tui/src/components/text.ts.md#Text), [`Input`](../../../../../tui/src/components/input.ts.md#Input), [`clear`](../../../../../tui/src/tui.ts.md#Container.clear), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`Key`](../../../../../tui/src/keys.ts.md#Key), [`setValue`](../../../../../tui/src/components/input.ts.md#Input.setValue), [`<constructor>`](dynamic-border.ts.md#DynamicBorder.-constructor), [`fuzzyFilter`](../../../../../tui/src/fuzzy.ts.md#fuzzyFilter), [`setText`](../../../../../tui/src/components/text.ts.md#Text.setText), [`EnabledIds`](scoped-models-selector.ts.md#EnabledIds), [`model`](scoped-models-selector.ts.md#ModelItem.model), [`focused`](../../../../../tui/src/components/input.ts.md#Input.focused), [`allModels`](scoped-models-selector.ts.md#ModelsConfig.allModels), [`fullId`](scoped-models-selector.ts.md#ModelItem.fullId), [`isEnabled`](scoped-models-selector.ts.md#isEnabled), [`enabledModelIds`](scoped-models-selector.ts.md#ModelsConfig.enabledModelIds), [`onCancel`](scoped-models-selector.ts.md#ModelsCallbacks.onCancel), [`clearAll`](scoped-models-selector.ts.md#clearAll), [`enableAll`](scoped-models-selector.ts.md#enableAll), [`onChange`](scoped-models-selector.ts.md#ModelsCallbacks.onChange), [`onPersist`](scoped-models-selector.ts.md#ModelsCallbacks.onPersist), [`getSortedIds`](scoped-models-selector.ts.md#getSortedIds), [`move`](scoped-models-selector.ts.md#move)  (+5 more)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`showModelsSelector`](../interactive-mode.ts.md#InteractiveMode.showModelsSelector)  (2 test-only)

## Functions
- `clearAll(enabledIds: EnabledIds, allIds: string[], targetIds?: string[] | undefined)` — [`L41`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L41)
- `enableAll(enabledIds: EnabledIds, allIds: string[], targetIds?: string[] | undefined)` — [`L31`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L31)
- `getSortedIds(enabledIds: EnabledIds, allIds: string[])` — [`L61`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L61)
- `isEnabled(enabledIds: EnabledIds, id: string)` — [`L20`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L20)
- `move(enabledIds: EnabledIds, id: string, delta: number)` — [`L49`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L49)
- `toggle(enabledIds: EnabledIds, id: string)` — [`L24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/scoped-models-selector.ts#L24)


---
title: 'Module: packages/coding-agent/src/modes/interactive/components/model-selector.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/model-selector.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`model-selector.ts`/
symbols:
  ModelSelectorComponent.-constructor: ModelSelectorComponent#`<constructor>`().
  ModelSelectorComponent.updateList: ModelSelectorComponent#updateList().
  ModelSelectorComponent.updateResponsiveLayout: ModelSelectorComponent#updateResponsiveLayout().
  ModelSelectorComponent.loadModels: ModelSelectorComponent#loadModels().
  ModelSelectorComponent.handleInput: ModelSelectorComponent#handleInput().
  ModelSelectorComponent.updateState: ModelSelectorComponent#updateState().
  ModelSelectorComponent.setScope: ModelSelectorComponent#setScope().
  ModelSelectorComponent.filterModels: ModelSelectorComponent#filterModels().
  ModelSelectorComponent.render: ModelSelectorComponent#render().
  ModelSelectorComponent.sortModels: ModelSelectorComponent#sortModels().
  ModelSelectorComponent.listLayout: ModelSelectorComponent#listLayout.
  ModelSelectorComponent.filteredModels: ModelSelectorComponent#filteredModels.
  ModelSelectorComponent.isProviderConfigured: ModelSelectorComponent#isProviderConfigured().
  ModelSelectorComponent.selectedIndex: ModelSelectorComponent#selectedIndex.
  ScopedModelItem.model: ScopedModelItem#model.
  ModelSelectorComponent: ModelSelectorComponent#
  ModelSelectorComponent.recentRankOf: ModelSelectorComponent#recentRankOf().
  ModelSelectorComponent.searchInput: ModelSelectorComponent#searchInput.
  ModelSelectorComponent.-set-focused: ModelSelectorComponent#`<set>focused`().
  ModelItem.model: ModelItem#model.
  ModelSelectorComponent.handleConfirm: ModelSelectorComponent#handleConfirm().
  ModelSelectorComponent.listContainer: ModelSelectorComponent#listContainer.
  ModelSelectorComponent.currentModel: ModelSelectorComponent#currentModel.
  ModelSelectorComponent.scope: ModelSelectorComponent#scope.
  ModelSelectorComponent.panel: ModelSelectorComponent#panel.
  ModelSelectorComponent.updateAvailableModels: ModelSelectorComponent#updateAvailableModels().
  ModelItem: ModelItem#
  ModelSelectorComponent.activeModels: ModelSelectorComponent#activeModels.
  ModelSelectorComponent.availableModels: ModelSelectorComponent#availableModels.
  ModelSelectorComponent.headerHelpContainer: ModelSelectorComponent#headerHelpContainer.
  ModelSelectorComponent.getModelKey: ModelSelectorComponent#getModelKey().
  ModelSelectorComponent.getScopeText: ModelSelectorComponent#getScopeText().
  ModelSelectorComponent.getScopeHintText: ModelSelectorComponent#getScopeHintText().
  ModelSelectorComponent.modelRegistry: ModelSelectorComponent#modelRegistry.
  ModelSelectorComponent.getSelectedModelKey: ModelSelectorComponent#getSelectedModelKey().
  ModelSelectorComponent.getSearchInput: ModelSelectorComponent#getSearchInput().
  ModelSelectorComponent.shouldShowSelectedDetails: ModelSelectorComponent#shouldShowSelectedDetails().
  ModelSelectorComponent.scopedModelItems: ModelSelectorComponent#scopedModelItems.
  ModelSelectorComponent.scopeText: ModelSelectorComponent#scopeText.
  ModelSelectorComponent.scopeHintText: ModelSelectorComponent#scopeHintText.
  ModelItem.provider: ModelItem#provider.
  ModelSelectorComponent.hasRows: ModelSelectorComponent#hasRows().
  ModelSelectorComponent.allModels: ModelSelectorComponent#allModels.
  ModelSelectorComponent.scopedModels: ModelSelectorComponent#scopedModels.
  ModelSelectorComponent.getSelectableCount: ModelSelectorComponent#getSelectableCount().
  ModelItem.id: ModelItem#id.
  ModelSelectorComponent.handleSelect: ModelSelectorComponent#handleSelect().
  ModelSelectorComponent.shouldShowHeaderHelp: ModelSelectorComponent#shouldShowHeaderHelp().
  ModelSelectorOptions.header: ModelSelectorOptions#header.
  ModelSelectorComponent.-get-focused: ModelSelectorComponent#`<get>focused`().
  ModelSelectorComponent.tui: ModelSelectorComponent#tui.
  ModelSelectorComponent.warningText: ModelSelectorComponent#warningText.
  ModelSelectorComponent.viewport: ModelSelectorComponent#viewport.
  ModelSelectorComponent.errorMessage: ModelSelectorComponent#errorMessage.
  ModelSelectorComponent.onSelectCallback: ModelSelectorComponent#onSelectCallback.
  ModelSelectorComponent.configuredProviders: ModelSelectorComponent#configuredProviders.
  ModelSelectorOptions.availableModels: ModelSelectorOptions#availableModels.
  ModelScope: ModelScope#
  MODEL_LIST_RESERVED_ROWS: MODEL_LIST_RESERVED_ROWS.
  ModelSelectorComponent.responsiveLayoutKey: ModelSelectorComponent#responsiveLayoutKey.
  ScopedModelItem: ScopedModelItem#
  PREFERRED_VISIBLE_MODELS: PREFERRED_VISIBLE_MODELS.
  ModelSelectorComponent._focused: ModelSelectorComponent#_focused.
  ModelSelectorComponent.searchQuery: ModelSelectorComponent#searchQuery.
  ModelSelectorComponent.onCancelCallback: ModelSelectorComponent#onCancelCallback.
  ModelSelectorComponent.recentRank: ModelSelectorComponent#recentRank.
  ModelSelectorComponent.getHeaderRows: ModelSelectorComponent#getHeaderRows.
  ModelSelectorOptions: ModelSelectorOptions#
  ModelSelectorOptions.configuredProviders: ModelSelectorOptions#configuredProviders.
  ModelSelectorOptions.getHeaderRows: ModelSelectorOptions#getHeaderRows.
  ModelSelectorOptions.subtitle: ModelSelectorOptions#subtitle.
  ModelSelectorOptions.getRows: ModelSelectorOptions#getRows.
  ModelSelectorOptions.recentModels: ModelSelectorOptions#recentModels.
  MODEL_SCROLL_INDICATOR_ROWS: MODEL_SCROLL_INDICATOR_ROWS.
  MODEL_HELP_MIN_ROWS: MODEL_HELP_MIN_ROWS.
  MODEL_DETAIL_MIN_ROWS: MODEL_DETAIL_MIN_ROWS.
  ScopedModelItem.thinkingLevel: ScopedModelItem#thinkingLevel.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/model-selector.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts)

## Classes
### `ModelItem`
- def: [`packages/coding-agent/src/modes/interactive/components/model-selector.ts:25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L25)
- signature: `interface ModelItem`
- members:
  - `id` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L27)
  - `model` — [`L28`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L28)
  - `provider` — [`L26`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L26)
- uses (calls/refs, reference-scoped): [`Model`](../../../../../ai/src/types.ts.md#Model)
- used by: [`updateList`](model-selector.ts.md#ModelSelectorComponent.updateList), [`loadModels`](model-selector.ts.md#ModelSelectorComponent.loadModels), [`setScope`](model-selector.ts.md#ModelSelectorComponent.setScope), [`filterModels`](model-selector.ts.md#ModelSelectorComponent.filterModels), [`sortModels`](model-selector.ts.md#ModelSelectorComponent.sortModels), [`filteredModels`](model-selector.ts.md#ModelSelectorComponent.filteredModels), [`isProviderConfigured`](model-selector.ts.md#ModelSelectorComponent.isProviderConfigured), [`recentRankOf`](model-selector.ts.md#ModelSelectorComponent.recentRankOf), [`handleConfirm`](model-selector.ts.md#ModelSelectorComponent.handleConfirm), [`activeModels`](model-selector.ts.md#ModelSelectorComponent.activeModels), [`getModelKey`](model-selector.ts.md#ModelSelectorComponent.getModelKey), [`scopedModelItems`](model-selector.ts.md#ModelSelectorComponent.scopedModelItems), [`allModels`](model-selector.ts.md#ModelSelectorComponent.allModels)

### `ModelScope`
- def: [`packages/coding-agent/src/modes/interactive/components/model-selector.ts:46`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L46)
- signature: `type ModelScope`
- used by: [`handleInput`](model-selector.ts.md#ModelSelectorComponent.handleInput), [`setScope`](model-selector.ts.md#ModelSelectorComponent.setScope), [`scope`](model-selector.ts.md#ModelSelectorComponent.scope)

### `ModelSelectorComponent`  ·  implements/extends Component, Container, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/model-selector.ts:60`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L60)
- doc: Component that renders a model selector with search
- signature: `class ModelSelectorComponent`
- members:
  - `<constructor>(tui: TUI, currentModel: Model<any> | undefined, modelRegistry: ModelRegistry, scopedModels: readonly ScopedModelItem[], onSelect: (model: Model<any>) => void, onCancel: () => void, initialSearchInput?: string | undefined, options?: ModelSelectorOptions)` — [`L105`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L105) — Component that renders a model selector with search
  - `<get>focused` — [`L65`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L65) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `<set>focused` — [`L68`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L68) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `filterModels(method)` — [`L320`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L320)
  - `getModelKey(method)` — [`L260`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L260)
  - `getScopeHintText(method)` — [`L304`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L304)
  - `getScopeText(method)` — [`L298`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L298)
  - `getSearchInput(method)` — [`L469`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L469)
  - `getSelectableCount(method)` — [`L465`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L465)
  - `getSelectedModelKey(method)` — [`L264`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L264)
  - `handleConfirm(method)` — [`L457`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L457)
  - `handleInput(method)` — [`L412`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L412)
  - `handleSelect(method)` — [`L453`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L453)
  - `hasRows(method)` — [`L523`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L523)
  - `isProviderConfigured(method)` — [`L274`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L274)
  - `loadModels(method)` — [`L206`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L206)
  - `recentRankOf(method)` — [`L269`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L269)
  - `render(method)` — [`L343`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L343) — Render the component to lines for the given viewport width
  - `setScope(method)` — [`L308`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L308)
  - `shouldShowHeaderHelp(method)` — [`L515`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L515)
  - `shouldShowSelectedDetails(method)` — [`L519`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L519)
  - `sortModels(method)` — [`L278`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L278)
  - `updateAvailableModels(method)` — [`L177`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L177)
  - `updateList(method)` — [`L352`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L352)
  - `updateResponsiveLayout(method)` — [`L473`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L473)
  - `updateState(method)` — [`L181`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L181)
  - `activeModels` — [`L75`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L75)
  - `allModels` — [`L73`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L73)
  - `availableModels` — [`L83`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L83)
  - `configuredProviders` — [`L84`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L84)
  - `currentModel` — [`L79`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L79)
  - `errorMessage` — [`L86`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L86)
  - `filteredModels` — [`L76`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L76)
  - `getHeaderRows` — [`L103`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L103)
  - `headerHelpContainer` — [`L93`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L93)
  - `listContainer` — [`L72`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L72)
  - `listLayout` — [`L95`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L95)
  - `modelRegistry` — [`L80`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L80)
  - `onCancelCallback` — [`L82`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L82)
  - `onSelectCallback` — [`L81`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L81)
  - `panel` — [`L92`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L92)
  - `recentRank` — [`L85`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L85)
  - `responsiveLayoutKey` — [`L101`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L101)
  - `scope` — [`L89`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L89)
  - `scopeHintText` — [`L91`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L91)
  - `scopeText` — [`L90`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L90)
  - `scopedModelItems` — [`L74`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L74)
  - `scopedModels` — [`L88`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L88)
  - `searchInput` — [`L61`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L61)
  - `searchQuery` — [`L78`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L78)
  - `selectedIndex` — [`L77`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L77)
  - `tui` — [`L87`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L87)
  - `viewport` — [`L102`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L102)
  - `warningText` — [`L94`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L94)
- protocol/private: `_focused`[`L64`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L64)
- uses (calls/refs, reference-scoped): [`Model`](../../../../../ai/src/types.ts.md#Model), [`id`](../../../../../ai/src/types.ts.md#Model.id), [`provider`](../../../../../ai/src/types.ts.md#Model.provider), [`name`](../../../../../ai/src/types.ts.md#Model.name), [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`requestRender`](../../../../../tui/src/tui.ts.md#TUI.requestRender), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`ModelRegistry`](../../../core/model-registry.ts.md#ModelRegistry), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`TUI`](../../../../../tui/src/tui.ts.md#TUI), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`render`](../../../../../tui/src/tui.ts.md#Container.render), [`Text`](../../../../../tui/src/components/text.ts.md#Text), [`clear`](../../../../../tui/src/tui.ts.md#Container.clear), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`refresh`](../../../core/model-registry.ts.md#ModelRegistry.refresh), [`find`](../../../core/model-registry.ts.md#ModelRegistry.find), [`getMenuListLayout`](menu-panel.ts.md#getMenuListLayout), [`keyHint`](keybinding-hints.ts.md#keyHint), [`featured`](../../../../../ai/src/types.ts.md#Model.featured), [`getAvailable`](../../../core/model-registry.ts.md#ModelRegistry.getAvailable), [`modelsAreEqual`](../../../../../ai/src/models.ts.md#modelsAreEqual), [`visibleItems`](menu-panel.ts.md#MenuListLayout.visibleItems), [`setText`](../../../../../tui/src/components/text.ts.md#Text.setText), [`hasConfiguredAuth`](../../../core/model-registry.ts.md#ModelRegistry.hasConfiguredAuth), [`fuzzyFilterScored`](../../../../../tui/src/fuzzy.ts.md#fuzzyFilterScored), [`MenuSearchInput`](menu-panel.ts.md#MenuSearchInput), [`compact`](menu-panel.ts.md#MenuListLayout.compact), [`<constructor>`](menu-panel.ts.md#MenuPanel.-constructor), [`getValue`](menu-panel.ts.md#MenuSearchInput.getValue), [`getRows`](menu-panel.ts.md#MenuViewportProvider.getRows), [`shouldTreatAsBack`](modal-back.ts.md#shouldTreatAsBack), [`model`](model-selector.ts.md#ScopedModelItem.model), [`reservedRows`](menu-panel.ts.md#MenuListLayoutOptions.reservedRows), [`getError`](../../../core/model-registry.ts.md#ModelRegistry.getError), [`compactItemRows`](menu-panel.ts.md#MenuListLayoutOptions.compactItemRows)  (+41 more)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`render`](../../../../../tui/src/tui.ts.md#Container.render), [`<constructor>`](configuration-menu.ts.md#ConfigurationMenuComponent.-constructor), [`configuration-menu.ts`](configuration-menu.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-configuration-menu.ts), [`handleInput`](configuration-menu.ts.md#ConfigurationMenuComponent.handleInput), [`setActiveTab`](configuration-menu.ts.md#ConfigurationMenuComponent.setActiveTab), [`getSearchValue`](configuration-menu.ts.md#ConfigurationMenuComponent.getSearchValue), [`updateModels`](configuration-menu.ts.md#ConfigurationMenuComponent.updateModels), [`<get>activeBody`](configuration-menu.ts.md#ConfigurationMenuComponent.-get-activeBody), [`<set>focused`](configuration-menu.ts.md#ConfigurationMenuComponent.-set-focused), [`models`](configuration-menu.ts.md#ConfigurationMenuComponent.bodies.typeLiteral48.models)  (4 test-only)

### `ModelSelectorOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/model-selector.ts:36`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L36)
- signature: `interface ModelSelectorOptions`
- members:
  - `availableModels` — [`L37`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L37)
  - `configuredProviders` — [`L38`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L38)
  - `getHeaderRows` — [`L40`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L40)
  - `getRows` — [`L42`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L42)
  - `header` — [`L39`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L39)
  - `recentModels` — [`L43`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L43)
  - `subtitle` — [`L41`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L41)
- uses (calls/refs, reference-scoped): [`Model`](../../../../../ai/src/types.ts.md#Model), [`Component`](../../../../../tui/src/tui.ts.md#Component)
- used by: [`<constructor>`](model-selector.ts.md#ModelSelectorComponent.-constructor)

### `ScopedModelItem`
- def: [`packages/coding-agent/src/modes/interactive/components/model-selector.ts:31`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L31)
- signature: `interface ScopedModelItem`
- members:
  - `model` — [`L32`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L32)
  - `thinkingLevel` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L33)
- uses (calls/refs, reference-scoped): [`Model`](../../../../../ai/src/types.ts.md#Model)
- used by: [`<constructor>`](model-selector.ts.md#ModelSelectorComponent.-constructor), [`loadModels`](model-selector.ts.md#ModelSelectorComponent.loadModels), [`scopedModels`](model-selector.ts.md#ModelSelectorComponent.scopedModels)  (2 test-only)

## Module values
- `MODEL_DETAIL_MIN_ROWS` — [`L55`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L55)
- `MODEL_HELP_MIN_ROWS` — [`L54`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L54)
- `MODEL_LIST_RESERVED_ROWS` — [`L49`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L49)
- `MODEL_SCROLL_INDICATOR_ROWS` — [`L53`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L53)
- `PREFERRED_VISIBLE_MODELS` — [`L48`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/model-selector.ts#L48)


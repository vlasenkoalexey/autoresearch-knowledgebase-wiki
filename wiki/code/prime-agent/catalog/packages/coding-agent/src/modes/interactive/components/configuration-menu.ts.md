---
title: 'Module: packages/coding-agent/src/modes/interactive/components/configuration-menu.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/configuration-menu.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`configuration-menu.ts`/
symbols:
  ConfigurationMenuComponent.-constructor: ConfigurationMenuComponent#`<constructor>`().
  ConfigurationMenuComponent.handleInput: ConfigurationMenuComponent#handleInput().
  ConfigurationMenuComponent.setActiveTab: ConfigurationMenuComponent#setActiveTab().
  ConfigurationMenuComponent.getSearchValue: ConfigurationMenuComponent#getSearchValue().
  ConfigurationMenuTabBar.getLines: ConfigurationMenuTabBar#getLines().
  ConfigurationMenuComponent.render: ConfigurationMenuComponent#render().
  ConfigurationMenuComponent.updateModels: ConfigurationMenuComponent#updateModels().
  ConfigurationMenuComponent.-set-focused: ConfigurationMenuComponent#`<set>focused`().
  ConfigurationMenuComponent.-get-activeBody: ConfigurationMenuComponent#`<get>activeBody`().
  ConfigurationMenuComponent: ConfigurationMenuComponent#
  ConfigurationMenuTab: ConfigurationMenuTab#
  ConfigurationMenuComponent.refreshAuthentication: ConfigurationMenuComponent#refreshAuthentication().
  ConfigurationMenuComponent.getActiveTab: ConfigurationMenuComponent#getActiveTab().
  ConfigurationMenuComponent.activeTab: ConfigurationMenuComponent#activeTab.
  ConfigurationMenuComponent.switchTab: ConfigurationMenuComponent#switchTab().
  ConfigurationMenuOptions.currentModel: ConfigurationMenuOptions#currentModel.
  ConfigurationMenuOptions.availableModels: ConfigurationMenuOptions#availableModels.
  ConfigurationMenuOptions.onSelectModel: ConfigurationMenuOptions#onSelectModel.
  ConfigurationMenuOptions.modelRegistry: ConfigurationMenuOptions#modelRegistry.
  ConfigurationMenuOptions.authStorage: ConfigurationMenuOptions#authStorage.
  ConfigurationMenuOptions.providerOptions: ConfigurationMenuOptions#providerOptions.
  ConfigurationMenuOptions.initialTab: ConfigurationMenuOptions#initialTab.
  ConfigurationMenuOptions.tui: ConfigurationMenuOptions#tui.
  ConfigurationMenuOptions.scopedModels: ConfigurationMenuOptions#scopedModels.
  ConfigurationMenuOptions.onSelectProvider: ConfigurationMenuOptions#onSelectProvider.
  ConfigurationMenuOptions.onSelectMcpConnection: ConfigurationMenuOptions#onSelectMcpConnection.
  CONFIGURATION_MENU_TABS: CONFIGURATION_MENU_TABS.
  ConfigurationMenuOptions.onCancel: ConfigurationMenuOptions#onCancel.
  ConfigurationMenuTabBar.wrapItems: ConfigurationMenuTabBar#wrapItems().
  ConfigurationMenuComponent.bodies: ConfigurationMenuComponent#bodies.
  ConfigurationMenuScopedModel.model: ConfigurationMenuScopedModel#model.
  ConfigurationMenuOptions.getRows: ConfigurationMenuOptions#getRows.
  ConfigurationMenuOptions.requestRender: ConfigurationMenuOptions#requestRender.
  ConfigurationMenuComponent.bodies.typeLiteral48.providers: ConfigurationMenuComponent#bodies.typeLiteral48:providers.
  ConfigurationMenuComponent.bodies.typeLiteral48.models: ConfigurationMenuComponent#bodies.typeLiteral48:models.
  ConfigurationMenuComponent.bodies.typeLiteral48.-mcp-connections: ConfigurationMenuComponent#bodies.typeLiteral48:`"mcp-connections"`.
  ConfigurationMenuComponent.-get-focused: ConfigurationMenuComponent#`<get>focused`().
  ConfigurationMenuOptions.configuredProviders: ConfigurationMenuOptions#configuredProviders.
  TAB_LABELS: TAB_LABELS.
  ConfigurationMenuTabBar.-constructor: ConfigurationMenuTabBar#`<constructor>`().
  ConfigurationMenuTabBar.getRowCount: ConfigurationMenuTabBar#getRowCount().
  ConfigurationMenuOptions.initialModelSearch: ConfigurationMenuOptions#initialModelSearch.
  ConfigurationMenuComponent._focused: ConfigurationMenuComponent#_focused.
  ConfigurationMenuTabBar: ConfigurationMenuTabBar#
  ConfigurationMenuTabBar.render: ConfigurationMenuTabBar#render().
  ConfigurationMenuOptions.recentModels: ConfigurationMenuOptions#recentModels.
  ConfigurationMenuComponent.renderWidth: ConfigurationMenuComponent#renderWidth.
  ConfigurationMenuScopedModel: ConfigurationMenuScopedModel#
  ConfigurationMenuOptions: ConfigurationMenuOptions#
  ConfigurationMenuScopedModel.thinkingLevel: ConfigurationMenuScopedModel#thinkingLevel.
  ConfigurationMenuTabBar.invalidate: ConfigurationMenuTabBar#invalidate().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/configuration-menu.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts)

## Classes
### `ConfigurationMenuComponent`  ·  implements/extends Component, Container, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/configuration-menu.ts:105`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L105)
- signature: `class ConfigurationMenuComponent`
- members:
  - `<constructor>(options: ConfigurationMenuOptions)` — [`L115`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L115)
  - `<get>activeBody` — [`L249`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L249)
  - `<get>focused` — [`L183`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L183) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `<set>focused` — [`L187`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L187) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `getActiveTab(method)` — [`L197`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L197)
  - `getSearchValue(method)` — [`L201`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L201)
  - `handleInput(method)` — [`L229`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L229)
  - `refreshAuthentication(method)` — [`L215`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L215)
  - `render(method)` — [`L192`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L192) — Render the component to lines for the given viewport width
  - `setActiveTab(method)` — [`L205`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L205)
  - `switchTab(method)` — [`L253`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L253)
  - `updateModels(method)` — [`L221`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L221)
  - `"mcp-connections"` — [`L109`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L109)
  - `activeTab` — [`L111`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L111)
  - `bodies` — [`L106`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L106)
  - `models` — [`L108`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L108)
  - `providers` — [`L107`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L107)
  - `renderWidth` — [`L113`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L113)
- protocol/private: `_focused`[`L112`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L112)
- uses (calls/refs, reference-scoped): [`Model`](../../../../../ai/src/types.ts.md#Model), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`Api`](../../../../../ai/src/types.ts.md#Api), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`<constructor>`](model-selector.ts.md#ModelSelectorComponent.-constructor), [`<constructor>`](oauth-selector.ts.md#OAuthSelectorComponent.-constructor), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`render`](../../../../../tui/src/tui.ts.md#Container.render), [`clear`](../../../../../tui/src/tui.ts.md#Container.clear), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`handleInput`](model-selector.ts.md#ModelSelectorComponent.handleInput), [`handleInput`](oauth-selector.ts.md#OAuthSelectorComponent.handleInput), [`updateState`](model-selector.ts.md#ModelSelectorComponent.updateState), [`getProviderAuthStatus`](../../../core/model-registry.ts.md#ModelRegistry.getProviderAuthStatus), [`refresh`](oauth-selector.ts.md#OAuthSelectorComponent.refresh), [`category`](oauth-selector.ts.md#AuthSelectorProvider.typeLiteral0.category), [`getValue`](menu-panel.ts.md#MenuSearchInput.getValue), [`ConfigurationMenuTab`](configuration-menu.ts.md#ConfigurationMenuTab), [`ModelSelectorComponent`](model-selector.ts.md#ModelSelectorComponent), [`OAuthSelectorComponent`](oauth-selector.ts.md#OAuthSelectorComponent), [`<set>focused`](model-selector.ts.md#ModelSelectorComponent.-set-focused), [`<set>focused`](oauth-selector.ts.md#OAuthSelectorComponent.-set-focused), [`handleInput`](menu-panel.ts.md#MenuSearchInput.handleInput), [`availableModels`](configuration-menu.ts.md#ConfigurationMenuOptions.availableModels), [`currentModel`](configuration-menu.ts.md#ConfigurationMenuOptions.currentModel), [`onSelectModel`](configuration-menu.ts.md#ConfigurationMenuOptions.onSelectModel), [`modelRegistry`](configuration-menu.ts.md#ConfigurationMenuOptions.modelRegistry), [`getSearchInput`](model-selector.ts.md#ModelSelectorComponent.getSearchInput), [`authStorage`](configuration-menu.ts.md#ConfigurationMenuOptions.authStorage), [`providerOptions`](configuration-menu.ts.md#ConfigurationMenuOptions.providerOptions), [`getSearchInput`](oauth-selector.ts.md#OAuthSelectorComponent.getSearchInput), [`initialTab`](configuration-menu.ts.md#ConfigurationMenuOptions.initialTab), [`onSelectMcpConnection`](configuration-menu.ts.md#ConfigurationMenuOptions.onSelectMcpConnection), [`onSelectProvider`](configuration-menu.ts.md#ConfigurationMenuOptions.onSelectProvider), [`scopedModels`](configuration-menu.ts.md#ConfigurationMenuOptions.scopedModels), [`tui`](configuration-menu.ts.md#ConfigurationMenuOptions.tui), [`CONFIGURATION_MENU_TABS`](configuration-menu.ts.md#CONFIGURATION_MENU_TABS), [`onCancel`](configuration-menu.ts.md#ConfigurationMenuOptions.onCancel), [`<get>focused`](model-selector.ts.md#ModelSelectorComponent.-get-focused)  (+10 more)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`showConfigurationMenu`](../interactive-mode.ts.md#InteractiveMode.showConfigurationMenu), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`render`](../../../../../tui/src/tui.ts.md#Container.render)  (3 test-only)

### `ConfigurationMenuOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/configuration-menu.ts:28`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L28)
- signature: `interface ConfigurationMenuOptions`
- members:
  - `authStorage` — [`L31`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L31)
  - `availableModels` — [`L36`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L36)
  - `configuredProviders` — [`L37`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L37)
  - `currentModel` — [`L34`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L34)
  - `getRows` — [`L40`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L40)
  - `initialModelSearch` — [`L39`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L39)
  - `initialTab` — [`L29`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L29)
  - `modelRegistry` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L33)
  - `onCancel` — [`L45`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L45)
  - `onSelectMcpConnection` — [`L43`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L43)
  - `onSelectModel` — [`L44`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L44)
  - `onSelectProvider` — [`L42`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L42)
  - `providerOptions` — [`L32`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L32)
  - `recentModels` — [`L38`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L38)
  - `requestRender` — [`L41`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L41)
  - `scopedModels` — [`L35`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L35)
  - `tui` — [`L30`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L30)
- uses (calls/refs, reference-scoped): [`Model`](../../../../../ai/src/types.ts.md#Model), [`Api`](../../../../../ai/src/types.ts.md#Api), [`AuthStorage`](../../../core/auth-storage.ts.md#AuthStorage), [`ModelRegistry`](../../../core/model-registry.ts.md#ModelRegistry), [`TUI`](../../../../../tui/src/tui.ts.md#TUI), [`AuthSelectorProvider`](oauth-selector.ts.md#AuthSelectorProvider), [`ConfigurationMenuTab`](configuration-menu.ts.md#ConfigurationMenuTab), [`ConfigurationMenuScopedModel`](configuration-menu.ts.md#ConfigurationMenuScopedModel)
- used by: [`showConfigurationMenu`](../interactive-mode.ts.md#InteractiveMode.showConfigurationMenu), [`<constructor>`](configuration-menu.ts.md#ConfigurationMenuComponent.-constructor), [`setActiveTab`](configuration-menu.ts.md#ConfigurationMenuComponent.setActiveTab), [`refreshAuthentication`](configuration-menu.ts.md#ConfigurationMenuComponent.refreshAuthentication)  (1 test-only)

### `ConfigurationMenuScopedModel`
- def: [`packages/coding-agent/src/modes/interactive/components/configuration-menu.ts:23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L23)
- signature: `interface ConfigurationMenuScopedModel`
- members:
  - `model` — [`L24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L24)
  - `thinkingLevel` — [`L25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L25)
- uses (calls/refs, reference-scoped): [`Model`](../../../../../ai/src/types.ts.md#Model), [`Api`](../../../../../ai/src/types.ts.md#Api)
- used by: [`scopedModels`](configuration-menu.ts.md#ConfigurationMenuOptions.scopedModels)

### `ConfigurationMenuTab`
- def: [`packages/coding-agent/src/modes/interactive/components/configuration-menu.ts:21`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L21)
- signature: `type ConfigurationMenuTab`
- uses (calls/refs, reference-scoped): [`CONFIGURATION_MENU_TABS`](configuration-menu.ts.md#CONFIGURATION_MENU_TABS)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`showConfigurationMenu`](../interactive-mode.ts.md#InteractiveMode.showConfigurationMenu), [`setActiveTab`](configuration-menu.ts.md#ConfigurationMenuComponent.setActiveTab), [`getSearchValue`](configuration-menu.ts.md#ConfigurationMenuComponent.getSearchValue), [`getActiveTab`](configuration-menu.ts.md#ConfigurationMenuComponent.getActiveTab), [`activeTab`](configuration-menu.ts.md#ConfigurationMenuComponent.activeTab), [`initialTab`](configuration-menu.ts.md#ConfigurationMenuOptions.initialTab), [`<constructor>`](configuration-menu.ts.md#ConfigurationMenuTabBar.-constructor), [`TAB_LABELS`](configuration-menu.ts.md#TAB_LABELS)  (1 test-only)

### `ConfigurationMenuTabBar`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/configuration-menu.ts:54`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L54)
- signature: `class ConfigurationMenuTabBar`
- members:
  - `<constructor>(getActiveTab: () => "models" | "providers" | "mcp-connections")` — [`L55`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L55)
  - `getLines(method)` — [`L65`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L65)
  - `getRowCount(method)` — [`L61`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L61)
  - `invalidate(method)` — [`L102`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L102) — Invalidate any cached rendering state.
  - `render(method)` — [`L57`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L57) — Render the component to lines for the given viewport width
  - `wrapItems(method)` — [`L84`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L84)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`keyText`](keybinding-hints.ts.md#keyText), [`bold`](../theme/theme.ts.md#Theme.bold), [`wrapTextWithAnsi`](../../../../../tui/src/utils.ts.md#wrapTextWithAnsi), [`ConfigurationMenuTab`](configuration-menu.ts.md#ConfigurationMenuTab), [`CONFIGURATION_MENU_TABS`](configuration-menu.ts.md#CONFIGURATION_MENU_TABS), [`TAB_LABELS`](configuration-menu.ts.md#TAB_LABELS)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`<constructor>`](configuration-menu.ts.md#ConfigurationMenuComponent.-constructor)

## Module values
- `CONFIGURATION_MENU_TABS` — [`L19`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L19)
- `TAB_LABELS` — [`L48`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/configuration-menu.ts#L48)


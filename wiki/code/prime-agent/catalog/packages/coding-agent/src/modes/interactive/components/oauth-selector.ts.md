---
title: 'Module: packages/coding-agent/src/modes/interactive/components/oauth-selector.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/oauth-selector.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`oauth-selector.ts`/
symbols:
  OAuthSelectorComponent.-constructor: OAuthSelectorComponent#`<constructor>`().
  AuthSelectorProvider.typeLiteral0.id: AuthSelectorProvider#typeLiteral0:id.
  OAuthSelectorComponent.updateList: OAuthSelectorComponent#updateList().
  AuthSelectorProvider.typeLiteral0.authType: AuthSelectorProvider#typeLiteral0:authType.
  AuthSelectorProvider.typeLiteral0.name: AuthSelectorProvider#typeLiteral0:name.
  OAuthSelectorComponent.handleInput: OAuthSelectorComponent#handleInput().
  AuthSelectorProvider: AuthSelectorProvider#
  OAuthSelectorComponent.updateLayout: OAuthSelectorComponent#updateLayout().
  OAuthSelectorComponent.render: OAuthSelectorComponent#render().
  OAuthSelectorComponent.formatStatusIndicator: OAuthSelectorComponent#formatStatusIndicator().
  OAuthSelectorComponent.filterProviders: OAuthSelectorComponent#filterProviders().
  OAuthSelectorComponent.refresh: OAuthSelectorComponent#refresh().
  OAuthSelectorComponent.isProviderStale: OAuthSelectorComponent#isProviderStale().
  OAuthSelectorComponent.listLayout: OAuthSelectorComponent#listLayout.
  OAuthSelectorComponent.updateTabBar: OAuthSelectorComponent#updateTabBar().
  OAuthSelectorComponent.isProviderConfigured: OAuthSelectorComponent#isProviderConfigured().
  AuthSelectorProvider.typeLiteral0.category: AuthSelectorProvider#typeLiteral0:category.
  OAuthSelectorComponent.filteredProviders: OAuthSelectorComponent#filteredProviders.
  OAuthSelectorComponent.switchCategory: OAuthSelectorComponent#switchCategory().
  OAuthSelectorComponent.sortProviders: OAuthSelectorComponent#sortProviders().
  OAuthSelectorComponent.categories: OAuthSelectorComponent#categories.
  OAuthSelectorComponent.formatApiKeyStatusIndicator: OAuthSelectorComponent#formatApiKeyStatusIndicator().
  OAuthSelectorComponent: OAuthSelectorComponent#
  OAuthSelectorComponent.selectedIndex: OAuthSelectorComponent#selectedIndex.
  OAuthSelectorComponent.searchInput: OAuthSelectorComponent#searchInput.
  OAuthSelectorComponent.-set-focused: OAuthSelectorComponent#`<set>focused`().
  compareAuthSelectorProviders: compareAuthSelectorProviders().
  OAuthSelectorComponent.-get-reservedRows: OAuthSelectorComponent#`<get>reservedRows`().
  OAuthSelectorComponent.getProviderSortRank: OAuthSelectorComponent#getProviderSortRank().
  OAuthSelectorComponent.listContainer: OAuthSelectorComponent#listContainer.
  OAuthSelectorComponent.allProviders: OAuthSelectorComponent#allProviders.
  OAuthSelectorComponent.authStorage: OAuthSelectorComponent#authStorage.
  OAuthSelectorComponent.inActiveCategory: OAuthSelectorComponent#inActiveCategory().
  OAuthSelectorComponent.tabBar: OAuthSelectorComponent#tabBar.
  OAuthSelectorComponent.activeCategory: OAuthSelectorComponent#activeCategory.
  AuthSelectorCategory: AuthSelectorCategory#
  OAuthSelectorComponent.getSearchInput: OAuthSelectorComponent#getSearchInput().
  OAuthSelectorComponent.getAuthStatus: OAuthSelectorComponent#getAuthStatus.
  OAuthSelectorOptions.initialCategory: OAuthSelectorOptions#initialCategory.
  OAuthSelectorOptions.header: OAuthSelectorOptions#header.
  OAuthSelectorComponent.-get-focused: OAuthSelectorComponent#`<get>focused`().
  OAuthSelectorComponent.onSelectCallback: OAuthSelectorComponent#onSelectCallback.
  OAuthSelectorComponent.viewport: OAuthSelectorComponent#viewport.
  OAuthSelectorOptions: OAuthSelectorOptions#
  OAuthSelectorComponent.mode: OAuthSelectorComponent#mode.
  PREFERRED_VISIBLE_PROVIDERS: PREFERRED_VISIBLE_PROVIDERS.
  PROVIDER_LIST_RESERVED_ROWS: PROVIDER_LIST_RESERVED_ROWS.
  TAB_BAR_RESERVED_ROWS: TAB_BAR_RESERVED_ROWS.
  OAuthSelectorComponent._focused: OAuthSelectorComponent#_focused.
  OAuthSelectorComponent.searchQuery: OAuthSelectorComponent#searchQuery.
  OAuthSelectorComponent.onCancelCallback: OAuthSelectorComponent#onCancelCallback.
  OAuthSelectorComponent.getHeaderRows: OAuthSelectorComponent#getHeaderRows.
  OAuthSelectorOptions.getHeaderRows: OAuthSelectorOptions#getHeaderRows.
  OAuthSelectorOptions.title: OAuthSelectorOptions#title.
  OAuthSelectorOptions.subtitle: OAuthSelectorOptions#subtitle.
  OAuthSelectorOptions.searchPlaceholder: OAuthSelectorOptions#searchPlaceholder.
  PROVIDER_SCROLL_INDICATOR_ROWS: PROVIDER_SCROLL_INDICATOR_ROWS.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/oauth-selector.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts)

## Classes
### `AuthSelectorCategory`
- def: [`packages/coding-agent/src/modes/interactive/components/oauth-selector.ts:22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L22)
- signature: `type AuthSelectorCategory`
- used by: [`auth-flows.ts`](../auth-flows.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-auth-flows.ts), [`updateTabBar`](oauth-selector.ts.md#OAuthSelectorComponent.updateTabBar), [`category`](oauth-selector.ts.md#AuthSelectorProvider.typeLiteral0.category), [`categories`](oauth-selector.ts.md#OAuthSelectorComponent.categories), [`activeCategory`](oauth-selector.ts.md#OAuthSelectorComponent.activeCategory), [`initialCategory`](oauth-selector.ts.md#OAuthSelectorOptions.initialCategory), [`ProviderLoginOptions`](../auth-flows.ts.md#ProviderLoginOptions)

### `AuthSelectorProvider`
- def: [`packages/coding-agent/src/modes/interactive/components/oauth-selector.ts:24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L24)
- signature: `type AuthSelectorProvider`
- members:
  - `authType` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L27)
  - `category` — [`L29`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L29) — Which tab the entry belongs to. Defaults to "provider" when omitted.
  - `id` — [`L25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L25)
  - `name` — [`L26`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L26)
- uses (calls/refs, reference-scoped): [`AuthSelectorCategory`](oauth-selector.ts.md#AuthSelectorCategory)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`showConfigurationMenu`](../interactive-mode.ts.md#InteractiveMode.showConfigurationMenu), [`<constructor>`](oauth-selector.ts.md#OAuthSelectorComponent.-constructor), [`auth-flows.ts`](../auth-flows.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-auth-flows.ts), [`<constructor>`](configuration-menu.ts.md#ConfigurationMenuComponent.-constructor), [`configuration-menu.ts`](configuration-menu.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-configuration-menu.ts), [`updateList`](oauth-selector.ts.md#OAuthSelectorComponent.updateList), [`runLogout`](../auth-flows.ts.md#ProviderAuthFlows.runLogout), [`getLogoutProviderOptions`](../auth-flows.ts.md#ProviderAuthFlows.getLogoutProviderOptions), [`runLogin`](../auth-flows.ts.md#ProviderAuthFlows.runLogin), [`getLoginProviderOptions`](../auth-flows.ts.md#ProviderAuthFlows.getLoginProviderOptions), [`formatStatusIndicator`](oauth-selector.ts.md#OAuthSelectorComponent.formatStatusIndicator), [`loginProvider`](../auth-flows.ts.md#ProviderAuthFlows.loginProvider), [`filterProviders`](oauth-selector.ts.md#OAuthSelectorComponent.filterProviders), [`ensureModelProviderConfigured`](../interactive-mode.ts.md#InteractiveMode.ensureModelProviderConfigured), [`refresh`](oauth-selector.ts.md#OAuthSelectorComponent.refresh), [`isProviderStale`](oauth-selector.ts.md#OAuthSelectorComponent.isProviderStale), [`isProviderConfigured`](oauth-selector.ts.md#OAuthSelectorComponent.isProviderConfigured), [`filteredProviders`](oauth-selector.ts.md#OAuthSelectorComponent.filteredProviders), [`sortProviders`](oauth-selector.ts.md#OAuthSelectorComponent.sortProviders), [`compareAuthSelectorProviders`](oauth-selector.ts.md#compareAuthSelectorProviders), [`getProviderSortRank`](oauth-selector.ts.md#OAuthSelectorComponent.getProviderSortRank), [`allProviders`](oauth-selector.ts.md#OAuthSelectorComponent.allProviders), [`inActiveCategory`](oauth-selector.ts.md#OAuthSelectorComponent.inActiveCategory), [`providerOptions`](configuration-menu.ts.md#ConfigurationMenuOptions.providerOptions), [`onSelectMcpConnection`](configuration-menu.ts.md#ConfigurationMenuOptions.onSelectMcpConnection), [`onSelectProvider`](configuration-menu.ts.md#ConfigurationMenuOptions.onSelectProvider), [`onSelectCallback`](oauth-selector.ts.md#OAuthSelectorComponent.onSelectCallback)  (4 test-only)

### `OAuthSelectorComponent`  ·  implements/extends Component, Container, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/oauth-selector.ts:57`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L57)
- doc: Component that renders an auth provider selector
- signature: `class OAuthSelectorComponent`
- members:
  - `<constructor>(mode: "login" | "logout", authStorage: AuthStorage, providers: AuthSelectorProvider[], onSelect: (provider: AuthSelectorProvider) => void, onCancel: () => void, getAuthStatus?: ((providerId: string) => AuthStatus) | undefined, options?: OAuthSelectorOptions)` — [`L93`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L93) — Component that renders an auth provider selector
  - `<get>focused` — [`L62`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L62) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `<get>reservedRows` — [`L416`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L416)
  - `<set>focused` — [`L65`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L65) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `filterProviders(method)` — [`L187`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L187)
  - `formatApiKeyStatusIndicator(method)` — [`L350`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L350)
  - `formatStatusIndicator(method)` — [`L327`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L327)
  - `getProviderSortRank(method)` — [`L234`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L234)
  - `getSearchInput(method)` — [`L230`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L230)
  - `handleInput(method)` — [`L369`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L369)
  - `inActiveCategory(method)` — [`L157`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L157)
  - `isProviderConfigured(method)` — [`L251`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L251)
  - `isProviderStale(method)` — [`L244`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L244)
  - `refresh(method)` — [`L215`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L215)
  - `render(method)` — [`L271`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L271) — Render the component to lines for the given viewport width
  - `sortProviders(method)` — [`L201`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L201)
  - `switchCategory(method)` — [`L161`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L161)
  - `updateLayout(method)` — [`L420`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L420)
  - `updateList(method)` — [`L283`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L283)
  - `updateTabBar(method)` — [`L171`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L171)
  - `activeCategory` — [`L79`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L79)
  - `allProviders` — [`L72`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L72)
  - `authStorage` — [`L80`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L80)
  - `categories` — [`L78`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L78) — Tabs present in the data, in display order. Empty/single → no tab bar.
  - `filteredProviders` — [`L73`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L73)
  - `getAuthStatus` — [`L81`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L81)
  - `getHeaderRows` — [`L91`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L91)
  - `listContainer` — [`L70`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L70)
  - `listLayout` — [`L84`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L84)
  - `mode` — [`L76`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L76)
  - `onCancelCallback` — [`L83`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L83)
  - `onSelectCallback` — [`L82`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L82)
  - `searchInput` — [`L58`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L58)
  - `searchQuery` — [`L75`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L75)
  - `selectedIndex` — [`L74`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L74)
  - `tabBar` — [`L71`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L71)
  - `viewport` — [`L90`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L90)
- protocol/private: `_focused`[`L61`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L61)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`AuthStorage`](../../../core/auth-storage.ts.md#AuthStorage), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`render`](../../../../../tui/src/tui.ts.md#Container.render), [`type`](../../../core/auth-storage.ts.md#ApiKeyCredential.typeLiteral1.type), [`bold`](../theme/theme.ts.md#Theme.bold), [`PRIME_INFERENCE_PROVIDER_ID`](../../../core/prime-inference-auth.ts.md#PRIME_INFERENCE_PROVIDER_ID), [`id`](oauth-selector.ts.md#AuthSelectorProvider.typeLiteral0.id), [`clear`](../../../../../tui/src/tui.ts.md#Container.clear), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`authType`](oauth-selector.ts.md#AuthSelectorProvider.typeLiteral0.authType), [`getMenuListLayout`](menu-panel.ts.md#getMenuListLayout), [`name`](oauth-selector.ts.md#AuthSelectorProvider.typeLiteral0.name), [`AuthSelectorProvider`](oauth-selector.ts.md#AuthSelectorProvider), [`<constructor>`](../../../../../tui/src/components/truncated-text.ts.md#TruncatedText.-constructor), [`source`](../../../core/auth-storage.ts.md#AuthStatus.typeLiteral5.source), [`getAuthStatus`](../../../core/auth-storage.ts.md#AuthStorage.getAuthStatus), [`fuzzyFilter`](../../../../../tui/src/fuzzy.ts.md#fuzzyFilter), [`visibleItems`](menu-panel.ts.md#MenuListLayout.visibleItems), [`AuthStatus`](../../../core/auth-storage.ts.md#AuthStatus), [`get`](../../../core/auth-storage.ts.md#AuthStorage.get), [`category`](oauth-selector.ts.md#AuthSelectorProvider.typeLiteral0.category), [`MenuSearchInput`](menu-panel.ts.md#MenuSearchInput), [`compact`](menu-panel.ts.md#MenuListLayout.compact), [`<constructor>`](menu-panel.ts.md#MenuPanel.-constructor), [`getValue`](menu-panel.ts.md#MenuSearchInput.getValue), [`getRows`](menu-panel.ts.md#MenuViewportProvider.getRows), [`reservedRows`](menu-panel.ts.md#MenuListLayoutOptions.reservedRows), [`compactItemRows`](menu-panel.ts.md#MenuListLayoutOptions.compactItemRows), [`preferredVisibleItems`](menu-panel.ts.md#MenuListLayoutOptions.preferredVisibleItems), [`<constructor>`](menu-panel.ts.md#MenuRow.-constructor), [`comfortableItemRows`](menu-panel.ts.md#MenuListLayoutOptions.comfortableItemRows), [`primary`](menu-panel.ts.md#MenuRowOptions.primary), [`selected`](menu-panel.ts.md#MenuRowOptions.selected), [`compareAuthSelectorProviders`](oauth-selector.ts.md#compareAuthSelectorProviders)  (+29 more)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`auth-flows.ts`](../auth-flows.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-auth-flows.ts), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`render`](../../../../../tui/src/tui.ts.md#Container.render), [`<constructor>`](configuration-menu.ts.md#ConfigurationMenuComponent.-constructor), [`configuration-menu.ts`](configuration-menu.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-configuration-menu.ts), [`handleInput`](configuration-menu.ts.md#ConfigurationMenuComponent.handleInput), [`runLogout`](../auth-flows.ts.md#ProviderAuthFlows.runLogout), [`runLogin`](../auth-flows.ts.md#ProviderAuthFlows.runLogin), [`setActiveTab`](configuration-menu.ts.md#ConfigurationMenuComponent.setActiveTab), [`getSearchValue`](configuration-menu.ts.md#ConfigurationMenuComponent.getSearchValue), [`<get>activeBody`](configuration-menu.ts.md#ConfigurationMenuComponent.-get-activeBody), [`<set>focused`](configuration-menu.ts.md#ConfigurationMenuComponent.-set-focused), [`refreshAuthentication`](configuration-menu.ts.md#ConfigurationMenuComponent.refreshAuthentication), [`"mcp-connections"`](configuration-menu.ts.md#ConfigurationMenuComponent.bodies.typeLiteral48.-mcp-connections), [`providers`](configuration-menu.ts.md#ConfigurationMenuComponent.bodies.typeLiteral48.providers)  (2 test-only)

### `OAuthSelectorOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/oauth-selector.ts:32`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L32)
- signature: `interface OAuthSelectorOptions`
- members:
  - `getHeaderRows` — [`L35`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L35)
  - `header` — [`L34`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L34)
  - `initialCategory` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L33)
  - `searchPlaceholder` — [`L38`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L38)
  - `subtitle` — [`L37`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L37)
  - `title` — [`L36`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L36)
- uses (calls/refs, reference-scoped): [`Component`](../../../../../tui/src/tui.ts.md#Component), [`MenuViewportProvider`](menu-panel.ts.md#MenuViewportProvider), [`AuthSelectorCategory`](oauth-selector.ts.md#AuthSelectorCategory)
- used by: [`<constructor>`](oauth-selector.ts.md#OAuthSelectorComponent.-constructor)

## Functions
- `compareAuthSelectorProviders(a: AuthSelectorProvider, b: AuthSelectorProvider)` — [`L41`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L41)

## Module values
- `PREFERRED_VISIBLE_PROVIDERS` — [`L48`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L48)
- `PROVIDER_LIST_RESERVED_ROWS` — [`L49`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L49)
- `PROVIDER_SCROLL_INDICATOR_ROWS` — [`L52`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L52)
- `TAB_BAR_RESERVED_ROWS` — [`L51`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/oauth-selector.ts#L51) — Extra fixed rows the Providers/MCP Connections tab bar (text + spacer) consumes.


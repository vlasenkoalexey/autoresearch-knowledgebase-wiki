---
title: 'Module: packages/coding-agent/src/modes/interactive/components/extension-selector.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/extension-selector.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`extension-selector.ts`/
symbols:
  ExtensionSelectorComponent.-constructor: ExtensionSelectorComponent#`<constructor>`().
  ExtensionSelectorComponent.updateList: ExtensionSelectorComponent#updateList().
  ExtensionSelectorComponent.updateLayout: ExtensionSelectorComponent#updateLayout().
  ExtensionSelectorComponent.listLayout: ExtensionSelectorComponent#listLayout.
  ExtensionSelectorComponent.handleInput: ExtensionSelectorComponent#handleInput().
  ExtensionSelectorComponent.render: ExtensionSelectorComponent#render().
  ExtensionSelectorComponent: ExtensionSelectorComponent#
  ExtensionSelectorComponent.options: ExtensionSelectorComponent#options.
  splitTitleAndDescription: splitTitleAndDescription().
  ExtensionSelectorComponent.panel: ExtensionSelectorComponent#panel.
  ExtensionSelectorComponent.selectedIndex: ExtensionSelectorComponent#selectedIndex.
  ExtensionSelectorComponent.listContainer: ExtensionSelectorComponent#listContainer.
  ExtensionSelectorComponent.dispose: ExtensionSelectorComponent#dispose().
  ExtensionSelectorOptions.tui: ExtensionSelectorOptions#tui.
  ExtensionSelectorComponent.countdown: ExtensionSelectorComponent#countdown.
  ExtensionSelectorComponent.viewport: ExtensionSelectorComponent#viewport.
  ExtensionSelectorOptions.timeout: ExtensionSelectorOptions#timeout.
  splitTitleAndDescription.typeLiteral0.title: splitTitleAndDescription().typeLiteral0:title.
  ExtensionSelectorComponent.onCancelCallback: ExtensionSelectorComponent#onCancelCallback.
  PREFERRED_VISIBLE_OPTIONS: PREFERRED_VISIBLE_OPTIONS.
  OPTION_LIST_RESERVED_BASE_ROWS: OPTION_LIST_RESERVED_BASE_ROWS.
  splitTitleAndDescription.typeLiteral0.description: splitTitleAndDescription().typeLiteral0:description.
  splitTitleAndDescription.typeLiteral0.descriptionRows: splitTitleAndDescription().typeLiteral0:descriptionRows.
  ExtensionSelectorComponent.onSelectCallback: ExtensionSelectorComponent#onSelectCallback.
  ExtensionSelectorComponent.baseTitle: ExtensionSelectorComponent#baseTitle.
  ExtensionSelectorComponent.reservedRows: ExtensionSelectorComponent#reservedRows.
  ExtensionSelectorOptions: ExtensionSelectorOptions#
  ExtensionSelectorOptions.getRows: ExtensionSelectorOptions#getRows.
  OPTION_SCROLL_INDICATOR_ROWS: OPTION_SCROLL_INDICATOR_ROWS.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/extension-selector.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts)

## Classes
### `ExtensionSelectorComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/extension-selector.ts:35`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L35)
- signature: `class ExtensionSelectorComponent`
- members:
  - `<constructor>(title: string, options: string[], onSelect: (option: string) => void, onCancel: () => void, opts?: ExtensionSelectorOptions | undefined)` — [`L53`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L53)
  - `dispose(method)` — [`L157`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L157)
  - `handleInput(method)` — [`L141`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L141)
  - `render(method)` — [`L104`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L104) — Render the component to lines for the given viewport width
  - `updateLayout(method)` — [`L161`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L161)
  - `updateList(method)` — [`L116`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L116)
  - `baseTitle` — [`L41`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L41)
  - `countdown` — [`L42`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L42)
  - `listContainer` — [`L38`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L38)
  - `listLayout` — [`L45`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L45)
  - `onCancelCallback` — [`L40`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L40)
  - `onSelectCallback` — [`L39`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L39)
  - `options` — [`L36`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L36)
  - `panel` — [`L43`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L43)
  - `reservedRows` — [`L44`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L44)
  - `selectedIndex` — [`L37`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L37)
  - `viewport` — [`L51`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L51)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`render`](../../../../../tui/src/tui.ts.md#Container.render), [`terminal`](../../../../../tui/src/tui.ts.md#TUI.terminal), [`clear`](../../../../../tui/src/tui.ts.md#Container.clear), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`getMenuListLayout`](menu-panel.ts.md#getMenuListLayout), [`keyHint`](keybinding-hints.ts.md#keyHint), [`visibleItems`](menu-panel.ts.md#MenuListLayout.visibleItems), [`<get>rows`](../../../../../tui/src/terminal.ts.md#Terminal.-get-rows), [`rawKeyHint`](keybinding-hints.ts.md#rawKeyHint), [`compact`](menu-panel.ts.md#MenuListLayout.compact), [`<constructor>`](menu-panel.ts.md#MenuPanel.-constructor), [`getRows`](menu-panel.ts.md#MenuViewportProvider.getRows), [`<constructor>`](countdown-timer.ts.md#CountdownTimer.-constructor), [`reservedRows`](menu-panel.ts.md#MenuListLayoutOptions.reservedRows), [`compactItemRows`](menu-panel.ts.md#MenuListLayoutOptions.compactItemRows), [`preferredVisibleItems`](menu-panel.ts.md#MenuListLayoutOptions.preferredVisibleItems), [`MenuPanel`](menu-panel.ts.md#MenuPanel), [`<constructor>`](menu-panel.ts.md#MenuRow.-constructor), [`comfortableItemRows`](menu-panel.ts.md#MenuListLayoutOptions.comfortableItemRows), [`primary`](menu-panel.ts.md#MenuRowOptions.primary), [`selected`](menu-panel.ts.md#MenuRowOptions.selected), [`title`](menu-panel.ts.md#MenuPanelOptions.title), [`<constructor>`](menu-panel.ts.md#MenuList.-constructor), [`MenuViewportProvider`](menu-panel.ts.md#MenuViewportProvider), [`subtitle`](menu-panel.ts.md#MenuPanelOptions.subtitle), [`dispose`](countdown-timer.ts.md#CountdownTimer.dispose), [`splitTitleAndDescription`](extension-selector.ts.md#splitTitleAndDescription), [`scrollIndicatorRows`](menu-panel.ts.md#MenuListLayoutOptions.scrollIndicatorRows), [`totalItems`](menu-panel.ts.md#MenuListLayoutOptions.totalItems), [`CountdownTimer`](countdown-timer.ts.md#CountdownTimer), [`tui`](extension-selector.ts.md#ExtensionSelectorOptions.tui), [`setTitle`](menu-panel.ts.md#MenuPanel.setTitle), [`timeout`](extension-selector.ts.md#ExtensionSelectorOptions.timeout)  (+8 more)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`main.ts`](../../../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`auth-flows.ts`](../auth-flows.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-auth-flows.ts), [`render`](../../../../../tui/src/tui.ts.md#Container.render), [`promptForMissingSessionCwd`](../../../main.ts.md#promptForMissingSessionCwd), [`showOAuthLoginSelect`](../auth-flows.ts.md#ProviderAuthFlows.showOAuthLoginSelect), [`showExtensionSelector`](../interactive-mode.ts.md#InteractiveMode.showExtensionSelector), [`hideExtensionSelector`](../interactive-mode.ts.md#InteractiveMode.hideExtensionSelector), [`extensionSelector`](../interactive-mode.ts.md#InteractiveMode.extensionSelector)  (1 test-only)

### `ExtensionSelectorOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/extension-selector.ts:12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L12)
- signature: `interface ExtensionSelectorOptions`
- members:
  - `getRows` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L15)
  - `timeout` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L14)
  - `tui` — [`L13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L13)
- uses (calls/refs, reference-scoped): [`TUI`](../../../../../tui/src/tui.ts.md#TUI)
- used by: [`<constructor>`](extension-selector.ts.md#ExtensionSelectorComponent.-constructor)

## Functions
- `splitTitleAndDescription(value: string)` — [`L22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L22)

## Module values
- `OPTION_LIST_RESERVED_BASE_ROWS` — [`L19`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L19)
- `OPTION_SCROLL_INDICATOR_ROWS` — [`L20`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L20)
- `PREFERRED_VISIBLE_OPTIONS` — [`L18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L18)
- `description` — [`L22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L22)
- `descriptionRows` — [`L22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L22)
- `title` — [`L22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/extension-selector.ts#L22)


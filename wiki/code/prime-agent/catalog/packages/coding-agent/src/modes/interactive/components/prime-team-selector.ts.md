---
title: 'Module: packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`prime-team-selector.ts`/
symbols:
  PrimeTeamSelectorComponent.-constructor: PrimeTeamSelectorComponent#`<constructor>`().
  PrimeTeamSelectorComponent.updateList: PrimeTeamSelectorComponent#updateList().
  PrimeTeamSelectorComponent.updateLayout: PrimeTeamSelectorComponent#updateLayout().
  PrimeTeamSelectorComponent.handleInput: PrimeTeamSelectorComponent#handleInput().
  PrimeTeamSelectorComponent.listLayout: PrimeTeamSelectorComponent#listLayout.
  PrimeTeamSelectorComponent.filterOptions: PrimeTeamSelectorComponent#filterOptions().
  PrimeTeamSelectorComponent.getSearchText: PrimeTeamSelectorComponent#getSearchText().
  PrimeTeamSelectorComponent.filteredOptions: PrimeTeamSelectorComponent#filteredOptions.
  PrimeTeamSelectorComponent.render: PrimeTeamSelectorComponent#render().
  PrimeTeamSelectorComponent.getMeta: PrimeTeamSelectorComponent#getMeta().
  PrimeTeamOption.typeLiteral0.team: PrimeTeamOption#typeLiteral0:team.
  PrimeTeamSelectorComponent.selectedIndex: PrimeTeamSelectorComponent#selectedIndex.
  PrimeTeamSelectorComponent.getSecondary: PrimeTeamSelectorComponent#getSecondary().
  PrimeTeamSelectorComponent.-set-focused: PrimeTeamSelectorComponent#`<set>focused`().
  PrimeTeamOption: PrimeTeamOption#
  PrimeTeamSelectorComponent.searchInput: PrimeTeamSelectorComponent#searchInput.
  PrimeTeamSelectorComponent.listContainer: PrimeTeamSelectorComponent#listContainer.
  PrimeTeamSelectorComponent.getPrimary: PrimeTeamSelectorComponent#getPrimary().
  PrimeTeamSelectorComponent: PrimeTeamSelectorComponent#
  PrimeTeamSelectorComponent.allOptions: PrimeTeamSelectorComponent#allOptions.
  PrimeTeamSelectorComponent.-get-focused: PrimeTeamSelectorComponent#`<get>focused`().
  PrimeTeamOption.typeLiteral0.type: PrimeTeamOption#typeLiteral0:type.
  PREFERRED_VISIBLE_TEAMS: PREFERRED_VISIBLE_TEAMS.
  TEAM_LIST_RESERVED_ROWS: TEAM_LIST_RESERVED_ROWS.
  PrimeTeamSelectorComponent.searchQuery: PrimeTeamSelectorComponent#searchQuery.
  PrimeTeamSelectorComponent._focused: PrimeTeamSelectorComponent#_focused.
  TEAM_SCROLL_INDICATOR_ROWS: TEAM_SCROLL_INDICATOR_ROWS.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts)

## Classes
### `PrimeTeamOption`
- def: [`packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts:13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L13)
- signature: `type PrimeTeamOption`
- members:
  - `team` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L15)
  - `type` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L14)
- uses (calls/refs, reference-scoped): [`PrimeTeam`](../../../core/prime-inference-auth.ts.md#PrimeTeam)
- used by: [`<constructor>`](prime-team-selector.ts.md#PrimeTeamSelectorComponent.-constructor), [`handleInput`](prime-team-selector.ts.md#PrimeTeamSelectorComponent.handleInput), [`getSearchText`](prime-team-selector.ts.md#PrimeTeamSelectorComponent.getSearchText), [`filteredOptions`](prime-team-selector.ts.md#PrimeTeamSelectorComponent.filteredOptions), [`getMeta`](prime-team-selector.ts.md#PrimeTeamSelectorComponent.getMeta), [`getSecondary`](prime-team-selector.ts.md#PrimeTeamSelectorComponent.getSecondary), [`getPrimary`](prime-team-selector.ts.md#PrimeTeamSelectorComponent.getPrimary), [`allOptions`](prime-team-selector.ts.md#PrimeTeamSelectorComponent.allOptions)

### `PrimeTeamSelectorComponent`  ·  implements/extends Component, Container, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts:22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L22)
- signature: `class PrimeTeamSelectorComponent`
- members:
  - `<constructor>(teams: PrimeTeam[], currentTeamId: string | undefined, onSelect: (team: PrimeTeam | null) => void, onCancel: () => void, viewport?: MenuViewportProvider)` — [`L37`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L37)
  - `<get>focused` — [`L70`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L70) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `<set>focused` — [`L74`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L74) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `filterOptions(method)` — [`L79`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L79)
  - `getMeta(method)` — [`L160`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L160)
  - `getPrimary(method)` — [`L148`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L148)
  - `getSearchText(method)` — [`L91`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L91)
  - `getSecondary(method)` — [`L152`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L152)
  - `handleInput(method)` — [`L165`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L165)
  - `render(method)` — [`L99`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L99) — Render the component to lines for the given viewport width
  - `updateLayout(method)` — [`L192`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L192)
  - `updateList(method)` — [`L111`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L111)
  - `allOptions` — [`L25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L25)
  - `filteredOptions` — [`L26`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L26)
  - `listContainer` — [`L24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L24)
  - `listLayout` — [`L30`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L30)
  - `searchInput` — [`L23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L23)
  - `searchQuery` — [`L28`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L28)
  - `selectedIndex` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L27)
- protocol/private: `_focused`[`L29`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L29)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`render`](../../../../../tui/src/tui.ts.md#Container.render), [`clear`](../../../../../tui/src/tui.ts.md#Container.clear), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`getMenuListLayout`](menu-panel.ts.md#getMenuListLayout), [`<constructor>`](../../../../../tui/src/components/truncated-text.ts.md#TruncatedText.-constructor), [`fuzzyFilter`](../../../../../tui/src/fuzzy.ts.md#fuzzyFilter), [`visibleItems`](menu-panel.ts.md#MenuListLayout.visibleItems), [`MenuSearchInput`](menu-panel.ts.md#MenuSearchInput), [`compact`](menu-panel.ts.md#MenuListLayout.compact), [`<constructor>`](menu-panel.ts.md#MenuPanel.-constructor), [`getValue`](menu-panel.ts.md#MenuSearchInput.getValue), [`getRows`](menu-panel.ts.md#MenuViewportProvider.getRows), [`PrimeTeam`](../../../core/prime-inference-auth.ts.md#PrimeTeam), [`reservedRows`](menu-panel.ts.md#MenuListLayoutOptions.reservedRows), [`compactItemRows`](menu-panel.ts.md#MenuListLayoutOptions.compactItemRows), [`preferredVisibleItems`](menu-panel.ts.md#MenuListLayoutOptions.preferredVisibleItems), [`teamId`](../../../core/prime-inference-auth.ts.md#PrimeTeam.typeLiteral17.teamId), [`<constructor>`](menu-panel.ts.md#MenuRow.-constructor), [`comfortableItemRows`](menu-panel.ts.md#MenuListLayoutOptions.comfortableItemRows), [`name`](../../../core/prime-inference-auth.ts.md#PrimeTeam.typeLiteral17.name), [`primary`](menu-panel.ts.md#MenuRowOptions.primary), [`role`](../../../core/prime-inference-auth.ts.md#PrimeTeam.typeLiteral17.role), [`selected`](menu-panel.ts.md#MenuRowOptions.selected), [`secondary`](menu-panel.ts.md#MenuRowOptions.secondary), [`team`](prime-team-selector.ts.md#PrimeTeamOption.typeLiteral0.team), [`title`](menu-panel.ts.md#MenuPanelOptions.title), [`<constructor>`](menu-panel.ts.md#MenuList.-constructor), [`MenuViewportProvider`](menu-panel.ts.md#MenuViewportProvider), [`<get>focused`](menu-panel.ts.md#MenuSearchInput.-get-focused), [`<set>focused`](menu-panel.ts.md#MenuSearchInput.-set-focused), [`handleInput`](menu-panel.ts.md#MenuSearchInput.handleInput), [`subtitle`](menu-panel.ts.md#MenuPanelOptions.subtitle), [`<set>onSubmit`](menu-panel.ts.md#MenuSearchInput.-set-onSubmit)  (+10 more)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`auth-flows.ts`](../auth-flows.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-auth-flows.ts), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`render`](../../../../../tui/src/tui.ts.md#Container.render), [`showPrimeTeamSelector`](../auth-flows.ts.md#ProviderAuthFlows.showPrimeTeamSelector)  (2 test-only)

## Module values
- `PREFERRED_VISIBLE_TEAMS` — [`L18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L18)
- `TEAM_LIST_RESERVED_ROWS` — [`L19`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L19)
- `TEAM_SCROLL_INDICATOR_ROWS` — [`L20`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-team-selector.ts#L20)


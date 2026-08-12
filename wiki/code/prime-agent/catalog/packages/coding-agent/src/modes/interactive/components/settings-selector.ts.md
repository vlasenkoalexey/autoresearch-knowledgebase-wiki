---
title: 'Module: packages/coding-agent/src/modes/interactive/components/settings-selector.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/settings-selector.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`settings-selector.ts`/
symbols:
  SettingsSelectorComponent.-constructor: SettingsSelectorComponent#`<constructor>`().
  SelectSubmenu.-constructor: SelectSubmenu#`<constructor>`().
  WarningSettingsSubmenu.-constructor: WarningSettingsSubmenu#`<constructor>`().
  SettingsConfig.idleEvictionMinutes: SettingsConfig#idleEvictionMinutes.
  SelectSubmenu.selectList: SelectSubmenu#selectList.
  SettingsSelectorComponent.getSettingsList: SettingsSelectorComponent#getSettingsList().
  SETTINGS_SUBMENU_SELECT_LIST_LAYOUT: SETTINGS_SUBMENU_SELECT_LIST_LAYOUT.
  SettingsCallbacks.onIdleEvictionMinutesChange: SettingsCallbacks#onIdleEvictionMinutesChange.
  WarningSettingsSubmenu.state: WarningSettingsSubmenu#state.
  SettingsSelectorComponent: SettingsSelectorComponent#
  SettingsConfig.transport: SettingsConfig#transport.
  SettingsConfig.thinkingLevel: SettingsConfig#thinkingLevel.
  SettingsConfig.availableThinkingLevels: SettingsConfig#availableThinkingLevels.
  SettingsConfig.warnings: SettingsConfig#warnings.
  SettingsCallbacks.onTransportChange: SettingsCallbacks#onTransportChange.
  SettingsCallbacks.onThinkingLevelChange: SettingsCallbacks#onThinkingLevelChange.
  SettingsCallbacks.onWarningsChange: SettingsCallbacks#onWarningsChange.
  WarningSettingsSubmenu.settingsList: WarningSettingsSubmenu#settingsList.
  SettingsSelectorComponent.settingsList: SettingsSelectorComponent#settingsList.
  SettingsConfig: SettingsConfig#
  SettingsCallbacks: SettingsCallbacks#
  WarningSettingsSubmenu.handleInput: WarningSettingsSubmenu#handleInput().
  SelectSubmenu.handleInput: SelectSubmenu#handleInput().
  THINKING_DESCRIPTIONS: THINKING_DESCRIPTIONS.
  SettingsConfig.autoCompact: SettingsConfig#autoCompact.
  SettingsConfig.showImages: SettingsConfig#showImages.
  SettingsConfig.autoResizeImages: SettingsConfig#autoResizeImages.
  SettingsConfig.blockImages: SettingsConfig#blockImages.
  SettingsConfig.enableSkillCommands: SettingsConfig#enableSkillCommands.
  SettingsConfig.enableBuiltinSkills: SettingsConfig#enableBuiltinSkills.
  SettingsConfig.steeringMode: SettingsConfig#steeringMode.
  SettingsConfig.followUpMode: SettingsConfig#followUpMode.
  SettingsConfig.currentTheme: SettingsConfig#currentTheme.
  SettingsConfig.availableThemes: SettingsConfig#availableThemes.
  SettingsConfig.hideThinkingBlock: SettingsConfig#hideThinkingBlock.
  SettingsConfig.treeFilterMode: SettingsConfig#treeFilterMode.
  SettingsConfig.showHardwareCursor: SettingsConfig#showHardwareCursor.
  SettingsConfig.editorPaddingX: SettingsConfig#editorPaddingX.
  SettingsConfig.autocompleteMaxVisible: SettingsConfig#autocompleteMaxVisible.
  SettingsConfig.quietStartup: SettingsConfig#quietStartup.
  SettingsConfig.clearOnShrink: SettingsConfig#clearOnShrink.
  SettingsConfig.showTerminalProgress: SettingsConfig#showTerminalProgress.
  SettingsConfig.fullscreen: SettingsConfig#fullscreen.
  SettingsCallbacks.onAutoCompactChange: SettingsCallbacks#onAutoCompactChange.
  SettingsCallbacks.onShowImagesChange: SettingsCallbacks#onShowImagesChange.
  SettingsCallbacks.onAutoResizeImagesChange: SettingsCallbacks#onAutoResizeImagesChange.
  SettingsCallbacks.onBlockImagesChange: SettingsCallbacks#onBlockImagesChange.
  SettingsCallbacks.onEnableSkillCommandsChange: SettingsCallbacks#onEnableSkillCommandsChange.
  SettingsCallbacks.onEnableBuiltinSkillsChange: SettingsCallbacks#onEnableBuiltinSkillsChange.
  SettingsCallbacks.onSteeringModeChange: SettingsCallbacks#onSteeringModeChange.
  SettingsCallbacks.onFollowUpModeChange: SettingsCallbacks#onFollowUpModeChange.
  SettingsCallbacks.onThemeChange: SettingsCallbacks#onThemeChange.
  SettingsCallbacks.onThemePreview: SettingsCallbacks#onThemePreview.
  SettingsCallbacks.onHideThinkingBlockChange: SettingsCallbacks#onHideThinkingBlockChange.
  SettingsCallbacks.onTreeFilterModeChange: SettingsCallbacks#onTreeFilterModeChange.
  SettingsCallbacks.onShowHardwareCursorChange: SettingsCallbacks#onShowHardwareCursorChange.
  SettingsCallbacks.onEditorPaddingXChange: SettingsCallbacks#onEditorPaddingXChange.
  SettingsCallbacks.onAutocompleteMaxVisibleChange: SettingsCallbacks#onAutocompleteMaxVisibleChange.
  SettingsCallbacks.onQuietStartupChange: SettingsCallbacks#onQuietStartupChange.
  SettingsCallbacks.onClearOnShrinkChange: SettingsCallbacks#onClearOnShrinkChange.
  SettingsCallbacks.onShowTerminalProgressChange: SettingsCallbacks#onShowTerminalProgressChange.
  SettingsCallbacks.onFullscreenChange: SettingsCallbacks#onFullscreenChange.
  SettingsCallbacks.onCancel: SettingsCallbacks#onCancel.
  WarningSettingsSubmenu: WarningSettingsSubmenu#
  SelectSubmenu: SelectSubmenu#
---
# Module: [`packages/coding-agent/src/modes/interactive/components/settings-selector.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts)

## Classes
### `SelectSubmenu`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/settings-selector.ts:132`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L132)
- signature: `class SelectSubmenu`
- members:
  - `<constructor>(title: string, description: string, options: SelectItem[], currentValue: string, onSelect: (value: string) => void, onCancel: () => void, onSelectionChange?: ((value: string) => void) | undefined)` — [`L135`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L135)
  - `handleInput(method)` — [`L191`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L191)
  - `selectList` — [`L133`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L133)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`bold`](../theme/theme.ts.md#Theme.bold), [`<constructor>`](../../../../../tui/src/components/select-list.ts.md#SelectList.-constructor), [`getSelectListTheme`](../theme/theme.ts.md#getSelectListTheme), [`SelectItem`](../../../../../tui/src/components/select-list.ts.md#SelectItem), [`SelectList`](../../../../../tui/src/components/select-list.ts.md#SelectList), [`handleInput`](../../../../../tui/src/components/select-list.ts.md#SelectList.handleInput), [`value`](../../../../../tui/src/components/select-list.ts.md#SelectItem.value), [`setSelectedIndex`](../../../../../tui/src/components/select-list.ts.md#SelectList.setSelectedIndex), [`onSelect`](../../../../../tui/src/components/select-list.ts.md#SelectList.onSelect), [`SETTINGS_SUBMENU_SELECT_LIST_LAYOUT`](settings-selector.ts.md#SETTINGS_SUBMENU_SELECT_LIST_LAYOUT), [`onCancel`](../../../../../tui/src/components/select-list.ts.md#SelectList.onCancel), [`onSelectionChange`](../../../../../tui/src/components/select-list.ts.md#SelectList.onSelectionChange)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`<constructor>`](settings-selector.ts.md#SettingsSelectorComponent.-constructor), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput)

### `SettingsCallbacks`
- def: [`packages/coding-agent/src/modes/interactive/components/settings-selector.ts:60`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L60)
- signature: `interface SettingsCallbacks`
- members:
  - `onAutoCompactChange` — [`L61`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L61)
  - `onAutoResizeImagesChange` — [`L64`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L64)
  - `onAutocompleteMaxVisibleChange` — [`L78`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L78)
  - `onBlockImagesChange` — [`L65`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L65)
  - `onCancel` — [`L84`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L84)
  - `onClearOnShrinkChange` — [`L80`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L80)
  - `onEditorPaddingXChange` — [`L77`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L77)
  - `onEnableBuiltinSkillsChange` — [`L67`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L67)
  - `onEnableSkillCommandsChange` — [`L66`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L66)
  - `onFollowUpModeChange` — [`L69`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L69)
  - `onFullscreenChange` — [`L82`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L82)
  - `onHideThinkingBlockChange` — [`L74`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L74)
  - `onIdleEvictionMinutesChange` — [`L62`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L62)
  - `onQuietStartupChange` — [`L79`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L79)
  - `onShowHardwareCursorChange` — [`L76`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L76)
  - `onShowImagesChange` — [`L63`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L63)
  - `onShowTerminalProgressChange` — [`L81`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L81)
  - `onSteeringModeChange` — [`L68`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L68)
  - `onThemeChange` — [`L72`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L72)
  - `onThemePreview` — [`L73`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L73)
  - `onThinkingLevelChange` — [`L71`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L71)
  - `onTransportChange` — [`L70`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L70)
  - `onTreeFilterModeChange` — [`L75`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L75)
  - `onWarningsChange` — [`L83`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L83)
- uses (calls/refs, reference-scoped): [`ThinkingLevel`](../../../../../agent/src/types.ts.md#ThinkingLevel), [`Transport`](../../../../../ai/src/types.ts.md#Transport), [`IdleEvictionMinutes`](../../../core/session-action-store.ts.md#IdleEvictionMinutes), [`WarningSettings`](../../../core/settings-manager.ts.md#WarningSettings)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`showSettingsSelector`](../interactive-mode.ts.md#InteractiveMode.showSettingsSelector), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`<constructor>`](settings-selector.ts.md#SettingsSelectorComponent.-constructor)  (1 test-only)

### `SettingsConfig`
- def: [`packages/coding-agent/src/modes/interactive/components/settings-selector.ts:33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L33)
- signature: `interface SettingsConfig`
- members:
  - `autoCompact` — [`L34`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L34)
  - `autoResizeImages` — [`L37`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L37)
  - `autocompleteMaxVisible` — [`L52`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L52)
  - `availableThemes` — [`L47`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L47)
  - `availableThinkingLevels` — [`L45`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L45)
  - `blockImages` — [`L38`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L38)
  - `clearOnShrink` — [`L54`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L54)
  - `currentTheme` — [`L46`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L46)
  - `editorPaddingX` — [`L51`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L51)
  - `enableBuiltinSkills` — [`L40`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L40)
  - `enableSkillCommands` — [`L39`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L39)
  - `followUpMode` — [`L42`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L42)
  - `fullscreen` — [`L56`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L56)
  - `hideThinkingBlock` — [`L48`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L48)
  - `idleEvictionMinutes` — [`L35`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L35)
  - `quietStartup` — [`L53`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L53)
  - `showHardwareCursor` — [`L50`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L50)
  - `showImages` — [`L36`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L36)
  - `showTerminalProgress` — [`L55`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L55)
  - `steeringMode` — [`L41`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L41)
  - `thinkingLevel` — [`L44`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L44)
  - `transport` — [`L43`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L43)
  - `treeFilterMode` — [`L49`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L49)
  - `warnings` — [`L57`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L57)
- uses (calls/refs, reference-scoped): [`ThinkingLevel`](../../../../../agent/src/types.ts.md#ThinkingLevel), [`Transport`](../../../../../ai/src/types.ts.md#Transport), [`IdleEvictionMinutes`](../../../core/session-action-store.ts.md#IdleEvictionMinutes), [`WarningSettings`](../../../core/settings-manager.ts.md#WarningSettings)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`showSettingsSelector`](../interactive-mode.ts.md#InteractiveMode.showSettingsSelector), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`<constructor>`](settings-selector.ts.md#SettingsSelectorComponent.-constructor)  (2 test-only)

### `SettingsSelectorComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/settings-selector.ts:199`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L199)
- doc: Main settings selector component.
- signature: `class SettingsSelectorComponent`
- members:
  - `<constructor>(config: SettingsConfig, callbacks: SettingsCallbacks)` — [`L202`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L202) — Main settings selector component.
  - `getSettingsList(method)` — [`L524`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L524)
  - `settingsList` — [`L200`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L200)
- uses (calls/refs, reference-scoped): [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`ThinkingLevel`](../../../../../agent/src/types.ts.md#ThinkingLevel), [`<constructor>`](settings-selector.ts.md#SelectSubmenu.-constructor), [`<constructor>`](dynamic-border.ts.md#DynamicBorder.-constructor), [`<constructor>`](../../../../../tui/src/components/settings-list.ts.md#SettingsList.-constructor), [`id`](../../../../../tui/src/components/settings-list.ts.md#SettingItem.id), [`<constructor>`](settings-selector.ts.md#WarningSettingsSubmenu.-constructor), [`currentValue`](../../../../../tui/src/components/settings-list.ts.md#SettingItem.currentValue), [`getSettingsListTheme`](../theme/theme.ts.md#getSettingsListTheme), [`label`](../../../../../tui/src/components/settings-list.ts.md#SettingItem.label), [`description`](../../../../../tui/src/components/settings-list.ts.md#SettingItem.description), [`values`](../../../../../tui/src/components/settings-list.ts.md#SettingItem.values), [`Transport`](../../../../../ai/src/types.ts.md#Transport), [`idleEvictionMinutes`](settings-selector.ts.md#SettingsConfig.idleEvictionMinutes), [`SettingItem`](../../../../../tui/src/components/settings-list.ts.md#SettingItem), [`SettingsList`](../../../../../tui/src/components/settings-list.ts.md#SettingsList), [`onIdleEvictionMinutesChange`](settings-selector.ts.md#SettingsCallbacks.onIdleEvictionMinutesChange), [`submenu`](../../../../../tui/src/components/settings-list.ts.md#SettingItem.submenu), [`availableThinkingLevels`](settings-selector.ts.md#SettingsConfig.availableThinkingLevels), [`onThinkingLevelChange`](settings-selector.ts.md#SettingsCallbacks.onThinkingLevelChange), [`onTransportChange`](settings-selector.ts.md#SettingsCallbacks.onTransportChange), [`onWarningsChange`](settings-selector.ts.md#SettingsCallbacks.onWarningsChange), [`thinkingLevel`](settings-selector.ts.md#SettingsConfig.thinkingLevel), [`transport`](settings-selector.ts.md#SettingsConfig.transport), [`warnings`](settings-selector.ts.md#SettingsConfig.warnings), [`SettingsCallbacks`](settings-selector.ts.md#SettingsCallbacks), [`SettingsConfig`](settings-selector.ts.md#SettingsConfig), [`THINKING_DESCRIPTIONS`](settings-selector.ts.md#THINKING_DESCRIPTIONS), [`autoCompact`](settings-selector.ts.md#SettingsConfig.autoCompact), [`autoResizeImages`](settings-selector.ts.md#SettingsConfig.autoResizeImages), [`autocompleteMaxVisible`](settings-selector.ts.md#SettingsConfig.autocompleteMaxVisible), [`availableThemes`](settings-selector.ts.md#SettingsConfig.availableThemes), [`blockImages`](settings-selector.ts.md#SettingsConfig.blockImages), [`clearOnShrink`](settings-selector.ts.md#SettingsConfig.clearOnShrink), [`currentTheme`](settings-selector.ts.md#SettingsConfig.currentTheme), [`editorPaddingX`](settings-selector.ts.md#SettingsConfig.editorPaddingX), [`enableBuiltinSkills`](settings-selector.ts.md#SettingsConfig.enableBuiltinSkills), [`enableSkillCommands`](settings-selector.ts.md#SettingsConfig.enableSkillCommands), [`followUpMode`](settings-selector.ts.md#SettingsConfig.followUpMode)  (+28 more)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`showSettingsSelector`](../interactive-mode.ts.md#InteractiveMode.showSettingsSelector), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts)  (1 test-only)

### `WarningSettingsSubmenu`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/settings-selector.ts:90`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L90)
- doc: A submenu component for selecting from a list of options.
- signature: `class WarningSettingsSubmenu`
- members:
  - `<constructor>(warnings: WarningSettings, onChange: (warnings: WarningSettings) => void, onCancel: () => void)` — [`L94`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L94) — A submenu component for selecting from a list of options.
  - `handleInput(method)` — [`L127`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L127)
  - `settingsList` — [`L91`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L91)
  - `state` — [`L92`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L92)
- uses (calls/refs, reference-scoped): [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`handleInput`](../../../../../tui/src/components/settings-list.ts.md#SettingsList.handleInput), [`<constructor>`](../../../../../tui/src/components/settings-list.ts.md#SettingsList.-constructor), [`id`](../../../../../tui/src/components/settings-list.ts.md#SettingItem.id), [`currentValue`](../../../../../tui/src/components/settings-list.ts.md#SettingItem.currentValue), [`getSettingsListTheme`](../theme/theme.ts.md#getSettingsListTheme), [`label`](../../../../../tui/src/components/settings-list.ts.md#SettingItem.label), [`description`](../../../../../tui/src/components/settings-list.ts.md#SettingItem.description), [`values`](../../../../../tui/src/components/settings-list.ts.md#SettingItem.values), [`SettingItem`](../../../../../tui/src/components/settings-list.ts.md#SettingItem), [`WarningSettings`](../../../core/settings-manager.ts.md#WarningSettings), [`SettingsList`](../../../../../tui/src/components/settings-list.ts.md#SettingsList), [`anthropicExtraUsage`](../../../core/settings-manager.ts.md#WarningSettings.anthropicExtraUsage)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`<constructor>`](settings-selector.ts.md#SettingsSelectorComponent.-constructor), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput)

## Module values
- `SETTINGS_SUBMENU_SELECT_LIST_LAYOUT` — [`L18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L18)
- `THINKING_DESCRIPTIONS` — [`L23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/settings-selector.ts#L23)


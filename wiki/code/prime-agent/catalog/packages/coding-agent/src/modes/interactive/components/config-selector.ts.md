---
title: 'Module: packages/coding-agent/src/modes/interactive/components/config-selector.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/config-selector.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`config-selector.ts`/
symbols:
  buildGroups: buildGroups().
  ResourceList.handleInput: ResourceList#handleInput().
  ResourceList.toggleTopLevelResource: ResourceList#toggleTopLevelResource().
  ResourceList.togglePackageResource: ResourceList#togglePackageResource().
  ResourceList.render: ResourceList#render().
  ResourceList.filterItems: ResourceList#filterItems().
  ConfigSelectorComponent.-constructor: ConfigSelectorComponent#`<constructor>`().
  ResourceList.-constructor: ResourceList#`<constructor>`().
  ResourceList.filteredItems: ResourceList#filteredItems.
  ResourceList.updateItem: ResourceList#updateItem().
  ResourceList.getResourcePattern: ResourceList#getResourcePattern().
  ResourceList.settingsManager: ResourceList#settingsManager.
  ResourceList.selectedIndex: ResourceList#selectedIndex.
  ConfigSelectorHeader.render: ConfigSelectorHeader#render().
  getGroupLabel: getGroupLabel().
  ResourceList.buildFlatList: ResourceList#buildFlatList().
  ResourceList.toggleResource: ResourceList#toggleResource().
  ResourceItem.metadata: ResourceItem#metadata.
  ResourceList.flatItems: ResourceList#flatItems.
  ResourceList.getPackageResourcePattern: ResourceList#getPackageResourcePattern().
  ResourceGroup.subgroups: ResourceGroup#subgroups.
  ResourceItem: ResourceItem#
  ConfigSelectorComponent.-set-focused: ConfigSelectorComponent#`<set>focused`().
  FlatEntry: FlatEntry#
  ConfigSelectorComponent.resourceList: ConfigSelectorComponent#resourceList.
  ResourceItem.resourceType: ResourceItem#resourceType.
  ResourceList.-set-focused: ResourceList#`<set>focused`().
  ResourceList.getTopLevelBaseDir: ResourceList#getTopLevelBaseDir().
  ResourceItem.path: ResourceItem#path.
  ResourceSubgroup.items: ResourceSubgroup#items.
  ResourceList.searchInput: ResourceList#searchInput.
  ResourceGroup: ResourceGroup#
  ResourceList: ResourceList#
  ResourceList.selectFirstItem: ResourceList#selectFirstItem().
  ResourceList.groups: ResourceList#groups.
  ResourceItem.displayName: ResourceItem#displayName.
  ConfigSelectorComponent: ConfigSelectorComponent#
  ConfigSelectorComponent.getResourceList: ConfigSelectorComponent#getResourceList().
  ResourceSubgroup.type: ResourceSubgroup#type.
  ResourceType: ResourceType#
  ResourceItem.enabled: ResourceItem#enabled.
  ResourceList.maxVisible: ResourceList#maxVisible.
  ResourceList.onToggle: ResourceList#onToggle.
  ResourceList.findNextItem: ResourceList#findNextItem().
  ResourceGroup.scope: ResourceGroup#scope.
  ResourceGroup.origin: ResourceGroup#origin.
  RESOURCE_TYPE_LABELS: RESOURCE_TYPE_LABELS.
  ConfigSelectorHeader: ConfigSelectorHeader#
  ResourceList.-get-focused: ResourceList#`<get>focused`().
  ResourceSubgroup: ResourceSubgroup#
  ResourceGroup.source: ResourceGroup#source.
  ConfigSelectorComponent.-get-focused: ConfigSelectorComponent#`<get>focused`().
  ResourceGroup.label: ResourceGroup#label.
  ResourceList.cwd: ResourceList#cwd.
  ResourceList.agentDir: ResourceList#agentDir.
  ResourceList.onCancel: ResourceList#onCancel.
  ResourceList.onExit: ResourceList#onExit.
  ResourceList._focused: ResourceList#_focused.
  ConfigSelectorComponent._focused: ConfigSelectorComponent#_focused.
  ResourceItem.groupKey: ResourceItem#groupKey.
  ResourceItem.subgroupKey: ResourceItem#subgroupKey.
  ResourceSubgroup.label: ResourceSubgroup#label.
  ResourceGroup.key: ResourceGroup#key.
  ConfigSelectorHeader.invalidate: ConfigSelectorHeader#invalidate().
  ResourceList.invalidate: ResourceList#invalidate().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/config-selector.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts)

## Classes
### `ConfigSelectorComponent`  ·  implements/extends Component, Container, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/config-selector.ts:556`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L556)
- signature: `class ConfigSelectorComponent`
- members:
  - `<constructor>(resolvedPaths: ResolvedPaths, settingsManager: SettingsManager, cwd: string, agentDir: string, onClose: () => void, onExit: () => void, requestRender: () => void)` — [`L568`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L568)
  - `<get>focused` — [`L560`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L560) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `<set>focused` — [`L563`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L563) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `getResourceList(method)` — [`L600`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L600)
  - `resourceList` — [`L557`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L557)
- protocol/private: `_focused`[`L559`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L559)
- uses (calls/refs, reference-scoped): [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`SettingsManager`](../../../core/settings-manager.ts.md#SettingsManager), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`buildGroups`](config-selector.ts.md#buildGroups), [`<constructor>`](dynamic-border.ts.md#DynamicBorder.-constructor), [`<constructor>`](config-selector.ts.md#ResourceList.-constructor), [`ResolvedPaths`](../../../core/package-manager.ts.md#ResolvedPaths), [`<set>focused`](config-selector.ts.md#ResourceList.-set-focused), [`ResourceList`](config-selector.ts.md#ResourceList), [`onToggle`](config-selector.ts.md#ResourceList.onToggle), [`ConfigSelectorHeader`](config-selector.ts.md#ConfigSelectorHeader), [`<get>focused`](config-selector.ts.md#ResourceList.-get-focused), [`onCancel`](config-selector.ts.md#ResourceList.onCancel), [`onExit`](config-selector.ts.md#ResourceList.onExit)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`selectConfig`](../../../cli/config-selector.ts.md#selectConfig), [`config-selector.ts`](../../../cli/config-selector.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-config-selector.ts)

### `ConfigSelectorHeader`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/config-selector.ts:160`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L160)
- signature: `class ConfigSelectorHeader`
- members:
  - `invalidate(method)` — [`L161`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L161) — Invalidate any cached rendering state.
  - `render(method)` — [`L163`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L163) — Render the component to lines for the given viewport width
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`bold`](../theme/theme.ts.md#Theme.bold), [`rawKeyHint`](keybinding-hints.ts.md#rawKeyHint)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`<constructor>`](config-selector.ts.md#ConfigSelectorComponent.-constructor)

### `FlatEntry`
- def: [`packages/coding-agent/src/modes/interactive/components/config-selector.ts:155`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L155)
- signature: `type FlatEntry`
- uses (calls/refs, reference-scoped): [`ResourceItem`](config-selector.ts.md#ResourceItem), [`ResourceGroup`](config-selector.ts.md#ResourceGroup), [`ResourceSubgroup`](config-selector.ts.md#ResourceSubgroup)
- used by: [`filteredItems`](config-selector.ts.md#ResourceList.filteredItems), [`flatItems`](config-selector.ts.md#ResourceList.flatItems)

### `ResourceGroup`
- def: [`packages/coding-agent/src/modes/interactive/components/config-selector.ts:49`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L49)
- signature: `interface ResourceGroup`
- members:
  - `key` — [`L50`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L50)
  - `label` — [`L51`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L51)
  - `origin` — [`L53`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L53)
  - `scope` — [`L52`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L52)
  - `source` — [`L54`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L54)
  - `subgroups` — [`L55`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L55)
- uses (calls/refs, reference-scoped): [`ResourceSubgroup`](config-selector.ts.md#ResourceSubgroup)
- used by: [`buildGroups`](config-selector.ts.md#buildGroups), [`render`](config-selector.ts.md#ResourceList.render), [`filterItems`](config-selector.ts.md#ResourceList.filterItems), [`<constructor>`](config-selector.ts.md#ResourceList.-constructor), [`updateItem`](config-selector.ts.md#ResourceList.updateItem), [`buildFlatList`](config-selector.ts.md#ResourceList.buildFlatList), [`FlatEntry`](config-selector.ts.md#FlatEntry), [`groups`](config-selector.ts.md#ResourceList.groups)

### `ResourceItem`
- def: [`packages/coding-agent/src/modes/interactive/components/config-selector.ts:33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L33)
- signature: `interface ResourceItem`
- members:
  - `displayName` — [`L38`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L38)
  - `enabled` — [`L35`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L35)
  - `groupKey` — [`L39`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L39)
  - `metadata` — [`L36`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L36)
  - `path` — [`L34`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L34)
  - `resourceType` — [`L37`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L37)
  - `subgroupKey` — [`L40`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L40)
- uses (calls/refs, reference-scoped): [`PathMetadata`](../../../core/package-manager.ts.md#PathMetadata), [`ResourceType`](config-selector.ts.md#ResourceType)
- used by: [`buildGroups`](config-selector.ts.md#buildGroups), [`handleInput`](config-selector.ts.md#ResourceList.handleInput), [`toggleTopLevelResource`](config-selector.ts.md#ResourceList.toggleTopLevelResource), [`togglePackageResource`](config-selector.ts.md#ResourceList.togglePackageResource), [`render`](config-selector.ts.md#ResourceList.render), [`filterItems`](config-selector.ts.md#ResourceList.filterItems), [`getResourcePattern`](config-selector.ts.md#ResourceList.getResourcePattern), [`updateItem`](config-selector.ts.md#ResourceList.updateItem), [`toggleResource`](config-selector.ts.md#ResourceList.toggleResource), [`getPackageResourcePattern`](config-selector.ts.md#ResourceList.getPackageResourcePattern), [`FlatEntry`](config-selector.ts.md#FlatEntry), [`items`](config-selector.ts.md#ResourceSubgroup.items), [`onToggle`](config-selector.ts.md#ResourceList.onToggle)

### `ResourceList`  ·  implements/extends Component, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/config-selector.ts:178`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L178)
- signature: `class ResourceList`
- members:
  - `<constructor>(groups: ResourceGroup[], settingsManager: SettingsManager, cwd: string, agentDir: string)` — [`L202`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L202)
  - `<get>focused` — [`L194`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L194) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `<set>focused` — [`L197`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L197) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `buildFlatList(method)` — [`L212`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L212)
  - `filterItems(method)` — [`L239`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L239)
  - `findNextItem(method)` — [`L228`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L228)
  - `getPackageResourcePattern(method)` — [`L550`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L550)
  - `getResourcePattern(method)` — [`L539`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L539)
  - `getTopLevelBaseDir(method)` — [`L535`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L535)
  - `handleInput(method)` — [`L363`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L363) — Optional handler for keyboard input when component has focus
  - `invalidate(method)` — [`L309`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L309) — Invalidate any cached rendering state.
  - `render(method)` — [`L311`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L311) — Render the component to lines for the given viewport width
  - `selectFirstItem(method)` — [`L290`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L290)
  - `togglePackageResource(method)` — [`L476`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L476)
  - `toggleResource(method)` — [`L420`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L420)
  - `toggleTopLevelResource(method)` — [`L428`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L428)
  - `updateItem(method)` — [`L295`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L295)
  - `agentDir` — [`L187`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L187)
  - `cwd` — [`L186`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L186)
  - `filteredItems` — [`L181`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L181)
  - `flatItems` — [`L180`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L180)
  - `groups` — [`L179`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L179)
  - `maxVisible` — [`L184`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L184)
  - `onCancel` — [`L189`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L189)
  - `onExit` — [`L190`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L190)
  - `onToggle` — [`L191`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L191)
  - `searchInput` — [`L183`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L183)
  - `selectedIndex` — [`L182`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L182)
  - `settingsManager` — [`L185`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L185)
- protocol/private: `_focused`[`L193`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L193)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`matchesKey`](../../../../../tui/src/keys.ts.md#matchesKey), [`handleInput`](../../../../../tui/src/components/input.ts.md#Input.handleInput), [`SettingsManager`](../../../core/settings-manager.ts.md#SettingsManager), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`getValue`](../../../../../tui/src/components/input.ts.md#Input.getValue), [`bold`](../theme/theme.ts.md#Theme.bold), [`Input`](../../../../../tui/src/components/input.ts.md#Input), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`CONFIG_DIR_NAME`](../../../config.ts.md#CONFIG_DIR_NAME), [`setProjectPackages`](../../../core/settings-manager.ts.md#SettingsManager.setProjectPackages), [`setPackages`](../../../core/settings-manager.ts.md#SettingsManager.setPackages), [`scope`](../../../core/package-manager.ts.md#PathMetadata.scope), [`render`](../../../../../tui/src/components/input.ts.md#Input.render), [`source`](../../../core/package-manager.ts.md#PathMetadata.source), [`packages`](../../../core/settings-manager.ts.md#Settings.packages), [`getGlobalSettings`](../../../core/settings-manager.ts.md#SettingsManager.getGlobalSettings), [`PackageSource`](../../../core/settings-manager.ts.md#PackageSource), [`origin`](../../../core/package-manager.ts.md#PathMetadata.origin), [`setExtensionPaths`](../../../core/settings-manager.ts.md#SettingsManager.setExtensionPaths), [`getProjectSettings`](../../../core/settings-manager.ts.md#SettingsManager.getProjectSettings), [`setSkillPaths`](../../../core/settings-manager.ts.md#SettingsManager.setSkillPaths), [`setProjectExtensionPaths`](../../../core/settings-manager.ts.md#SettingsManager.setProjectExtensionPaths), [`setPromptTemplatePaths`](../../../core/settings-manager.ts.md#SettingsManager.setPromptTemplatePaths), [`baseDir`](../../../core/package-manager.ts.md#PathMetadata.baseDir), [`setThemePaths`](../../../core/settings-manager.ts.md#SettingsManager.setThemePaths), [`metadata`](config-selector.ts.md#ResourceItem.metadata), [`setProjectPromptTemplatePaths`](../../../core/settings-manager.ts.md#SettingsManager.setProjectPromptTemplatePaths), [`setProjectSkillPaths`](../../../core/settings-manager.ts.md#SettingsManager.setProjectSkillPaths), [`setProjectThemePaths`](../../../core/settings-manager.ts.md#SettingsManager.setProjectThemePaths), [`subgroups`](config-selector.ts.md#ResourceGroup.subgroups), [`ResourceItem`](config-selector.ts.md#ResourceItem), [`FlatEntry`](config-selector.ts.md#FlatEntry), [`focused`](../../../../../tui/src/components/input.ts.md#Input.focused), [`resourceType`](config-selector.ts.md#ResourceItem.resourceType), [`path`](config-selector.ts.md#ResourceItem.path)  (+7 more)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`<constructor>`](config-selector.ts.md#ConfigSelectorComponent.-constructor), [`<set>focused`](config-selector.ts.md#ConfigSelectorComponent.-set-focused), [`resourceList`](config-selector.ts.md#ConfigSelectorComponent.resourceList), [`getResourceList`](config-selector.ts.md#ConfigSelectorComponent.getResourceList)

### `ResourceSubgroup`
- def: [`packages/coding-agent/src/modes/interactive/components/config-selector.ts:43`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L43)
- signature: `interface ResourceSubgroup`
- members:
  - `items` — [`L46`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L46)
  - `label` — [`L45`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L45)
  - `type` — [`L44`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L44)
- uses (calls/refs, reference-scoped): [`ResourceItem`](config-selector.ts.md#ResourceItem), [`ResourceType`](config-selector.ts.md#ResourceType)
- used by: [`buildGroups`](config-selector.ts.md#buildGroups), [`render`](config-selector.ts.md#ResourceList.render), [`filterItems`](config-selector.ts.md#ResourceList.filterItems), [`updateItem`](config-selector.ts.md#ResourceList.updateItem), [`buildFlatList`](config-selector.ts.md#ResourceList.buildFlatList), [`subgroups`](config-selector.ts.md#ResourceGroup.subgroups), [`FlatEntry`](config-selector.ts.md#FlatEntry)

### `ResourceType`
- def: [`packages/coding-agent/src/modes/interactive/components/config-selector.ts:24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L24)
- signature: `type ResourceType`
- used by: [`buildGroups`](config-selector.ts.md#buildGroups), [`resourceType`](config-selector.ts.md#ResourceItem.resourceType), [`type`](config-selector.ts.md#ResourceSubgroup.type), [`RESOURCE_TYPE_LABELS`](config-selector.ts.md#RESOURCE_TYPE_LABELS)

## Functions
- `buildGroups(resolved: ResolvedPaths)` — [`L72`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L72)
- `getGroupLabel(metadata: PathMetadata)` — [`L58`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L58)

## Module values
- `RESOURCE_TYPE_LABELS` — [`L26`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/config-selector.ts#L26)


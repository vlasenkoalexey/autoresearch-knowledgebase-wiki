---
title: 'Module: packages/coding-agent/src/core/keybindings.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/keybindings.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`keybindings.ts`/
symbols:
  KeybindingsManager.-constructor: KeybindingsManager#`<constructor>`().
  KeybindingsManager: KeybindingsManager#
  KEYBINDINGS: KEYBINDINGS.
  migrateKeybindingsConfig: migrateKeybindingsConfig().
  AppKeybinding: AppKeybinding#
  KeybindingsManager.loadFromFile: KeybindingsManager#loadFromFile().
  KeybindingsManager.create: KeybindingsManager#create().
  KeybindingsManager.reload: KeybindingsManager#reload().
  KeybindingsManager.getEffectiveConfig: KeybindingsManager#getEffectiveConfig().
  toKeybindingsConfig: toKeybindingsConfig().
  KEYBINDING_NAME_MIGRATIONS: KEYBINDING_NAME_MIGRATIONS.
  Keybindings: '`"@earendil-works/pi-tui"`/Keybindings#'
  isLegacyKeybindingName: isLegacyKeybindingName().
  orderKeybindingsConfig: orderKeybindingsConfig().
  loadRawConfig: loadRawConfig().
  migrateKeybindingsConfig.typeLiteral17.config: migrateKeybindingsConfig().typeLiteral17:config.
  KeybindingsManager.configPath: KeybindingsManager#configPath.
  AppKeybindings: AppKeybindings#
  isRecord: isRecord().
  migrateKeybindingsConfig.typeLiteral17.migrated: migrateKeybindingsConfig().typeLiteral17:migrated.
  AppKeybindings.-app.interrupt: AppKeybindings#`"app.interrupt"`.
  AppKeybindings.-app.clear: AppKeybindings#`"app.clear"`.
  AppKeybindings.-app.input.clear: AppKeybindings#`"app.input.clear"`.
  AppKeybindings.-app.shortcuts: AppKeybindings#`"app.shortcuts"`.
  AppKeybindings.-app.exit: AppKeybindings#`"app.exit"`.
  AppKeybindings.-app.suspend: AppKeybindings#`"app.suspend"`.
  AppKeybindings.-app.model.select: AppKeybindings#`"app.model.select"`.
  AppKeybindings.-app.model.toggleScope: AppKeybindings#`"app.model.toggleScope"`.
  AppKeybindings.-app.configuration.previousTab: AppKeybindings#`"app.configuration.previousTab"`.
  AppKeybindings.-app.tools.expand: AppKeybindings#`"app.tools.expand"`.
  AppKeybindings.-app.messages.expand: AppKeybindings#`"app.messages.expand"`.
  AppKeybindings.-app.thinking.toggle: AppKeybindings#`"app.thinking.toggle"`.
  AppKeybindings.-app.subagents.focus: AppKeybindings#`"app.subagents.focus"`.
  AppKeybindings.-app.heartbeats.open: AppKeybindings#`"app.heartbeats.open"`.
  AppKeybindings.-app.heartbeats.openSelected: AppKeybindings#`"app.heartbeats.openSelected"`.
  AppKeybindings.-app.editor.external: AppKeybindings#`"app.editor.external"`.
  AppKeybindings.-app.prompt.stash: AppKeybindings#`"app.prompt.stash"`.
  AppKeybindings.-app.message.followUp: AppKeybindings#`"app.message.followUp"`.
  AppKeybindings.-app.message.navigateOlder: AppKeybindings#`"app.message.navigateOlder"`.
  AppKeybindings.-app.message.navigateNewer: AppKeybindings#`"app.message.navigateNewer"`.
  AppKeybindings.-app.message.moveEarlier: AppKeybindings#`"app.message.moveEarlier"`.
  AppKeybindings.-app.message.moveLater: AppKeybindings#`"app.message.moveLater"`.
  AppKeybindings.-app.clipboard.pasteImage: AppKeybindings#`"app.clipboard.pasteImage"`.
  AppKeybindings.-app.clipboard.copyLoginUrl: AppKeybindings#`"app.clipboard.copyLoginUrl"`.
  AppKeybindings.-app.session.new: AppKeybindings#`"app.session.new"`.
  AppKeybindings.-app.session.tree: AppKeybindings#`"app.session.tree"`.
  AppKeybindings.-app.session.fork: AppKeybindings#`"app.session.fork"`.
  AppKeybindings.-app.session.resume: AppKeybindings#`"app.session.resume"`.
  AppKeybindings.-app.agents.back: AppKeybindings#`"app.agents.back"`.
  AppKeybindings.-app.agents.open: AppKeybindings#`"app.agents.open"`.
  AppKeybindings.-app.modal.back: AppKeybindings#`"app.modal.back"`.
  AppKeybindings.-app.agents.reply: AppKeybindings#`"app.agents.reply"`.
  AppKeybindings.-app.agents.new: AppKeybindings#`"app.agents.new"`.
  AppKeybindings.-app.agents.delete: AppKeybindings#`"app.agents.delete"`.
  AppKeybindings.-app.agents.program: AppKeybindings#`"app.agents.program"`.
  AppKeybindings.-app.agents.rename: AppKeybindings#`"app.agents.rename"`.
  AppKeybindings.-app.tree.foldOrUp: AppKeybindings#`"app.tree.foldOrUp"`.
  AppKeybindings.-app.tree.unfoldOrDown: AppKeybindings#`"app.tree.unfoldOrDown"`.
  AppKeybindings.-app.tree.editLabel: AppKeybindings#`"app.tree.editLabel"`.
  AppKeybindings.-app.tree.toggleLabelTimestamp: AppKeybindings#`"app.tree.toggleLabelTimestamp"`.
  AppKeybindings.-app.models.save: AppKeybindings#`"app.models.save"`.
  AppKeybindings.-app.models.enableAll: AppKeybindings#`"app.models.enableAll"`.
  AppKeybindings.-app.models.clearAll: AppKeybindings#`"app.models.clearAll"`.
  AppKeybindings.-app.models.toggleProvider: AppKeybindings#`"app.models.toggleProvider"`.
  AppKeybindings.-app.models.reorderUp: AppKeybindings#`"app.models.reorderUp"`.
  AppKeybindings.-app.models.reorderDown: AppKeybindings#`"app.models.reorderDown"`.
  AppKeybindings.-app.tree.filter.default: AppKeybindings#`"app.tree.filter.default"`.
  AppKeybindings.-app.tree.filter.noTools: AppKeybindings#`"app.tree.filter.noTools"`.
  AppKeybindings.-app.tree.filter.userOnly: AppKeybindings#`"app.tree.filter.userOnly"`.
  AppKeybindings.-app.tree.filter.labeledOnly: AppKeybindings#`"app.tree.filter.labeledOnly"`.
  AppKeybindings.-app.tree.filter.all: AppKeybindings#`"app.tree.filter.all"`.
  AppKeybindings.-app.tree.filter.cycleForward: AppKeybindings#`"app.tree.filter.cycleForward"`.
  AppKeybindings.-app.tree.filter.cycleBackward: AppKeybindings#`"app.tree.filter.cycleBackward"`.
---
# Module: [`packages/coding-agent/src/core/keybindings.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts)

## Classes
### `AppKeybinding`
- def: [`packages/coding-agent/src/core/keybindings.ts:69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L69)
- signature: `type AppKeybinding`
- uses (calls/refs, reference-scoped): [`AppKeybindings`](keybindings.ts.md#AppKeybindings)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../modes/interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](extensions/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-index.ts), [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`init`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.init), [`getAppKeyDisplay`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.getAppKeyDisplay), [`custom-editor.ts`](../modes/interactive/components/custom-editor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-custom-editor.ts), [`onAction`](../modes/interactive/components/custom-editor.ts.md#CustomEditor.onAction), [`getKeybinding`](../modes/interactive/feature-hints.ts.md#FeatureHintContext.getKeybinding), [`splitRepeatedKeybinding`](../modes/interactive/components/custom-editor.ts.md#CustomEditor.splitRepeatedKeybinding), [`actionHandlers`](../modes/interactive/components/custom-editor.ts.md#CustomEditor.actionHandlers), [`feature-hints.ts`](../modes/interactive/feature-hints.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-feature-hints.ts)

### `AppKeybindings`
- def: [`packages/coding-agent/src/core/keybindings.ts:13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L13)
- signature: `interface AppKeybindings`
- members:
  - `"app.agents.back"` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L42)
  - `"app.agents.delete"` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L47)
  - `"app.agents.new"` — [`L46`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L46)
  - `"app.agents.open"` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L43)
  - `"app.agents.program"` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L48)
  - `"app.agents.rename"` — [`L49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L49)
  - `"app.agents.reply"` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L45)
  - `"app.clear"` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L15)
  - `"app.clipboard.copyLoginUrl"` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L37)
  - `"app.clipboard.pasteImage"` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L36)
  - `"app.configuration.previousTab"` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L22)
  - `"app.editor.external"` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L29)
  - `"app.exit"` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L18)
  - `"app.heartbeats.open"` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L27)
  - `"app.heartbeats.openSelected"` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L28)
  - `"app.input.clear"` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L16)
  - `"app.interrupt"` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L14)
  - `"app.message.followUp"` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L31)
  - `"app.message.moveEarlier"` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L34)
  - `"app.message.moveLater"` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L35)
  - `"app.message.navigateNewer"` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L33)
  - `"app.message.navigateOlder"` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L32)
  - `"app.messages.expand"` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L24)
  - `"app.modal.back"` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L44)
  - `"app.model.select"` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L20)
  - `"app.model.toggleScope"` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L21)
  - `"app.models.clearAll"` — [`L56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L56)
  - `"app.models.enableAll"` — [`L55`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L55)
  - `"app.models.reorderDown"` — [`L59`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L59)
  - `"app.models.reorderUp"` — [`L58`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L58)
  - `"app.models.save"` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L54)
  - `"app.models.toggleProvider"` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L57)
  - `"app.prompt.stash"` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L30)
  - `"app.session.fork"` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L40)
  - `"app.session.new"` — [`L38`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L38)
  - `"app.session.resume"` — [`L41`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L41)
  - `"app.session.tree"` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L39)
  - `"app.shortcuts"` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L17)
  - `"app.subagents.focus"` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L26)
  - `"app.suspend"` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L19)
  - `"app.thinking.toggle"` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L25)
  - `"app.tools.expand"` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L23)
  - `"app.tree.editLabel"` — [`L52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L52)
  - `"app.tree.filter.all"` — [`L64`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L64)
  - `"app.tree.filter.cycleBackward"` — [`L66`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L66)
  - `"app.tree.filter.cycleForward"` — [`L65`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L65)
  - `"app.tree.filter.default"` — [`L60`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L60)
  - `"app.tree.filter.labeledOnly"` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L63)
  - `"app.tree.filter.noTools"` — [`L61`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L61)
  - `"app.tree.filter.userOnly"` — [`L62`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L62)
  - `"app.tree.foldOrUp"` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L50)
  - `"app.tree.toggleLabelTimestamp"` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L53)
  - `"app.tree.unfoldOrDown"` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L51)
- used by: [`AppKeybinding`](keybindings.ts.md#AppKeybinding), [`Keybindings`](keybindings.ts.md#Keybindings)

### `Keybindings`
- def: [`packages/coding-agent/src/core/keybindings.ts:72`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L72)
- doc: Global keybinding registry.
- signature: `interface Keybindings`
- uses (calls/refs, reference-scoped): [`AppKeybindings`](keybindings.ts.md#AppKeybindings)
- used by: [`Keybinding`](../../../tui/src/keybindings.ts.md#Keybinding)

### `KeybindingsManager`  ·  implements/extends KeybindingsManager
- def: [`packages/coding-agent/src/core/keybindings.ts:366`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L366)
- signature: `class KeybindingsManager`
- members:
  - `<constructor>(userBindings?: KeybindingsConfig, configPath?: string | undefined)` — [`L369`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L369)
  - `create(method)` — [`L374`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L374)
  - `getEffectiveConfig(method)` — [`L385`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L385)
  - `loadFromFile(method)` — [`L389`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L389)
  - `reload(method)` — [`L380`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L380)
  - `configPath` — [`L367`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L367)
- uses (calls/refs, reference-scoped): [`getAgentDir`](../config.ts.md#getAgentDir), [`KeybindingsConfig`](../../../tui/src/keybindings.ts.md#KeybindingsConfig), [`KEYBINDINGS`](keybindings.ts.md#KEYBINDINGS), [`migrateKeybindingsConfig`](keybindings.ts.md#migrateKeybindingsConfig), [`getResolvedBindings`](../../../tui/src/keybindings.ts.md#KeybindingsManager.getResolvedBindings), [`KeybindingsManager`](../../../tui/src/keybindings.ts.md#KeybindingsManager), [`setUserBindings`](../../../tui/src/keybindings.ts.md#KeybindingsManager.setUserBindings), [`toKeybindingsConfig`](keybindings.ts.md#toKeybindingsConfig), [`loadRawConfig`](keybindings.ts.md#loadRawConfig), [`config`](keybindings.ts.md#migrateKeybindingsConfig.typeLiteral17.config)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../modes/interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`index.ts`](extensions/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-index.ts), [`agents-view-mode.ts`](../modes/agents-view/agents-view-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agents-view-agents-view-mode.ts), [`<constructor>`](../modes/agents-view/agents-view-mode.ts.md#AgentsViewMode.-constructor), [`<constructor>`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.-constructor), [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`handleReloadCommand`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleReloadCommand), [`setupExtensionShortcuts`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.setupExtensionShortcuts), [`<constructor>`](../modes/interactive/components/custom-editor.ts.md#CustomEditor.-constructor), [`extension-editor.ts`](../modes/interactive/components/extension-editor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-extension-editor.ts), [`<constructor>`](../modes/interactive/components/extension-editor.ts.md#ExtensionEditorComponent.-constructor), [`promptForMissingSessionCwd`](../main.ts.md#promptForMissingSessionCwd), [`custom`](extensions/types.ts.md#ExtensionUIContext.custom), [`custom-editor.ts`](../modes/interactive/components/custom-editor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-custom-editor.ts), [`getHotkeysGuide`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.getHotkeysGuide), [`keybindings`](../modes/agents-view/agents-view-mode.ts.md#AgentsViewMode.keybindings), [`EditorFactory`](extensions/types.ts.md#EditorFactory), [`keybindings`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.keybindings), [`showExtensionCustom`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.showExtensionCustom), [`keybindings`](../modes/interactive/components/custom-editor.ts.md#CustomEditor.keybindings), [`KeybindingsManager`](../../../tui/src/keybindings.ts.md#KeybindingsManager), [`keybindings`](../modes/interactive/components/extension-editor.ts.md#ExtensionEditorComponent.keybindings)  (27 test-only)

## Functions
- `isLegacyKeybindingName(key: string)` — [`L296`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L296)
- `isRecord(value: unknown)` — [`L292`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L292)
- `loadRawConfig(path: string)` — [`L356`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L356)
- `migrateKeybindingsConfig(rawConfig: Record<string, unknown>)` — [`L316`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L316)
- `orderKeybindingsConfig(config: Record<string, unknown>)` — [`L338`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L338)
- `toKeybindingsConfig(value: unknown)` — [`L300`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L300)

## Module values
- `KEYBINDINGS` — [`L75`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L75)
- `KEYBINDING_NAME_MIGRATIONS` — [`L230`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L230)
- `config` — [`L317`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L317)
- `migrated` — [`L318`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/keybindings.ts#L318)


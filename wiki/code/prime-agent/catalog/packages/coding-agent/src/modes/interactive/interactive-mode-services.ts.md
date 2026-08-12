---
title: 'Module: packages/coding-agent/src/modes/interactive/interactive-mode-services.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/interactive-mode-services.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/`interactive-mode-services.ts`/
symbols:
  createInteractiveModeLocalSessionHost: createInteractiveModeLocalSessionHost().
  createInteractiveModeUiServicesFromServices: createInteractiveModeUiServicesFromServices().
  createInteractiveModeUiServices: createInteractiveModeUiServices().
  InteractiveModeUiServices.settingsManager: InteractiveModeUiServices#settingsManager.
  InteractiveModeUiServices: InteractiveModeUiServices#
  InteractiveModeUiServices.getThemes: InteractiveModeUiServices#getThemes().
  InteractiveModeUiServices.getInitialCwd: InteractiveModeUiServices#getInitialCwd().
  InteractiveModeUiServices.modelRegistry: InteractiveModeUiServices#modelRegistry.
  InteractiveModeLocalSessionHost.getExtensionRunner: InteractiveModeLocalSessionHost#getExtensionRunner().
  InteractiveModeUiServices.getInitialSessionName: InteractiveModeUiServices#getInitialSessionName().
  InteractiveModeLocalSessionHost: InteractiveModeLocalSessionHost#
  InteractiveModeLocalToolRendererDefinition: InteractiveModeLocalToolRendererDefinition#
  LocalExtensionNewSessionOptions: LocalExtensionNewSessionOptions#
  LocalExtensionForkOptions: LocalExtensionForkOptions#
  LocalExtensionSwitchOptions: LocalExtensionSwitchOptions#
  InteractiveModeLocalSessionHost.createUiServices: InteractiveModeLocalSessionHost#createUiServices().
  InteractiveModeLocalSessionHost.getToolRendererDefinition: InteractiveModeLocalSessionHost#getToolRendererDefinition().
  InteractiveModeLocalSessionHost.switchSession: InteractiveModeLocalSessionHost#switchSession().
  createInteractiveModeUiServicesFromServices.options-typeLiteral6.services: createInteractiveModeUiServicesFromServices().(options)typeLiteral6:services.
  InteractiveModeLocalSessionHost.getSessionManager: InteractiveModeLocalSessionHost#getSessionManager().
  InteractiveModeLocalSessionHost.bindExtensions: InteractiveModeLocalSessionHost#bindExtensions().
  InteractiveModeLocalSessionHost.newSession: InteractiveModeLocalSessionHost#newSession().
  InteractiveModeLocalSessionHost.fork: InteractiveModeLocalSessionHost#fork().
  createInteractiveModeUiServicesFromServices.options-typeLiteral6.sessionManager: createInteractiveModeUiServicesFromServices().(options)typeLiteral6:sessionManager.
  InteractiveModeLocalSessionHost.getSystemPrompt: InteractiveModeLocalSessionHost#getSystemPrompt().
  InteractiveModeLocalSessionHost.getAbortSignal: InteractiveModeLocalSessionHost#getAbortSignal().
  InteractiveModeLocalSessionHost.newSession.Promise.typeLiteral3.cancelled: InteractiveModeLocalSessionHost#newSession().Promise:typeLiteral3:cancelled.
  InteractiveModeLocalSessionHost.fork.Promise.typeLiteral4.cancelled: InteractiveModeLocalSessionHost#fork().Promise:typeLiteral4:cancelled.
  InteractiveModeLocalSessionHost.fork.Promise.typeLiteral4.selectedText: InteractiveModeLocalSessionHost#fork().Promise:typeLiteral4:selectedText.
  InteractiveModeLocalSessionHost.switchSession.Promise.typeLiteral5.cancelled: InteractiveModeLocalSessionHost#switchSession().Promise:typeLiteral5:cancelled.
---
# Module: [`packages/coding-agent/src/modes/interactive/interactive-mode-services.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts)

## Classes
### `InteractiveModeLocalSessionHost`
- def: [`packages/coding-agent/src/modes/interactive/interactive-mode-services.ts:43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L43)
- doc: In-process compatibility adapter for local-only extension hooks.
- signature: `interface InteractiveModeLocalSessionHost`
- members:
  - `bindExtensions(method)` — [`L50`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L50)
  - `createUiServices(method)` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L44)
  - `fork(method)` — [`L52`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L52)
  - `getAbortSignal(method)` — [`L49`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L49)
  - `getExtensionRunner(method)` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L46)
  - `getSessionManager(method)` — [`L45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L45)
  - `getSystemPrompt(method)` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L48)
  - `getToolRendererDefinition(method)` — [`L47`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L47)
  - `newSession(method)` — [`L51`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L51)
  - `switchSession(method)` — [`L53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L53)
  - `cancelled` — [`L51`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L51)
  - `cancelled` — [`L52`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L52)
  - `cancelled` — [`L53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L53)
  - `selectedText` — [`L52`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L52)
- uses (calls/refs, reference-scoped): [`SessionManager`](../../core/session-manager.ts.md#SessionManager), [`ExtensionRunner`](../../core/extensions/runner.ts.md#ExtensionRunner), [`InteractiveModeUiServices`](interactive-mode-services.ts.md#InteractiveModeUiServices), [`InteractiveModeLocalToolRendererDefinition`](interactive-mode-services.ts.md#InteractiveModeLocalToolRendererDefinition), [`LocalExtensionForkOptions`](interactive-mode-services.ts.md#LocalExtensionForkOptions), [`LocalExtensionNewSessionOptions`](interactive-mode-services.ts.md#LocalExtensionNewSessionOptions), [`LocalExtensionSwitchOptions`](interactive-mode-services.ts.md#LocalExtensionSwitchOptions), [`ExtensionBindings`](../../core/agent-session.ts.md#ExtensionBindings)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`<constructor>`](interactive-mode.ts.md#InteractiveMode.-constructor), [`addMessageToChat`](interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`handleReloadCommand`](interactive-mode.ts.md#InteractiveMode.handleReloadCommand), [`showLoadedResources`](interactive-mode.ts.md#InteractiveMode.showLoadedResources), [`bindCurrentSessionExtensions`](interactive-mode.ts.md#InteractiveMode.bindCurrentSessionExtensions), [`setupExtensionShortcuts`](interactive-mode.ts.md#InteractiveMode.setupExtensionShortcuts), [`createBaseAutocompleteProvider`](interactive-mode.ts.md#InteractiveMode.createBaseAutocompleteProvider), [`createInteractiveModeLocalSessionHost`](interactive-mode-services.ts.md#createInteractiveModeLocalSessionHost), [`rebindCurrentSession`](interactive-mode.ts.md#InteractiveMode.rebindCurrentSession), [`cancelled`](interactive-mode.ts.md#InteractiveMode.handleResumeSession.Promise.typeLiteral3694.cancelled), [`getHotkeysGuide`](interactive-mode.ts.md#InteractiveMode.getHotkeysGuide), [`loadToolDefinition`](interactive-mode.ts.md#InteractiveMode.loadToolDefinition), [`preloadToolDefinitions`](interactive-mode.ts.md#InteractiveMode.preloadToolDefinitions), [`getLocalSessionHost`](interactive-mode.ts.md#InteractiveMode.getLocalSessionHost), [`localSessionHost`](interactive-mode.ts.md#InteractiveMode.localSessionHost), [`localSessionHost`](interactive-mode.ts.md#InteractiveModeOptions.localSessionHost)

### `InteractiveModeLocalToolRendererDefinition`
- def: [`packages/coding-agent/src/modes/interactive/interactive-mode-services.ts:30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L30)
- signature: `type InteractiveModeLocalToolRendererDefinition`
- uses (calls/refs, reference-scoped): [`ToolDefinition`](../../core/extensions/types.ts.md#ToolDefinition)
- used by: [`interactive-mode.ts`](interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`createInteractiveModeLocalSessionHost`](interactive-mode-services.ts.md#createInteractiveModeLocalSessionHost), [`createToolExecutionDefinition`](interactive-mode.ts.md#InteractiveMode.createToolExecutionDefinition), [`getToolRendererDefinition`](interactive-mode-services.ts.md#InteractiveModeLocalSessionHost.getToolRendererDefinition)

### `InteractiveModeUiServices`
- def: [`packages/coding-agent/src/modes/interactive/interactive-mode-services.ts:17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L17)
- doc: Local UI services that are intentionally separate from AgentConnection.
- signature: `interface InteractiveModeUiServices`
- members:
  - `getInitialCwd(method)` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L20)
  - `getInitialSessionName(method)` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L21)
  - `getThemes(method)` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L22)
  - `modelRegistry` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L19)
  - `settingsManager` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L18)
- uses (calls/refs, reference-scoped): [`SettingsManager`](../../core/settings-manager.ts.md#SettingsManager), [`ModelRegistry`](../../core/model-registry.ts.md#ModelRegistry), [`Theme`](theme/theme.ts.md#Theme)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`agents-view-mode.ts`](../agents-view/agents-view-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agents-view-agents-view-mode.ts), [`<constructor>`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.-constructor), [`<constructor>`](interactive-mode.ts.md#InteractiveMode.-constructor), [`handleReloadCommand`](interactive-mode.ts.md#InteractiveMode.handleReloadCommand), [`bindCurrentSessionExtensions`](interactive-mode.ts.md#InteractiveMode.bindCurrentSessionExtensions), [`<get>settingsManager`](interactive-mode.ts.md#InteractiveMode.-get-settingsManager), [`rebindCurrentSession`](interactive-mode.ts.md#InteractiveMode.rebindCurrentSession), [`createInteractiveModeUiServicesFromServices`](interactive-mode-services.ts.md#createInteractiveModeUiServicesFromServices), [`createInteractiveModeUiServices`](interactive-mode-services.ts.md#createInteractiveModeUiServices), [`loadStartupNotices`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.loadStartupNotices), [`<get>modelRegistry`](interactive-mode.ts.md#InteractiveMode.-get-modelRegistry), [`uiServices`](../agents-view/agents-view-mode.ts.md#AgentsViewModeOptions.uiServices), [`getCurrentCwd`](interactive-mode.ts.md#InteractiveMode.getCurrentCwd), [`getSplashCwd`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.getSplashCwd), [`resolveAgentsViewSessionUiServices`](../agents-view/agents-view-mode.ts.md#resolveAgentsViewSessionUiServices), [`uiServices`](interactive-mode.ts.md#InteractiveMode.uiServices), [`getCurrentSessionName`](interactive-mode.ts.md#InteractiveMode.getCurrentSessionName), [`getSavedSessionCwd`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.getSavedSessionCwd), [`createUiServicesForSession`](../agents-view/agents-view-mode.ts.md#AgentsViewModeOptions.createUiServicesForSession), [`createUiServices`](interactive-mode-services.ts.md#InteractiveModeLocalSessionHost.createUiServices), [`uiServices`](interactive-mode.ts.md#InteractiveModeOptions.uiServices)  (5 test-only)

### `LocalExtensionForkOptions`
- def: [`packages/coding-agent/src/modes/interactive/interactive-mode-services.ts:26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L26)
- signature: `type LocalExtensionForkOptions`
- uses (calls/refs, reference-scoped): [`ExtensionCommandContext`](../../core/extensions/types.ts.md#ExtensionCommandContext), [`fork`](../../core/extensions/types.ts.md#ExtensionCommandContext.fork)
- used by: [`fork`](interactive-mode-services.ts.md#InteractiveModeLocalSessionHost.fork)

### `LocalExtensionNewSessionOptions`
- def: [`packages/coding-agent/src/modes/interactive/interactive-mode-services.ts:25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L25)
- signature: `type LocalExtensionNewSessionOptions`
- uses (calls/refs, reference-scoped): [`ExtensionCommandContext`](../../core/extensions/types.ts.md#ExtensionCommandContext), [`newSession`](../../core/extensions/types.ts.md#ExtensionCommandContext.newSession)
- used by: [`newSession`](interactive-mode-services.ts.md#InteractiveModeLocalSessionHost.newSession)

### `LocalExtensionSwitchOptions`
- def: [`packages/coding-agent/src/modes/interactive/interactive-mode-services.ts:27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L27)
- signature: `type LocalExtensionSwitchOptions`
- uses (calls/refs, reference-scoped): [`ExtensionCommandContext`](../../core/extensions/types.ts.md#ExtensionCommandContext), [`switchSession`](../../core/extensions/types.ts.md#ExtensionCommandContext.switchSession)
- used by: [`switchSession`](interactive-mode-services.ts.md#InteractiveModeLocalSessionHost.switchSession)

## Functions
- `createInteractiveModeLocalSessionHost(runtimeHost: AgentSessionRuntime)` — [`L81`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L81)
- `createInteractiveModeUiServices(session: AgentSession)` — [`L56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L56)
- `createInteractiveModeUiServicesFromServices(options: { services: AgentSessionServices; sessionManager: SessionManager; })` — [`L66`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L66)

## Module values
- `services` — [`L67`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L67)
- `sessionManager` — [`L68`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/interactive-mode-services.ts#L68)


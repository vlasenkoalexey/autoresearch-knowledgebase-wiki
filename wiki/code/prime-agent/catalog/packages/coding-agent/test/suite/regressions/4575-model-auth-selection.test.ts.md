---
title: 'Module: packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/regressions/`4575-model-auth-selection.test.ts`/
symbols:
  ConnectionAuthRefreshHarness.connectionModels: ConnectionAuthRefreshHarness#connectionModels.
  ConnectionAuthRefreshHarness.connectionModelCatalog: ConnectionAuthRefreshHarness#connectionModelCatalog.
  ConnectionAuthRefreshHarness.agentConnection.typeLiteral0.getModelCatalog: ConnectionAuthRefreshHarness#agentConnection.typeLiteral0:getModelCatalog().
  ConnectionAuthRefreshHarness.connectionModelsRefreshInFlight: ConnectionAuthRefreshHarness#connectionModelsRefreshInFlight.
  ConnectionAuthRefreshHarness.getConnectionModelCatalog: ConnectionAuthRefreshHarness#getConnectionModelCatalog().
  InteractiveAutocompleteHarness: InteractiveAutocompleteHarness#
  InteractiveAutocompleteHarness.connectionState.typeLiteral5.scopedModels.Array.typeLiteral6.model: InteractiveAutocompleteHarness#connectionState.typeLiteral5:scopedModels.Array:typeLiteral6:model.
  InteractiveAutocompleteHarness.connectionModelCatalog: InteractiveAutocompleteHarness#connectionModelCatalog.
  ConnectionAuthRefreshHarness.connectionConfiguredProviders: ConnectionAuthRefreshHarness#connectionConfiguredProviders.
  ConnectionAuthRefreshHarness.applyConnectionModelCatalog: ConnectionAuthRefreshHarness#applyConnectionModelCatalog().
  ConnectionAuthRefreshHarness.getConnectionAvailableModels: ConnectionAuthRefreshHarness#getConnectionAvailableModels().
  ConnectionAuthRefreshHarness: ConnectionAuthRefreshHarness#
  ConnectionAuthRefreshHarness.agentConnection: ConnectionAuthRefreshHarness#agentConnection.
  ConnectionAuthRefreshHarness.connectionModelsFetchedAt: ConnectionAuthRefreshHarness#connectionModelsFetchedAt.
  ConnectionAuthRefreshHarness.connectionModelsRefreshVersion: ConnectionAuthRefreshHarness#connectionModelsRefreshVersion.
  ConnectionAuthRefreshHarness.refreshConnectionModelsAfterAuthChange: ConnectionAuthRefreshHarness#refreshConnectionModelsAfterAuthChange().
  InteractiveAutocompleteHarness.connectionState: InteractiveAutocompleteHarness#connectionState.
  InteractiveAutocompleteHarness.connectionState.typeLiteral5.scopedModels: InteractiveAutocompleteHarness#connectionState.typeLiteral5:scopedModels.
  InteractiveAutocompleteHarness.connectionCommands: InteractiveAutocompleteHarness#connectionCommands.
  InteractiveAutocompleteHarness.skillCommands: InteractiveAutocompleteHarness#skillCommands.
  InteractiveAutocompleteHarness.uiServices: InteractiveAutocompleteHarness#uiServices.
  InteractiveAutocompleteHarness.uiServices.typeLiteral7.settingsManager: InteractiveAutocompleteHarness#uiServices.typeLiteral7:settingsManager.
  InteractiveAutocompleteHarness.uiServices.typeLiteral7.settingsManager.typeLiteral8.getEnableSkillCommands: InteractiveAutocompleteHarness#uiServices.typeLiteral7:settingsManager.typeLiteral8:getEnableSkillCommands().
  InteractiveAutocompleteHarness.bindLocalSessionExtensions: InteractiveAutocompleteHarness#bindLocalSessionExtensions.
  InteractiveAutocompleteHarness.fdPath: InteractiveAutocompleteHarness#fdPath.
  InteractiveAutocompleteHarness.currentModelSupportsFastMode: InteractiveAutocompleteHarness#currentModelSupportsFastMode().
  InteractiveAutocompleteHarness.getAvailableThinkingLevels: InteractiveAutocompleteHarness#getAvailableThinkingLevels().
  InteractiveAutocompleteHarness.getCurrentCwd: InteractiveAutocompleteHarness#getCurrentCwd().
  InteractiveAutocompleteHarness.createBaseAutocompleteProvider: InteractiveAutocompleteHarness#createBaseAutocompleteProvider().
  ConnectionAuthRefreshHarness.invalidateConnectionModels: ConnectionAuthRefreshHarness#invalidateConnectionModels().
---
# Module: [`packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts)

## Classes
### `ConnectionAuthRefreshHarness`
- def: [`packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts:12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L12)
- signature: `interface ConnectionAuthRefreshHarness`
- members:
  - `applyConnectionModelCatalog(method)` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L21)
  - `getConnectionAvailableModels(method)` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L22)
  - `getConnectionModelCatalog(method)` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L23)
  - `getModelCatalog(method)` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L13)
  - `invalidateConnectionModels(method)` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L20)
  - `refreshConnectionModelsAfterAuthChange(method)` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L24)
  - `agentConnection` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L13)
  - `connectionConfiguredProviders` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L16)
  - `connectionModelCatalog` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L15)
  - `connectionModels` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L14)
  - `connectionModelsFetchedAt` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L17)
  - `connectionModelsRefreshInFlight` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L19)
  - `connectionModelsRefreshVersion` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L18)
- uses (calls/refs, reference-scoped): [`AgentConnectionModel`](../../../src/modes/agent-connection/types.ts.md#AgentConnectionModel), [`AgentConnectionModelCatalog`](../../../src/modes/agent-connection/types.ts.md#AgentConnectionModelCatalog)
- used by: (1 test-only callers)

### `InteractiveAutocompleteHarness`
- def: [`packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts:27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L27)
- signature: `interface InteractiveAutocompleteHarness`
- members:
  - `createBaseAutocompleteProvider(method)` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L38)
  - `currentModelSupportsFastMode(method)` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L35)
  - `getAvailableThinkingLevels(method)` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L36)
  - `getCurrentCwd(method)` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L37)
  - `getEnableSkillCommands(method)` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L32)
  - `bindLocalSessionExtensions` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L33)
  - `connectionCommands` — [`L30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L30)
  - `connectionModelCatalog` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L29)
  - `connectionState` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L28)
  - `fdPath` — [`L34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L34)
  - `model` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L28)
  - `scopedModels` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L28)
  - `settingsManager` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L32)
  - `skillCommands` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L31)
  - `uiServices` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4575-model-auth-selection.test.ts#L32)
- uses (calls/refs, reference-scoped): [`AgentConnectionModel`](../../../src/modes/agent-connection/types.ts.md#AgentConnectionModel), [`AutocompleteProvider`](../../../../tui/src/autocomplete.ts.md#AutocompleteProvider)
- used by: (1 test-only callers)


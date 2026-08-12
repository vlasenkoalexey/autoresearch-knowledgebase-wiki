---
title: 'Module: packages/coding-agent/test/suite/harness.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/harness.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/`harness.ts`/
symbols:
  Harness.session: Harness#session.
  createHarness: createHarness().
  Harness.setResponses: Harness#setResponses.
  Harness: Harness#
  Harness.tempDir: Harness#tempDir.
  getUserTexts: getUserTexts().
  Harness.cleanup: Harness#cleanup.
  Harness.sessionManager: Harness#sessionManager.
  getMessageText: getMessageText().
  Harness.getModel: Harness#getModel().
  getAssistantTexts: getAssistantTexts().
  Harness.eventsOfType: Harness#eventsOfType().
  Harness.getPendingResponseCount: Harness#getPendingResponseCount.
  Harness.authStorage: Harness#authStorage.
  Harness.faux: Harness#faux.
  Harness.settingsManager: Harness#settingsManager.
  Harness.events: Harness#events.
  Harness.models: Harness#models.
  HarnessOptions.extensionFactories: HarnessOptions#extensionFactories.
  HarnessOptions.subagentRuntimeHost: HarnessOptions#subagentRuntimeHost.
  HarnessOptions.tools: HarnessOptions#tools.
  Harness.appendResponses: Harness#appendResponses.
  HarnessOptions.models: HarnessOptions#models.
  HarnessOptions.settings: HarnessOptions#settings.
  HarnessOptions.resourceLoader: HarnessOptions#resourceLoader.
  HarnessOptions.agentObserveController: HarnessOptions#agentObserveController.
  HarnessOptions.agentMessageController: HarnessOptions#agentMessageController.
  HarnessOptions.autonomous: HarnessOptions#autonomous.
  HarnessOptions.autoRefineReviewer: HarnessOptions#autoRefineReviewer.
  MessageTextPart: MessageTextPart#
  MessageTextPart.typeLiteral0.text: MessageTextPart#typeLiteral0:text.
  HarnessOptions: HarnessOptions#
  HarnessOptions.api: HarnessOptions#api.
  HarnessOptions.provider: HarnessOptions#provider.
  HarnessOptions.systemPrompt: HarnessOptions#systemPrompt.
  HarnessOptions.withConfiguredAuth: HarnessOptions#withConfiguredAuth.
  HarnessOptions.persistSession: HarnessOptions#persistSession.
  HarnessOptions.rlmDepth: HarnessOptions#rlmDepth.
  HarnessOptions.rlmMaxDepth: HarnessOptions#rlmMaxDepth.
  HarnessOptions.serializedRefine: HarnessOptions#serializedRefine.
  HarnessOptions.initialGoal: HarnessOptions#initialGoal.
  createTempDir: createTempDir().
  MessageTextPart.typeLiteral0.type: MessageTextPart#typeLiteral0:type.
  HarnessOptions.initialGoal.typeLiteral40.objective: HarnessOptions#initialGoal.typeLiteral40:objective.
  HarnessOptions.initialGoal.typeLiteral40.tokenBudget: HarnessOptions#initialGoal.typeLiteral40:tokenBudget.
---
# Module: [`packages/coding-agent/test/suite/harness.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts)

## Classes
### `Harness`
- def: [`packages/coding-agent/test/suite/harness.ts:84`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L84)
- signature: `interface Harness`
- members:
  - `eventsOfType(method)` — [`L97`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L97)
  - `getModel(method)` — [`L91`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L91)
  - `appendResponses` — [`L94`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L94)
  - `authStorage` — [`L88`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L88)
  - `cleanup` — [`L99`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L99)
  - `events` — [`L96`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L96)
  - `faux` — [`L89`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L89)
  - `getPendingResponseCount` — [`L95`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L95)
  - `models` — [`L90`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L90)
  - `session` — [`L85`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L85)
  - `sessionManager` — [`L86`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L86)
  - `setResponses` — [`L93`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L93)
  - `settingsManager` — [`L87`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L87)
  - `tempDir` — [`L98`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L98)
- uses (calls/refs, reference-scoped): [`Model`](../../../ai/src/types.ts.md#Model), [`SessionManager`](../../src/core/session-manager.ts.md#SessionManager), [`SettingsManager`](../../src/core/settings-manager.ts.md#SettingsManager), [`AuthStorage`](../../src/core/auth-storage.ts.md#AuthStorage), [`AgentSession`](../../src/core/agent-session.ts.md#AgentSession), [`AgentSessionEvent`](../../src/core/agent-session.ts.md#AgentSessionEvent), [`FauxResponseStep`](../../../ai/src/providers/faux.ts.md#FauxResponseStep), [`FauxProviderRegistration`](../../../ai/src/providers/faux.ts.md#FauxProviderRegistration)
- used by: (105 test-only callers)

### `HarnessOptions`
- def: [`packages/coding-agent/test/suite/harness.ts:62`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L62)
- signature: `interface HarnessOptions`
- members:
  - `agentMessageController` — [`L73`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L73)
  - `agentObserveController` — [`L72`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L72)
  - `api` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L63)
  - `autoRefineReviewer` — [`L79`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L79)
  - `autonomous` — [`L78`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L78)
  - `extensionFactories` — [`L70`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L70)
  - `initialGoal` — [`L81`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L81)
  - `models` — [`L65`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L65)
  - `objective` — [`L81`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L81)
  - `persistSession` — [`L75`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L75)
  - `provider` — [`L64`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L64)
  - `resourceLoader` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L69)
  - `rlmDepth` — [`L76`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L76)
  - `rlmMaxDepth` — [`L77`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L77)
  - `serializedRefine` — [`L80`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L80)
  - `settings` — [`L66`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L66)
  - `subagentRuntimeHost` — [`L74`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L74)
  - `systemPrompt` — [`L67`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L67)
  - `tokenBudget` — [`L81`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L81)
  - `tools` — [`L68`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L68)
  - `withConfiguredAuth` — [`L71`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L71)
- uses (calls/refs, reference-scoped): [`AgentTool`](../../../agent/src/types.ts.md#AgentTool), [`AgentSessionMessageController`](../../src/core/agent-messages.ts.md#AgentSessionMessageController), [`ExtensionFactory`](../../src/core/extensions/types.ts.md#ExtensionFactory), [`Settings`](../../src/core/settings-manager.ts.md#Settings), [`SubagentRuntimeHost`](../../src/core/rlm-runtime.ts.md#SubagentRuntimeHost), [`ResourceLoader`](../../src/core/resource-loader.ts.md#ResourceLoader), [`AgentObserveController`](../../src/core/agent-observe.ts.md#AgentObserveController), [`AgentAutonomousConfig`](../../src/core/autonomous.ts.md#AgentAutonomousConfig), [`AutoRefineReviewer`](../../src/core/agent-session.ts.md#AutoRefineReviewer), [`FauxModelDefinition`](../../../ai/src/providers/faux.ts.md#FauxModelDefinition)  (2 test-only)
- used by: (1 test-only callers)

### `MessageTextPart`
- def: [`packages/coding-agent/test/suite/harness.ts:31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L31)
- signature: `type MessageTextPart`
- members:
  - `text` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L31)
  - `type` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L31)
- used by: (1 test-only callers)

## Functions
- `createHarness(options?: HarnessOptions)` — [`L108`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L108)
- `createTempDir()` — [`L102`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L102)
- `getAssistantTexts(harness: Harness)` — [`L56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L56)
- `getMessageText(message: unknown)` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L33)
- `getUserTexts(harness: Harness)` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/harness.ts#L50)


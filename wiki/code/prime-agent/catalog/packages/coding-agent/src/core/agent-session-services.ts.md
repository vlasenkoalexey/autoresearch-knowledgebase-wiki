---
title: 'Module: packages/coding-agent/src/core/agent-session-services.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/agent-session-services.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`agent-session-services.ts`/
symbols:
  createAgentSessionServices: createAgentSessionServices().
  createAgentSessionFromServices: createAgentSessionFromServices().
  CreateAgentSessionFromServicesOptions.services: CreateAgentSessionFromServicesOptions#services.
  AgentSessionServices.agentDir: AgentSessionServices#agentDir.
  applyExtensionFlagValues: applyExtensionFlagValues().
  CreateAgentSessionFromServicesOptions.sessionManager: CreateAgentSessionFromServicesOptions#sessionManager.
  AgentSessionRuntimeDiagnostic: AgentSessionRuntimeDiagnostic#
  CreateAgentSessionServicesOptions.cwd: CreateAgentSessionServicesOptions#cwd.
  AgentSessionServices: AgentSessionServices#
  CreateAgentSessionServicesOptions.resourceLoaderOptions: CreateAgentSessionServicesOptions#resourceLoaderOptions.
  AgentSessionServices.diagnostics: AgentSessionServices#diagnostics.
  AgentSessionRuntimeDiagnostic.type: AgentSessionRuntimeDiagnostic#type.
  AgentSessionServices.cwd: AgentSessionServices#cwd.
  AgentSessionCreationOptions.model: AgentSessionCreationOptions#model.
  CreateAgentSessionServicesOptions.agentDir: CreateAgentSessionServicesOptions#agentDir.
  AgentSessionCreationOptions.rlmDepth: AgentSessionCreationOptions#rlmDepth.
  CreateAgentSessionServicesOptions.authStorage: CreateAgentSessionServicesOptions#authStorage.
  AgentSessionServices.settingsManager: AgentSessionServices#settingsManager.
  CreateAgentSessionFromServicesOptions.sessionStartEvent: CreateAgentSessionFromServicesOptions#sessionStartEvent.
  AgentSessionCreationOptions.agentMessageController: AgentSessionCreationOptions#agentMessageController.
  AgentSessionServices.modelRegistry: AgentSessionServices#modelRegistry.
  AgentSessionCreationOptions: AgentSessionCreationOptions#
  AgentSessionCreationOptions.subagentRuntimeHost: AgentSessionCreationOptions#subagentRuntimeHost.
  CreateAgentSessionFromServicesOptions: CreateAgentSessionFromServicesOptions#
  AgentSessionRuntimeDiagnostic.message: AgentSessionRuntimeDiagnostic#message.
  CreateAgentSessionServicesOptions.settingsManager: CreateAgentSessionServicesOptions#settingsManager.
  AgentSessionCreationOptions.thinkingLevel: AgentSessionCreationOptions#thinkingLevel.
  AgentSessionCreationOptions.serviceTier: AgentSessionCreationOptions#serviceTier.
  AgentSessionCreationOptions.agentObserveController: AgentSessionCreationOptions#agentObserveController.
  AgentSessionCreationOptions.rlmHeartbeatController: AgentSessionCreationOptions#rlmHeartbeatController.
  AgentSessionCreationOptions.rlmSessionDir: AgentSessionCreationOptions#rlmSessionDir.
  AgentSessionCreationOptions.initialActiveToolNames: AgentSessionCreationOptions#initialActiveToolNames.
  AgentSessionCreationOptions.allowedToolNames: AgentSessionCreationOptions#allowedToolNames.
  AgentSessionCreationOptions.includeGoals: AgentSessionCreationOptions#includeGoals.
  AgentSessionCreationOptions.rlmMaxDepth: AgentSessionCreationOptions#rlmMaxDepth.
  AgentSessionCreationOptions.rlmParentNodeId: AgentSessionCreationOptions#rlmParentNodeId.
  CreateAgentSessionServicesOptions.modelRegistry: CreateAgentSessionServicesOptions#modelRegistry.
  AgentSessionCreationOptions.customTools: AgentSessionCreationOptions#customTools.
  AgentSessionServices.resourceLoader: AgentSessionServices#resourceLoader.
  AgentSessionCreationOptions.rlmParentAgent: AgentSessionCreationOptions#rlmParentAgent.
  AgentSessionCreationOptions.executionMode: AgentSessionCreationOptions#executionMode.
  AgentSessionServices.authStorage: AgentSessionServices#authStorage.
  CreateAgentSessionServicesOptions: CreateAgentSessionServicesOptions#
  AgentSessionCreationOptions.includeCompactSkill: AgentSessionCreationOptions#includeCompactSkill.
  AgentSessionCreationOptions.autonomous: AgentSessionCreationOptions#autonomous.
  AgentSessionServices.mcpManager: AgentSessionServices#mcpManager.
  CreateAgentSessionServicesOptions.noBuiltinHerdrReporter: CreateAgentSessionServicesOptions#noBuiltinHerdrReporter.
  CreateAgentSessionServicesOptions.telemetryDisabled: CreateAgentSessionServicesOptions#telemetryDisabled.
  AgentSessionCreationOptions.scopedModels: AgentSessionCreationOptions#scopedModels.
  AgentSessionCreationOptions.prewarmIpythonKernel: AgentSessionCreationOptions#prewarmIpythonKernel.
  AgentSessionCreationOptions.serializedRefine: AgentSessionCreationOptions#serializedRefine.
  AgentSessionCreationOptions.telemetryDisabled: AgentSessionCreationOptions#telemetryDisabled.
  AgentSessionCreationOptions.initialGoal: AgentSessionCreationOptions#initialGoal.
  AgentSessionCreationOptions.scopedModels.Array.typeLiteral0.model: AgentSessionCreationOptions#scopedModels.Array:typeLiteral0:model.
  AgentSessionCreationOptions.scopedModels.Array.typeLiteral0.thinkingLevel: AgentSessionCreationOptions#scopedModels.Array:typeLiteral0:thinkingLevel.
  CreateAgentSessionServicesOptions.extensionFlagValues: CreateAgentSessionServicesOptions#extensionFlagValues.
  AgentSessionCreationOptions.noTools: AgentSessionCreationOptions#noTools.
  AgentSessionCreationOptions.tools: AgentSessionCreationOptions#tools.
  AgentSessionCreationOptions.initialGoal.typeLiteral1.objective: AgentSessionCreationOptions#initialGoal.typeLiteral1:objective.
  AgentSessionCreationOptions.initialGoal.typeLiteral1.tokenBudget: AgentSessionCreationOptions#initialGoal.typeLiteral1:tokenBudget.
---
# Module: [`packages/coding-agent/src/core/agent-session-services.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts)

## Classes
### `AgentSessionCreationOptions`
- def: [`packages/coding-agent/src/core/agent-session-services.ts:61`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L61)
- signature: `interface AgentSessionCreationOptions`
- members:
  - `agentMessageController` — [`L74`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L74)
  - `agentObserveController` — [`L75`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L75)
  - `allowedToolNames` — [`L71`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L71)
  - `autonomous` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L84)
  - `customTools` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L69)
  - `executionMode` — [`L88`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L88) — User-facing client mode that created the top-level session.
  - `includeCompactSkill` — [`L73`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L73)
  - `includeGoals` — [`L72`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L72)
  - `initialActiveToolNames` — [`L70`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L70)
  - `initialGoal` — [`L92`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L92) — Initial goal to seed at session creation (rlmDepth 0 only, idempotent).
  - `model` — [`L62`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L62)
  - `model` — [`L66`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L66)
  - `noTools` — [`L68`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L68)
  - `objective` — [`L92`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L92)
  - `prewarmIpythonKernel` — [`L83`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L83)
  - `rlmDepth` — [`L76`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L76)
  - `rlmHeartbeatController` — [`L82`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L82)
  - `rlmMaxDepth` — [`L77`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L77)
  - `rlmParentAgent` — [`L80`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L80)
  - `rlmParentNodeId` — [`L79`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L79)
  - `rlmSessionDir` — [`L78`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L78)
  - `scopedModels` — [`L66`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L66)
  - `serializedRefine` — [`L86`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L86) — Serialized refine mode for print/headless autonomous runs.
  - `serviceTier` — [`L65`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L65) — Provider service tier. Fast mode uses "priority".
  - `subagentRuntimeHost` — [`L81`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L81)
  - `telemetryDisabled` — [`L90`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L90) — Explicit daemon-carried opt-out; cannot enable telemetry.
  - `thinkingLevel` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L63)
  - `thinkingLevel` — [`L66`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L66)
  - `tokenBudget` — [`L92`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L92)
  - `tools` — [`L67`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L67)
- uses (calls/refs, reference-scoped): [`Model`](../../../ai/src/types.ts.md#Model), [`ThinkingLevel`](../../../agent/src/types.ts.md#ThinkingLevel), [`ToolDefinition`](extensions/types.ts.md#ToolDefinition), [`ServiceTier`](../../../ai/src/types.ts.md#ServiceTier), [`AgentSessionMessageController`](agent-messages.ts.md#AgentSessionMessageController), [`SubagentRuntimeHost`](rlm-runtime.ts.md#SubagentRuntimeHost), [`AgentObserveController`](agent-observe.ts.md#AgentObserveController), [`AgentAutonomousConfig`](autonomous.ts.md#AgentAutonomousConfig), [`AgentExecutionMode`](agent-session-config.ts.md#AgentExecutionMode), [`AgentRlmHeartbeatController`](cron-jobs.ts.md#AgentRlmHeartbeatController)  (1 test-only)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`main`](../main.ts.md#main), [`createAgentSession`](sdk.ts.md#createAgentSession), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`createAgentSessionFromServices`](agent-session-services.ts.md#createAgentSessionFromServices), [`sdk.ts`](sdk.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-sdk.ts), [`sessionOptionsOverride`](../main.ts.md#prepareRuntimeServices.options-typeLiteral166.sessionOptionsOverride), [`agent-session-runtime.ts`](agent-session-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-runtime.ts), [`CreateAgentSessionRuntimeFactory`](agent-session-runtime.ts.md#CreateAgentSessionRuntimeFactory), [`modelFallbackMessage`](sdk.ts.md#CreateAgentSessionResult.modelFallbackMessage), [`resolveRuntimeSessionOptions`](../main.ts.md#resolveRuntimeSessionOptions), [`CreateAgentSessionOptions`](sdk.ts.md#CreateAgentSessionOptions), [`CreateAgentSessionFromServicesOptions`](agent-session-services.ts.md#CreateAgentSessionFromServicesOptions), [`sessionOptions`](agent-session-runtime.ts.md#createAgentSessionRuntime.options-typeLiteral97.sessionOptions)  (10 test-only)

### `AgentSessionRuntimeDiagnostic`
- def: [`packages/coding-agent/src/core/agent-session-services.ts:30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L30)
- doc: Non-fatal issues collected while creating services or sessions.
- signature: `interface AgentSessionRuntimeDiagnostic`
- members:
  - `message` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L32)
  - `type` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L31)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`main`](../main.ts.md#main), [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`createAgentSessionServices`](agent-session-services.ts.md#createAgentSessionServices), [`sessionOptionsOverride`](../main.ts.md#prepareRuntimeServices.options-typeLiteral166.sessionOptionsOverride), [`agent-session-runtime.ts`](agent-session-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-runtime.ts), [`daemon-session-list.ts`](../modes/daemon/daemon-session-list.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-session-list.ts), [`diagnostics`](../main.ts.md#buildSessionOptions.typeLiteral122.diagnostics), [`<constructor>`](agent-session-runtime.ts.md#AgentSessionRuntime.-constructor), [`applyExtensionFlagValues`](agent-session-services.ts.md#applyExtensionFlagValues), [`collectSettingsDiagnostics`](../main.ts.md#collectSettingsDiagnostics), [`diagnostics`](agent-session-services.ts.md#AgentSessionServices.diagnostics), [`reportDiagnostics`](../main.ts.md#reportDiagnostics), [`CreateAgentSessionRuntimeResult`](agent-session-runtime.ts.md#CreateAgentSessionRuntimeResult), [`<get>diagnostics`](agent-session-runtime.ts.md#AgentSessionRuntime.-get-diagnostics), [`diagnostics`](../main.ts.md#PreparedRuntimeServices.diagnostics), [`diagnostics`](../modes/daemon/daemon-session-list.ts.md#SessionSummary.diagnostics)

### `AgentSessionServices`
- def: [`packages/coding-agent/src/core/agent-session-services.ts:113`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L113)
- doc: Coherent cwd-bound runtime services for one effective session cwd.
- signature: `interface AgentSessionServices`
- members:
  - `agentDir` — [`L115`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L115)
  - `authStorage` — [`L116`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L116)
  - `cwd` — [`L114`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L114)
  - `diagnostics` — [`L121`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L121)
  - `mcpManager` — [`L120`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L120)
  - `modelRegistry` — [`L118`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L118)
  - `resourceLoader` — [`L119`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L119)
  - `settingsManager` — [`L117`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L117)
- uses (calls/refs, reference-scoped): [`SettingsManager`](settings-manager.ts.md#SettingsManager), [`AuthStorage`](auth-storage.ts.md#AuthStorage), [`ModelRegistry`](model-registry.ts.md#ModelRegistry), [`ResourceLoader`](resource-loader.ts.md#ResourceLoader), [`AgentSessionRuntimeDiagnostic`](agent-session-services.ts.md#AgentSessionRuntimeDiagnostic), [`McpManager`](mcp/mcp-manager.ts.md#McpManager)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`main`](../main.ts.md#main), [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`createRlmSubagentRuntime`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRlmSubagentRuntime), [`rehydrateCompletedRlmSubagentOnce`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.rehydrateCompletedRlmSubagentOnce), [`createAgentSessionServices`](agent-session-services.ts.md#createAgentSessionServices), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`createAgentSessionFromServices`](agent-session-services.ts.md#createAgentSessionFromServices), [`sessionOptionsOverride`](../main.ts.md#prepareRuntimeServices.options-typeLiteral166.sessionOptionsOverride), [`agent-session-runtime.ts`](agent-session-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-runtime.ts), [`createRlmSubagentRuntime`](agent-session-runtime.ts.md#AgentSessionRuntime.createRlmSubagentRuntime), [`cancelled`](agent-session-runtime.ts.md#AgentSessionRuntime.newSession.Promise.typeLiteral136.cancelled), [`modelFallbackMessage`](../main.ts.md#resolvePreparedStartupModel.Promise.typeLiteral217.modelFallbackMessage), [`importFromJsonl`](agent-session-runtime.ts.md#AgentSessionRuntime.importFromJsonl), [`interactive-mode-services.ts`](../modes/interactive/interactive-mode-services.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode-services.ts), [`cancelled`](agent-session-runtime.ts.md#AgentSessionRuntime.switchSession.Promise.typeLiteral115.cancelled), [`createInteractiveModeUiServicesFromServices`](../modes/interactive/interactive-mode-services.ts.md#createInteractiveModeUiServicesFromServices), [`services`](agent-session-services.ts.md#CreateAgentSessionFromServicesOptions.services), [`<constructor>`](agent-session-runtime.ts.md#AgentSessionRuntime.-constructor), [`acquireReplacementLease`](agent-session-runtime.ts.md#AgentSessionRuntime.acquireReplacementLease), [`<get>services`](agent-session-runtime.ts.md#AgentSessionRuntime.-get-services), [`<get>cwd`](agent-session-runtime.ts.md#AgentSessionRuntime.-get-cwd), [`services`](agent-session-runtime.ts.md#CreateAgentSessionRuntimeResult.services), [`services`](../main.ts.md#PreparedRuntimeServices.services), [`services`](../modes/interactive/interactive-mode-services.ts.md#createInteractiveModeUiServicesFromServices.options-typeLiteral6.services)  (12 test-only)

### `CreateAgentSessionFromServicesOptions`
- def: [`packages/coding-agent/src/core/agent-session-services.ts:101`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L101)
- doc: Inputs for creating an AgentSession from already-created services.
- signature: `interface CreateAgentSessionFromServicesOptions`
- members:
  - `services` — [`L102`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L102)
  - `sessionManager` — [`L103`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L103)
  - `sessionStartEvent` — [`L104`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L104)
- uses (calls/refs, reference-scoped): [`SessionManager`](session-manager.ts.md#SessionManager), [`AgentSessionServices`](agent-session-services.ts.md#AgentSessionServices), [`SessionStartEvent`](extensions/types.ts.md#SessionStartEvent), [`AgentSessionCreationOptions`](agent-session-services.ts.md#AgentSessionCreationOptions)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`main`](../main.ts.md#main), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`createAgentSessionFromServices`](agent-session-services.ts.md#createAgentSessionFromServices), [`agent-session-runtime.ts`](agent-session-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-runtime.ts)  (9 test-only)

### `CreateAgentSessionServicesOptions`
- def: [`packages/coding-agent/src/core/agent-session-services.ts:42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L42)
- doc: Inputs for creating cwd-bound runtime services.
- signature: `interface CreateAgentSessionServicesOptions`
- members:
  - `agentDir` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L44)
  - `authStorage` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L45)
  - `cwd` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L43)
  - `extensionFlagValues` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L48)
  - `modelRegistry` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L47)
  - `noBuiltinHerdrReporter` — [`L56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L56) — Skip the built-in Herdr reporter for these services. Set for RLM subagent
  - `resourceLoaderOptions` — [`L49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L49)
  - `settingsManager` — [`L46`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L46)
  - `telemetryDisabled` — [`L58`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L58) — Explicit daemon-carried opt-out; cannot enable telemetry.
- uses (calls/refs, reference-scoped): [`SettingsManager`](settings-manager.ts.md#SettingsManager), [`AuthStorage`](auth-storage.ts.md#AuthStorage), [`ModelRegistry`](model-registry.ts.md#ModelRegistry), [`DefaultResourceLoaderOptions`](resource-loader.ts.md#DefaultResourceLoaderOptions)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`createAgentSessionServices`](agent-session-services.ts.md#createAgentSessionServices), [`sessionOptionsOverride`](../main.ts.md#prepareRuntimeServices.options-typeLiteral166.sessionOptionsOverride), [`agent-session-runtime.ts`](agent-session-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-runtime.ts)  (9 test-only)

## Functions
- `applyExtensionFlagValues(resourceLoader: ResourceLoader, extensionFlagValues: Map<string, string | boolean> | undefined)` — [`L124`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L124)
- `createAgentSessionFromServices(options: CreateAgentSessionFromServicesOptions)` — [`L264`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L264) — Create an AgentSession from previously created services.
- `createAgentSessionServices(options: CreateAgentSessionServicesOptions)` — [`L177`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-services.ts#L177) — Create cwd-bound runtime services.


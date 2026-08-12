---
title: 'Module: packages/coding-agent/src/core/agent-session-config.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/agent-session-config.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`agent-session-config.ts`/
symbols:
  AgentSessionRuntimeConfig.cwd: AgentSessionRuntimeConfig#cwd.
  AgentSessionRuntimeConfig.agentDir: AgentSessionRuntimeConfig#agentDir.
  mergeAgentSessionRuntimeConfig: mergeAgentSessionRuntimeConfig().
  AgentSessionRuntimeConfig: AgentSessionRuntimeConfig#
  AgentSessionRuntimeConfig.sessionDir: AgentSessionRuntimeConfig#sessionDir.
  cloneAgentSessionRuntimeConfig: cloneAgentSessionRuntimeConfig().
  AgentSessionRuntimeConfig.initialGoal: AgentSessionRuntimeConfig#initialGoal.
  AgentSessionRuntimeConfig.extensionFlagValues: AgentSessionRuntimeConfig#extensionFlagValues.
  AgentSessionRuntimeConfig.telemetryDisabled: AgentSessionRuntimeConfig#telemetryDisabled.
  AgentSessionRuntimeConfig.serializedRefine: AgentSessionRuntimeConfig#serializedRefine.
  AgentSessionRuntimeConfig.autonomous: AgentSessionRuntimeConfig#autonomous.
  AgentSessionRuntimeConfig.tools: AgentSessionRuntimeConfig#tools.
  cloneArray: cloneArray().
  AgentSessionRuntimeConfig.thinking: AgentSessionRuntimeConfig#thinking.
  AgentSessionRuntimeConfig.executionMode: AgentSessionRuntimeConfig#executionMode.
  mergeAutonomousConfig: mergeAutonomousConfig().
  AgentSessionRuntimeConfig.model: AgentSessionRuntimeConfig#model.
  AgentSessionRuntimeConfig.extensions: AgentSessionRuntimeConfig#extensions.
  AgentSessionRuntimeConfig.models: AgentSessionRuntimeConfig#models.
  mergeAutonomousGateConfig: mergeAutonomousGateConfig().
  AgentSessionRuntimeConfig.appendSystemPrompt: AgentSessionRuntimeConfig#appendSystemPrompt.
  AgentSessionRuntimeConfig.skills: AgentSessionRuntimeConfig#skills.
  AgentSessionRuntimeConfig.promptTemplates: AgentSessionRuntimeConfig#promptTemplates.
  AgentSessionRuntimeConfig.themes: AgentSessionRuntimeConfig#themes.
  AgentSessionRuntimeConfig.noTools: AgentSessionRuntimeConfig#noTools.
  AgentExecutionMode: AgentExecutionMode#
  AgentSessionRuntimeConfig.apiKey: AgentSessionRuntimeConfig#apiKey.
  AgentSessionRuntimeConfig.noExtensions: AgentSessionRuntimeConfig#noExtensions.
  AgentSessionRuntimeConfig.noSkills: AgentSessionRuntimeConfig#noSkills.
  AgentSessionRuntimeConfig.noContextFiles: AgentSessionRuntimeConfig#noContextFiles.
  AgentSessionRuntimeConfig.provider: AgentSessionRuntimeConfig#provider.
  AgentSessionRuntimeConfig.systemPrompt: AgentSessionRuntimeConfig#systemPrompt.
  AgentSessionRuntimeConfig.noBuiltinTools: AgentSessionRuntimeConfig#noBuiltinTools.
  AgentSessionRuntimeConfig.noPromptTemplates: AgentSessionRuntimeConfig#noPromptTemplates.
  AgentSessionRuntimeConfig.noThemes: AgentSessionRuntimeConfig#noThemes.
  AgentSessionRuntimeConfig.initialGoal.typeLiteral0.objective: AgentSessionRuntimeConfig#initialGoal.typeLiteral0:objective.
  AgentSessionRuntimeConfig.initialGoal.typeLiteral0.tokenBudget: AgentSessionRuntimeConfig#initialGoal.typeLiteral0:tokenBudget.
---
# Module: [`packages/coding-agent/src/core/agent-session-config.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts)

## Classes
### `AgentExecutionMode`
- def: [`packages/coding-agent/src/core/agent-session-config.ts:4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L4)
- signature: `type AgentExecutionMode`
- used by: [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`agent-session-services.ts`](agent-session-services.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-services.ts), [`telemetry.ts`](telemetry.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-telemetry.ts), [`executionMode`](agent-session-config.ts.md#AgentSessionRuntimeConfig.executionMode), [`executionMode`](telemetry.ts.md#InstallAgentTelemetryOptions.executionMode), [`executionMode`](agent-session-services.ts.md#AgentSessionCreationOptions.executionMode), [`ClientMode`](../main.ts.md#ClientMode), [`TelemetryExecutionMode`](telemetry.ts.md#TelemetryExecutionMode)

### `AgentSessionRuntimeConfig`
- def: [`packages/coding-agent/src/core/agent-session-config.ts:6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L6)
- signature: `interface AgentSessionRuntimeConfig`
- members:
  - `agentDir` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L8)
  - `apiKey` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L12)
  - `appendSystemPrompt` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L14)
  - `autonomous` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L29)
  - `cwd` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L7)
  - `executionMode` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L39) — User-facing client mode that created this session. The daemon is transport, not an execution mode.
  - `extensionFlagValues` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L30)
  - `extensions` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L20)
  - `initialGoal` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L47) — Initial goal to seed when creating a new top-level session (rlmDepth 0).
  - `model` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L11)
  - `models` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L16)
  - `noBuiltinTools` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L19)
  - `noContextFiles` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L28)
  - `noExtensions` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L21)
  - `noPromptTemplates` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L25)
  - `noSkills` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L23)
  - `noThemes` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L27)
  - `noTools` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L18)
  - `objective` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L47)
  - `promptTemplates` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L24)
  - `provider` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L10)
  - `serializedRefine` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L37) — When true, auto-refine runs synchronously between turns at the
  - `sessionDir` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L9)
  - `skills` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L22)
  - `systemPrompt` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L13)
  - `telemetryDisabled` — [`L41`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L41) — Opt-out-only policy carried across daemon process boundaries.
  - `themes` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L26)
  - `thinking` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L15)
  - `tokenBudget` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L47)
  - `tools` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L17)
- uses (calls/refs, reference-scoped): [`ThinkingLevel`](../../../agent/src/types.ts.md#ThinkingLevel), [`AgentAutonomousConfig`](autonomous.ts.md#AgentAutonomousConfig), [`AgentExecutionMode`](agent-session-config.ts.md#AgentExecutionMode)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`main`](../main.ts.md#main), [`handleCommand`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.handleCommand), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`daemon-supervisor.ts`](../modes/daemon/daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`handleCommand`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.handleCommand), [`agents-view-mode.ts`](../modes/agents-view/agents-view-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agents-view-agents-view-mode.ts), [`DaemonCommand`](../modes/daemon/daemon-protocol.ts.md#DaemonCommand), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`<constructor>`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.-constructor), [`launchWorker`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.launchWorker), [`daemon-protocol.ts`](../modes/daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`createRuntime`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRuntime), [`defaultSessionConfig`](../modes/daemon/daemon-mode.ts.md#DaemonModeOptions.defaultSessionConfig), [`sessionOptionsOverride`](../main.ts.md#prepareRuntimeServices.options-typeLiteral166.sessionOptionsOverride), [`runtimeConfigFromArgs`](../main.ts.md#runtimeConfigFromArgs), [`agent-session-runtime.ts`](agent-session-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-runtime.ts), [`start`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.start), [`shutdown`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.shutdown), [`createAgentFamilyCatalog`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentFamilyCatalog), [`mergeAgentSessionRuntimeConfig`](agent-session-config.ts.md#mergeAgentSessionRuntimeConfig), [`CreateAgentSessionRuntimeFactory`](agent-session-runtime.ts.md#CreateAgentSessionRuntimeFactory), [`parseSessionOption`](../cli/daemon-command.ts.md#parseSessionOption), [`diagnostics`](../main.ts.md#buildSessionOptions.typeLiteral122.diagnostics), [`<constructor>`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.-constructor), [`daemon-command.ts`](../cli/daemon-command.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-daemon-command.ts), [`modelFallbackMessage`](sdk.ts.md#CreateAgentSessionResult.modelFallbackMessage), [`createOrReuseWorker`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.createOrReuseWorker), [`summary`](../main.ts.md#createDaemonClientConnection.Promise.typeLiteral503.summary), [`createUpdateRestartSession`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createUpdateRestartSession), [`deactivatePendingAgent`](../modes/agents-view/agents-view-mode.ts.md#AgentsViewMode.deactivatePendingAgent), [`launchReplacementSupervisor`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.launchReplacementSupervisor), [`parseSessionArgs`](../cli/daemon-command.ts.md#parseSessionArgs), [`openAgentsViewSession`](../modes/agents-view/agents-view-mode.ts.md#openAgentsViewSession), [`type`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.handleList.command-Extract.typeLiteral1418.type), [`cloneAgentSessionRuntimeConfig`](agent-session-config.ts.md#cloneAgentSessionRuntimeConfig), [`defaultSessionConfig`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisorOptions.defaultSessionConfig), [`type`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.handleSavedSessionList.command-Extract.typeLiteral1475.type), [`sendPrompt`](../modes/agents-view/agents-view-mode.ts.md#AgentsViewMode.sendPrompt)  (+24 more; 25 test-only)

## Functions
- `cloneAgentSessionRuntimeConfig(config: AgentSessionRuntimeConfig)` — [`L92`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L92)
- `cloneArray(value: T[] | undefined)` — [`L142`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L142)
- `mergeAgentSessionRuntimeConfig(base: AgentSessionRuntimeConfig, override?: AgentSessionRuntimeConfig | undefined)` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L50)
- `mergeAutonomousConfig(base: AgentAutonomousConfig | undefined, override: AgentAutonomousConfig | undefined)` — [`L111`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L111)
- `mergeAutonomousGateConfig(base: AgentAutonomousGateConfig | undefined, override: AgentAutonomousGateConfig | undefined)` — [`L126`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session-config.ts#L126)


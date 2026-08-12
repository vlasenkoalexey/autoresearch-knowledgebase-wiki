---
title: 'Module: packages/coding-agent/src/core/sdk.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/sdk.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`sdk.ts`/
symbols:
  createAgentSession: createAgentSession().
  CreateAgentSessionResult.modelFallbackMessage: CreateAgentSessionResult#modelFallbackMessage.
  CreateAgentSessionResult.session: CreateAgentSessionResult#session.
  CreateAgentSessionOptions: CreateAgentSessionOptions#
  CreateAgentSessionOptions.model: CreateAgentSessionOptions#model.
  CreateAgentSessionResult.extensionsResult: CreateAgentSessionResult#extensionsResult.
  CreateAgentSessionOptions.autonomous: CreateAgentSessionOptions#autonomous.
  CreateAgentSessionOptions.thinkingLevel: CreateAgentSessionOptions#thinkingLevel.
  CreateAgentSessionOptions.tools: CreateAgentSessionOptions#tools.
  CreateAgentSessionOptions.noTools: CreateAgentSessionOptions#noTools.
  CreateAgentSessionOptions.customTools: CreateAgentSessionOptions#customTools.
  CreateAgentSessionResult: CreateAgentSessionResult#
  CreateAgentSessionOptions.scopedModels: CreateAgentSessionOptions#scopedModels.
  CreateAgentSessionOptions.sessionManager: CreateAgentSessionOptions#sessionManager.
  CreateAgentSessionOptions.agentDir: CreateAgentSessionOptions#agentDir.
  CreateAgentSessionOptions.authStorage: CreateAgentSessionOptions#authStorage.
  CreateAgentSessionOptions.modelRegistry: CreateAgentSessionOptions#modelRegistry.
  CreateAgentSessionOptions.resourceLoader: CreateAgentSessionOptions#resourceLoader.
  CreateAgentSessionOptions.mcpManager: CreateAgentSessionOptions#mcpManager.
  CreateAgentSessionOptions.settingsManager: CreateAgentSessionOptions#settingsManager.
  CreateAgentSessionOptions.sessionStartEvent: CreateAgentSessionOptions#sessionStartEvent.
  getDefaultAgentDir: getDefaultAgentDir().
  CreateAgentSessionOptions.scopedModels.Array.typeLiteral0.model: CreateAgentSessionOptions#scopedModels.Array:typeLiteral0:model.
  CreateAgentSessionOptions.scopedModels.Array.typeLiteral0.thinkingLevel: CreateAgentSessionOptions#scopedModels.Array:typeLiteral0:thinkingLevel.
  CreateAgentSessionOptions.cwd: CreateAgentSessionOptions#cwd.
---
# Module: [`packages/coding-agent/src/core/sdk.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts)

## Classes
### `CreateAgentSessionOptions`
- def: [`packages/coding-agent/src/core/sdk.ts:23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L23)
- signature: `interface CreateAgentSessionOptions`
- members:
  - `agentDir` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L27) — Global config directory. Default: ~/.pi/agent
  - `authStorage` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L30) — Auth storage for credentials. Default: AuthStorage.create(agentDir/auth.json)
  - `autonomous` — [`L74`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L74) — Host-side autonomous continuation policy.
  - `customTools` — [`L58`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L58) — Custom tools to register (in addition to built-in tools).
  - `cwd` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L25) — Working directory for project-local discovery. Default: process.cwd()
  - `mcpManager` — [`L64`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L64) — MCP integration manager. When omitted, MCP host handlers are not wired.
  - `model` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L35) — Model to use. Default: from settings, else first available
  - `model` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L39)
  - `modelRegistry` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L32) — Model registry. Default: ModelRegistry.create(authStorage, agentDir/models.json)
  - `noTools` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L48) — Optional default tool suppression mode when no explicit allowlist is provided.
  - `resourceLoader` — [`L61`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L61) — Resource loader. When omitted, DefaultResourceLoader is used.
  - `scopedModels` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L39) — Models available for cycling (Ctrl+P in interactive mode)
  - `sessionManager` — [`L67`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L67) — Session manager. Default: SessionManager.create(cwd)
  - `sessionStartEvent` — [`L72`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L72) — Session start event metadata for extension runtime startup.
  - `settingsManager` — [`L70`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L70) — Settings manager. Default: SettingsManager.create(cwd, agentDir)
  - `thinkingLevel` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L37) — Thinking level. Default: from settings, else 'medium' (clamped to model capabilities)
  - `thinkingLevel` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L39)
  - `tools` — [`L56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L56) — Optional allowlist of tool names.
- uses (calls/refs, reference-scoped): [`Model`](../../../ai/src/types.ts.md#Model), [`SessionManager`](session-manager.ts.md#SessionManager), [`SettingsManager`](settings-manager.ts.md#SettingsManager), [`AuthStorage`](auth-storage.ts.md#AuthStorage), [`ModelRegistry`](model-registry.ts.md#ModelRegistry), [`ThinkingLevel`](../../../agent/src/types.ts.md#ThinkingLevel), [`ToolDefinition`](extensions/types.ts.md#ToolDefinition), [`ResourceLoader`](resource-loader.ts.md#ResourceLoader), [`AgentAutonomousConfig`](autonomous.ts.md#AgentAutonomousConfig), [`SessionStartEvent`](extensions/types.ts.md#SessionStartEvent), [`AgentSessionCreationOptions`](agent-session-services.ts.md#AgentSessionCreationOptions), [`McpManager`](mcp/mcp-manager.ts.md#McpManager)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`createAgentSession`](sdk.ts.md#createAgentSession), [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`sessionOptionsOverride`](../main.ts.md#prepareRuntimeServices.options-typeLiteral166.sessionOptionsOverride), [`diagnostics`](../main.ts.md#buildSessionOptions.typeLiteral122.diagnostics), [`modelFallbackMessage`](../main.ts.md#resolvePreparedStartupModel.Promise.typeLiteral217.modelFallbackMessage), [`resolveRuntimeSessionOptions`](../main.ts.md#resolveRuntimeSessionOptions), [`options`](../main.ts.md#buildSessionOptions.typeLiteral122.options), [`sessionOptions`](../main.ts.md#PreparedRuntimeServices.sessionOptions)  (1 test-only)

### `CreateAgentSessionResult`
- def: [`packages/coding-agent/src/core/sdk.ts:78`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L78)
- doc: Result from createAgentSession
- signature: `interface CreateAgentSessionResult`
- members:
  - `extensionsResult` — [`L82`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L82) — Extensions result (for UI context setup in interactive mode)
  - `modelFallbackMessage` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L84) — Warning if session was restored with a different model than saved
  - `session` — [`L80`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L80) — The created session
- uses (calls/refs, reference-scoped): [`index.ts`](extensions/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-index.ts), [`ExtensionAPI`](extensions/types.ts.md#ExtensionAPI), [`agent-session-runtime.ts`](agent-session-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-runtime.ts), [`agent-session-services.ts`](agent-session-services.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-services.ts), [`AgentSession`](agent-session.ts.md#AgentSession), [`index.ts`](tools/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`ToolDefinition`](extensions/types.ts.md#ToolDefinition), [`ExtensionContext`](extensions/types.ts.md#ExtensionContext), [`AgentSessionRuntimeConfig`](agent-session-config.ts.md#AgentSessionRuntimeConfig), [`skills.ts`](skills.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-skills.ts), [`Skill`](skills.ts.md#Skill), [`createBashTool`](tools/bash.ts.md#createBashTool), [`rlm-runtime.ts`](rlm-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-rlm-runtime.ts), [`ExtensionCommandContext`](extensions/types.ts.md#ExtensionCommandContext), [`ExtensionFactory`](extensions/types.ts.md#ExtensionFactory), [`SubagentRuntimeHost`](rlm-runtime.ts.md#SubagentRuntimeHost), [`prompt-templates.ts`](prompt-templates.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-prompt-templates.ts), [`agent-session-config.ts`](agent-session-config.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-config.ts), [`createEditTool`](tools/edit.ts.md#createEditTool), [`PromptTemplate`](prompt-templates.ts.md#PromptTemplate), [`CreateRlmSubagentRuntimeOptions`](rlm-runtime.ts.md#CreateRlmSubagentRuntimeOptions), [`withFileMutationQueue`](tools/file-mutation-queue.ts.md#withFileMutationQueue), [`LoadExtensionsResult`](extensions/types.ts.md#LoadExtensionsResult), [`createIpythonTool`](tools/ipython.ts.md#createIpythonTool), [`RlmSubagentRuntime`](rlm-runtime.ts.md#RlmSubagentRuntime), [`SlashCommandInfo`](slash-commands.ts.md#SlashCommandInfo), [`AgentSessionCreationOptions`](agent-session-services.ts.md#AgentSessionCreationOptions), [`Tool`](tools/index.ts.md#Tool), [`SlashCommandSource`](slash-commands.ts.md#SlashCommandSource)  (2 test-only)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`main`](../main.ts.md#main), [`createAgentSession`](sdk.ts.md#createAgentSession), [`createAgentSessionFromServices`](agent-session-services.ts.md#createAgentSessionFromServices), [`agent-session-runtime.ts`](agent-session-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-runtime.ts), [`agent-session-services.ts`](agent-session-services.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-services.ts), [`createAgentSessionRuntime`](agent-session-runtime.ts.md#createAgentSessionRuntime), [`apply`](agent-session-runtime.ts.md#AgentSessionRuntime.apply), [`CreateAgentSessionRuntimeResult`](agent-session-runtime.ts.md#CreateAgentSessionRuntimeResult)  (22 test-only)

## Functions
- `createAgentSession(options?: CreateAgentSessionOptions)` — [`L155`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L155) — Create an AgentSession with the specified options.
- `getDefaultAgentDir()` — [`L116`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/sdk.ts#L116)


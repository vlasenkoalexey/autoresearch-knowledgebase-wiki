---
title: 'Module: packages/coding-agent/src/core/mcp/mcp-manager.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/mcp/mcp-manager.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/mcp/`mcp-manager.ts`/
symbols:
  McpManager.resolveIntegrations: McpManager#resolveIntegrations().
  McpManager.registerUserProviders: McpManager#registerUserProviders().
  McpManager.-constructor: McpManager#`<constructor>`().
  McpManager.isAuthed: McpManager#isAuthed().
  McpManager.hostHandlers: McpManager#hostHandlers().
  McpManagerOptions.authStorage: McpManagerOptions#authStorage.
  McpManager.listStatus: McpManager#listStatus().
  McpManager.getDisabledBuiltinSkillOverrides: McpManager#getDisabledBuiltinSkillOverrides().
  McpManagerOptions.getUserServers: McpManagerOptions#getUserServers.
  ResolvedIntegration.server: ResolvedIntegration#server.
  McpManager: McpManager#
  McpManager.refresh: McpManager#refresh().
  McpManager.integrations: McpManager#integrations.
  McpManager.registerProviders: McpManager#registerProviders().
  McpManager.authStorage: McpManager#authStorage.
  McpManager.listStatus.Array.typeLiteral90.server: McpManager#listStatus().Array:typeLiteral90:server.
  McpManager.getUserServers: McpManager#getUserServers.
  ResolvedIntegration.label: ResolvedIntegration#label.
  ResolvedIntegration.url: ResolvedIntegration#url.
  ResolvedIntegration.usesOAuth: ResolvedIntegration#usesOAuth.
  ResolvedIntegration.headers: ResolvedIntegration#headers.
  ResolvedIntegration: ResolvedIntegration#
  ResolvedIntegration.bearerTokenEnvVar: ResolvedIntegration#bearerTokenEnvVar.
  ResolvedIntegration.userDeclared: ResolvedIntegration#userDeclared.
  McpManager.providerId: McpManager#providerId().
  McpManager.listStatus.Array.typeLiteral90.enabled: McpManager#listStatus().Array:typeLiteral90:enabled.
  McpManagerOptions.beginLogin: McpManagerOptions#beginLogin.
  ResolvedIntegration.enabled: ResolvedIntegration#enabled.
  McpManager.beginLogin: McpManager#beginLogin.
  McpManager.registeredUserProviderIds: McpManager#registeredUserProviderIds.
  McpManagerOptions: McpManagerOptions#
  McpManager.listStatus.Array.typeLiteral90.label: McpManager#listStatus().Array:typeLiteral90:label.
  McpManager.listStatus.Array.typeLiteral90.usesOAuth: McpManager#listStatus().Array:typeLiteral90:usesOAuth.
---
# Module: [`packages/coding-agent/src/core/mcp/mcp-manager.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts)

## Classes
### `McpManager`
- def: [`packages/coding-agent/src/core/mcp/mcp-manager.ts:36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L36)
- signature: `class McpManager`
- members:
  - `<constructor>(options: McpManagerOptions)` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L44)
  - `getDisabledBuiltinSkillOverrides(method)` — [`L144`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L144) — `-<server>/SKILL.md` overrides for every built-in integration the user isn't logged into.
  - `hostHandlers(method)` — [`L156`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L156) — Host-request handlers exposed to the kernel.
  - `isAuthed(method)` — [`L127`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L127) — True when valid credentials exist for the integration (drives enablement).
  - `listStatus(method)` — [`L197`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L197) — Status for the /mcp list command.
  - `providerId(method)` — [`L58`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L58)
  - `refresh(method)` — [`L53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L53) — Re-read settings and re-register providers; call after a session reload.
  - `registerProviders(method)` — [`L88`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L88)
  - `registerUserProviders(method)` — [`L98`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L98) — Register OAuth providers for user-declared (non-catalog) servers. Public so it
  - `resolveIntegrations(method)` — [`L62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L62)
  - `authStorage` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L37)
  - `beginLogin` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L39)
  - `enabled` — [`L197`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L197)
  - `getUserServers` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L38)
  - `integrations` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L40)
  - `label` — [`L197`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L197)
  - `registeredUserProviderIds` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L42) — Provider ids we registered for user servers, so refresh can drop removed ones.
  - `server` — [`L197`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L197)
  - `usesOAuth` — [`L197`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L197)
- uses (calls/refs, reference-scoped): [`AuthStorage`](../auth-storage.ts.md#AuthStorage), [`createMcpOAuthProvider`](../../../../ai/src/mcp/oauth.ts.md#createMcpOAuthProvider), [`getApiKey`](../auth-storage.ts.md#AuthStorage.getApiKey), [`registerBuiltinMcpOAuthProviders`](../../../../ai/src/mcp/catalog.ts.md#registerBuiltinMcpOAuthProviders), [`BUILTIN_MCP_CATALOG`](../../../../ai/src/mcp/catalog.ts.md#BUILTIN_MCP_CATALOG), [`get`](../auth-storage.ts.md#AuthStorage.get), [`authStorage`](mcp-manager.ts.md#McpManagerOptions.authStorage), [`registerOAuthProvider`](../../../../ai/src/utils/oauth/index.ts.md#registerOAuthProvider), [`getUserServers`](mcp-manager.ts.md#McpManagerOptions.getUserServers), [`getCatalogEntry`](../../../../ai/src/mcp/catalog.ts.md#getCatalogEntry), [`unregisterOAuthProvider`](../../../../ai/src/utils/oauth/index.ts.md#unregisterOAuthProvider), [`server`](../../../../ai/src/mcp/catalog.ts.md#McpCatalogEntry.server), [`server`](../../../../ai/src/mcp/oauth.ts.md#McpOAuthConfig.server), [`url`](../../../../ai/src/mcp/oauth.ts.md#McpOAuthConfig.url), [`oauth`](../../../../ai/src/mcp/catalog.ts.md#McpCatalogEntry.oauth), [`McpServerConfig`](../settings-manager.ts.md#McpServerConfig), [`server`](mcp-manager.ts.md#ResolvedIntegration.server), [`label`](../../../../ai/src/mcp/catalog.ts.md#McpCatalogEntry.label), [`headers`](mcp-manager.ts.md#ResolvedIntegration.headers), [`label`](../../../../ai/src/mcp/oauth.ts.md#McpOAuthConfig.label), [`label`](mcp-manager.ts.md#ResolvedIntegration.label), [`url`](../../../../ai/src/mcp/catalog.ts.md#McpCatalogEntry.url), [`url`](mcp-manager.ts.md#ResolvedIntegration.url), [`usesOAuth`](mcp-manager.ts.md#ResolvedIntegration.usesOAuth), [`ResolvedIntegration`](mcp-manager.ts.md#ResolvedIntegration), [`bearerTokenEnvVar`](mcp-manager.ts.md#ResolvedIntegration.bearerTokenEnvVar), [`userDeclared`](mcp-manager.ts.md#ResolvedIntegration.userDeclared), [`beginLogin`](mcp-manager.ts.md#McpManagerOptions.beginLogin), [`enabled`](mcp-manager.ts.md#ResolvedIntegration.enabled), [`McpManagerOptions`](mcp-manager.ts.md#McpManagerOptions)
- used by: [`agent-session.ts`](../agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`createAgentSession`](../sdk.ts.md#createAgentSession), [`createAgentSessionServices`](../agent-session-services.ts.md#createAgentSessionServices), [`_createKernelHostHandlers`](../agent-session.ts.md#AgentSession._createKernelHostHandlers), [`sdk.ts`](../sdk.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-sdk.ts), [`agent-session-services.ts`](../agent-session-services.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-services.ts), [`reload`](../agent-session.ts.md#AgentSession.reload), [`_mcpManager`](../agent-session.ts.md#AgentSession._mcpManager), [`mcpManager`](../agent-session.ts.md#AgentSessionConfig.mcpManager), [`mcpManager`](../agent-session-services.ts.md#AgentSessionServices.mcpManager), [`mcpManager`](../sdk.ts.md#CreateAgentSessionOptions.mcpManager)  (1 test-only)

### `McpManagerOptions`
- def: [`packages/coding-agent/src/core/mcp/mcp-manager.ts:14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L14)
- signature: `interface McpManagerOptions`
- members:
  - `authStorage` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L15)
  - `beginLogin` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L19) — Start an interactive host-side login for a server. Provided by the UI mode.
  - `getUserServers` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L17) — Reads the current Settings.mcpServers (name → config). Re-read on refresh().
- uses (calls/refs, reference-scoped): [`AuthStorage`](../auth-storage.ts.md#AuthStorage), [`McpServerConfig`](../settings-manager.ts.md#McpServerConfig)
- used by: [`createAgentSession`](../sdk.ts.md#createAgentSession), [`createAgentSessionServices`](../agent-session-services.ts.md#createAgentSessionServices), [`<constructor>`](mcp-manager.ts.md#McpManager.-constructor)  (1 test-only)

### `ResolvedIntegration`
- def: [`packages/coding-agent/src/core/mcp/mcp-manager.ts:23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L23)
- doc: A resolved integration: a catalog/user entry plus its provider id.
- signature: `interface ResolvedIntegration`
- members:
  - `bearerTokenEnvVar` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L28)
  - `enabled` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L29)
  - `headers` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L31) — Extra static HTTP headers from the user config.
  - `label` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L25)
  - `server` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L24)
  - `url` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L26)
  - `userDeclared` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L33) — True when this came from Settings.mcpServers (may override a catalog name).
  - `usesOAuth` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/mcp/mcp-manager.ts#L27)
- used by: [`resolveIntegrations`](mcp-manager.ts.md#McpManager.resolveIntegrations), [`registerUserProviders`](mcp-manager.ts.md#McpManager.registerUserProviders), [`isAuthed`](mcp-manager.ts.md#McpManager.isAuthed), [`hostHandlers`](mcp-manager.ts.md#McpManager.hostHandlers), [`listStatus`](mcp-manager.ts.md#McpManager.listStatus), [`integrations`](mcp-manager.ts.md#McpManager.integrations)


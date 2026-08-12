---
title: 'Module: packages/ai/src/mcp/catalog.ts'
type: catalog
provenance: extracted
module: packages/ai/src/mcp/catalog.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/mcp/`catalog.ts`/
symbols:
  registerBuiltinMcpOAuthProviders: registerBuiltinMcpOAuthProviders().
  BUILTIN_MCP_CATALOG: BUILTIN_MCP_CATALOG.
  getCatalogEntry: getCatalogEntry().
  McpCatalogEntry.server: McpCatalogEntry#server.
  McpCatalogEntry.oauth: McpCatalogEntry#oauth.
  McpCatalogEntry.label: McpCatalogEntry#label.
  McpCatalogEntry.url: McpCatalogEntry#url.
  McpCatalogEntry: McpCatalogEntry#
---
# Module: [`packages/ai/src/mcp/catalog.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/catalog.ts)

## Classes
### `McpCatalogEntry`
- def: [`packages/ai/src/mcp/catalog.ts:6`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/catalog.ts#L6)
- signature: `interface McpCatalogEntry`
- members:
  - `label` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/catalog.ts#L9)
  - `oauth` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/catalog.ts#L11)
  - `server` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/catalog.ts#L8) — Matches the skill package import name and the auth.json key `mcp:<server>`.
  - `url` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/catalog.ts#L10)
- uses (calls/refs, reference-scoped): [`McpOAuthConfig`](oauth.ts.md#McpOAuthConfig)
- used by: [`resolveIntegrations`](../../../coding-agent/src/core/mcp/mcp-manager.ts.md#McpManager.resolveIntegrations), [`handleMcpCommand`](../../../coding-agent/src/modes/interactive/interactive-mode.ts.md#InteractiveMode.handleMcpCommand), [`registerBuiltinMcpOAuthProviders`](catalog.ts.md#registerBuiltinMcpOAuthProviders), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-mcp-index.ts), [`BUILTIN_MCP_CATALOG`](catalog.ts.md#BUILTIN_MCP_CATALOG), [`getDisabledBuiltinSkillOverrides`](../../../coding-agent/src/core/mcp/mcp-manager.ts.md#McpManager.getDisabledBuiltinSkillOverrides), [`getCatalogEntry`](catalog.ts.md#getCatalogEntry)

## Functions
- `getCatalogEntry(server: string)` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/catalog.ts#L29)
- `registerBuiltinMcpOAuthProviders()` — [`L38`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/catalog.ts#L38) — Register the built-in catalog's OAuth providers. Idempotent. Must be called

## Module values
- `BUILTIN_MCP_CATALOG` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/catalog.ts#L14)


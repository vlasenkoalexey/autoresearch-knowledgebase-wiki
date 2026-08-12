---
title: 'Module: packages/coding-agent/src/core/tools/index.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/tools/index.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/tools/`index.ts`/
symbols:
  createAllToolDefinitions: createAllToolDefinitions().
  createToolDefinition: createToolDefinition().
  createTool: createTool().
  createAllTools: createAllTools().
  ToolsOptions: ToolsOptions#
  Tool: Tool#
  ToolName: ToolName#
  ToolDef: ToolDef#
  allToolNames: allToolNames.
  ToolsOptions.ipython: ToolsOptions#ipython.
---
# Module: [`packages/coding-agent/src/core/tools/index.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/index.ts)

## Classes
### `Tool`
- def: [`packages/coding-agent/src/core/tools/index.ts:44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/index.ts#L44)
- signature: `type Tool`
- uses (calls/refs, reference-scoped): [`AgentTool`](../../../../agent/src/types.ts.md#AgentTool)
- used by: [`modelFallbackMessage`](../sdk.ts.md#CreateAgentSessionResult.modelFallbackMessage), [`createAllTools`](index.ts.md#createAllTools), [`createTool`](index.ts.md#createTool)

### `ToolDef`
- def: [`packages/coding-agent/src/core/tools/index.ts:45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/index.ts#L45)
- signature: `type ToolDef`
- uses (calls/refs, reference-scoped): [`ToolDefinition`](../extensions/types.ts.md#ToolDefinition)
- used by: [`createAllToolDefinitions`](index.ts.md#createAllToolDefinitions), [`createToolDefinition`](index.ts.md#createToolDefinition)

### `ToolName`
- def: [`packages/coding-agent/src/core/tools/index.ts:46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/index.ts#L46)
- signature: `type ToolName`
- used by: [`createAllToolDefinitions`](index.ts.md#createAllToolDefinitions), [`createAllTools`](index.ts.md#createAllTools), [`createTool`](index.ts.md#createTool), [`createToolDefinition`](index.ts.md#createToolDefinition), [`allToolNames`](index.ts.md#allToolNames)

### `ToolsOptions`
- def: [`packages/coding-agent/src/core/tools/index.ts:49`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/index.ts#L49)
- signature: `interface ToolsOptions`
- members:
  - `ipython` — [`L50`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/index.ts#L50)
- uses (calls/refs, reference-scoped): [`IpythonToolOptions`](ipython.ts.md#IpythonToolOptions)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`createAllToolDefinitions`](index.ts.md#createAllToolDefinitions), [`createAllTools`](index.ts.md#createAllTools), [`createTool`](index.ts.md#createTool), [`createToolDefinition`](index.ts.md#createToolDefinition)

## Functions
- `createAllToolDefinitions(cwd: string, options?: ToolsOptions | undefined)` — [`L71`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/index.ts#L71)
- `createAllTools(cwd: string, options?: ToolsOptions | undefined)` — [`L77`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/index.ts#L77)
- `createTool(toolName: "ipython", cwd: string, options?: ToolsOptions | undefined)` — [`L62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/index.ts#L62)
- `createToolDefinition(toolName: "ipython", cwd: string, options?: ToolsOptions | undefined)` — [`L53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/index.ts#L53)

## Module values
- `allToolNames` — [`L47`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/index.ts#L47)


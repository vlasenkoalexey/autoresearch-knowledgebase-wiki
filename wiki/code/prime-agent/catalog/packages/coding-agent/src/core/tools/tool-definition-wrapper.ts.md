---
title: 'Module: packages/coding-agent/src/core/tools/tool-definition-wrapper.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/tools/tool-definition-wrapper.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/tools/`tool-definition-wrapper.ts`/
symbols:
  wrapToolDefinition: wrapToolDefinition().
  createToolDefinitionFromAgentTool: createToolDefinitionFromAgentTool().
  wrapToolDefinitions: wrapToolDefinitions().
---
# Module: [`packages/coding-agent/src/core/tools/tool-definition-wrapper.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/tool-definition-wrapper.ts)

## Functions
- `createToolDefinitionFromAgentTool(tool: AgentTool<any, any>)` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/tool-definition-wrapper.ts#L35) — Synthesize a minimal ToolDefinition from an AgentTool.
- `wrapToolDefinition(definition: ToolDefinition<any, TDetails, any>, ctxFactory?: (() => ExtensionContext) | undefined)` — [`L5`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/tool-definition-wrapper.ts#L5) — Wrap a ToolDefinition into an AgentTool for the core runtime.
- `wrapToolDefinitions(definitions: ToolDefinition<any, any, any>[], ctxFactory?: (() => ExtensionContext) | undefined)` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/tool-definition-wrapper.ts#L22) — Wrap multiple ToolDefinitions into AgentTools for the core runtime.


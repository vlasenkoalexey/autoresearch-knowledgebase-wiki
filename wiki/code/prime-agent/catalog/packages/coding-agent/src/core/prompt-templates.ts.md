---
title: 'Module: packages/coding-agent/src/core/prompt-templates.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/prompt-templates.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`prompt-templates.ts`/
symbols:
  substituteArgs: substituteArgs().
  loadPromptTemplates: loadPromptTemplates().
  PromptTemplate: PromptTemplate#
  PromptTemplate.name: PromptTemplate#name.
  parseCommandArgs: parseCommandArgs().
  expandPromptTemplate: expandPromptTemplate().
  loadTemplateFromFile: loadTemplateFromFile().
  PromptTemplate.sourceInfo: PromptTemplate#sourceInfo.
  PromptTemplate.filePath: PromptTemplate#filePath.
  loadTemplatesFromDir: loadTemplatesFromDir().
  PromptTemplate.description: PromptTemplate#description.
  LoadPromptTemplatesOptions.agentDir: LoadPromptTemplatesOptions#agentDir.
  PromptTemplate.argumentHint: PromptTemplate#argumentHint.
  LoadPromptTemplatesOptions.cwd: LoadPromptTemplatesOptions#cwd.
  LoadPromptTemplatesOptions.promptPaths: LoadPromptTemplatesOptions#promptPaths.
  LoadPromptTemplatesOptions.includeDefaults: LoadPromptTemplatesOptions#includeDefaults.
  PromptTemplate.content: PromptTemplate#content.
  resolvePromptPath: resolvePromptPath().
  LoadPromptTemplatesOptions: LoadPromptTemplatesOptions#
  normalizePath: normalizePath().
---
# Module: [`packages/coding-agent/src/core/prompt-templates.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts)

## Classes
### `LoadPromptTemplatesOptions`
- def: [`packages/coding-agent/src/core/prompt-templates.ts:179`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L179)
- signature: `interface LoadPromptTemplatesOptions`
- members:
  - `agentDir` — [`L183`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L183) — Agent config directory for global templates.
  - `cwd` — [`L181`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L181) — Working directory for project-local templates.
  - `includeDefaults` — [`L187`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L187) — Include default prompt directories.
  - `promptPaths` — [`L185`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L185) — Explicit prompt template paths (files or directories).
- used by: [`updatePromptsFromPaths`](resource-loader.ts.md#DefaultResourceLoader.updatePromptsFromPaths), [`loadPromptTemplates`](prompt-templates.ts.md#loadPromptTemplates)  (1 test-only)

### `PromptTemplate`
- def: [`packages/coding-agent/src/core/prompt-templates.ts:12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L12)
- doc: Represents a prompt template loaded from a markdown file
- signature: `interface PromptTemplate`
- members:
  - `argumentHint` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L15)
  - `content` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L16)
  - `description` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L14)
  - `filePath` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L18)
  - `name` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L13)
  - `sourceInfo` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L17)
- uses (calls/refs, reference-scoped): [`SourceInfo`](source-info.ts.md#SourceInfo)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`_bindExtensionCore`](agent-session.ts.md#AgentSession._bindExtensionCore), [`createAgentConnectionResourceSnapshot`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionResourceSnapshot), [`resource-loader.ts`](resource-loader.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-resource-loader.ts), [`modelFallbackMessage`](sdk.ts.md#CreateAgentSessionResult.modelFallbackMessage), [`createAgentConnectionCommands`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionCommands), [`updatePromptsFromPaths`](resource-loader.ts.md#DefaultResourceLoader.updatePromptsFromPaths), [`loadPromptTemplates`](prompt-templates.ts.md#loadPromptTemplates), [`dedupePrompts`](resource-loader.ts.md#DefaultResourceLoader.dedupePrompts), [`expandPromptTemplate`](prompt-templates.ts.md#expandPromptTemplate), [`<get>promptTemplates`](agent-session.ts.md#AgentSession.-get-promptTemplates), [`loadTemplateFromFile`](prompt-templates.ts.md#loadTemplateFromFile), [`loadTemplatesFromDir`](prompt-templates.ts.md#loadTemplatesFromDir), [`prompts`](resource-loader.ts.md#DefaultResourceLoader.getPrompts.typeLiteral157.prompts), [`prompts`](resource-loader.ts.md#ResourceLoader.getPrompts.typeLiteral4.prompts), [`promptsOverride`](resource-loader.ts.md#DefaultResourceLoader.promptsOverride), [`promptsOverride`](resource-loader.ts.md#DefaultResourceLoaderOptions.promptsOverride), [`prompts`](resource-loader.ts.md#DefaultResourceLoader.prompts), [`prompts`](resource-loader.ts.md#DefaultResourceLoader.dedupePrompts.typeLiteral577.prompts)  (6 test-only)

## Functions
- `expandPromptTemplate(text: string, templates: PromptTemplate[])` — [`L284`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L284) — Expand a prompt template if it matches a template name.
- `loadPromptTemplates(options: LoadPromptTemplatesOptions)` — [`L209`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L209) — Load all prompt templates from:
- `loadTemplateFromFile(filePath: string, sourceInfo: SourceInfo)` — [`L105`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L105)
- `loadTemplatesFromDir(dir: string, getSourceInfo: (filePath: string) => SourceInfo)` — [`L140`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L140) — Scan a directory for .md files (non-recursive) and load them as prompt templates.
- `normalizePath(input: string)` — [`L190`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L190)
- `parseCommandArgs(argsString: string)` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L25) — Parse command arguments respecting quoted strings (bash-style)
- `resolvePromptPath(p: string, cwd: string)` — [`L198`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L198)
- `substituteArgs(content: string, args: string[])` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-templates.ts#L69) — Substitute argument placeholders in template content


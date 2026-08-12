---
title: 'Module: packages/coding-agent/src/core/source-info.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/source-info.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`source-info.ts`/
symbols:
  createSyntheticSourceInfo: createSyntheticSourceInfo().
  createSourceInfo: createSourceInfo().
  SourceInfo: SourceInfo#
  createSyntheticSourceInfo.options-typeLiteral0.source: createSyntheticSourceInfo().(options)typeLiteral0:source.
  SourceInfo.path: SourceInfo#path.
  SourceInfo.source: SourceInfo#source.
  SourceInfo.scope: SourceInfo#scope.
  createSyntheticSourceInfo.options-typeLiteral0.scope: createSyntheticSourceInfo().(options)typeLiteral0:scope.
  createSyntheticSourceInfo.options-typeLiteral0.baseDir: createSyntheticSourceInfo().(options)typeLiteral0:baseDir.
  SourceInfo.origin: SourceInfo#origin.
  createSyntheticSourceInfo.options-typeLiteral0.origin: createSyntheticSourceInfo().(options)typeLiteral0:origin.
  SourceInfo.baseDir: SourceInfo#baseDir.
  SourceScope: SourceScope#
  SourceOrigin: SourceOrigin#
---
# Module: [`packages/coding-agent/src/core/source-info.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/source-info.ts)

## Classes
### `SourceInfo`
- def: [`packages/coding-agent/src/core/source-info.ts:6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/source-info.ts#L6)
- signature: `interface SourceInfo`
- members:
  - `baseDir` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/source-info.ts#L11)
  - `origin` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/source-info.ts#L10)
  - `path` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/source-info.ts#L7)
  - `scope` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/source-info.ts#L9)
  - `source` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/source-info.ts#L8)
- uses (calls/refs, reference-scoped): [`SourceOrigin`](source-info.ts.md#SourceOrigin), [`SourceScope`](source-info.ts.md#SourceScope)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`index.ts`](extensions/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-index.ts), [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`theme.ts`](../modes/interactive/theme/theme.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-theme-theme.ts), [`resource-loader.ts`](resource-loader.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-resource-loader.ts), [`createSyntheticSourceInfo`](source-info.ts.md#createSyntheticSourceInfo), [`skills.ts`](skills.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-skills.ts), [`loadPromptTemplates`](prompt-templates.ts.md#loadPromptTemplates), [`sourceInfo`](../modes/interactive/theme/theme.ts.md#Theme.-constructor-.options-typeLiteral88.sourceInfo), [`createSourceInfo`](source-info.ts.md#createSourceInfo), [`getDefaultSourceInfoForPath`](resource-loader.ts.md#DefaultResourceLoader.getDefaultSourceInfoForPath), [`prompt-templates.ts`](prompt-templates.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-prompt-templates.ts), [`slash-commands.ts`](slash-commands.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-slash-commands.ts), [`sourceInfo`](skills.ts.md#BaseSkill.sourceInfo), [`RegisteredTool`](extensions/types.ts.md#RegisteredTool), [`loadTemplateFromFile`](prompt-templates.ts.md#loadTemplateFromFile), [`findSourceInfoForPath`](resource-loader.ts.md#DefaultResourceLoader.findSourceInfoForPath), [`createSkillSourceInfo`](skills.ts.md#createSkillSourceInfo), [`sourceInfo`](extensions/types.ts.md#Extension.sourceInfo), [`ToolInfo`](extensions/types.ts.md#ToolInfo), [`sourceInfo`](prompt-templates.ts.md#PromptTemplate.sourceInfo), [`loadTemplatesFromDir`](prompt-templates.ts.md#loadTemplatesFromDir), [`sourceInfo`](../modes/interactive/theme/theme.ts.md#Theme.sourceInfo), [`extensionPromptSourceInfos`](resource-loader.ts.md#DefaultResourceLoader.extensionPromptSourceInfos), [`extensionSkillSourceInfos`](resource-loader.ts.md#DefaultResourceLoader.extensionSkillSourceInfos), [`extensionThemeSourceInfos`](resource-loader.ts.md#DefaultResourceLoader.extensionThemeSourceInfos), [`sourceInfo`](extensions/types.ts.md#RegisteredCommand.sourceInfo), [`sourceInfo`](slash-commands.ts.md#SlashCommandInfo.sourceInfo), [`ToolDefinitionEntry`](agent-session.ts.md#ToolDefinitionEntry)  (5 test-only)

### `SourceOrigin`
- def: [`packages/coding-agent/src/core/source-info.ts:4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/source-info.ts#L4)
- signature: `type SourceOrigin`
- used by: [`origin`](source-info.ts.md#SourceInfo.origin), [`origin`](source-info.ts.md#createSyntheticSourceInfo.options-typeLiteral0.origin)

### `SourceScope`
- def: [`packages/coding-agent/src/core/source-info.ts:3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/source-info.ts#L3)
- signature: `type SourceScope`
- used by: [`scope`](source-info.ts.md#SourceInfo.scope), [`scope`](source-info.ts.md#createSyntheticSourceInfo.options-typeLiteral0.scope)

## Functions
- `createSourceInfo(path: string, metadata: PathMetadata)` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/source-info.ts#L14)
- `createSyntheticSourceInfo(path: string, options: { source: string; scope?: SourceScope | undefined; origin?: SourceOrigin | undefined; baseDir?: string | undefined; })` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/source-info.ts#L24)

## Module values
- `baseDir` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/source-info.ts#L30)
- `origin` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/source-info.ts#L29)
- `scope` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/source-info.ts#L28)
- `source` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/source-info.ts#L27)


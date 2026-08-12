---
title: 'Module: packages/coding-agent/src/core/skills.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/skills.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`skills.ts`/
symbols:
  loadSkills: loadSkills().
  BaseSkill.name: BaseSkill#name.
  loadSkillFromFile: loadSkillFromFile().
  Skill: Skill#
  loadSkillsFromDir: loadSkillsFromDir().
  LoadSkillsResult.skills: LoadSkillsResult#skills.
  loadSkillsFromDirInternal: loadSkillsFromDirInternal().
  formatSkillsForPrompt: formatSkillsForPrompt().
  SkillPythonMetadata.importName: SkillPythonMetadata#importName.
  getPythonSkillRuntimeInfo: getPythonSkillRuntimeInfo().
  SkillPythonMetadata.packagePath: SkillPythonMetadata#packagePath.
  SkillPythonMetadata.pyprojectPath: SkillPythonMetadata#pyprojectPath.
  LoadSkillsFromDirOptions.dir: LoadSkillsFromDirOptions#dir.
  LoadSkillsFromDirOptions.source: LoadSkillsFromDirOptions#source.
  BaseSkill.filePath: BaseSkill#filePath.
  MarkdownSkill.kind: MarkdownSkill#kind.
  PythonSkill.kind: PythonSkill#kind.
  LoadSkillsResult.diagnostics: LoadSkillsResult#diagnostics.
  BaseSkill.description: BaseSkill#description.
  PythonSkillRuntimeInfo: PythonSkillRuntimeInfo#
  BaseSkill.sourceInfo: BaseSkill#sourceInfo.
  detectPythonSkill: detectPythonSkill().
  PythonSkill.python: PythonSkill#python.
  createSkillSourceInfo: createSkillSourceInfo().
  BaseSkill.disableModelInvocation: BaseSkill#disableModelInvocation.
  loadSkillFromFile.typeLiteral101.skill: loadSkillFromFile().typeLiteral101:skill.
  addIgnoreRules: addIgnoreRules().
  PythonSkillRuntimeInfo.name: PythonSkillRuntimeInfo#name.
  BaseSkill.baseDir: BaseSkill#baseDir.
  PythonSkill: PythonSkill#
  LoadSkillsResult: LoadSkillsResult#
  loadSkillFromFile.typeLiteral101.diagnostics: loadSkillFromFile().typeLiteral101:diagnostics.
  LoadSkillsOptions.cwd: LoadSkillsOptions#cwd.
  LoadSkillsOptions.agentDir: LoadSkillsOptions#agentDir.
  LoadSkillsOptions.skillPaths: LoadSkillsOptions#skillPaths.
  LoadSkillsOptions.includeDefaults: LoadSkillsOptions#includeDefaults.
  SkillPythonMetadata: SkillPythonMetadata#
  MarkdownSkill: MarkdownSkill#
  SkillFrontmatter.description: SkillFrontmatter#description.
  MarkdownSkill.python: MarkdownSkill#python.
  escapeXml: escapeXml().
  log: log.
  validateName: validateName().
  validateDescription: validateDescription().
  resolveSkillPath: resolveSkillPath().
  toPosixPath: toPosixPath().
  BaseSkill: BaseSkill#
  MAX_NAME_LENGTH: MAX_NAME_LENGTH.
  MAX_DESCRIPTION_LENGTH: MAX_DESCRIPTION_LENGTH.
  IgnoreMatcher: IgnoreMatcher#
  SkillFrontmatter: SkillFrontmatter#
  LoadSkillsFromDirOptions: LoadSkillsFromDirOptions#
  IGNORE_FILE_NAMES: IGNORE_FILE_NAMES.
  prefixIgnorePattern: prefixIgnorePattern().
  SkillFrontmatter.name: SkillFrontmatter#name.
  SkillFrontmatter.-disable-model-invocation: SkillFrontmatter#`"disable-model-invocation"`.
  SkillKind: SkillKind#
  pythonImportNameForSkill: pythonImportNameForSkill().
  isValidPythonImportName: isValidPythonImportName().
  LoadSkillsOptions: LoadSkillsOptions#
  normalizePath: normalizePath().
---
# Module: [`packages/coding-agent/src/core/skills.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts)

## Classes
### `BaseSkill`
- def: [`packages/coding-agent/src/core/skills.ts:88`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L88)
- signature: `interface BaseSkill`
- members:
  - `baseDir` — [`L92`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L92)
  - `description` — [`L90`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L90)
  - `disableModelInvocation` — [`L94`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L94)
  - `filePath` — [`L91`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L91)
  - `name` — [`L89`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L89)
  - `sourceInfo` — [`L93`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L93)
- uses (calls/refs, reference-scoped): [`SourceInfo`](source-info.ts.md#SourceInfo)
- used by: [`_bindExtensionCore`](agent-session.ts.md#AgentSession._bindExtensionCore), [`_createKernelHostHandlers`](agent-session.ts.md#AgentSession._createKernelHostHandlers), [`createAgentConnectionResourceSnapshot`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionResourceSnapshot), [`buildSystemPrompt`](system-prompt.ts.md#buildSystemPrompt), [`loadSkills`](skills.ts.md#loadSkills), [`loadSkillFromFile`](skills.ts.md#loadSkillFromFile), [`createAgentConnectionCommands`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionCommands), [`updateSkillsFromPaths`](resource-loader.ts.md#DefaultResourceLoader.updateSkillsFromPaths), [`_modelVisibleSkills`](agent-session.ts.md#AgentSession._modelVisibleSkills), [`_expandSkillCommand`](agent-session.ts.md#AgentSession._expandSkillCommand), [`formatSkillsForPrompt`](skills.ts.md#formatSkillsForPrompt), [`_addWebsearchKeyEnv`](agent-session.ts.md#AgentSession._addWebsearchKeyEnv), [`getPythonSkillRuntimeInfo`](skills.ts.md#getPythonSkillRuntimeInfo), [`PythonSkill`](skills.ts.md#PythonSkill), [`MarkdownSkill`](skills.ts.md#MarkdownSkill)  (11 test-only)

### `IgnoreMatcher`
- def: [`packages/coding-agent/src/core/skills.ts:22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L22)
- signature: `type IgnoreMatcher`
- used by: [`loadSkillsFromDirInternal`](skills.ts.md#loadSkillsFromDirInternal), [`addIgnoreRules`](skills.ts.md#addIgnoreRules)

### `LoadSkillsFromDirOptions`
- def: [`packages/coding-agent/src/core/skills.ts:163`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L163)
- signature: `interface LoadSkillsFromDirOptions`
- members:
  - `dir` — [`L165`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L165) — Directory to scan for skills
  - `source` — [`L167`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L167) — Source identifier for these skills
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`loadSkillsFromDir`](skills.ts.md#loadSkillsFromDir)  (2 test-only)

### `LoadSkillsOptions`
- def: [`packages/coding-agent/src/core/skills.ts:492`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L492)
- signature: `interface LoadSkillsOptions`
- members:
  - `agentDir` — [`L496`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L496) — Agent config directory for global skills.
  - `cwd` — [`L494`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L494) — Working directory for project-local skills.
  - `includeDefaults` — [`L500`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L500) — Include default skills directories.
  - `skillPaths` — [`L498`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L498) — Explicit skill paths (files or directories)
- used by: [`loadSkills`](skills.ts.md#loadSkills), [`updateSkillsFromPaths`](resource-loader.ts.md#DefaultResourceLoader.updateSkillsFromPaths)  (1 test-only)

### `LoadSkillsResult`
- def: [`packages/coding-agent/src/core/skills.ts:113`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L113)
- signature: `interface LoadSkillsResult`
- members:
  - `diagnostics` — [`L115`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L115)
  - `skills` — [`L114`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L114)
- uses (calls/refs, reference-scoped): [`ResourceDiagnostic`](diagnostics.ts.md#ResourceDiagnostic), [`Skill`](skills.ts.md#Skill)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`loadSkills`](skills.ts.md#loadSkills), [`loadSkillsFromDir`](skills.ts.md#loadSkillsFromDir), [`loadSkillsFromDirInternal`](skills.ts.md#loadSkillsFromDirInternal)  (2 test-only)

### `MarkdownSkill`
- def: [`packages/coding-agent/src/core/skills.ts:97`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L97)
- signature: `interface MarkdownSkill`
- members:
  - `kind` — [`L98`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L98)
  - `python` — [`L99`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L99)
- uses (calls/refs, reference-scoped): [`BaseSkill`](skills.ts.md#BaseSkill)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`loadSkills`](skills.ts.md#loadSkills), [`Skill`](skills.ts.md#Skill), [`formatSkillsForPrompt`](skills.ts.md#formatSkillsForPrompt), [`getPythonSkillRuntimeInfo`](skills.ts.md#getPythonSkillRuntimeInfo)  (9 test-only)

### `PythonSkill`
- def: [`packages/coding-agent/src/core/skills.ts:102`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L102)
- signature: `interface PythonSkill`
- members:
  - `kind` — [`L103`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L103)
  - `python` — [`L104`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L104)
- uses (calls/refs, reference-scoped): [`SkillPythonMetadata`](skills.ts.md#SkillPythonMetadata), [`BaseSkill`](skills.ts.md#BaseSkill)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`loadSkills`](skills.ts.md#loadSkills), [`Skill`](skills.ts.md#Skill), [`formatSkillsForPrompt`](skills.ts.md#formatSkillsForPrompt), [`getPythonSkillRuntimeInfo`](skills.ts.md#getPythonSkillRuntimeInfo)  (9 test-only)

### `PythonSkillRuntimeInfo`
- def: [`packages/coding-agent/src/core/skills.ts:109`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L109)
- signature: `interface PythonSkillRuntimeInfo`
- members:
  - `name` — [`L110`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L110)
- uses (calls/refs, reference-scoped): [`SkillPythonMetadata`](skills.ts.md#SkillPythonMetadata)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`ipython.ts`](tools/ipython.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-ipython.ts), [`getPythonSkillRuntimeInfo`](skills.ts.md#getPythonSkillRuntimeInfo), [`bootstrap.ts`](kernel/bootstrap.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-kernel-bootstrap.ts), [`buildRlmBootstrapCode`](tools/ipython.ts.md#buildRlmBootstrapCode), [`KernelPythonSkill`](kernel/bootstrap.ts.md#KernelPythonSkill), [`missingPythonSkillImportLabels`](kernel/bootstrap.ts.md#missingPythonSkillImportLabels), [`pythonSkills`](tools/ipython.ts.md#IpythonToolOptions.pythonSkills)  (15 test-only)

### `Skill`
- def: [`packages/coding-agent/src/core/skills.ts:107`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L107)
- signature: `type Skill`
- uses (calls/refs, reference-scoped): [`PythonSkill`](skills.ts.md#PythonSkill), [`MarkdownSkill`](skills.ts.md#MarkdownSkill)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`resource-loader.ts`](resource-loader.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-resource-loader.ts), [`loadSkills`](skills.ts.md#loadSkills), [`modelFallbackMessage`](sdk.ts.md#CreateAgentSessionResult.modelFallbackMessage), [`updateSkillsFromPaths`](resource-loader.ts.md#DefaultResourceLoader.updateSkillsFromPaths), [`_modelVisibleSkills`](agent-session.ts.md#AgentSession._modelVisibleSkills), [`skills`](skills.ts.md#LoadSkillsResult.skills), [`loadSkillsFromDirInternal`](skills.ts.md#loadSkillsFromDirInternal), [`formatSkillsForPrompt`](skills.ts.md#formatSkillsForPrompt), [`system-prompt.ts`](system-prompt.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-system-prompt.ts), [`getPythonSkillRuntimeInfo`](skills.ts.md#getPythonSkillRuntimeInfo), [`skills`](resource-loader.ts.md#DefaultResourceLoader.getSkills.typeLiteral156.skills), [`skills`](system-prompt.ts.md#BuildSystemPromptOptions.skills), [`skills`](resource-loader.ts.md#ResourceLoader.getSkills.typeLiteral3.skills), [`skill`](skills.ts.md#loadSkillFromFile.typeLiteral101.skill), [`skillsOverride`](resource-loader.ts.md#DefaultResourceLoader.skillsOverride), [`skillsOverride`](resource-loader.ts.md#DefaultResourceLoaderOptions.skillsOverride), [`skills`](resource-loader.ts.md#DefaultResourceLoader.skills)  (11 test-only)

### `SkillFrontmatter`
- def: [`packages/coding-agent/src/core/skills.ts:73`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L73)
- signature: `interface SkillFrontmatter`
- members:
  - `"disable-model-invocation"` — [`L76`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L76)
  - `description` — [`L75`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L75)
  - `name` — [`L74`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L74)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`loadSkillFromFile`](skills.ts.md#loadSkillFromFile)

### `SkillKind`
- def: [`packages/coding-agent/src/core/skills.ts:80`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L80)
- signature: `type SkillKind`
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts)

### `SkillPythonMetadata`
- def: [`packages/coding-agent/src/core/skills.ts:82`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L82)
- signature: `interface SkillPythonMetadata`
- members:
  - `importName` — [`L83`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L83)
  - `packagePath` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L84)
  - `pyprojectPath` — [`L85`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L85)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`buildSystemPrompt`](system-prompt.ts.md#buildSystemPrompt), [`loadSkills`](skills.ts.md#loadSkills), [`formatSkillsForPrompt`](skills.ts.md#formatSkillsForPrompt), [`getPythonSkillRuntimeInfo`](skills.ts.md#getPythonSkillRuntimeInfo), [`normalizePythonSkills`](kernel/bootstrap.ts.md#normalizePythonSkills), [`PythonSkillRuntimeInfo`](skills.ts.md#PythonSkillRuntimeInfo), [`detectPythonSkill`](skills.ts.md#detectPythonSkill), [`buildRlmBootstrapCode`](tools/ipython.ts.md#buildRlmBootstrapCode), [`missingPythonSkillImportLabels`](kernel/bootstrap.ts.md#missingPythonSkillImportLabels), [`PythonSkill`](skills.ts.md#PythonSkill)  (17 test-only)

## Functions
- `addIgnoreRules(ig: Ignore, dir: string, rootDir: string)` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L51)
- `createSkillSourceInfo(filePath: string, baseDir: string, source: string)` — [`L170`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L170)
- `detectPythonSkill(skillDir: string, name: string, diagnostics: ResourceDiagnostic[])` — [`L202`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L202)
- `escapeXml(str: string)` — [`L483`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L483)
- `formatSkillsForPrompt(skills: Skill[])` — [`L450`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L450) — Format skills for inclusion in a system prompt.
- `getPythonSkillRuntimeInfo(skills: readonly Skill[])` — [`L256`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L256)
- `isValidPythonImportName(name: string)` — [`L198`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L198)
- `loadSkillFromFile(filePath: string, source: string)` — [`L389`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L389)
- `loadSkills(options: LoadSkillsOptions)` — [`L520`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L520) — Load skills from all configured locations.
- `loadSkillsFromDir(options: LoadSkillsFromDirOptions)` — [`L275`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L275) — Load skills from a directory.
- `loadSkillsFromDirInternal(dir: string, source: string, includeRootFiles: boolean, ignoreMatcher?: Ignore | undefined, rootDir?: string | undefined)` — [`L280`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L280)
- `normalizePath(input: string)` — [`L503`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L503)
- `prefixIgnorePattern(line: string, prefix: string)` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L28)
- `pythonImportNameForSkill(name: string)` — [`L194`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L194)
- `resolveSkillPath(p: string, cwd: string)` — [`L511`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L511)
- `toPosixPath(p: string)` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L24)
- `validateDescription(description: string | undefined)` — [`L151`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L151) — Validate description per Agent Skills spec.
- `validateName(name: string, parentDirName: string)` — [`L122`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L122) — Validate skill name per Agent Skills spec.

## Module values
- `IGNORE_FILE_NAMES` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L20)
- `MAX_DESCRIPTION_LENGTH` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L18) — Max description length per spec
- `MAX_NAME_LENGTH` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L15) — Max name length per spec
- `diagnostics` — [`L392`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L392)
- `log` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L12)
- `skill` — [`L392`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skills.ts#L392)


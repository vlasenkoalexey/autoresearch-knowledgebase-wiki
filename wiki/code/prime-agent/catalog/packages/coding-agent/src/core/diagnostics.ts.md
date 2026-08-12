---
title: 'Module: packages/coding-agent/src/core/diagnostics.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/diagnostics.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`diagnostics.ts`/Resource
symbols:
  ResourceDiagnostic: Diagnostic#
  ResourceDiagnostic.message: Diagnostic#message.
  ResourceDiagnostic.path: Diagnostic#path.
  ResourceDiagnostic.type: Diagnostic#type.
  ResourceDiagnostic.collision: Diagnostic#collision.
  ResourceCollision: Collision#
  ResourceCollision.name: Collision#name.
  ResourceCollision.loserPath: Collision#loserPath.
  ResourceCollision.resourceType: Collision#resourceType.
  ResourceCollision.winnerPath: Collision#winnerPath.
  ResourceCollision.winnerSource: Collision#winnerSource.
  ResourceCollision.loserSource: Collision#loserSource.
---
# Module: [`packages/coding-agent/src/core/diagnostics.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/diagnostics.ts)

## Classes
### `ResourceCollision`
- def: [`packages/coding-agent/src/core/diagnostics.ts:1`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/diagnostics.ts#L1)
- signature: `interface ResourceCollision`
- members:
  - `loserPath` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/diagnostics.ts#L5)
  - `loserSource` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/diagnostics.ts#L7)
  - `name` — [`L3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/diagnostics.ts#L3)
  - `resourceType` — [`L2`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/diagnostics.ts#L2)
  - `winnerPath` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/diagnostics.ts#L4)
  - `winnerSource` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/diagnostics.ts#L6)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`resource-loader.ts`](resource-loader.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-resource-loader.ts), [`ResourceDiagnostic`](diagnostics.ts.md#ResourceDiagnostic)  (2 test-only)

### `ResourceDiagnostic`
- def: [`packages/coding-agent/src/core/diagnostics.ts:10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/diagnostics.ts#L10)
- signature: `interface ResourceDiagnostic`
- members:
  - `collision` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/diagnostics.ts#L14)
  - `message` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/diagnostics.ts#L12)
  - `path` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/diagnostics.ts#L13)
  - `type` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/diagnostics.ts#L11)
- uses (calls/refs, reference-scoped): [`ResourceCollision`](diagnostics.ts.md#ResourceCollision)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`reload`](resource-loader.ts.md#DefaultResourceLoader.reload), [`runner.ts`](extensions/runner.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-runner.ts), [`resource-loader.ts`](resource-loader.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-resource-loader.ts), [`addAutoDiscoveredResources`](package-manager.ts.md#DefaultPackageManager.addAutoDiscoveredResources), [`loadSkills`](skills.ts.md#loadSkills), [`loadSkillFromFile`](skills.ts.md#loadSkillFromFile), [`package-manager.ts`](package-manager.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-package-manager.ts), [`skills.ts`](skills.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-skills.ts), [`updatePromptsFromPaths`](resource-loader.ts.md#DefaultResourceLoader.updatePromptsFromPaths), [`updateSkillsFromPaths`](resource-loader.ts.md#DefaultResourceLoader.updateSkillsFromPaths), [`updateThemesFromPaths`](resource-loader.ts.md#DefaultResourceLoader.updateThemesFromPaths), [`getShortcuts`](extensions/runner.ts.md#ExtensionRunner.getShortcuts), [`loadSkillsFromDirInternal`](skills.ts.md#loadSkillsFromDirInternal), [`getSkills`](resource-loader.ts.md#DefaultResourceLoader.getSkills), [`diagnostics`](resource-loader.ts.md#DefaultResourceLoader.loadThemes.typeLiteral415.diagnostics), [`dedupePrompts`](resource-loader.ts.md#DefaultResourceLoader.dedupePrompts), [`dedupeThemes`](resource-loader.ts.md#DefaultResourceLoader.dedupeThemes), [`detectPythonSkill`](skills.ts.md#detectPythonSkill), [`getPrompts`](resource-loader.ts.md#DefaultResourceLoader.getPrompts), [`loadThemeFromFile`](resource-loader.ts.md#DefaultResourceLoader.loadThemeFromFile), [`loadThemesFromDir`](resource-loader.ts.md#DefaultResourceLoader.loadThemesFromDir), [`getThemes`](resource-loader.ts.md#DefaultResourceLoader.getThemes), [`diagnostics`](resource-loader.ts.md#ResourceLoader.getSkills.typeLiteral3.diagnostics), [`ResourceAccumulator`](package-manager.ts.md#ResourceAccumulator), [`diagnostics`](package-manager.ts.md#ResolvedPaths.diagnostics), [`diagnostics`](resource-loader.ts.md#ResourceLoader.getPrompts.typeLiteral4.diagnostics), [`diagnostics`](resource-loader.ts.md#ResourceLoader.getThemes.typeLiteral5.diagnostics), [`skillDiagnostics`](resource-loader.ts.md#DefaultResourceLoader.skillDiagnostics), [`promptsOverride`](resource-loader.ts.md#DefaultResourceLoader.promptsOverride), [`skillsOverride`](resource-loader.ts.md#DefaultResourceLoader.skillsOverride), [`skillsOverride`](resource-loader.ts.md#DefaultResourceLoaderOptions.skillsOverride), [`themesOverride`](resource-loader.ts.md#DefaultResourceLoader.themesOverride), [`LoadSkillsResult`](skills.ts.md#LoadSkillsResult), [`promptDiagnostics`](resource-loader.ts.md#DefaultResourceLoader.promptDiagnostics), [`themeDiagnostics`](resource-loader.ts.md#DefaultResourceLoader.themeDiagnostics), [`getCommandDiagnostics`](extensions/runner.ts.md#ExtensionRunner.getCommandDiagnostics), [`promptsOverride`](resource-loader.ts.md#DefaultResourceLoaderOptions.promptsOverride), [`getShortcutDiagnostics`](extensions/runner.ts.md#ExtensionRunner.getShortcutDiagnostics), [`themesOverride`](resource-loader.ts.md#DefaultResourceLoaderOptions.themesOverride)  (+2 more; 4 test-only)


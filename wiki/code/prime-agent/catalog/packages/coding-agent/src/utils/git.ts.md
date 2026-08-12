---
title: 'Module: packages/coding-agent/src/utils/git.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/utils/git.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/utils/`git.ts`/
symbols:
  captureGitContext: captureGitContext().
  parseGitUrl: parseGitUrl().
  GitSource.typeLiteral0.type: GitSource#typeLiteral0:type.
  splitRef.typeLiteral1.repo: splitRef().typeLiteral1:repo.
  gitContextsEqual: gitContextsEqual().
  splitRef.typeLiteral1.ref: splitRef().typeLiteral1:ref.
  parseGenericGitUrl: parseGenericGitUrl().
  GitContext.commit: GitContext#commit.
  GitSource: GitSource#
  GitSource.typeLiteral0.path: GitSource#typeLiteral0:path.
  GitSource.typeLiteral0.host: GitSource#typeLiteral0:host.
  GitContext: GitContext#
  GitContext.branch: GitContext#branch.
  splitRef: splitRef().
  GitSource.typeLiteral0.ref: GitSource#typeLiteral0:ref.
  findGitPaths: findGitPaths().
  GitContext.repoUrl: GitContext#repoUrl.
  GitSource.typeLiteral0.pinned: GitSource#typeLiteral0:pinned.
  GitPaths: GitPaths#
  GitPaths.typeLiteral116.headPath: GitPaths#typeLiteral116:headPath.
  runGit: runGit().
  GitSource.typeLiteral0.repo: GitSource#typeLiteral0:repo.
  GitPaths.typeLiteral116.repoDir: GitPaths#typeLiteral116:repoDir.
  GitPaths.typeLiteral116.commonGitDir: GitPaths#typeLiteral116:commonGitDir.
---
# Module: [`packages/coding-agent/src/utils/git.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts)

## Classes
### `GitContext`
- def: [`packages/coding-agent/src/utils/git.ts:241`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L241)
- signature: `interface GitContext`
- members:
  - `branch` — [`L244`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L244)
  - `commit` — [`L243`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L243)
  - `repoUrl` — [`L242`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L242)
- used by: [`session-manager.ts`](../core/session-manager.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-session-manager.ts), [`getActiveGitContext`](../core/session-manager.ts.md#SessionManager.getActiveGitContext), [`captureGitContext`](git.ts.md#captureGitContext), [`appendGitState`](../core/session-manager.ts.md#SessionManager.appendGitState), [`gitContextsEqual`](git.ts.md#gitContextsEqual), [`git`](../core/session-manager.ts.md#SessionHeader.git), [`GitStateEntry`](../core/session-manager.ts.md#GitStateEntry)  (1 test-only)

### `GitPaths`
- def: [`packages/coding-agent/src/utils/git.ts:197`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L197)
- signature: `type GitPaths`
- members:
  - `commonGitDir` — [`L199`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L199)
  - `headPath` — [`L200`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L200)
  - `repoDir` — [`L198`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L198)
- used by: [`setupGitWatcher`](../core/footer-data-provider.ts.md#FooterDataProvider.setupGitWatcher), [`footer-data-provider.ts`](../core/footer-data-provider.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-footer-data-provider.ts), [`gitPaths`](../core/footer-data-provider.ts.md#FooterDataProvider.gitPaths), [`resolveGitBranchAsync`](../core/footer-data-provider.ts.md#FooterDataProvider.resolveGitBranchAsync), [`resolveGitBranchSync`](../core/footer-data-provider.ts.md#FooterDataProvider.resolveGitBranchSync), [`findGitPaths`](git.ts.md#findGitPaths)

### `GitSource`
- def: [`packages/coding-agent/src/utils/git.ts:9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L9)
- doc: Parsed git URL information.
- signature: `type GitSource`
- members:
  - `host` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L15) — Git host domain (e.g., "github.com")
  - `path` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L17) — Repository path (e.g., "user/repo")
  - `pinned` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L21) — True if ref was specified (package won't be auto-updated)
  - `ref` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L19) — Git ref (branch, tag, commit) if specified
  - `repo` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L13) — Clone URL (always valid for git clone, without ref suffix)
  - `type` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L11) — Always "git" for git sources
- used by: [`checkForAvailableUpdates`](../core/package-manager.ts.md#DefaultPackageManager.checkForAvailableUpdates), [`resolvePackageSources`](../core/package-manager.ts.md#DefaultPackageManager.resolvePackageSources), [`package-manager.ts`](../core/package-manager.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-package-manager.ts), [`updateConfiguredSources`](../core/package-manager.ts.md#DefaultPackageManager.updateConfiguredSources), [`getPackageIdentity`](../core/package-manager.ts.md#DefaultPackageManager.getPackageIdentity), [`install`](../core/package-manager.ts.md#DefaultPackageManager.install), [`parseSource`](../core/package-manager.ts.md#DefaultPackageManager.parseSource), [`updateGit`](../core/package-manager.ts.md#DefaultPackageManager.updateGit), [`captureGitContext`](git.ts.md#captureGitContext), [`findSuggestedConfiguredSource`](../core/package-manager.ts.md#DefaultPackageManager.findSuggestedConfiguredSource), [`getSourceMatchKeyForSettings`](../core/package-manager.ts.md#DefaultPackageManager.getSourceMatchKeyForSettings), [`installGit`](../core/package-manager.ts.md#DefaultPackageManager.installGit), [`parseGitUrl`](git.ts.md#parseGitUrl), [`getInstalledPath`](../core/package-manager.ts.md#DefaultPackageManager.getInstalledPath), [`getGitInstallPath`](../core/package-manager.ts.md#DefaultPackageManager.getGitInstallPath), [`getSourceMatchKeyForInput`](../core/package-manager.ts.md#DefaultPackageManager.getSourceMatchKeyForInput), [`remove`](../core/package-manager.ts.md#DefaultPackageManager.remove), [`normalizePackageSourceForSettings`](../core/package-manager.ts.md#DefaultPackageManager.normalizePackageSourceForSettings), [`installParsedSource`](../core/package-manager.ts.md#DefaultPackageManager.installParsedSource), [`getAutocompleteSourceTag`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.getAutocompleteSourceTag), [`removeGit`](../core/package-manager.ts.md#DefaultPackageManager.removeGit), [`getCompactPackageSourceLabel`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.getCompactPackageSourceLabel), [`parseGenericGitUrl`](git.ts.md#parseGenericGitUrl), [`refreshTemporaryGitSource`](../core/package-manager.ts.md#DefaultPackageManager.refreshTemporaryGitSource), [`ParsedSource`](../core/package-manager.ts.md#ParsedSource), [`GitUpdateTarget`](../core/package-manager.ts.md#GitUpdateTarget)

## Functions
- `captureGitContext(cwd: string)` — [`L261`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L261)
- `findGitPaths(cwd: string)` — [`L207`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L207) — Find git metadata paths by walking up from cwd.
- `gitContextsEqual(a: GitContext, b: GitContext)` — [`L247`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L247)
- `parseGenericGitUrl(url: string)` — [`L79`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L79)
- `parseGitUrl(source: string)` — [`L137`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L137) — Parse git source into a GitSource.
- `runGit(cwd: string, args: string[])` — [`L251`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L251)
- `splitRef(url: string)` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L24)

## Module values
- `ref` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L24)
- `repo` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/git.ts#L24)


---
title: 'Module: packages/coding-agent/src/core/footer-data-provider.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/footer-data-provider.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`footer-data-provider.ts`/
symbols:
  FooterDataProvider.setupGitWatcher: FooterDataProvider#setupGitWatcher().
  FooterDataProvider.scheduleRefresh: FooterDataProvider#scheduleRefresh().
  FooterDataProvider.setCwd: FooterDataProvider#setCwd().
  FooterDataProvider.-constructor: FooterDataProvider#`<constructor>`().
  FooterDataProvider.dispose: FooterDataProvider#dispose().
  FooterDataProvider.clearGitWatchers: FooterDataProvider#clearGitWatchers().
  FooterDataProvider.refreshGitBranchAsync: FooterDataProvider#refreshGitBranchAsync().
  FooterDataProvider.getGitBranch: FooterDataProvider#getGitBranch().
  FooterDataProvider.gitPaths: FooterDataProvider#gitPaths.
  ReadonlyFooterDataProvider: ReadonlyFooterDataProvider#
  FooterDataProvider.resolveGitBranchSync: FooterDataProvider#resolveGitBranchSync().
  FooterDataProvider.resolveGitBranchAsync: FooterDataProvider#resolveGitBranchAsync().
  FooterDataProvider.scheduleGitWatcherRetry: FooterDataProvider#scheduleGitWatcherRetry().
  FooterDataProvider.refreshTimer: FooterDataProvider#refreshTimer.
  FooterDataProvider.cachedBranch: FooterDataProvider#cachedBranch.
  FooterDataProvider.handleGitWatcherError: FooterDataProvider#handleGitWatcherError().
  FooterDataProvider.onBranchChange: FooterDataProvider#onBranchChange().
  FooterDataProvider.gitWatcherRetryTimer: FooterDataProvider#gitWatcherRetryTimer.
  FooterDataProvider.disposed: FooterDataProvider#disposed.
  FooterDataProvider: FooterDataProvider#
  FooterDataProvider.notifyBranchChange: FooterDataProvider#notifyBranchChange().
  FooterDataProvider.extensionStatuses: FooterDataProvider#extensionStatuses.
  FooterDataProvider.headWatcher: FooterDataProvider#headWatcher.
  FooterDataProvider.reftableWatcher: FooterDataProvider#reftableWatcher.
  FooterDataProvider.reftableTablesListWatcher: FooterDataProvider#reftableTablesListWatcher.
  FooterDataProvider.reftableTablesListPath: FooterDataProvider#reftableTablesListPath.
  FooterDataProvider.branchChangeCallbacks: FooterDataProvider#branchChangeCallbacks.
  FooterDataProvider.refreshInFlight: FooterDataProvider#refreshInFlight.
  FooterDataProvider.refreshPending: FooterDataProvider#refreshPending.
  FooterDataProvider.setExtensionStatus: FooterDataProvider#setExtensionStatus().
  FooterDataProvider.clearExtensionStatuses: FooterDataProvider#clearExtensionStatuses().
  FooterDataProvider.setAvailableProviderCount: FooterDataProvider#setAvailableProviderCount().
  FooterDataProvider.cwd: FooterDataProvider#cwd.
  FooterDataProvider.getExtensionStatuses: FooterDataProvider#getExtensionStatuses().
  FooterDataProvider.getAvailableProviderCount: FooterDataProvider#getAvailableProviderCount().
  FooterDataProvider.availableProviderCount: FooterDataProvider#availableProviderCount.
  resolveBranchWithGitSync: resolveBranchWithGitSync().
  resolveBranchWithGitAsync: resolveBranchWithGitAsync().
  FooterDataProvider.WATCH_DEBOUNCE_MS: FooterDataProvider#WATCH_DEBOUNCE_MS.
---
# Module: [`packages/coding-agent/src/core/footer-data-provider.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts)

## Classes
### `FooterDataProvider`
- def: [`packages/coding-agent/src/core/footer-data-provider.ts:44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L44)
- doc: Provides git branch and extension statuses - data not otherwise accessible to extensions.
- signature: `class FooterDataProvider`
- members:
  - `<constructor>(cwd: string)` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L63) — Provides git branch and extension statuses - data not otherwise accessible to extensions.
  - `clearExtensionStatuses(method)` — [`L98`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L98) — Internal: clear extension statuses
  - `clearGitWatchers(method)` — [`L212`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L212)
  - `dispose(method)` — [`L130`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L130) — Internal: cleanup
  - `getAvailableProviderCount(method)` — [`L103`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L103) — Number of unique providers with available models (for footer display)
  - `getExtensionStatuses(method)` — [`L78`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L78) — Extension status texts set via ctx.ui.setStatus()
  - `getGitBranch(method)` — [`L70`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L70) — Current git branch, null if not in repo, "detached" if detached HEAD
  - `handleGitWatcherError(method)` — [`L240`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L240)
  - `notifyBranchChange(method)` — [`L140`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L140)
  - `onBranchChange(method)` — [`L83`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L83) — Subscribe to git branch changes. Returns unsubscribe function.
  - `refreshGitBranchAsync(method)` — [`L156`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L156)
  - `resolveGitBranchAsync(method)` — [`L196`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L196)
  - `resolveGitBranchSync(method)` — [`L182`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L182)
  - `scheduleGitWatcherRetry(method)` — [`L229`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L229)
  - `scheduleRefresh(method)` — [`L144`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L144)
  - `setAvailableProviderCount(method)` — [`L108`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L108) — Internal: update available provider count
  - `setCwd(method)` — [`L112`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L112)
  - `setExtensionStatus(method)` — [`L89`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L89) — Internal: set extension status
  - `setupGitWatcher(method)` — [`L245`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L245)
  - `WATCH_DEBOUNCE_MS` — [`L46`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L46)
  - `availableProviderCount` — [`L56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L56)
  - `branchChangeCallbacks` — [`L55`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L55)
  - `cachedBranch` — [`L49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L49)
  - `cwd` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L45)
  - `disposed` — [`L61`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L61)
  - `extensionStatuses` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L48)
  - `gitPaths` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L50)
  - `gitWatcherRetryTimer` — [`L58`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L58)
  - `headWatcher` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L51)
  - `refreshInFlight` — [`L59`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L59)
  - `refreshPending` — [`L60`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L60)
  - `refreshTimer` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L57)
  - `reftableTablesListPath` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L54)
  - `reftableTablesListWatcher` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L53)
  - `reftableWatcher` — [`L52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L52)
- uses (calls/refs, reference-scoped): [`closeWatcher`](../utils/fs-watch.ts.md#closeWatcher), [`watchWithErrorHandler`](../utils/fs-watch.ts.md#watchWithErrorHandler), [`findGitPaths`](../utils/git.ts.md#findGitPaths), [`GitPaths`](../utils/git.ts.md#GitPaths), [`headPath`](../utils/git.ts.md#GitPaths.typeLiteral116.headPath), [`FS_WATCH_RETRY_DELAY_MS`](../utils/fs-watch.ts.md#FS_WATCH_RETRY_DELAY_MS), [`repoDir`](../utils/git.ts.md#GitPaths.typeLiteral116.repoDir), [`commonGitDir`](../utils/git.ts.md#GitPaths.typeLiteral116.commonGitDir), [`resolveBranchWithGitAsync`](footer-data-provider.ts.md#resolveBranchWithGitAsync), [`resolveBranchWithGitSync`](footer-data-provider.ts.md#resolveBranchWithGitSync)
- used by: [`interactive-mode.ts`](../modes/interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`<constructor>`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.-constructor), [`init`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.init), [`resetExtensionUI`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.resetExtensionUI), [`applyRuntimeSettings`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.applyRuntimeSettings), [`stop`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.stop), [`updateAvailableProviderCount`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.updateAvailableProviderCount), [`setExtensionStatus`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.setExtensionStatus), [`ReadonlyFooterDataProvider`](footer-data-provider.ts.md#ReadonlyFooterDataProvider), [`footerDataProvider`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.footerDataProvider)  (3 test-only)

### `ReadonlyFooterDataProvider`
- def: [`packages/coding-agent/src/core/footer-data-provider.ts:308`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L308)
- doc: Read-only view for extensions - excludes setExtensionStatus, setAvailableProviderCount and dispose
- signature: `type ReadonlyFooterDataProvider`
- uses (calls/refs, reference-scoped): [`FooterDataProvider`](footer-data-provider.ts.md#FooterDataProvider)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../modes/interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`setExtensionFooter`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.setExtensionFooter), [`setFooter`](extensions/types.ts.md#ExtensionUIContext.setFooter), [`footer.ts`](../modes/interactive/components/footer.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-footer.ts), [`<constructor>`](../modes/interactive/components/footer.ts.md#FooterComponent.-constructor)  (2 test-only)

## Functions
- `resolveBranchWithGitAsync(repoDir: string)` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L19) — Ask git for the current branch asynchronously. Returns null on detached HEAD or if git is unavailable.
- `resolveBranchWithGitSync(repoDir: string)` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/footer-data-provider.ts#L8) — Ask git for the current branch. Returns null on detached HEAD or if git is unavailable.


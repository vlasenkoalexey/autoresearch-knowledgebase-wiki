---
title: 'Module: packages/coding-agent/src/modes/shared/startup-notices.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/shared/startup-notices.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/shared/`startup-notices.ts`/
symbols:
  checkForPackageUpdates.options-typeLiteral7.settingsManager: checkForPackageUpdates().(options)typeLiteral7:settingsManager.
  gatherStartupNotices: gatherStartupNotices().
  formatUpdateAvailableNotice: formatUpdateAvailableNotice().
  formatPackageUpdateNotice: formatPackageUpdateNotice().
  formatTmuxWarningNotice: formatTmuxWarningNotice().
  StartupNotices: StartupNotices#
  StartupNoticeCheckOptions.settingsManager: StartupNoticeCheckOptions#settingsManager.
  checkForPackageUpdates: checkForPackageUpdates().
  checkTmuxKeyboardSetup: checkTmuxKeyboardSetup().
  StartupNotices.newVersion: StartupNotices#newVersion.
  StartupNotices.packageUpdates: StartupNotices#packageUpdates.
  StartupNotices.tmuxWarning: StartupNotices#tmuxWarning.
  StartupNoticeCheckOptions.version: StartupNoticeCheckOptions#version.
  checkForPackageUpdates.options-typeLiteral7.cwd: checkForPackageUpdates().(options)typeLiteral7:cwd.
  checkForPackageUpdates.options-typeLiteral7.agentDir: checkForPackageUpdates().(options)typeLiteral7:agentDir.
  StartupNoticeCheckOptions: StartupNoticeCheckOptions#
  StartupNoticeCheckOptions.cwd: StartupNoticeCheckOptions#cwd.
  StartupNoticeCheckOptions.agentDir: StartupNoticeCheckOptions#agentDir.
---
# Module: [`packages/coding-agent/src/modes/shared/startup-notices.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts)

## Classes
### `StartupNoticeCheckOptions`
- def: [`packages/coding-agent/src/modes/shared/startup-notices.ts:25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L25)
- signature: `interface StartupNoticeCheckOptions`
- members:
  - `agentDir` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L28)
  - `cwd` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L27)
  - `settingsManager` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L29)
  - `version` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L26)
- uses (calls/refs, reference-scoped): [`SettingsManager`](../../core/settings-manager.ts.md#SettingsManager)
- used by: [`loadStartupNotices`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.loadStartupNotices), [`gatherStartupNotices`](startup-notices.ts.md#gatherStartupNotices)

### `StartupNotices`
- def: [`packages/coding-agent/src/modes/shared/startup-notices.ts:16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L16)
- signature: `interface StartupNotices`
- members:
  - `newVersion` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L18) — Newer Prime Agent version available, if any.
  - `packageUpdates` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L20) — Display names of extensions with available updates.
  - `tmuxWarning` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L22) — tmux keyboard setup warning, if the current tmux config is suboptimal.
- used by: [`agents-view-mode.ts`](../agents-view/agents-view-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agents-view-agents-view-mode.ts), [`renderStartupNotices`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.renderStartupNotices), [`gatherStartupNotices`](startup-notices.ts.md#gatherStartupNotices), [`startupNotices`](../agents-view/agents-view-mode.ts.md#AgentsViewPersistentState.typeLiteral18.startupNotices), [`startupNoticesPromise`](../agents-view/agents-view-mode.ts.md#AgentsViewPersistentState.typeLiteral18.startupNoticesPromise)

## Functions
- `checkForPackageUpdates(options: { cwd: string; agentDir: string; settingsManager: SettingsManager; })` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L42)
- `checkTmuxKeyboardSetup()` — [`L64`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L64)
- `formatPackageUpdateNotice(packages: string[])` — [`L118`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L118)
- `formatTmuxWarningNotice(message: string)` — [`L126`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L126)
- `formatUpdateAvailableNotice(newVersion: string)` — [`L111`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L111)
- `gatherStartupNotices(options: StartupNoticeCheckOptions)` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L33) — Run every startup check in parallel and collect the results.

## Module values
- `agentDir` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L44)
- `cwd` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L43)
- `settingsManager` — [`L45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/shared/startup-notices.ts#L45)


---
title: 'Module: packages/coding-agent/src/cli/config-selector.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/config-selector.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`config-selector.ts`/
symbols:
  selectConfig: selectConfig().
  ConfigSelectorOptions.settingsManager: ConfigSelectorOptions#settingsManager.
  ConfigSelectorOptions.resolvedPaths: ConfigSelectorOptions#resolvedPaths.
  ConfigSelectorOptions.cwd: ConfigSelectorOptions#cwd.
  ConfigSelectorOptions.agentDir: ConfigSelectorOptions#agentDir.
  ConfigSelectorOptions: ConfigSelectorOptions#
---
# Module: [`packages/coding-agent/src/cli/config-selector.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/config-selector.ts)

## Classes
### `ConfigSelectorOptions`
- def: [`packages/coding-agent/src/cli/config-selector.ts:11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/config-selector.ts#L11)
- signature: `interface ConfigSelectorOptions`
- members:
  - `agentDir` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/config-selector.ts#L15)
  - `cwd` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/config-selector.ts#L14)
  - `resolvedPaths` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/config-selector.ts#L12)
  - `settingsManager` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/config-selector.ts#L13)
- uses (calls/refs, reference-scoped): [`SettingsManager`](../core/settings-manager.ts.md#SettingsManager), [`ResolvedPaths`](../core/package-manager.ts.md#ResolvedPaths)
- used by: [`selectConfig`](config-selector.ts.md#selectConfig), [`handleConfigCommand`](../package-manager-cli.ts.md#handleConfigCommand)

## Functions
- `selectConfig(options: ConfigSelectorOptions)` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/config-selector.ts#L19) — Show TUI config selector and return when closed


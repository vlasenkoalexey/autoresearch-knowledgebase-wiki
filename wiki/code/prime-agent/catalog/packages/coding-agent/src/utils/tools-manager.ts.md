---
title: 'Module: packages/coding-agent/src/utils/tools-manager.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/utils/tools-manager.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/utils/`tools-manager.ts`/
symbols:
  downloadTool: downloadTool().
  ensureToolWithStatus: ensureToolWithStatus().
  formatMissingRipgrepMessage: formatMissingRipgrepMessage().
  TOOLS: TOOLS.
  getToolPath: getToolPath().
  ensureTool: ensureTool().
  ToolConfig.name: ToolConfig#name.
  TOOLS_DIR: TOOLS_DIR.
  ToolConfig.binaryName: ToolConfig#binaryName.
  ToolEnsureResult: ToolEnsureResult#
  getLatestVersion: getLatestVersion().
  ToolUnavailableResult.reason: ToolUnavailableResult#reason.
  commandWorks: commandWorks().
  ToolUnavailableResult: ToolUnavailableResult#
  ManagedTool: ManagedTool#
  ToolConfig.repo: ToolConfig#repo.
  ToolConfig.getAssetName: ToolConfig#getAssetName.
  downloadFile: downloadFile().
  getRipgrepInstallHint: getRipgrepInstallHint().
  ToolUnavailableResult.status: ToolUnavailableResult#status.
  ToolUnavailableResult.platform: ToolUnavailableResult#platform.
  ToolConfig.tagPrefix: ToolConfig#tagPrefix.
  UnsupportedToolPlatformError: UnsupportedToolPlatformError#
  RIPGREP_INSTALL_URL: RIPGREP_INSTALL_URL.
  ToolAvailableResult.status: ToolAvailableResult#status.
  ToolUnavailableResult.architecture: ToolUnavailableResult#architecture.
  ToolConfig.systemBinaryNames: ToolConfig#systemBinaryNames.
  NETWORK_TIMEOUT_MS: NETWORK_TIMEOUT_MS.
  DOWNLOAD_TIMEOUT_MS: DOWNLOAD_TIMEOUT_MS.
  COMMAND_TIMEOUT_MS: COMMAND_TIMEOUT_MS.
  ToolUnavailableReason: ToolUnavailableReason#
  ToolAvailableResult: ToolAvailableResult#
  ToolAvailableResult.path: ToolAvailableResult#path.
  ToolUnavailableResult.detail: ToolUnavailableResult#detail.
  isOfflineModeEnabled: isOfflineModeEnabled().
  ToolConfig: ToolConfig#
  findBinaryRecursively: findBinaryRecursively().
  TERMUX_PACKAGES: TERMUX_PACKAGES.
---
# Module: [`packages/coding-agent/src/utils/tools-manager.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts)

## Classes
### `ManagedTool`
- def: [`packages/coding-agent/src/utils/tools-manager.ts:17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L17)
- signature: `type ManagedTool`
- used by: [`downloadTool`](tools-manager.ts.md#downloadTool), [`ensureToolWithStatus`](tools-manager.ts.md#ensureToolWithStatus), [`getToolPath`](tools-manager.ts.md#getToolPath), [`ensureTool`](tools-manager.ts.md#ensureTool)

### `ToolAvailableResult`
- def: [`packages/coding-agent/src/utils/tools-manager.ts:21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L21)
- signature: `interface ToolAvailableResult`
- members:
  - `path` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L23)
  - `status` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L22)
- used by: [`init`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.init), [`ensureTool`](tools-manager.ts.md#ensureTool), [`ToolEnsureResult`](tools-manager.ts.md#ToolEnsureResult)

### `ToolConfig`
- def: [`packages/coding-agent/src/utils/tools-manager.ts:42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L42)
- signature: `interface ToolConfig`
- members:
  - `binaryName` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L45)
  - `getAssetName` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L48)
  - `name` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L43)
  - `repo` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L44)
  - `systemBinaryNames` — [`L46`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L46)
  - `tagPrefix` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L47)
- used by: [`downloadTool`](tools-manager.ts.md#downloadTool), [`ensureToolWithStatus`](tools-manager.ts.md#ensureToolWithStatus), [`TOOLS`](tools-manager.ts.md#TOOLS), [`getToolPath`](tools-manager.ts.md#getToolPath)

### `ToolEnsureResult`
- def: [`packages/coding-agent/src/utils/tools-manager.ts:34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L34)
- signature: `type ToolEnsureResult`
- uses (calls/refs, reference-scoped): [`ToolUnavailableResult`](tools-manager.ts.md#ToolUnavailableResult), [`ToolAvailableResult`](tools-manager.ts.md#ToolAvailableResult)
- used by: [`ensureToolWithStatus`](tools-manager.ts.md#ensureToolWithStatus)

### `ToolUnavailableReason`
- def: [`packages/coding-agent/src/utils/tools-manager.ts:19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L19)
- signature: `type ToolUnavailableReason`
- used by: [`reason`](tools-manager.ts.md#ToolUnavailableResult.reason)

### `ToolUnavailableResult`
- def: [`packages/coding-agent/src/utils/tools-manager.ts:26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L26)
- signature: `interface ToolUnavailableResult`
- members:
  - `architecture` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L30)
  - `detail` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L31)
  - `platform` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L29)
  - `reason` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L28)
  - `status` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L27)
- uses (calls/refs, reference-scoped): [`ToolUnavailableReason`](tools-manager.ts.md#ToolUnavailableReason)
- used by: [`init`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.init), [`formatMissingRipgrepMessage`](tools-manager.ts.md#formatMissingRipgrepMessage), [`ensureTool`](tools-manager.ts.md#ensureTool), [`ToolEnsureResult`](tools-manager.ts.md#ToolEnsureResult)  (2 test-only)

### `UnsupportedToolPlatformError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/utils/tools-manager.ts:188`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L188)
- signature: `class UnsupportedToolPlatformError`
- used by: [`downloadTool`](tools-manager.ts.md#downloadTool), [`ensureToolWithStatus`](tools-manager.ts.md#ensureToolWithStatus)

## Functions
- `commandWorks(cmd: string)` — [`L101`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L101)
- `downloadFile(url: string, dest: string)` — [`L148`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L148)
- `downloadTool(tool: ManagedTool)` — [`L190`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L190)
- `ensureTool(tool: ManagedTool, silent?: boolean)` — [`L381`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L381)
- `ensureToolWithStatus(tool: ManagedTool, silent?: boolean)` — [`L323`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L323)
- `findBinaryRecursively(rootDir: string, binaryFileName: string)` — [`L165`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L165)
- `formatMissingRipgrepMessage(result: ToolUnavailableResult)` — [`L294`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L294)
- `getLatestVersion(repo: string)` — [`L133`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L133)
- `getRipgrepInstallHint(platformName: string)` — [`L279`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L279)
- `getToolPath(tool: ManagedTool)` — [`L111`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L111)
- `isOfflineModeEnabled()` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L36)

## Module values
- `COMMAND_TIMEOUT_MS` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L14)
- `DOWNLOAD_TIMEOUT_MS` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L13)
- `NETWORK_TIMEOUT_MS` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L12)
- `RIPGREP_INSTALL_URL` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L15)
- `TERMUX_PACKAGES` — [`L274`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L274)
- `TOOLS` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L51)
- `TOOLS_DIR` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/tools-manager.ts#L11)


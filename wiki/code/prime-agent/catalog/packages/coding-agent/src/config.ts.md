---
title: 'Module: packages/coding-agent/src/config.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/config.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/`config.ts`/
symbols:
  APP_NAME: APP_NAME.
  getAgentDir: getAgentDir().
  ENV_AGENT_DIR: ENV_AGENT_DIR.
  VERSION: VERSION.
  CONFIG_DIR_NAME: CONFIG_DIR_NAME.
  getSelfUpdateCommand: getSelfUpdateCommand().
  getBundledSkillsDir: getBundledSkillsDir().
  detectInstallMethod: detectInstallMethod().
  getPackageDir: getPackageDir().
  PACKAGE_NAME: PACKAGE_NAME.
  getSelfUpdateUnavailableInstruction: getSelfUpdateUnavailableInstruction().
  SELF_UPDATE_INTERACTIVE_CHILD_ENV: SELF_UPDATE_INTERACTIVE_CHILD_ENV.
  getSelfUpdateCommandForMethod: getSelfUpdateCommandForMethod().
  getDaemonUpdateRestartManifestPath: getDaemonUpdateRestartManifestPath().
  makeSelfUpdateCommandStep: makeSelfUpdateCommandStep().
  getSessionsDir: getSessionsDir().
  getDaemonLogPath: getDaemonLogPath().
  appendRotatingLog: appendRotatingLog().
  getUpdateInstruction: getUpdateInstruction().
  SelfUpdateCommandStep.display: SelfUpdateCommandStep#display.
  ENV_SESSION_DIR: ENV_SESSION_DIR.
  getCronJobsPath: getCronJobsPath().
  isManagedByGlobalPackageManager: isManagedByGlobalPackageManager().
  expandTildePath: expandTildePath().
  makeSelfUpdateCommand.options-typeLiteral0.uninstallAfterInstall: makeSelfUpdateCommand().(options)typeLiteral0:uninstallAfterInstall.
  piConfigName: piConfigName.
  getSessionDirEnvOverride: getSessionDirEnvOverride().
  isBunBinary: isBunBinary.
  APP_TITLE: APP_TITLE.
  getDebugLogPath: getDebugLogPath().
  getAgentTracesLogPath: getAgentTracesLogPath().
  pkg: pkg.
  SelfUpdateCommand: SelfUpdateCommand#
  getGlobalPackageRoots: getGlobalPackageRoots().
  ENV_LEGACY_SESSION_DIR: ENV_LEGACY_SESSION_DIR.
  getLogsDir: getLogsDir().
  getBinDir: getBinDir().
  getThemesDir: getThemesDir().
  getDocsPath: getDocsPath().
  getCustomThemesDir: getCustomThemesDir().
  getAgentLogPath: getAgentLogPath().
  getLegacyDaemonUpdateRestartManifestPath: getLegacyDaemonUpdateRestartManifestPath().
  getExportTemplateDir: getExportTemplateDir().
  makeSelfUpdateCommand: makeSelfUpdateCommand().
  getClientErrorLogPath: getClientErrorLogPath().
  SELF_UPDATE_NOT_ATTEMPTED_EXIT_CODE: SELF_UPDATE_NOT_ATTEMPTED_EXIT_CODE.
  readCommandOutput.options-typeLiteral55.requireSuccess: readCommandOutput().(options)typeLiteral55:requireSuccess.
  getInteractiveAssetsDir: getInteractiveAssetsDir().
  __dirname: __dirname.
  getDefaultUpdatePackageName: getDefaultUpdatePackageName().
  getChangelogPath: getChangelogPath().
  envPrefix: envPrefix.
  getAuthPath: getAuthPath().
  SelfUpdateCommandStep: SelfUpdateCommandStep#
  readCommandOutput: readCommandOutput().
  getInferredNpmInstall: getInferredNpmInstall().
  isSelfUpdatePathWritable: isSelfUpdatePathWritable().
  getBundledInteractiveAssetPath: getBundledInteractiveAssetPath().
  getShareViewerUrl: getShareViewerUrl().
  InstallMethod: InstallMethod#
  isHomebrewInstall: isHomebrewInstall().
  getPackageJsonPath: getPackageJsonPath().
  SelfUpdateCommandStep.command: SelfUpdateCommandStep#command.
  SelfUpdateCommandStep.args: SelfUpdateCommandStep#args.
  SelfUpdateCommand.steps: SelfUpdateCommand#steps.
  getReadmePath: getReadmePath().
  getExamplesPath: getExamplesPath().
  getModelsPath: getModelsPath().
  getSettingsPath: getSettingsPath().
  getToolsDir: getToolsDir().
  getPromptsDir: getPromptsDir().
  isDirectPackageArtifactSpec: isDirectPackageArtifactSpec().
  normalizeExistingPathForComparison: normalizeExistingPathForComparison().
  PackageJson.piConfig: PackageJson#piConfig.
  __filename: __filename.
  isBunRuntime: isBunRuntime.
  PackageJson: PackageJson#
  PackageJson.name: PackageJson#name.
  PackageJson.version: PackageJson#version.
  PackageJson.piConfig.typeLiteral168.name: PackageJson#piConfig.typeLiteral168:name.
  PackageJson.piConfig.typeLiteral168.configDir: PackageJson#piConfig.typeLiteral168:configDir.
  DEFAULT_SHARE_VIEWER_URL: DEFAULT_SHARE_VIEWER_URL.
  MAX_LOG_BYTES: MAX_LOG_BYTES.
---
# Module: [`packages/coding-agent/src/config.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts)

## Classes
### `InstallMethod`
- def: [`packages/coding-agent/src/config.ts:44`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L44)
- signature: `type InstallMethod`
- used by: [`detectInstallMethod`](config.ts.md#detectInstallMethod), [`getSelfUpdateCommandForMethod`](config.ts.md#getSelfUpdateCommandForMethod), [`isManagedByGlobalPackageManager`](config.ts.md#isManagedByGlobalPackageManager), [`getGlobalPackageRoots`](config.ts.md#getGlobalPackageRoots)

### `PackageJson`
- def: [`packages/coding-agent/src/config.ts:487`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L487)
- signature: `interface PackageJson`
- members:
  - `configDir` — [`L492`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L492)
  - `name` — [`L488`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L488)
  - `name` — [`L491`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L491)
  - `piConfig` — [`L490`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L490)
  - `version` — [`L489`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L489)
- used by: [`VERSION`](config.ts.md#VERSION), [`CONFIG_DIR_NAME`](config.ts.md#CONFIG_DIR_NAME), [`PACKAGE_NAME`](config.ts.md#PACKAGE_NAME), [`piConfigName`](config.ts.md#piConfigName), [`pkg`](config.ts.md#pkg)

### `SelfUpdateCommand`
- def: [`packages/coding-agent/src/config.ts:52`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L52)
- signature: `interface SelfUpdateCommand`
- members:
  - `steps` — [`L53`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L53)
- uses (calls/refs, reference-scoped): [`SelfUpdateCommandStep`](config.ts.md#SelfUpdateCommandStep)
- used by: [`package-manager-cli.ts`](package-manager-cli.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-package-manager-cli.ts), [`getSelfUpdateCommand`](config.ts.md#getSelfUpdateCommand), [`getSelfUpdateCommandForMethod`](config.ts.md#getSelfUpdateCommandForMethod), [`runSelfUpdate`](package-manager-cli.ts.md#runSelfUpdate), [`uninstallAfterInstall`](config.ts.md#makeSelfUpdateCommand.options-typeLiteral0.uninstallAfterInstall), [`printSelfUpdateFallback`](package-manager-cli.ts.md#printSelfUpdateFallback)

### `SelfUpdateCommandStep`
- def: [`packages/coding-agent/src/config.ts:46`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L46)
- signature: `interface SelfUpdateCommandStep`
- members:
  - `args` — [`L48`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L48)
  - `command` — [`L47`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L47)
  - `display` — [`L49`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L49)
- used by: [`getSelfUpdateUnavailableInstruction`](config.ts.md#getSelfUpdateUnavailableInstruction), [`runSelfUpdate`](package-manager-cli.ts.md#runSelfUpdate), [`makeSelfUpdateCommandStep`](config.ts.md#makeSelfUpdateCommandStep), [`getUpdateInstruction`](config.ts.md#getUpdateInstruction), [`uninstallAfterInstall`](config.ts.md#makeSelfUpdateCommand.options-typeLiteral0.uninstallAfterInstall), [`SelfUpdateCommand`](config.ts.md#SelfUpdateCommand), [`makeSelfUpdateCommand`](config.ts.md#makeSelfUpdateCommand), [`printSelfUpdateFallback`](package-manager-cli.ts.md#printSelfUpdateFallback)  (1 test-only)

## Functions
- `appendRotatingLog(logPath: string, message: string, maxBytes?: number)` — [`L594`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L594) — Append a line to a log file, keeping its size bounded with a single-generation
- `detectInstallMethod()` — [`L84`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L84)
- `expandTildePath(path: string)` — [`L515`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L515)
- `getAgentDir()` — [`L534`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L534) — Get the agent config directory (e.g., ~/.prime/agent/)
- `getAgentLogPath()` — [`L562`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L562) — Shared structured (JSON lines) log for client, daemon, and provider diagnostics.
- `getAgentTracesLogPath()` — [`L557`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L557)
- `getAuthPath()` — [`L618`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L618) — Get path to auth.json
- `getBinDir()` — [`L638`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L638) — Get path to managed binaries directory (fd, rg)
- `getBundledInteractiveAssetPath(name: string)` — [`L461`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L461) — Get path to a bundled interactive asset
- `getBundledSkillsDir()` — [`L471`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L471) — Get the directory containing built-in skills shipped with the package.
- `getChangelogPath()` — [`L441`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L441) — Get path to CHANGELOG.md
- `getClientErrorLogPath()` — [`L553`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L553) — Log file capturing client-side agent-open failures.
- `getCronJobsPath(agentDir?: string)` — [`L628`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L628) — Get path to cron jobs store
- `getCustomThemesDir()` — [`L543`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L543) — Get path to user's custom themes directory
- `getDaemonLogPath(socketPath: string)` — [`L571`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L571) — Log file for a daemon. The basename keeps it readable; a hash of the full
- `getDaemonUpdateRestartManifestPath(socketPath: string, agentDir?: string)` — [`L576`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L576)
- `getDebugLogPath()` — [`L662`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L662) — Get path to debug log file
- `getDefaultUpdatePackageName(installedPackageName: string, updateSpec: string)` — [`L145`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L145)
- `getDocsPath()` — [`L431`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L431) — Get path to docs directory
- `getExamplesPath()` — [`L436`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L436) — Get path to examples directory
- `getExportTemplateDir()` — [`L411`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L411) — Get path to HTML export template directory (shipped with package)
- `getGlobalPackageRoots(method: InstallMethod, _packageName: string, npmCommand?: string[] | undefined)` — [`L222`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L222)
- `getInferredNpmInstall()` — [`L115`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L115)
- `getInteractiveAssetsDir()` — [`L451`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L451) — Get path to built-in interactive assets directory.
- `getLegacyDaemonUpdateRestartManifestPath(agentDir?: string)` — [`L582`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L582)
- `getLogsDir()` — [`L548`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L548) — Directory where daemon and client diagnostic logs are written (e.g. ~/.prime/agent/logs/).
- `getModelsPath()` — [`L613`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L613) — Get path to models.json
- `getPackageDir()` — [`L364`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L364) — Get the base directory for resolving package assets (themes, package.json, README.md, CHANGELOG.md).
- `getPackageJsonPath()` — [`L421`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L421) — Get path to package.json
- `getPromptsDir()` — [`L643`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L643) — Get path to prompt templates directory
- `getReadmePath()` — [`L426`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L426) — Get path to README.md
- `getSelfUpdateCommand(packageName: string, npmCommand?: string[] | undefined, updateSpec?: string, updatePackageName?: string)` — [`L308`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L308)
- `getSelfUpdateCommandForMethod(method: InstallMethod, installedPackageName: string, updateSpec?: string, npmCommand?: string[] | undefined, updatePackageName?: string)` — [`L152`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L152)
- `getSelfUpdateUnavailableInstruction(packageName: string, npmCommand?: string[] | undefined, updateSpec?: string, updatePackageName?: string)` — [`L322`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L322)
- `getSessionDirEnvOverride()` — [`L656`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L656)
- `getSessionsDir(agentDir?: string)` — [`L648`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L648) — Get path to sessions directory
- `getSettingsPath()` — [`L623`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L623) — Get path to settings.json
- `getShareViewerUrl(gistId: string)` — [`L524`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L524) — Get the share viewer URL for a gist ID
- `getThemesDir()` — [`L395`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L395) — Get path to built-in themes directory (shipped with package)
- `getToolsDir()` — [`L633`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L633) — Get path to tools directory
- `getUpdateInstruction(packageName: string)` — [`L345`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L345)
- `isDirectPackageArtifactSpec(updateSpec: string)` — [`L134`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L134)
- `isHomebrewInstall()` — [`L110`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L110)
- `isManagedByGlobalPackageManager(method: InstallMethod, packageName: string, npmCommand?: string[] | undefined)` — [`L294`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L294)
- `isSelfUpdatePathWritable()` — [`L283`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L283)
- `makeSelfUpdateCommand(installStep: SelfUpdateCommandStep, uninstallStep?: SelfUpdateCommandStep | undefined, options?: { uninstallAfterInstall?: boolean | undefined; })` — [`L56`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L56)
- `makeSelfUpdateCommandStep(command: string, args: string[])` — [`L76`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L76)
- `normalizeExistingPathForComparison(path: string)` — [`L266`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L266)
- `readCommandOutput(command: string, args: string[], options?: { requireSuccess?: boolean | undefined; })` — [`L204`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L204)

## Module values
- `APP_NAME` — [`L505`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L505)
- `APP_TITLE` — [`L506`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L506)
- `CONFIG_DIR_NAME` — [`L507`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L507)
- `DEFAULT_SHARE_VIEWER_URL` — [`L521`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L521)
- `ENV_AGENT_DIR` — [`L511`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L511)
- `ENV_LEGACY_SESSION_DIR` — [`L513`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L513)
- `ENV_SESSION_DIR` — [`L512`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L512)
- `MAX_LOG_BYTES` — [`L586`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L586)
- `PACKAGE_NAME` — [`L504`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L504)
- `SELF_UPDATE_INTERACTIVE_CHILD_ENV` — [`L37`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L37)
- `SELF_UPDATE_NOT_ATTEMPTED_EXIT_CODE` — [`L38`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L38)
- `VERSION` — [`L508`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L508)
- `__dirname` — [`L25`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L25)
- `__filename` — [`L24`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L24)
- `envPrefix` — [`L499`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L499)
- `isBunBinary` — [`L31`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L31) — Detect if we're running as a Bun compiled binary.
- `isBunRuntime` — [`L35`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L35) — Detect if Bun is the runtime (compiled binary or bun run)
- `piConfigName` — [`L498`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L498)
- `pkg` — [`L496`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L496)
- `requireSuccess` — [`L207`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L207)
- `uninstallAfterInstall` — [`L59`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/config.ts#L59)


---
title: 'Module: packages/coding-agent/src/package-manager-cli.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/package-manager-cli.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/`package-manager-cli.ts`/
symbols:
  handlePackageCommand: handlePackageCommand().
  runDaemonUpdateRestartCoordinator.options-typeLiteral607.originActiveSessionId: runDaemonUpdateRestartCoordinator().(options)typeLiteral607:originActiveSessionId.
  restoreDaemonUpdateRestartSession: restoreDaemonUpdateRestartSession().
  parseDaemonUpdateRestartSession: parseDaemonUpdateRestartSession().
  restoreDaemonUpdateRestart: restoreDaemonUpdateRestart().
  prepareConnectedDaemonUpdateRestart: prepareConnectedDaemonUpdateRestart().
  handleConfigCommand: handleConfigCommand().
  prepareDaemonUpdateRestart: prepareDaemonUpdateRestart().
  validateReplacementDaemon: validateReplacementDaemon().
  getSelfUpdatePlan: getSelfUpdatePlan().
  isSessionActionRecoveryAction: isSessionActionRecoveryAction().
  parseDaemonUpdateRestartManifest: parseDaemonUpdateRestartManifest().
  UPDATE_SESSION_LOSS_COPY: UPDATE_SESSION_LOSS_COPY.
  runDaemonUpdateRestartCoordinator.options-typeLiteral607.socketPath: runDaemonUpdateRestartCoordinator().(options)typeLiteral607:socketPath.
  parsePackageCommand: parsePackageCommand().
  runSelfUpdate: runSelfUpdate().
  isRecord: isRecord().
  parseSessionActionRecoverySnapshot: parseSessionActionRecoverySnapshot().
  PackageCommandOptions.command: PackageCommandOptions#command.
  getPackageCommandUsage: getPackageCommandUsage().
  confirmDaemonSessionLossBeforeUpdate: confirmDaemonSessionLossBeforeUpdate().
  parseDaemonUpdateRestartRuntimeMetadata: parseDaemonUpdateRestartRuntimeMetadata().
  remapDaemonUpdateRestartRuntimeMetadata: remapDaemonUpdateRestartRuntimeMetadata().
  reportSettingsErrors: reportSettingsErrors().
  readPreparedDaemonUpdateRestartManifest: readPreparedDaemonUpdateRestartManifest().
  isMessageContentBlock: isMessageContentBlock().
  printPackageCommandHelp: printPackageCommandHelp().
  reportDaemonUpdateRestartStatus: reportDaemonUpdateRestartStatus().
  isImageContent: isImageContent().
  isQueuedAgentMessage: isQueuedAgentMessage().
  isCustomMessage: isCustomMessage().
  tryReadPreparedDaemonUpdateRestartManifest: tryReadPreparedDaemonUpdateRestartManifest().
  clearPreparedDaemonUpdateRestartManifest: clearPreparedDaemonUpdateRestartManifest().
  printSelfUpdateUnavailable: printSelfUpdateUnavailable().
  isUserMessage: isUserMessage().
  restoreNextTurnMessages: restoreNextTurnMessages().
  readOptionalString: readOptionalString().
  RestoreDaemonUpdateRestartResult: RestoreDaemonUpdateRestartResult#
  isSelfUpdateSource: isSelfUpdateSource().
  readBoolean: readBoolean().
  hasFixedDaemonSupervisorOwnerIdentity: hasFixedDaemonSupervisorOwnerIdentity().
  processIdentityFromDaemonHello: processIdentityFromDaemonHello().
  runDaemonUpdateRestartCoordinator.options-typeLiteral607.agentDir: runDaemonUpdateRestartCoordinator().(options)typeLiteral607:agentDir.
  resolveUpdateDaemonSocketPath: resolveUpdateDaemonSocketPath().
  printSelfUpdateFallback: printSelfUpdateFallback().
  setSelfUpdateNoChangeExitCode: setSelfUpdateNoChangeExitCode().
  daemonProbeMayHaveBusySessions: daemonProbeMayHaveBusySessions().
  readString: readString().
  readCustomMessages: readCustomMessages().
  hasRestorableDaemonUpdateRestart: hasRestorableDaemonUpdateRestart().
  readCreatedActiveSessionId: readCreatedActiveSessionId().
  formatUnknownError: formatUnknownError().
  runDaemonUpdateRestartCoordinator.options-typeLiteral607.statusPath: runDaemonUpdateRestartCoordinator().(options)typeLiteral607:statusPath.
  PackageCommand: PackageCommand#
  UpdateTarget: UpdateTarget#
  isStringEnum: isStringEnum().
  RestoreDaemonUpdateRestartResult.failures: RestoreDaemonUpdateRestartResult#failures.
  runDaemonUpdateRestartCoordinator: runDaemonUpdateRestartCoordinator().
  PackageCommandOptions.updateTarget: PackageCommandOptions#updateTarget.
  updateTargetIncludesSelf: updateTargetIncludesSelf().
  updateTargetIncludesExtensions: updateTargetIncludesExtensions().
  readOptionalStringRecord: readOptionalStringRecord().
  responseHasActiveDaemonSessions: responseHasActiveDaemonSessions().
  PackageCommandOptions.invalidOption: PackageCommandOptions#invalidOption.
  PackageCommandOptions.local: PackageCommandOptions#local.
  PackageCommandOptions.force: PackageCommandOptions#force.
  PackageCommandOptions.daemonSocketPath: PackageCommandOptions#daemonSocketPath.
  PackageCommandOptions.restartStatusPath: PackageCommandOptions#restartStatusPath.
  PackageCommandOptions.restartOriginActiveSessionId: PackageCommandOptions#restartOriginActiveSessionId.
  PackageCommandOptions.invalidArgument: PackageCommandOptions#invalidArgument.
  PackageCommandOptions.missingOptionValue: PackageCommandOptions#missingOptionValue.
  PackageCommandOptions.conflictingOptions: PackageCommandOptions#conflictingOptions.
  SelfUpdatePlan.installSpec: SelfUpdatePlan#installSpec.
  SelfUpdatePlan.packageName: SelfUpdatePlan#packageName.
  SelfUpdatePlan.targetVersion: SelfUpdatePlan#targetVersion.
  FixedDaemonSupervisorOwnerIdentity: FixedDaemonSupervisorOwnerIdentity#
  RestoreDaemonUpdateRestartSessionResult.restored: RestoreDaemonUpdateRestartSessionResult#restored.
  normalizedSocketPath: normalizedSocketPath().
  UPDATE_RESTART_PREDECESSOR_FENCE_TIMEOUT_MS: UPDATE_RESTART_PREDECESSOR_FENCE_TIMEOUT_MS.
  PackageCommandOptions: PackageCommandOptions#
  PackageCommandOptions.source: PackageCommandOptions#source.
  PackageCommandOptions.help: PackageCommandOptions#help.
  PackageCommandOptions.restartCoordinator: PackageCommandOptions#restartCoordinator.
  SelfUpdatePlan: SelfUpdatePlan#
  SelfUpdatePlan.shouldRun: SelfUpdatePlan#shouldRun.
  UPDATE_RESTART_CONTINUATION_PROMPT: UPDATE_RESTART_CONTINUATION_PROMPT.
  readNumber: readNumber().
  RestoreDaemonUpdateRestartSessionResult: RestoreDaemonUpdateRestartSessionResult#
  RestoreDaemonUpdateRestartSessionResult.resumed: RestoreDaemonUpdateRestartSessionResult#resumed.
  RestoreDaemonUpdateRestartSessionResult.failureMessage: RestoreDaemonUpdateRestartSessionResult#failureMessage.
  FixedDaemonSupervisorOwnerIdentity.supervisorGeneration: FixedDaemonSupervisorOwnerIdentity#supervisorGeneration.
  FixedDaemonSupervisorOwnerIdentity.supervisorOwnerToken: FixedDaemonSupervisorOwnerIdentity#supervisorOwnerToken.
  FixedDaemonSupervisorOwnerIdentity.supervisorPid: FixedDaemonSupervisorOwnerIdentity#supervisorPid.
  FixedDaemonSupervisorOwnerIdentity.supervisorProcessStartId: FixedDaemonSupervisorOwnerIdentity#supervisorProcessStartId.
  FixedDaemonSupervisorOwnerIdentity.supervisorSocketPath: FixedDaemonSupervisorOwnerIdentity#supervisorSocketPath.
---
# Module: [`packages/coding-agent/src/package-manager-cli.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts)

## Classes
### `FixedDaemonSupervisorOwnerIdentity`
- def: [`packages/coding-agent/src/package-manager-cli.ts:825`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L825)
- signature: `interface FixedDaemonSupervisorOwnerIdentity`
- members:
  - `supervisorGeneration` — [`L826`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L826)
  - `supervisorOwnerToken` — [`L827`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L827)
  - `supervisorPid` — [`L828`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L828)
  - `supervisorProcessStartId` — [`L829`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L829)
  - `supervisorSocketPath` — [`L830`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L830)
- used by: [`prepareConnectedDaemonUpdateRestart`](package-manager-cli.ts.md#prepareConnectedDaemonUpdateRestart), [`hasFixedDaemonSupervisorOwnerIdentity`](package-manager-cli.ts.md#hasFixedDaemonSupervisorOwnerIdentity)

### `PackageCommand`
- def: [`packages/coding-agent/src/package-manager-cli.ts:73`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L73)
- signature: `type PackageCommand`
- used by: [`parsePackageCommand`](package-manager-cli.ts.md#parsePackageCommand), [`command`](package-manager-cli.ts.md#PackageCommandOptions.command), [`getPackageCommandUsage`](package-manager-cli.ts.md#getPackageCommandUsage), [`printPackageCommandHelp`](package-manager-cli.ts.md#printPackageCommandHelp)

### `PackageCommandOptions`
- def: [`packages/coding-agent/src/package-manager-cli.ts:83`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L83)
- signature: `interface PackageCommandOptions`
- members:
  - `command` — [`L84`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L84)
  - `conflictingOptions` — [`L97`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L97)
  - `daemonSocketPath` — [`L90`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L90)
  - `force` — [`L88`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L88)
  - `help` — [`L89`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L89)
  - `invalidArgument` — [`L95`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L95)
  - `invalidOption` — [`L94`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L94)
  - `local` — [`L87`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L87)
  - `missingOptionValue` — [`L96`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L96)
  - `restartCoordinator` — [`L91`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L91)
  - `restartOriginActiveSessionId` — [`L93`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L93)
  - `restartStatusPath` — [`L92`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L92)
  - `source` — [`L85`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L85)
  - `updateTarget` — [`L86`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L86)
- uses (calls/refs, reference-scoped): [`PackageCommand`](package-manager-cli.ts.md#PackageCommand), [`UpdateTarget`](package-manager-cli.ts.md#UpdateTarget)
- used by: [`handlePackageCommand`](package-manager-cli.ts.md#handlePackageCommand), [`parsePackageCommand`](package-manager-cli.ts.md#parsePackageCommand)

### `RestoreDaemonUpdateRestartResult`
- def: [`packages/coding-agent/src/package-manager-cli.ts:958`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L958)
- signature: `interface RestoreDaemonUpdateRestartResult`
- members:
  - `failures` — [`L959`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L959)
- uses (calls/refs, reference-scoped): [`DaemonUpdateRestartFailure`](cli/daemon-update-restart.ts.md#DaemonUpdateRestartFailure), [`DaemonUpdateRestartCounts`](cli/daemon-update-restart.ts.md#DaemonUpdateRestartCounts)
- used by: [`originActiveSessionId`](package-manager-cli.ts.md#runDaemonUpdateRestartCoordinator.options-typeLiteral607.originActiveSessionId), [`restoreDaemonUpdateRestart`](package-manager-cli.ts.md#restoreDaemonUpdateRestart)

### `RestoreDaemonUpdateRestartSessionResult`
- def: [`packages/coding-agent/src/package-manager-cli.ts:952`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L952)
- signature: `interface RestoreDaemonUpdateRestartSessionResult`
- members:
  - `failureMessage` — [`L955`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L955)
  - `restored` — [`L953`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L953)
  - `resumed` — [`L954`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L954)
- used by: [`restoreDaemonUpdateRestartSession`](package-manager-cli.ts.md#restoreDaemonUpdateRestartSession), [`restoreDaemonUpdateRestart`](package-manager-cli.ts.md#restoreDaemonUpdateRestart)

### `SelfUpdatePlan`
- def: [`packages/coding-agent/src/package-manager-cli.ts:427`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L427)
- signature: `interface SelfUpdatePlan`
- members:
  - `installSpec` — [`L428`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L428)
  - `packageName` — [`L429`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L429)
  - `shouldRun` — [`L430`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L430)
  - `targetVersion` — [`L431`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L431)
- used by: [`handlePackageCommand`](package-manager-cli.ts.md#handlePackageCommand), [`getSelfUpdatePlan`](package-manager-cli.ts.md#getSelfUpdatePlan)

### `UpdateTarget`
- def: [`packages/coding-agent/src/package-manager-cli.ts:77`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L77)
- signature: `type UpdateTarget`
- used by: [`parsePackageCommand`](package-manager-cli.ts.md#parsePackageCommand), [`updateTarget`](package-manager-cli.ts.md#PackageCommandOptions.updateTarget), [`updateTargetIncludesExtensions`](package-manager-cli.ts.md#updateTargetIncludesExtensions), [`updateTargetIncludesSelf`](package-manager-cli.ts.md#updateTargetIncludesSelf)

## Functions
- `clearPreparedDaemonUpdateRestartManifest(socketPath: string, agentDir: string)` — [`L765`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L765)
- `confirmDaemonSessionLossBeforeUpdate(probe: RunningDaemonProbe, force: boolean)` — [`L501`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L501)
- `daemonProbeMayHaveBusySessions(probe: RunningDaemonProbe)` — [`L505`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L505)
- `formatUnknownError(error: unknown)` — [`L1161`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L1161)
- `getPackageCommandUsage(command: PackageCommand)` — [`L110`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L110)
- `getSelfUpdatePlan(force: boolean)` — [`L439`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L439)
- `handleConfigCommand(args: string[])` — [`L1388`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L1388)
- `handlePackageCommand(args: string[])` — [`L1410`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L1410)
- `hasFixedDaemonSupervisorOwnerIdentity(value: unknown)` — [`L833`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L833)
- `hasRestorableDaemonUpdateRestart(manifest: DaemonUpdateRestartManifest | undefined)` — [`L814`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L814)
- `isCustomMessage(value: unknown)` — [`L575`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L575)
- `isImageContent(value: unknown)` — [`L571`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L571)
- `isMessageContentBlock(value: unknown)` — [`L563`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L563)
- `isQueuedAgentMessage(value: unknown)` — [`L597`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L597)
- `isRecord(value: unknown)` — [`L514`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L514)
- `isSelfUpdateSource(source: string)` — [`L79`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L79)
- `isSessionActionRecoveryAction(value: unknown)` — [`L609`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L609)
- `isStringEnum(value: unknown, allowed: readonly string[])` — [`L518`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L518)
- `isUserMessage(value: unknown)` — [`L587`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L587)
- `normalizedSocketPath(socketPath: string)` — [`L1179`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L1179)
- `parseDaemonUpdateRestartManifest(value: unknown)` — [`L747`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L747)
- `parseDaemonUpdateRestartRuntimeMetadata(value: unknown)` — [`L675`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L675)
- `parseDaemonUpdateRestartSession(value: unknown)` — [`L711`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L711)
- `parsePackageCommand(args: string[])` — [`L188`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L188)
- `parseSessionActionRecoverySnapshot(value: unknown)` — [`L661`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L661)
- `prepareConnectedDaemonUpdateRestart(client: DaemonClient, socketPath: string, agentDir: string, hello: { type: "daemon_hello"; socketPath: string; protocol: DaemonProtocolInfo; schemaId?: string | undefined; ... 9 more ...; serverCapabilities: readonly DaemonServerCapability[]; } | undefined)` — [`L847`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L847)
- `prepareDaemonUpdateRestart(socketPath: string, agentDir: string)` — [`L903`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L903)
- `printPackageCommandHelp(command: PackageCommand)` — [`L123`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L123)
- `printSelfUpdateFallback(command: SelfUpdateCommand)` — [`L423`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L423)
- `printSelfUpdateUnavailable(npmCommand?: string[] | undefined, updateSpec?: string, updatePackageName?: string)` — [`L408`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L408)
- `processIdentityFromDaemonHello(hello: { type: "daemon_hello"; socketPath: string; protocol: DaemonProtocolInfo; schemaId?: string | undefined; schemaRevision?: number | undefined; appVersion?: string | undefined; ... 7 more ...; serverCapabilities: readonly DaemonServerCapability[]; } | undefined)` — [`L1165`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L1165)
- `readBoolean(value: unknown, fieldName: string)` — [`L539`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L539)
- `readCreatedActiveSessionId(value: unknown)` — [`L925`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L925)
- `readCustomMessages(value: unknown, fieldName: string)` — [`L601`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L601)
- `readNumber(value: unknown, fieldName: string)` — [`L546`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L546)
- `readOptionalString(value: unknown, fieldName: string)` — [`L529`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L529)
- `readOptionalStringRecord(value: unknown, fieldName: string)` — [`L553`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L553)
- `readPreparedDaemonUpdateRestartManifest(socketPath: string, agentDir: string, notBeforeMs?: number | undefined)` — [`L778`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L778)
- `readString(value: unknown, fieldName: string)` — [`L522`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L522)
- `remapDaemonUpdateRestartRuntimeMetadata(session: DaemonUpdateRestartSession, restoredActiveSessionIds: ReadonlyMap<string, string>)` — [`L962`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L962)
- `reportDaemonUpdateRestartStatus(status: DaemonUpdateRestartStatus)` — [`L398`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L398)
- `reportSettingsErrors(settingsManager: SettingsManager, context: string)` — [`L100`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L100)
- `resolveUpdateDaemonSocketPath(explicitSocketPath?: string | undefined)` — [`L394`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L394)
- `responseHasActiveDaemonSessions(data: unknown)` — [`L818`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L818)
- `restoreDaemonUpdateRestart(socketPath: string, manifest: DaemonUpdateRestartManifest, restartOriginActiveSessionId?: string | undefined, onProgress?: ((progress: RestoreDaemonUpdateRestartResult) => void) | undefined)` — [`L1096`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L1096)
- `restoreDaemonUpdateRestartSession(client: DaemonClient, session: DaemonUpdateRestartSession, restoredActiveSessionIds: Map<string, string>, restartOriginActiveSessionId?: string | undefined)` — [`L983`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L983)
- `restoreNextTurnMessages(client: DaemonClient, activeSessionId: string, sessionFile: string, messages: readonly CustomMessage<unknown>[])` — [`L932`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L932)
- `runDaemonUpdateRestartCoordinator(options: { socketPath: string; agentDir: string; statusPath: string; originActiveSessionId?: string | undefined; })` — [`L1223`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L1223)
- `runSelfUpdate(command: SelfUpdateCommand)` — [`L461`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L461)
- `setSelfUpdateNoChangeExitCode()` — [`L434`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L434)
- `tryReadPreparedDaemonUpdateRestartManifest(socketPath: string, agentDir: string)` — [`L802`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L802)
- `updateTargetIncludesExtensions(target: UpdateTarget)` — [`L390`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L390)
- `updateTargetIncludesSelf(target: UpdateTarget)` — [`L386`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L386)
- `validateReplacementDaemon(socketPath: string, hello: { type: "daemon_hello"; socketPath: string; protocol: DaemonProtocolInfo; schemaId?: string | undefined; schemaRevision?: number | undefined; ... 8 more ...; serverCapabilities: readonly DaemonServerCapability[]; }, predecessor: DaemonUpdateRestartProcessIdentity | undefined)` — [`L1183`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L1183)

## Module values
- `UPDATE_RESTART_CONTINUATION_PROMPT` — [`L486`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L486)
- `UPDATE_RESTART_PREDECESSOR_FENCE_TIMEOUT_MS` — [`L75`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L75)
- `UPDATE_SESSION_LOSS_COPY` — [`L489`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L489)
- `agentDir` — [`L1225`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L1225)
- `originActiveSessionId` — [`L1227`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L1227)
- `socketPath` — [`L1224`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L1224)
- `statusPath` — [`L1226`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/package-manager-cli.ts#L1226)


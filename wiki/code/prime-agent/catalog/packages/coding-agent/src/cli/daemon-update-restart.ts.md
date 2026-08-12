---
title: 'Module: packages/coding-agent/src/cli/daemon-update-restart.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/daemon-update-restart.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`daemon-update-restart.ts`/
symbols:
  launchDaemonUpdateRestartCoordinator: launchDaemonUpdateRestartCoordinator().
  acquireDaemonUpdateRestartCoordinator: acquireDaemonUpdateRestartCoordinator().
  DaemonUpdateRestartStatusWriter.-constructor: DaemonUpdateRestartStatusWriter#`<constructor>`().
  isDaemonUpdateRestartStatus: isDaemonUpdateRestartStatus().
  buildDaemonUpdateRestartReport: buildDaemonUpdateRestartReport().
  waitForActiveDaemonUpdateRestartCoordinator: waitForActiveDaemonUpdateRestartCoordinator().
  DaemonUpdateRestartStatusWriter.update: DaemonUpdateRestartStatusWriter#update().
  DaemonUpdateRestartStatus.phase: DaemonUpdateRestartStatus#phase.
  DaemonUpdateRestartStatus.counts: DaemonUpdateRestartStatus#counts.
  coordinatorEnvironment: coordinatorEnvironment().
  readCoordinatorRecord: readCoordinatorRecord().
  DaemonUpdateRestartStatus.failures: DaemonUpdateRestartStatus#failures.
  isProcessIdentity: isProcessIdentity().
  DaemonUpdateRestartStatus: DaemonUpdateRestartStatus#
  createProcessIdentityLivenessCheck: createProcessIdentityLivenessCheck().
  DaemonUpdateRestartProcessIdentity: DaemonUpdateRestartProcessIdentity#
  DaemonUpdateRestartProcessIdentity.pid: DaemonUpdateRestartProcessIdentity#pid.
  DaemonUpdateRestartStatusWriter.current: DaemonUpdateRestartStatusWriter#current().
  isCounts: isCounts().
  DaemonUpdateRestartStatusWriter.status: DaemonUpdateRestartStatusWriter#status.
  DaemonUpdateRestartCounts.failed: DaemonUpdateRestartCounts#failed.
  DaemonUpdateRestartCoordinatorLease.release: DaemonUpdateRestartCoordinatorLease#release().
  DaemonUpdateRestartStatus.message: DaemonUpdateRestartStatus#message.
  readTerminalDaemonUpdateRestartStatus: readTerminalDaemonUpdateRestartStatus().
  withCoordinatorRegistryGuard: withCoordinatorRegistryGuard().
  matchesProcessStartId: matchesProcessStartId().
  statusLivenessId: statusLivenessId().
  readDaemonUpdateRestartStatus: readDaemonUpdateRestartStatus().
  isProcessIdentityAlive: isProcessIdentityAlive().
  DaemonUpdateRestartStatus.predecessor: DaemonUpdateRestartStatus#predecessor.
  DaemonUpdateRestartStatus.successor: DaemonUpdateRestartStatus#successor.
  DaemonUpdateRestartCounts.resumed: DaemonUpdateRestartCounts#resumed.
  DaemonUpdateRestartProcessIdentity.processStartId: DaemonUpdateRestartProcessIdentity#processStartId.
  DaemonUpdateRestartCoordinatorRecord: DaemonUpdateRestartCoordinatorRecord#
  DaemonUpdateRestartCounts.restored: DaemonUpdateRestartCounts#restored.
  DaemonUpdateRestartStatus.updatedAt: DaemonUpdateRestartStatus#updatedAt.
  isFailures: isFailures().
  DaemonUpdateRestartStatusWriter.touch: DaemonUpdateRestartStatusWriter#touch().
  DaemonUpdateRestartCounts.total: DaemonUpdateRestartCounts#total.
  DaemonUpdateRestartFailure: DaemonUpdateRestartFailure#
  DaemonUpdateRestartStatusWriter.persist: DaemonUpdateRestartStatusWriter#persist().
  DAEMON_UPDATE_RESTART_COORDINATOR_FLAG: DAEMON_UPDATE_RESTART_COORDINATOR_FLAG.
  DaemonUpdateRestartReport.warnings: DaemonUpdateRestartReport#warnings.
  DaemonUpdateRestartCoordinatorRecord.socketPath: DaemonUpdateRestartCoordinatorRecord#socketPath.
  LaunchDaemonUpdateRestartCoordinatorOptions.socketPath: LaunchDaemonUpdateRestartCoordinatorOptions#socketPath.
  LaunchDaemonUpdateRestartCoordinatorOptions.agentDir: LaunchDaemonUpdateRestartCoordinatorOptions#agentDir.
  LaunchDaemonUpdateRestartCoordinatorOptions.cwd: LaunchDaemonUpdateRestartCoordinatorOptions#cwd.
  DaemonUpdateRestartStatusWriter.startHeartbeat: DaemonUpdateRestartStatusWriter#startHeartbeat().
  DaemonUpdateRestartCounts: DaemonUpdateRestartCounts#
  DaemonUpdateRestartProcessIdentity.supervisorGeneration: DaemonUpdateRestartProcessIdentity#supervisorGeneration.
  DaemonUpdateRestartProcessIdentity.supervisorOwnerToken: DaemonUpdateRestartProcessIdentity#supervisorOwnerToken.
  DaemonUpdateRestartStatus.heartbeatAt: DaemonUpdateRestartStatus#heartbeatAt.
  DaemonUpdateRestartReport.info: DaemonUpdateRestartReport#info.
  AcquireDaemonUpdateRestartCoordinatorOptions.socketPath: AcquireDaemonUpdateRestartCoordinatorOptions#socketPath.
  DaemonUpdateRestartCoordinatorAlreadyRunningError.-constructor: DaemonUpdateRestartCoordinatorAlreadyRunningError#`<constructor>`().
  DaemonUpdateRestartStatus.coordinator: DaemonUpdateRestartStatus#coordinator.
  resolveDaemonUpdateRestartSocketPath: resolveDaemonUpdateRestartSocketPath().
  TERMINAL_PHASES: TERMINAL_PHASES.
  DaemonUpdateRestartFailure.sessionFile: DaemonUpdateRestartFailure#sessionFile.
  DaemonUpdateRestartFailure.message: DaemonUpdateRestartFailure#message.
  DaemonUpdateRestartCoordinatorRecord.token: DaemonUpdateRestartCoordinatorRecord#token.
  DaemonUpdateRestartCoordinatorRecord.statusPath: DaemonUpdateRestartCoordinatorRecord#statusPath.
  AcquireDaemonUpdateRestartCoordinatorOptions.requestId: AcquireDaemonUpdateRestartCoordinatorOptions#requestId.
  AcquireDaemonUpdateRestartCoordinatorOptions.statusPath: AcquireDaemonUpdateRestartCoordinatorOptions#statusPath.
  DAEMON_UPDATE_RESTART_STATUS_FLAG: DAEMON_UPDATE_RESTART_STATUS_FLAG.
  DaemonUpdateRestartPhase: DaemonUpdateRestartPhase#
  DaemonUpdateRestartStatus.requestId: DaemonUpdateRestartStatus#requestId.
  LaunchDaemonUpdateRestartCoordinatorOptions.originActiveSessionId: LaunchDaemonUpdateRestartCoordinatorOptions#originActiveSessionId.
  LaunchDaemonUpdateRestartCoordinatorOptions.timeoutMs: LaunchDaemonUpdateRestartCoordinatorOptions#timeoutMs.
  ALL_PHASES: ALL_PHASES.
  defaultCoordinatorRegistryDir: defaultCoordinatorRegistryDir().
  coordinatorRecordPath: coordinatorRecordPath().
  DaemonUpdateRestartCoordinatorLease.-constructor: DaemonUpdateRestartCoordinatorLease#`<constructor>`().
  createStatusPath: createStatusPath().
  DAEMON_UPDATE_RESTART_ORIGIN_FLAG: DAEMON_UPDATE_RESTART_ORIGIN_FLAG.
  DaemonUpdateRestartStatus.version: DaemonUpdateRestartStatus#version.
  DaemonUpdateRestartStatus.socketPath: DaemonUpdateRestartStatus#socketPath.
  DaemonUpdateRestartStatus.startedAt: DaemonUpdateRestartStatus#startedAt.
  DaemonUpdateRestartCoordinatorRecord.version: DaemonUpdateRestartCoordinatorRecord#version.
  DaemonUpdateRestartCoordinatorRecord.requestId: DaemonUpdateRestartCoordinatorRecord#requestId.
  DaemonUpdateRestartCoordinatorRecord.createdAt: DaemonUpdateRestartCoordinatorRecord#createdAt.
  AcquireDaemonUpdateRestartCoordinatorOptions.registryDir: AcquireDaemonUpdateRestartCoordinatorOptions#registryDir.
  DaemonUpdateRestartStatusWriter: DaemonUpdateRestartStatusWriter#
  DaemonUpdateRestartReport: DaemonUpdateRestartReport#
  DEFAULT_COORDINATOR_PROGRESS_TIMEOUT_MS: DEFAULT_COORDINATOR_PROGRESS_TIMEOUT_MS.
  COORDINATOR_LIVENESS_TIMEOUT_MS: COORDINATOR_LIVENESS_TIMEOUT_MS.
  COORDINATOR_REGISTRY_LOCK_RETRY_MS: COORDINATOR_REGISTRY_LOCK_RETRY_MS.
  delay: delay().
  socketKey: socketKey().
  writeJsonAtomically: writeJsonAtomically().
  isProcessAlive: isProcessAlive().
  DaemonUpdateRestartCoordinatorLease.released: DaemonUpdateRestartCoordinatorLease#released.
  DaemonUpdateRestartCoordinatorAlreadyRunningError: DaemonUpdateRestartCoordinatorAlreadyRunningError#
  LaunchDaemonUpdateRestartCoordinatorOptions: LaunchDaemonUpdateRestartCoordinatorOptions#
  AcquireDaemonUpdateRestartCoordinatorOptions: AcquireDaemonUpdateRestartCoordinatorOptions#
  COORDINATOR_STATUS_HEARTBEAT_MS: COORDINATOR_STATUS_HEARTBEAT_MS.
  COORDINATOR_REGISTRY_LOCK_STALE_MS: COORDINATOR_REGISTRY_LOCK_STALE_MS.
  COORDINATOR_REGISTRY_LOCK_UPDATE_MS: COORDINATOR_REGISTRY_LOCK_UPDATE_MS.
  COORDINATOR_REGISTRY_LOCK_RETRIES: COORDINATOR_REGISTRY_LOCK_RETRIES.
  PROCESS_START_ID_RECHECK_MS: PROCESS_START_ID_RECHECK_MS.
  DaemonUpdateRestartCoordinatorLease: DaemonUpdateRestartCoordinatorLease#
---
# Module: [`packages/coding-agent/src/cli/daemon-update-restart.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts)

## Classes
### `AcquireDaemonUpdateRestartCoordinatorOptions`
- def: [`packages/coding-agent/src/cli/daemon-update-restart.ts:90`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L90)
- signature: `interface AcquireDaemonUpdateRestartCoordinatorOptions`
- members:
  - `registryDir` — [`L94`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L94)
  - `requestId` — [`L91`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L91)
  - `socketPath` — [`L92`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L92)
  - `statusPath` — [`L93`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L93)
- used by: [`originActiveSessionId`](../package-manager-cli.ts.md#runDaemonUpdateRestartCoordinator.options-typeLiteral607.originActiveSessionId), [`acquireDaemonUpdateRestartCoordinator`](daemon-update-restart.ts.md#acquireDaemonUpdateRestartCoordinator)  (1 test-only)

### `DaemonUpdateRestartCoordinatorAlreadyRunningError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/cli/daemon-update-restart.ts:437`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L437)
- signature: `class DaemonUpdateRestartCoordinatorAlreadyRunningError`
- members:
  - `<constructor>(record: DaemonUpdateRestartCoordinatorRecord)` — [`L438`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L438)
- uses (calls/refs, reference-scoped): [`DaemonUpdateRestartCoordinatorRecord`](daemon-update-restart.ts.md#DaemonUpdateRestartCoordinatorRecord), [`socketPath`](daemon-update-restart.ts.md#DaemonUpdateRestartCoordinatorRecord.socketPath)
- used by: [`package-manager-cli.ts`](../package-manager-cli.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-package-manager-cli.ts), [`originActiveSessionId`](../package-manager-cli.ts.md#runDaemonUpdateRestartCoordinator.options-typeLiteral607.originActiveSessionId), [`acquireDaemonUpdateRestartCoordinator`](daemon-update-restart.ts.md#acquireDaemonUpdateRestartCoordinator)

### `DaemonUpdateRestartCoordinatorLease`
- def: [`packages/coding-agent/src/cli/daemon-update-restart.ts:414`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L414)
- signature: `class DaemonUpdateRestartCoordinatorLease`
- members:
  - `<constructor>(record: DaemonUpdateRestartCoordinatorRecord, registryDir: string, path: string)` — [`L417`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L417)
  - `release(method)` — [`L423`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L423)
  - `released` — [`L415`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L415)
- uses (calls/refs, reference-scoped): [`readCoordinatorRecord`](daemon-update-restart.ts.md#readCoordinatorRecord), [`withCoordinatorRegistryGuard`](daemon-update-restart.ts.md#withCoordinatorRegistryGuard), [`DaemonUpdateRestartCoordinatorRecord`](daemon-update-restart.ts.md#DaemonUpdateRestartCoordinatorRecord), [`token`](daemon-update-restart.ts.md#DaemonUpdateRestartCoordinatorRecord.token)
- used by: [`originActiveSessionId`](../package-manager-cli.ts.md#runDaemonUpdateRestartCoordinator.options-typeLiteral607.originActiveSessionId), [`acquireDaemonUpdateRestartCoordinator`](daemon-update-restart.ts.md#acquireDaemonUpdateRestartCoordinator)  (1 test-only)

### `DaemonUpdateRestartCoordinatorRecord`
- def: [`packages/coding-agent/src/cli/daemon-update-restart.ts:73`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L73)
- signature: `interface DaemonUpdateRestartCoordinatorRecord`
- members:
  - `createdAt` — [`L79`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L79)
  - `requestId` — [`L76`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L76)
  - `socketPath` — [`L77`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L77)
  - `statusPath` — [`L78`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L78)
  - `token` — [`L75`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L75)
  - `version` — [`L74`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L74)
- uses (calls/refs, reference-scoped): [`DaemonUpdateRestartProcessIdentity`](daemon-update-restart.ts.md#DaemonUpdateRestartProcessIdentity)
- used by: [`acquireDaemonUpdateRestartCoordinator`](daemon-update-restart.ts.md#acquireDaemonUpdateRestartCoordinator), [`waitForActiveDaemonUpdateRestartCoordinator`](daemon-update-restart.ts.md#waitForActiveDaemonUpdateRestartCoordinator), [`readCoordinatorRecord`](daemon-update-restart.ts.md#readCoordinatorRecord), [`release`](daemon-update-restart.ts.md#DaemonUpdateRestartCoordinatorLease.release), [`<constructor>`](daemon-update-restart.ts.md#DaemonUpdateRestartCoordinatorAlreadyRunningError.-constructor), [`<constructor>`](daemon-update-restart.ts.md#DaemonUpdateRestartCoordinatorLease.-constructor)  (1 test-only)

### `DaemonUpdateRestartCounts`
- def: [`packages/coding-agent/src/cli/daemon-update-restart.ts:33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L33)
- signature: `interface DaemonUpdateRestartCounts`
- members:
  - `failed` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L37)
  - `restored` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L35)
  - `resumed` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L36)
  - `total` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L34)
- used by: [`package-manager-cli.ts`](../package-manager-cli.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-package-manager-cli.ts), [`originActiveSessionId`](../package-manager-cli.ts.md#runDaemonUpdateRestartCoordinator.options-typeLiteral607.originActiveSessionId), [`restoreDaemonUpdateRestart`](../package-manager-cli.ts.md#restoreDaemonUpdateRestart), [`<constructor>`](daemon-update-restart.ts.md#DaemonUpdateRestartStatusWriter.-constructor), [`buildDaemonUpdateRestartReport`](daemon-update-restart.ts.md#buildDaemonUpdateRestartReport), [`counts`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.counts), [`isCounts`](daemon-update-restart.ts.md#isCounts), [`RestoreDaemonUpdateRestartResult`](../package-manager-cli.ts.md#RestoreDaemonUpdateRestartResult)  (1 test-only)

### `DaemonUpdateRestartFailure`
- def: [`packages/coding-agent/src/cli/daemon-update-restart.ts:40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L40)
- signature: `interface DaemonUpdateRestartFailure`
- members:
  - `message` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L42)
  - `sessionFile` — [`L41`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L41)
- used by: [`package-manager-cli.ts`](../package-manager-cli.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-package-manager-cli.ts), [`originActiveSessionId`](../package-manager-cli.ts.md#runDaemonUpdateRestartCoordinator.options-typeLiteral607.originActiveSessionId), [`restoreDaemonUpdateRestart`](../package-manager-cli.ts.md#restoreDaemonUpdateRestart), [`buildDaemonUpdateRestartReport`](daemon-update-restart.ts.md#buildDaemonUpdateRestartReport), [`failures`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.failures), [`isFailures`](daemon-update-restart.ts.md#isFailures), [`RestoreDaemonUpdateRestartResult`](../package-manager-cli.ts.md#RestoreDaemonUpdateRestartResult)  (1 test-only)

### `DaemonUpdateRestartPhase`
- def: [`packages/coding-agent/src/cli/daemon-update-restart.ts:23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L23)
- signature: `type DaemonUpdateRestartPhase`
- used by: [`isDaemonUpdateRestartStatus`](daemon-update-restart.ts.md#isDaemonUpdateRestartStatus), [`phase`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.phase), [`TERMINAL_PHASES`](daemon-update-restart.ts.md#TERMINAL_PHASES), [`ALL_PHASES`](daemon-update-restart.ts.md#ALL_PHASES)

### `DaemonUpdateRestartProcessIdentity`
- def: [`packages/coding-agent/src/cli/daemon-update-restart.ts:45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L45)
- signature: `interface DaemonUpdateRestartProcessIdentity`
- members:
  - `pid` — [`L46`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L46)
  - `processStartId` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L47)
  - `supervisorGeneration` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L48)
  - `supervisorOwnerToken` — [`L49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L49)
- used by: [`package-manager-cli.ts`](../package-manager-cli.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-package-manager-cli.ts), [`originActiveSessionId`](../package-manager-cli.ts.md#runDaemonUpdateRestartCoordinator.options-typeLiteral607.originActiveSessionId), [`acquireDaemonUpdateRestartCoordinator`](daemon-update-restart.ts.md#acquireDaemonUpdateRestartCoordinator), [`<constructor>`](daemon-update-restart.ts.md#DaemonUpdateRestartStatusWriter.-constructor), [`validateReplacementDaemon`](../package-manager-cli.ts.md#validateReplacementDaemon), [`isProcessIdentity`](daemon-update-restart.ts.md#isProcessIdentity), [`createProcessIdentityLivenessCheck`](daemon-update-restart.ts.md#createProcessIdentityLivenessCheck), [`matchesProcessStartId`](daemon-update-restart.ts.md#matchesProcessStartId), [`isProcessIdentityAlive`](daemon-update-restart.ts.md#isProcessIdentityAlive), [`predecessor`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.predecessor), [`successor`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.successor), [`DaemonUpdateRestartCoordinatorRecord`](daemon-update-restart.ts.md#DaemonUpdateRestartCoordinatorRecord), [`processIdentityFromDaemonHello`](../package-manager-cli.ts.md#processIdentityFromDaemonHello), [`coordinator`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.coordinator)  (3 test-only)

### `DaemonUpdateRestartReport`
- def: [`packages/coding-agent/src/cli/daemon-update-restart.ts:68`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L68)
- signature: `interface DaemonUpdateRestartReport`
- members:
  - `info` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L69)
  - `warnings` — [`L70`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L70)
- used by: [`handleUpdateCommand`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleUpdateCommand), [`buildDaemonUpdateRestartReport`](daemon-update-restart.ts.md#buildDaemonUpdateRestartReport), [`reportDaemonUpdateRestartStatus`](../package-manager-cli.ts.md#reportDaemonUpdateRestartStatus)  (1 test-only)

### `DaemonUpdateRestartStatus`
- def: [`packages/coding-agent/src/cli/daemon-update-restart.ts:52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L52)
- signature: `interface DaemonUpdateRestartStatus`
- members:
  - `coordinator` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L57)
  - `counts` — [`L60`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L60)
  - `failures` — [`L61`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L61)
  - `heartbeatAt` — [`L65`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L65)
  - `message` — [`L62`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L62)
  - `phase` — [`L56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L56)
  - `predecessor` — [`L58`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L58)
  - `requestId` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L54)
  - `socketPath` — [`L55`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L55)
  - `startedAt` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L63)
  - `successor` — [`L59`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L59)
  - `updatedAt` — [`L64`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L64)
  - `version` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L53)
- uses (calls/refs, reference-scoped): [`DaemonUpdateRestartProcessIdentity`](daemon-update-restart.ts.md#DaemonUpdateRestartProcessIdentity), [`DaemonUpdateRestartFailure`](daemon-update-restart.ts.md#DaemonUpdateRestartFailure), [`DaemonUpdateRestartCounts`](daemon-update-restart.ts.md#DaemonUpdateRestartCounts), [`DaemonUpdateRestartPhase`](daemon-update-restart.ts.md#DaemonUpdateRestartPhase)
- used by: [`package-manager-cli.ts`](../package-manager-cli.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-package-manager-cli.ts), [`handlePackageCommand`](../package-manager-cli.ts.md#handlePackageCommand), [`originActiveSessionId`](../package-manager-cli.ts.md#runDaemonUpdateRestartCoordinator.options-typeLiteral607.originActiveSessionId), [`launchDaemonUpdateRestartCoordinator`](daemon-update-restart.ts.md#launchDaemonUpdateRestartCoordinator), [`<constructor>`](daemon-update-restart.ts.md#DaemonUpdateRestartStatusWriter.-constructor), [`isDaemonUpdateRestartStatus`](daemon-update-restart.ts.md#isDaemonUpdateRestartStatus), [`buildDaemonUpdateRestartReport`](daemon-update-restart.ts.md#buildDaemonUpdateRestartReport), [`waitForActiveDaemonUpdateRestartCoordinator`](daemon-update-restart.ts.md#waitForActiveDaemonUpdateRestartCoordinator), [`update`](daemon-update-restart.ts.md#DaemonUpdateRestartStatusWriter.update), [`current`](daemon-update-restart.ts.md#DaemonUpdateRestartStatusWriter.current), [`status`](daemon-update-restart.ts.md#DaemonUpdateRestartStatusWriter.status), [`readTerminalDaemonUpdateRestartStatus`](daemon-update-restart.ts.md#readTerminalDaemonUpdateRestartStatus), [`statusLivenessId`](daemon-update-restart.ts.md#statusLivenessId), [`readDaemonUpdateRestartStatus`](daemon-update-restart.ts.md#readDaemonUpdateRestartStatus), [`reportDaemonUpdateRestartStatus`](../package-manager-cli.ts.md#reportDaemonUpdateRestartStatus), [`touch`](daemon-update-restart.ts.md#DaemonUpdateRestartStatusWriter.touch)  (5 test-only)

### `DaemonUpdateRestartStatusWriter`
- def: [`packages/coding-agent/src/cli/daemon-update-restart.ts:248`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L248)
- signature: `class DaemonUpdateRestartStatusWriter`
- members:
  - `<constructor>(path: string, requestId: string, socketPath: string)` — [`L251`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L251)
  - `current(method)` — [`L289`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L289)
  - `persist(method)` — [`L314`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L314)
  - `startHeartbeat(method)` — [`L302`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L302)
  - `touch(method)` — [`L297`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L297)
  - `update(method)` — [`L272`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L272)
  - `status` — [`L249`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L249)
- uses (calls/refs, reference-scoped): [`getProcessStartId`](../core/session-lease.ts.md#getProcessStartId), [`phase`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.phase), [`counts`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.counts), [`failures`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.failures), [`DaemonUpdateRestartStatus`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus), [`pid`](daemon-update-restart.ts.md#DaemonUpdateRestartProcessIdentity.pid), [`failed`](daemon-update-restart.ts.md#DaemonUpdateRestartCounts.failed), [`processStartId`](daemon-update-restart.ts.md#DaemonUpdateRestartProcessIdentity.processStartId), [`resumed`](daemon-update-restart.ts.md#DaemonUpdateRestartCounts.resumed), [`restored`](daemon-update-restart.ts.md#DaemonUpdateRestartCounts.restored), [`updatedAt`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.updatedAt), [`total`](daemon-update-restart.ts.md#DaemonUpdateRestartCounts.total), [`heartbeatAt`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.heartbeatAt), [`coordinator`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.coordinator), [`requestId`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.requestId), [`socketPath`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.socketPath), [`startedAt`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.startedAt), [`version`](daemon-update-restart.ts.md#DaemonUpdateRestartStatus.version), [`writeJsonAtomically`](daemon-update-restart.ts.md#writeJsonAtomically), [`COORDINATOR_STATUS_HEARTBEAT_MS`](daemon-update-restart.ts.md#COORDINATOR_STATUS_HEARTBEAT_MS)
- used by: [`package-manager-cli.ts`](../package-manager-cli.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-package-manager-cli.ts), [`originActiveSessionId`](../package-manager-cli.ts.md#runDaemonUpdateRestartCoordinator.options-typeLiteral607.originActiveSessionId)  (2 test-only)

### `LaunchDaemonUpdateRestartCoordinatorOptions`
- def: [`packages/coding-agent/src/cli/daemon-update-restart.ts:82`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L82)
- signature: `interface LaunchDaemonUpdateRestartCoordinatorOptions`
- members:
  - `agentDir` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L84)
  - `cwd` — [`L85`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L85)
  - `originActiveSessionId` — [`L86`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L86)
  - `socketPath` — [`L83`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L83)
  - `timeoutMs` — [`L87`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L87)
- used by: [`handlePackageCommand`](../package-manager-cli.ts.md#handlePackageCommand), [`handleUpdateCommand`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleUpdateCommand), [`launchDaemonUpdateRestartCoordinator`](daemon-update-restart.ts.md#launchDaemonUpdateRestartCoordinator)  (2 test-only)

## Functions
- `acquireDaemonUpdateRestartCoordinator(options: AcquireDaemonUpdateRestartCoordinatorOptions)` — [`L444`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L444)
- `buildDaemonUpdateRestartReport(status: DaemonUpdateRestartStatus)` — [`L122`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L122)
- `coordinatorEnvironment(agentDir: string)` — [`L517`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L517)
- `coordinatorRecordPath(registryDir: string, socketPath: string)` — [`L323`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L323)
- `createProcessIdentityLivenessCheck(identity: DaemonUpdateRestartProcessIdentity)` — [`L369`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L369)
- `createStatusPath(agentDir: string, socketPath: string, requestId: string)` — [`L511`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L511)
- `defaultCoordinatorRegistryDir()` — [`L319`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L319)
- `delay(ms: number)` — [`L147`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L147)
- `isCounts(value: unknown)` — [`L185`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L185)
- `isDaemonUpdateRestartStatus(value: unknown)` — [`L208`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L208)
- `isFailures(value: unknown)` — [`L195`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L195)
- `isProcessAlive(pid: number)` — [`L348`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L348)
- `isProcessIdentity(value: unknown)` — [`L171`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L171)
- `isProcessIdentityAlive(identity: DaemonUpdateRestartProcessIdentity)` — [`L365`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L365)
- `launchDaemonUpdateRestartCoordinator(options: LaunchDaemonUpdateRestartCoordinatorOptions)` — [`L532`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L532)
- `matchesProcessStartId(identity: DaemonUpdateRestartProcessIdentity)` — [`L357`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L357)
- `readCoordinatorRecord(path: string)` — [`L387`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L387)
- `readDaemonUpdateRestartStatus(path: string)` — [`L231`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L231)
- `readTerminalDaemonUpdateRestartStatus(path: string)` — [`L243`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L243)
- `resolveDaemonUpdateRestartSocketPath(socketPath?: string | undefined)` — [`L97`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L97)
- `socketKey(socketPath: string)` — [`L155`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L155)
- `statusLivenessId(status: DaemonUpdateRestartStatus)` — [`L151`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L151)
- `waitForActiveDaemonUpdateRestartCoordinator(record: DaemonUpdateRestartCoordinatorRecord, progressTimeoutMs?: number)` — [`L472`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L472)
- `withCoordinatorRegistryGuard(registryDir: string, action: () => T | Promise<T>)` — [`L327`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L327)
- `writeJsonAtomically(path: string, value: unknown)` — [`L160`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L160)

## Module values
- `ALL_PHASES` — [`L103`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L103)
- `COORDINATOR_LIVENESS_TIMEOUT_MS` — [`L114`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L114)
- `COORDINATOR_REGISTRY_LOCK_RETRIES` — [`L118`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L118)
- `COORDINATOR_REGISTRY_LOCK_RETRY_MS` — [`L119`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L119)
- `COORDINATOR_REGISTRY_LOCK_STALE_MS` — [`L116`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L116)
- `COORDINATOR_REGISTRY_LOCK_UPDATE_MS` — [`L117`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L117)
- `COORDINATOR_STATUS_HEARTBEAT_MS` — [`L115`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L115)
- `DAEMON_UPDATE_RESTART_COORDINATOR_FLAG` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L19)
- `DAEMON_UPDATE_RESTART_ORIGIN_FLAG` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L21)
- `DAEMON_UPDATE_RESTART_STATUS_FLAG` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L20)
- `DEFAULT_COORDINATOR_PROGRESS_TIMEOUT_MS` — [`L113`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L113)
- `PROCESS_START_ID_RECHECK_MS` — [`L120`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L120)
- `TERMINAL_PHASES` — [`L102`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-update-restart.ts#L102)


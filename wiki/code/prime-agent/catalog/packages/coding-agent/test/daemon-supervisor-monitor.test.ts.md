---
title: 'Module: packages/coding-agent/test/daemon-supervisor-monitor.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/daemon-supervisor-monitor.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`daemon-supervisor-monitor.test.ts`/
symbols:
  workerLaunchTestState: workerLaunchTestState.
  recoveryEligibilityInvalidations.Array.typeLiteral100.invalidate: recoveryEligibilityInvalidations.Array:typeLiteral100:invalidate().
  DeferredRecoveryWorker.descriptor: DeferredRecoveryWorker#descriptor.
  createHarness: createHarness().
  supervisorRegistryDirs: supervisorRegistryDirs.
  DeferredRecoveryWorker.descriptor.typeLiteral79.lifecycle: DeferredRecoveryWorker#descriptor.typeLiteral79:lifecycle.
  createSupervisorSnapshotState: createSupervisorSnapshotState().
  DeferredRecoveryWorker.descriptor.typeLiteral79.workerId: DeferredRecoveryWorker#descriptor.typeLiteral79:workerId.
  DeferredRecoveryWorker: DeferredRecoveryWorker#
  DeferredRecoveryWorker.deferredRecovery: DeferredRecoveryWorker#deferredRecovery.
  recoveryDeniedError: recoveryDeniedError().
  createExistingLaunchWorker: createExistingLaunchWorker().
  DeferredRecoveryWorker.snapshotCache: DeferredRecoveryWorker#snapshotCache.
  DeferredRecoveryHarness.handleWorkerClose: DeferredRecoveryHarness#handleWorkerClose().
  supervisorRegistryDirEnv: supervisorRegistryDirEnv.
  SupervisorMonitorHarness.canConnectToSupervisor: SupervisorMonitorHarness#canConnectToSupervisor.
  DeferredRecoveryWorker.client: DeferredRecoveryWorker#client.
  DeferredRecoveryWorker.intentionalStop: DeferredRecoveryWorker#intentionalStop.
  DeferredRecoveryHarness: DeferredRecoveryHarness#
  recoveryEligibilityInvalidations.Array.typeLiteral100.name: recoveryEligibilityInvalidations.Array:typeLiteral100:name.
  previousSupervisorRegistryDir: previousSupervisorRegistryDir.
  DeferredRecoveryWorker.descriptor.typeLiteral79.pid: DeferredRecoveryWorker#descriptor.typeLiteral79:pid.
  DeferredRecoveryWorker.descriptor.typeLiteral79.rootActiveSessionId: DeferredRecoveryWorker#descriptor.typeLiteral79:rootActiveSessionId.
  DeferredRecoveryWorker.descriptor.typeLiteral79.lastError: DeferredRecoveryWorker#descriptor.typeLiteral79:lastError.
  DeferredRecoveryWorker.incomingTranscriptActiveSessionIds: DeferredRecoveryWorker#incomingTranscriptActiveSessionIds.
  DeferredRecoveryWorker.transcriptCaches: DeferredRecoveryWorker#transcriptCaches.
  DeferredRecoveryWorker.duplicateIncomingTranscriptChunkIndexes: DeferredRecoveryWorker#duplicateIncomingTranscriptChunkIndexes.
  DeferredRecoveryWorker.snapshotTransferFrames: DeferredRecoveryWorker#snapshotTransferFrames.
  DeferredRecoveryWorker.recovery: DeferredRecoveryWorker#recovery.
  DeferredRecoveryWorker.stopRevision: DeferredRecoveryWorker#stopRevision.
  waitForFile: waitForFile().
  DeferredRecoveryHarness.workers: DeferredRecoveryHarness#workers.
  DeferredRecoveryHarness.deferWorkerRecovery: DeferredRecoveryHarness#deferWorkerRecovery().
  SupervisorMonitorHarness.scheduleSupervisorAvailabilityCheck: SupervisorMonitorHarness#scheduleSupervisorAvailabilityCheck.
  SupervisorMonitorHarness: SupervisorMonitorHarness#
  SupervisorMonitorHarness.supervisorMonitorTimer: SupervisorMonitorHarness#supervisorMonitorTimer.
  SupervisorMonitorHarness.clients: SupervisorMonitorHarness#clients.
  SupervisorMonitorHarness.clients.Set.typeLiteral71.authenticated: SupervisorMonitorHarness#clients.Set:typeLiteral71:authenticated.
  SupervisorMonitorHarness.supervisorClaims: SupervisorMonitorHarness#supervisorClaims.
  DeferredRecoveryWorker.descriptor.typeLiteral79.stopRequestedAt: DeferredRecoveryWorker#descriptor.typeLiteral79:stopRequestedAt.
  DeferredRecoveryHarness.shuttingDown: DeferredRecoveryHarness#shuttingDown.
  waitForCapturedChildClose: waitForCapturedChildClose().
  recoveryEligibilityInvalidations: recoveryEligibilityInvalidations.
  SupervisorMonitorHarness.options: SupervisorMonitorHarness#options.
  SupervisorMonitorHarness.options.typeLiteral70.worker: SupervisorMonitorHarness#options.typeLiteral70:worker.
  SupervisorMonitorHarness.shuttingDown: SupervisorMonitorHarness#shuttingDown.
  SupervisorMonitorHarness.launchReplacementSupervisor: SupervisorMonitorHarness#launchReplacementSupervisor.
  DeferredRecoveryWorker.transcriptCaches.Map.typeLiteral80.markFailed: DeferredRecoveryWorker#transcriptCaches.Map:typeLiteral80:markFailed().
  DeferredRecoveryHarness.assertRecoveryAllowed: DeferredRecoveryHarness#assertRecoveryAllowed.
  DeferredRecoveryHarness.persistWorker: DeferredRecoveryHarness#persistWorker.
  DeferredRecoveryHarness.syncAgentPeers: DeferredRecoveryHarness#syncAgentPeers.
  DeferredRecoveryHarness.recoverWorker: DeferredRecoveryHarness#recoverWorker.
---
# Module: [`packages/coding-agent/test/daemon-supervisor-monitor.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts)

## Classes
### `DeferredRecoveryHarness`
- def: [`packages/coding-agent/test/daemon-supervisor-monitor.test.ts:153`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L153)
- signature: `interface DeferredRecoveryHarness`
- members:
  - `deferWorkerRecovery(method)` — [`L161`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L161)
  - `handleWorkerClose(method)` — [`L160`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L160)
  - `assertRecoveryAllowed` — [`L156`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L156)
  - `persistWorker` — [`L157`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L157)
  - `recoverWorker` — [`L159`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L159)
  - `shuttingDown` — [`L155`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L155)
  - `syncAgentPeers` — [`L158`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L158)
  - `workers` — [`L154`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L154)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `DeferredRecoveryWorker`
- def: [`packages/coding-agent/test/daemon-supervisor-monitor.test.ts:132`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L132)
- signature: `interface DeferredRecoveryWorker`
- members:
  - `markFailed(method)` — [`L144`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L144)
  - `client` — [`L141`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L141)
  - `deferredRecovery` — [`L148`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L148)
  - `descriptor` — [`L133`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L133)
  - `duplicateIncomingTranscriptChunkIndexes` — [`L145`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L145)
  - `incomingTranscriptActiveSessionIds` — [`L143`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L143)
  - `intentionalStop` — [`L149`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L149)
  - `lastError` — [`L138`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L138)
  - `lifecycle` — [`L137`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L137)
  - `pid` — [`L135`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L135)
  - `recovery` — [`L147`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L147)
  - `rootActiveSessionId` — [`L136`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L136)
  - `snapshotCache` — [`L142`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L142)
  - `snapshotTransferFrames` — [`L146`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L146)
  - `stopRequestedAt` — [`L139`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L139)
  - `stopRevision` — [`L150`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L150)
  - `transcriptCaches` — [`L144`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L144)
  - `workerId` — [`L134`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L134)
- uses (calls/refs, reference-scoped): [`DaemonAttachResult`](../src/modes/daemon/daemon-protocol.ts.md#DaemonAttachResult)
- used by: (5 test-only callers)

### `SupervisorMonitorHarness`
- def: [`packages/coding-agent/test/daemon-supervisor-monitor.test.ts:121`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L121)
- signature: `interface SupervisorMonitorHarness`
- members:
  - `authenticated` — [`L123`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L123)
  - `canConnectToSupervisor` — [`L127`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L127)
  - `clients` — [`L123`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L123)
  - `launchReplacementSupervisor` — [`L128`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L128)
  - `options` — [`L122`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L122)
  - `scheduleSupervisorAvailabilityCheck` — [`L129`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L129)
  - `shuttingDown` — [`L125`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L125)
  - `supervisorClaims` — [`L124`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L124)
  - `supervisorMonitorTimer` — [`L126`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L126)
  - `worker` — [`L122`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L122)
- used by: (2 test-only callers)

## Functions
- `createExistingLaunchWorker(root: string, descriptorDir: string)` — [`L185`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L185)
- `createHarness(canConnect: () => Promise<boolean>)` — [`L262`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L262)
- `createSupervisorSnapshotState()` — [`L220`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L220)
- `invalidate(method)` — [`L229`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L229)
- `recoveryDeniedError(code: "supervisor_generation_stale" | "supervisor_recovery_cancelled")` — [`L164`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L164)
- `waitForCapturedChildClose(child: ChildProcess)` — [`L168`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L168)
- `waitForFile(path: string)` — [`L175`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L175)

## Module values
- `name` — [`L228`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L228)
- `previousSupervisorRegistryDir` — [`L118`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L118)
- `recoveryEligibilityInvalidations` — [`L227`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L227)
- `supervisorRegistryDirEnv` — [`L117`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L117)
- `supervisorRegistryDirs` — [`L119`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L119)
- `workerLaunchTestState` — [`L34`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-monitor.test.ts#L34)


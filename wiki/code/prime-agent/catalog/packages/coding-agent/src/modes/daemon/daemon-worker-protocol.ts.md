---
title: 'Module: packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`daemon-worker-protocol.ts`/
symbols:
  DaemonWorkerDescriptor.workerId: DaemonWorkerDescriptor#workerId.
  DaemonWorkerFrameHeader: DaemonWorkerFrameHeader#
  DAEMON_WORKER_SUPERVISOR_SOCKET_ENV: DAEMON_WORKER_SUPERVISOR_SOCKET_ENV.
  DaemonWorkerDescriptor.lifecycle: DaemonWorkerDescriptor#lifecycle.
  DaemonWorkerDescriptor.pid: DaemonWorkerDescriptor#pid.
  DaemonWorkerCommand: DaemonWorkerCommand#
  DaemonWorkerDescriptor.processStartId: DaemonWorkerDescriptor#processStartId.
  DaemonWorkerDescriptor.ownerClientId: DaemonWorkerDescriptor#ownerClientId.
  DaemonWorkerDescriptor.rootActiveSessionId: DaemonWorkerDescriptor#rootActiveSessionId.
  DaemonWorkerDescriptor.stopRequestedAt: DaemonWorkerDescriptor#stopRequestedAt.
  DAEMON_WORKER_ACTIVE_SESSION_ID_ENV: DAEMON_WORKER_ACTIVE_SESSION_ID_ENV.
  DaemonWorkerDescriptor: DaemonWorkerDescriptor#
  DaemonWorkerDescriptor.createCommand: DaemonWorkerDescriptor#createCommand.
  DAEMON_WORKER_ROLE_ENV: DAEMON_WORKER_ROLE_ENV.
  DAEMON_WORKER_TOKEN_ENV: DAEMON_WORKER_TOKEN_ENV.
  DAEMON_WORKER_RECOVERY_JOURNAL_ENV: DAEMON_WORKER_RECOVERY_JOURNAL_ENV.
  DaemonWorkerDescriptor.orphanProcessJournalPath: DaemonWorkerDescriptor#orphanProcessJournalPath.
  DaemonWorkerDescriptor.rootSessionId: DaemonWorkerDescriptor#rootSessionId.
  isDaemonWorkerFrameHeader: isDaemonWorkerFrameHeader().
  DaemonCreateCommand: DaemonCreateCommand#
  DaemonWorkerCommandBody: DaemonWorkerCommandBody#
  DaemonWorkerDescriptor.consecutiveFailures: DaemonWorkerDescriptor#consecutiveFailures.
  DaemonWorkerDescriptor.recoveryJournalPath: DaemonWorkerDescriptor#recoveryJournalPath.
  DaemonWorkerDescriptor.archiveOnStop: DaemonWorkerDescriptor#archiveOnStop.
  DaemonWorkerDescriptor.lastError: DaemonWorkerDescriptor#lastError.
  waitForDaemonWorkerStartupGate: waitForDaemonWorkerStartupGate().
  DaemonWorkerDescriptor.socketPath: DaemonWorkerDescriptor#socketPath.
  isDaemonWorkerProcess: isDaemonWorkerProcess().
  DAEMON_WORKER_STARTUP_GATE_COMMIT: DAEMON_WORKER_STARTUP_GATE_COMMIT.
  DaemonWorkerDescriptor.supervisorSocketPath: DaemonWorkerDescriptor#supervisorSocketPath.
  DaemonWorkerDescriptor.authenticationToken: DaemonWorkerDescriptor#authenticationToken.
  DaemonWorkerDescriptor.sessionFile: DaemonWorkerDescriptor#sessionFile.
  requireDaemonWorkerAuthenticationToken: requireDaemonWorkerAuthenticationToken().
  DAEMON_WORKER_STARTUP_GATE_FD_ENV: DAEMON_WORKER_STARTUP_GATE_FD_ENV.
  DaemonWorkerLifecycle: DaemonWorkerLifecycle#
  DaemonWorkerDescriptor.version: DaemonWorkerDescriptor#version.
  DaemonWorkerDescriptor.createdAt: DaemonWorkerDescriptor#createdAt.
  DaemonWorkerDescriptor.updatedAt: DaemonWorkerDescriptor#updatedAt.
  DaemonWorkerDescriptor.lastFailureAt: DaemonWorkerDescriptor#lastFailureAt.
  DaemonCreateCommand.Extract.typeLiteral59.type: DaemonCreateCommand#Extract:typeLiteral59:type.
---
# Module: [`packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts)

## Classes
### `DaemonCreateCommand`
- def: [`packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts:39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L39)
- signature: `type DaemonCreateCommand`
- members:
  - `type` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L39)
- uses (calls/refs, reference-scoped): [`DaemonCommand`](daemon-protocol.ts.md#DaemonCommand)
- used by: [`daemon-supervisor.ts`](daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`launchWorker`](daemon-supervisor.ts.md#DaemonSupervisor.launchWorker), [`createOrReuseWorker`](daemon-supervisor.ts.md#DaemonSupervisor.createOrReuseWorker), [`createCommand`](daemon-worker-protocol.ts.md#DaemonWorkerDescriptor.createCommand), [`withoutSupervisorCreateFields`](daemon-supervisor.ts.md#withoutSupervisorCreateFields)

### `DaemonWorkerCommand`
- def: [`packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts:41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L41)
- signature: `type DaemonWorkerCommand`
- uses (calls/refs, reference-scoped): [`DaemonClientCapability`](daemon-protocol.ts.md#DaemonClientCapability), [`AgentSessionMessageAgentSummary`](../../core/agent-messages.ts.md#AgentSessionMessageAgentSummary), [`IdleEvictionMinutes`](../../core/session-action-store.ts.md#IdleEvictionMinutes), [`AgentSessionMessageSender`](../../core/agent-messages.ts.md#AgentSessionMessageSender), [`AgentSessionMessageDeliveryMode`](../../core/agent-messages.ts.md#AgentSessionMessageDeliveryMode)
- used by: [`daemon-mode.ts`](daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`handleWorkerCommand`](daemon-mode.ts.md#AgentDaemon.handleWorkerCommand), [`handleLine`](daemon-mode.ts.md#AgentDaemon.handleLine), [`daemon-client.ts`](daemon-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-client.ts), [`requestWire`](daemon-client.ts.md#DaemonClient.requestWire), [`daemon-worker-client.ts`](daemon-worker-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-worker-client.ts), [`writeWorkerSuccess`](daemon-mode.ts.md#AgentDaemon.writeWorkerSuccess), [`DaemonWorkerCommandBody`](daemon-worker-protocol.ts.md#DaemonWorkerCommandBody), [`DaemonWorkerWireCommand`](daemon-worker-client.ts.md#DaemonWorkerWireCommand), [`SupervisorGenerationClaim`](daemon-mode.ts.md#SupervisorGenerationClaim), [`DaemonWorkerAuthentication`](daemon-worker-client.ts.md#DaemonWorkerAuthentication)

### `DaemonWorkerCommandBody`
- def: [`packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts:80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L80)
- signature: `type DaemonWorkerCommandBody`
- uses (calls/refs, reference-scoped): [`DaemonWorkerCommand`](daemon-worker-protocol.ts.md#DaemonWorkerCommand)
- used by: [`daemon-client.ts`](daemon-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-client.ts), [`daemon-worker-client.ts`](daemon-worker-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-worker-client.ts), [`requestWorker`](daemon-worker-client.ts.md#DaemonWorkerClient.requestWorker), [`requestWorker`](daemon-client.ts.md#DaemonClient.requestWorker), [`DaemonWireCommandBody`](daemon-client.ts.md#DaemonWireCommandBody), [`DaemonWorkerWireCommandBody`](daemon-worker-client.ts.md#DaemonWorkerWireCommandBody), [`authenticateWorker`](daemon-client.ts.md#DaemonClient.authenticateWorker)

### `DaemonWorkerDescriptor`
- def: [`packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts:86`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L86)
- signature: `interface DaemonWorkerDescriptor`
- members:
  - `archiveOnStop` — [`L109`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L109) — Complete the root's archived lifecycle state after its process has stopped.
  - `authenticationToken` — [`L95`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L95)
  - `consecutiveFailures` — [`L105`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L105)
  - `createCommand` — [`L104`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L104)
  - `createdAt` — [`L101`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L101)
  - `lastError` — [`L111`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L111)
  - `lastFailureAt` — [`L110`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L110)
  - `lifecycle` — [`L103`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L103)
  - `orphanProcessJournalPath` — [`L93`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L93)
  - `ownerClientId` — [`L98`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L98) — Stable protocol client that owns this worker. Omitted for resident sessions.
  - `pid` — [`L89`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L89)
  - `processStartId` — [`L90`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L90)
  - `recoveryJournalPath` — [`L92`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L92)
  - `rootActiveSessionId` — [`L96`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L96)
  - `rootSessionId` — [`L99`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L99)
  - `sessionFile` — [`L100`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L100)
  - `socketPath` — [`L91`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L91)
  - `stopRequestedAt` — [`L107`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L107) — Durable intent written before root termination so replacement supervisors never recover it.
  - `supervisorSocketPath` — [`L94`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L94)
  - `updatedAt` — [`L102`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L102)
  - `version` — [`L87`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L87)
  - `workerId` — [`L88`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L88)
- uses (calls/refs, reference-scoped): [`DaemonCreateCommand`](daemon-worker-protocol.ts.md#DaemonCreateCommand), [`DaemonWorkerLifecycle`](daemon-worker-protocol.ts.md#DaemonWorkerLifecycle)
- used by: [`daemon-supervisor.ts`](daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`handleCommand`](daemon-supervisor.ts.md#DaemonSupervisor.handleCommand), [`handleWorkerFrame`](daemon-supervisor.ts.md#DaemonSupervisor.handleWorkerFrame), [`descriptor`](daemon-supervisor.ts.md#ResidentWorker.descriptor), [`launchWorker`](daemon-supervisor.ts.md#DaemonSupervisor.launchWorker), [`type`](daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type), [`start`](daemon-supervisor.ts.md#DaemonSupervisor.start), [`stopWorkerUntracked`](daemon-supervisor.ts.md#DaemonSupervisor.stopWorkerUntracked), [`shutdown`](daemon-supervisor.ts.md#DaemonSupervisor.shutdown), [`cleanupSupervisorResourcesOnce`](daemon-supervisor.ts.md#DaemonSupervisor.cleanupSupervisorResourcesOnce), [`refreshWorkerSummaries`](daemon-supervisor.ts.md#DaemonSupervisor.refreshWorkerSummaries), [`recoverWorker`](daemon-supervisor.ts.md#DaemonSupervisor.recoverWorker), [`discoverDaemons`](../../cli/daemon-ps.ts.md#discoverDaemons), [`daemon-ps.ts`](../../cli/daemon-ps.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-daemon-ps.ts), [`runIdleEvictionSweep`](daemon-supervisor.ts.md#DaemonSupervisor.runIdleEvictionSweep), [`recoverUncertainWorkerOperations`](daemon-supervisor.ts.md#DaemonSupervisor.recoverUncertainWorkerOperations), [`workerEvictionSnapshot`](daemon-supervisor.ts.md#DaemonSupervisor.workerEvictionSnapshot), [`prepareUpdateRestartFenced`](daemon-supervisor.ts.md#DaemonSupervisor.prepareUpdateRestartFenced), [`adoptOrRecoverWorker`](daemon-supervisor.ts.md#DaemonSupervisor.adoptOrRecoverWorker), [`handleWorkerClose`](daemon-supervisor.ts.md#DaemonSupervisor.handleWorkerClose), [`finalizeTimedOutWorkerStop`](daemon-supervisor.ts.md#DaemonSupervisor.finalizeTimedOutWorkerStop), [`connectWorker`](daemon-supervisor.ts.md#DaemonSupervisor.connectWorker), [`loadWorkerDescriptors`](daemon-supervisor.ts.md#DaemonSupervisor.loadWorkerDescriptors), [`syncAgentPeers`](daemon-supervisor.ts.md#DaemonSupervisor.syncAgentPeers), [`forceStopTrackedWorkers`](../../cli/daemon-ps.ts.md#forceStopTrackedWorkers), [`reclaimStaleWorkerRegistration`](daemon-supervisor.ts.md#DaemonSupervisor.reclaimStaleWorkerRegistration), [`publicSummary`](daemon-supervisor.ts.md#DaemonSupervisor.publicSummary), [`isDaemonWorkerDescriptor`](daemon-supervisor.ts.md#isDaemonWorkerDescriptor), [`resumeDeferredWorkerRecovery`](daemon-supervisor.ts.md#DaemonSupervisor.resumeDeferredWorkerRecovery), [`finalizeArchivedWorkerStop`](daemon-supervisor.ts.md#DaemonSupervisor.finalizeArchivedWorkerStop), [`promoteOwnedWorker`](daemon-supervisor.ts.md#DaemonSupervisor.promoteOwnedWorker), [`scheduleOwnedWorkerCleanup`](daemon-supervisor.ts.md#DaemonSupervisor.scheduleOwnedWorkerCleanup), [`persistWorker`](daemon-supervisor.ts.md#DaemonSupervisor.persistWorker), [`isWorkerRecoveryCancelled`](daemon-supervisor.ts.md#DaemonSupervisor.isWorkerRecoveryCancelled), [`isWorkerRecoveryCandidate`](daemon-supervisor.ts.md#DaemonSupervisor.isWorkerRecoveryCandidate), [`requireAvailableWorkerClient`](daemon-supervisor.ts.md#DaemonSupervisor.requireAvailableWorkerClient), [`isTrackedWorkerDescriptor`](../../cli/daemon-ps.ts.md#isTrackedWorkerDescriptor), [`effectiveWorkerState`](daemon-supervisor.ts.md#DaemonSupervisor.effectiveWorkerState), [`deleteWorkerDescriptor`](daemon-supervisor.ts.md#DaemonSupervisor.deleteWorkerDescriptor), [`isWorkerStopping`](daemon-supervisor.ts.md#DaemonSupervisor.isWorkerStopping)  (+10 more; 5 test-only)

### `DaemonWorkerFrameHeader`
- def: [`packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts:22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L22)
- signature: `type DaemonWorkerFrameHeader`
- uses (calls/refs, reference-scoped): [`DaemonOutbound`](daemon-protocol.ts.md#DaemonOutbound)
- used by: [`daemon-mode.ts`](daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`daemon-supervisor.ts`](daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`handleWorkerFrame`](daemon-supervisor.ts.md#DaemonSupervisor.handleWorkerFrame), [`daemon-worker-client.ts`](daemon-worker-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-worker-client.ts), [`handleFrame`](daemon-worker-client.ts.md#DaemonWorkerClient.handleFrame), [`writeSerialized`](daemon-mode.ts.md#AgentDaemon.writeSerialized), [`channel`](daemon-worker-client.ts.md#DaemonWorkerClient.channel), [`isDaemonWorkerFrameHeader`](daemon-worker-protocol.ts.md#isDaemonWorkerFrameHeader), [`DaemonWorkerFrameListener`](daemon-worker-client.ts.md#DaemonWorkerFrameListener)  (8 test-only)

### `DaemonWorkerLifecycle`
- def: [`packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts:20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L20)
- signature: `type DaemonWorkerLifecycle`
- used by: [`daemon-supervisor.ts`](daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`lifecycle`](daemon-worker-protocol.ts.md#DaemonWorkerDescriptor.lifecycle), [`effectiveWorkerState`](daemon-supervisor.ts.md#DaemonSupervisor.effectiveWorkerState)

## Functions
- `isDaemonWorkerFrameHeader(value: unknown)` — [`L147`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L147)
- `isDaemonWorkerProcess(environment?: ProcessEnv)` — [`L114`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L114)
- `requireDaemonWorkerAuthenticationToken(environment?: ProcessEnv)` — [`L139`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L139)
- `waitForDaemonWorkerStartupGate(environment?: ProcessEnv)` — [`L118`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L118)

## Module values
- `DAEMON_WORKER_ACTIVE_SESSION_ID_ENV` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L15)
- `DAEMON_WORKER_RECOVERY_JOURNAL_ENV` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L17)
- `DAEMON_WORKER_ROLE_ENV` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L13)
- `DAEMON_WORKER_STARTUP_GATE_COMMIT` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L19)
- `DAEMON_WORKER_STARTUP_GATE_FD_ENV` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L18)
- `DAEMON_WORKER_SUPERVISOR_SOCKET_ENV` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L16)
- `DAEMON_WORKER_TOKEN_ENV` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-protocol.ts#L14)


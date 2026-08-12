---
title: 'Module: packages/coding-agent/src/modes/daemon/daemon-supervisor.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/daemon-supervisor.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`daemon-supervisor.ts`/
symbols:
  DaemonSupervisor.handleCommand: DaemonSupervisor#handleCommand().
  DaemonSupervisor.handleWorkerFrame: DaemonSupervisor#handleWorkerFrame().
  ResidentWorker.descriptor: ResidentWorker#descriptor.
  DaemonSupervisor.launchWorker: DaemonSupervisor#launchWorker().
  DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type: DaemonSupervisor#attachClient().(command)Extract:typeLiteral2177:type.
  DaemonSupervisor.start: DaemonSupervisor#start().
  DaemonSupervisor.stopWorkerUntracked: DaemonSupervisor#stopWorkerUntracked().
  DaemonSupervisor.shutdown: DaemonSupervisor#shutdown().
  DaemonSupervisor.handleLine: DaemonSupervisor#handleLine().
  DaemonSupervisor.handleConnection: DaemonSupervisor#handleConnection().
  DaemonSupervisor.cleanupSupervisorResourcesOnce: DaemonSupervisor#cleanupSupervisorResourcesOnce().
  DaemonSupervisor.refreshWorkerSummaries: DaemonSupervisor#refreshWorkerSummaries().
  DaemonSupervisor.-constructor: DaemonSupervisor#`<constructor>`().
  DaemonSupervisor.agentPeerSummary: DaemonSupervisor#agentPeerSummary().
  DaemonSupervisor.recoverWorker: DaemonSupervisor#recoverWorker().
  DaemonSupervisor: DaemonSupervisor#
  DaemonSupervisor.getOrCreateTranscriptCache: DaemonSupervisor#getOrCreateTranscriptCache().
  DaemonSupervisor.createOrReuseWorker: DaemonSupervisor#createOrReuseWorker().
  DaemonSupervisor.runIdleEvictionSweep: DaemonSupervisor#runIdleEvictionSweep().
  ResidentWorker: ResidentWorker#
  DaemonSupervisor.drainClientCatchups: DaemonSupervisor#drainClientCatchups().
  DaemonSupervisor.recoverUncertainWorkerOperations: DaemonSupervisor#recoverUncertainWorkerOperations().
  DaemonSupervisor.workerEvictionSnapshot: DaemonSupervisor#workerEvictionSnapshot().
  WorkerMatch.worker: WorkerMatch#worker.
  DaemonSupervisor.prepareUpdateRestartFenced: DaemonSupervisor#prepareUpdateRestartFenced().
  DaemonSupervisor.adoptOrRecoverWorker: DaemonSupervisor#adoptOrRecoverWorker().
  DaemonSupervisor.handleWorkerClose: DaemonSupervisor#handleWorkerClose().
  DaemonSupervisor.log: DaemonSupervisor#log().
  DaemonSupervisor.finalizeTimedOutWorkerStop: DaemonSupervisor#finalizeTimedOutWorkerStop().
  DaemonSupervisor.cacheLoadedSnapshot: DaemonSupervisor#cacheLoadedSnapshot().
  DaemonSupervisor.streamSnapshot: DaemonSupervisor#streamSnapshot().
  DaemonSupervisor.connectWorker: DaemonSupervisor#connectWorker().
  DaemonSupervisor.forwardToWorker: DaemonSupervisor#forwardToWorker().
  ResidentWorker.client: ResidentWorker#client.
  DaemonSupervisor.loadWorkerDescriptors: DaemonSupervisor#loadWorkerDescriptors().
  DaemonSupervisor.failWorkerSnapshotCache: DaemonSupervisor#failWorkerSnapshotCache().
  DaemonSupervisor.familyCatalogEntry: DaemonSupervisor#familyCatalogEntry().
  DaemonSupervisor.workers: DaemonSupervisor#workers.
  DaemonSupervisor.syncAgentPeers: DaemonSupervisor#syncAgentPeers().
  DaemonSupervisor.handleList.command-Extract.typeLiteral1418.type: DaemonSupervisor#handleList().(command)Extract:typeLiteral1418:type.
  DaemonSupervisor.parseCommandAndRegisterPromptAdmission.typeLiteral846.admission: DaemonSupervisor#parseCommandAndRegisterPromptAdmission().typeLiteral846:admission.
  DaemonSupervisor.reclaimStaleWorkerRegistration: DaemonSupervisor#reclaimStaleWorkerRegistration().
  DaemonSupervisor.assertSavedSiblingNameAvailable: DaemonSupervisor#assertSavedSiblingNameAvailable().
  DaemonSupervisor.publicSummary: DaemonSupervisor#publicSummary().
  DaemonSupervisorOptions.defaultSessionConfig: DaemonSupervisorOptions#defaultSessionConfig.
  SnapshotTranscriptGeneration.transcript: SnapshotTranscriptGeneration#transcript.
  WorkerMatch.summary: WorkerMatch#summary.
  DaemonSupervisor.retireWorkerSnapshotCache: DaemonSupervisor#retireWorkerSnapshotCache().
  DaemonSupervisor.assertSupervisorSessionNameAvailable: DaemonSupervisor#assertSupervisorSessionNameAvailable().
  isDaemonWorkerDescriptor: isDaemonWorkerDescriptor().
  DaemonSupervisor.handleSavedSessionList.command-Extract.typeLiteral1475.type: DaemonSupervisor#handleSavedSessionList().(command)Extract:typeLiteral1475:type.
  DaemonSupervisor.write: DaemonSupervisor#write().
  DaemonSupervisorOptions.descriptorDir: DaemonSupervisorOptions#descriptorDir.
  mergeSessionLists: mergeSessionLists().
  DaemonSupervisor.resumeDeferredWorkerRecovery: DaemonSupervisor#resumeDeferredWorkerRecovery().
  DaemonSupervisor.failSnapshotGeneration: DaemonSupervisor#failSnapshotGeneration().
  ResidentWorker.transcriptCaches: ResidentWorker#transcriptCaches.
  DaemonSupervisor.familyCatalogEntries: DaemonSupervisor#familyCatalogEntries().
  DaemonSupervisor.assertSupervisorSavedSessionNameAvailable: DaemonSupervisor#assertSupervisorSavedSessionNameAvailable().
  DaemonSupervisor.finalizeArchivedWorkerStop: DaemonSupervisor#finalizeArchivedWorkerStop().
  DaemonSupervisor.promoteOwnedWorker: DaemonSupervisor#promoteOwnedWorker().
  DaemonSupervisor.findWorkerForClient: DaemonSupervisor#findWorkerForClient().
  DaemonSupervisor.assertRecoveryAllowed: DaemonSupervisor#assertRecoveryAllowed().
  DaemonSupervisor.scheduleOwnedWorkerCleanup: DaemonSupervisor#scheduleOwnedWorkerCleanup().
  DaemonSupervisor.findSummaryInWorker: DaemonSupervisor#findSummaryInWorker().
  DaemonSupervisor.persistWorker: DaemonSupervisor#persistWorker().
  DaemonSupervisor.detachClient: DaemonSupervisor#detachClient().
  DaemonSupervisor.validateAndPersistUpdateManifest: DaemonSupervisor#validateAndPersistUpdateManifest().
  DaemonSupervisor.createStreamedAttachResult: DaemonSupervisor#createStreamedAttachResult().
  ResidentWorker.snapshotCache: ResidentWorker#snapshotCache.
  DaemonSupervisor.matchWorkers: DaemonSupervisor#matchWorkers().
  DaemonSupervisor.supervisorAuthenticationClaim.typeLiteral584.supervisorSocketPath: DaemonSupervisor#supervisorAuthenticationClaim().typeLiteral584:supervisorSocketPath.
  DaemonSupervisor.savedSessionNameReservationInput.Promise.typeLiteral1261.parentSessionPath: DaemonSupervisor#savedSessionNameReservationInput().Promise:typeLiteral1261:parentSessionPath.
  DaemonSupervisor.scheduleIdleEvictionSweep: DaemonSupervisor#scheduleIdleEvictionSweep().
  DaemonSupervisor.isWorkerRecoveryCancelled: DaemonSupervisor#isWorkerRecoveryCancelled().
  DaemonSupervisor.reserveSnapshotStream: DaemonSupervisor#reserveSnapshotStream().
  DaemonSupervisor.cancelWaitingPromptAdmissionsForClient: DaemonSupervisor#cancelWaitingPromptAdmissionsForClient().
  DaemonSupervisor.deletePromptAdmission: DaemonSupervisor#deletePromptAdmission().
  DaemonSupervisor.isWorkerRecoveryCandidate: DaemonSupervisor#isWorkerRecoveryCandidate().
  DaemonSupervisor.scheduleCompactCatchup: DaemonSupervisor#scheduleCompactCatchup().
  DaemonSupervisor.requireAvailableWorkerClient: DaemonSupervisor#requireAvailableWorkerClient().
  ResidentWorker.summaries: ResidentWorker#summaries.
  DaemonSupervisor.shuttingDown: DaemonSupervisor#shuttingDown.
  DaemonSupervisor.clients: DaemonSupervisor#clients.
  DaemonSupervisor.syncWorkerExtensionUi: DaemonSupervisor#syncWorkerExtensionUi().
  DaemonSupervisor.currentSnapshotGeneration: DaemonSupervisor#currentSnapshotGeneration().
  ResidentWorker.ownerCleanupTimer: ResidentWorker#ownerCleanupTimer.
  DaemonSupervisor.subscribeWorker: DaemonSupervisor#subscribeWorker().
  DaemonSupervisor.catalog: DaemonSupervisor#catalog.
  DaemonSupervisor.loadPersistedSupervisorConfig: DaemonSupervisor#loadPersistedSupervisorConfig().
  DaemonSupervisor.summaryNameReservationInput.typeLiteral1414.parentSessionPath: DaemonSupervisor#summaryNameReservationInput().typeLiteral1414:parentSessionPath.
  DaemonSupervisor.prepareUpdateRestart: DaemonSupervisor#prepareUpdateRestart().
  DaemonSupervisor.effectiveWorkerState: DaemonSupervisor#effectiveWorkerState().
  DaemonSupervisor.protocolClientId: DaemonSupervisor#protocolClientId().
  DaemonSupervisor.catchUpClient: DaemonSupervisor#catchUpClient().
  DaemonSupervisor.runCleanupStep: DaemonSupervisor#runCleanupStep().
  ResidentWorker.intentionalStop: ResidentWorker#intentionalStop.
  DaemonSupervisor.deleteWorkerDescriptor: DaemonSupervisor#deleteWorkerDescriptor().
  DaemonSupervisor.isWorkerStopping: DaemonSupervisor#isWorkerStopping().
  DaemonSupervisor.persistWorkerStopTombstone: DaemonSupervisor#persistWorkerStopTombstone().
  ResidentWorker.snapshotGenerations: ResidentWorker#snapshotGenerations.
  WorkerAttachData.result: WorkerAttachData#result.
  DaemonSupervisor.deleteSnapshotGeneration: DaemonSupervisor#deleteSnapshotGeneration().
  SupervisorPromptAdmission.status: SupervisorPromptAdmission#status.
  DaemonSupervisor.persistSupervisorConfig: DaemonSupervisor#persistSupervisorConfig().
  DaemonSupervisor.scheduleOwnedWorkerCleanupForClient: DaemonSupervisor#scheduleOwnedWorkerCleanupForClient().
  DaemonSupervisor.drainClientCatchupQueue: DaemonSupervisor#drainClientCatchupQueue().
  runDaemonSupervisorMode: runDaemonSupervisorMode().
  DaemonSupervisor.withSessionNameReservation: DaemonSupervisor#withSessionNameReservation().
  DaemonSupervisor.isWorkerAccessibleToClient: DaemonSupervisor#isWorkerAccessibleToClient().
  DaemonSupervisor.updateRestartPhase: DaemonSupervisor#updateRestartPhase.
  DaemonSupervisor.descriptorDir: DaemonSupervisor#descriptorDir.
  ResidentWorker.snapshotLoads: ResidentWorker#snapshotLoads.
  SnapshotTranscriptGeneration.result: SnapshotTranscriptGeneration#result.
  DaemonSupervisor.defaultSessionConfig: DaemonSupervisor#defaultSessionConfig.
  DaemonSupervisor.reuseWorkerForCreate: DaemonSupervisor#reuseWorkerForCreate().
  DaemonSupervisor.findWorker: DaemonSupervisor#findWorker().
  DaemonSupervisor.findWorkerBySessionFile: DaemonSupervisor#findWorkerBySessionFile().
  DaemonSupervisor.invalidateWorkerSnapshot: DaemonSupervisor#invalidateWorkerSnapshot().
  DaemonSupervisor.stopWorker: DaemonSupervisor#stopWorker().
  DaemonSupervisor.workerSessionArtifactContext: DaemonSupervisor#workerSessionArtifactContext().
  DaemonSupervisor.settleSnapshotDuplicateValidation: DaemonSupervisor#settleSnapshotDuplicateValidation().
  attachResultFromResponse: attachResultFromResponse().
  idleEvictionSweepIntervalMs: idleEvictionSweepIntervalMs().
  DaemonSupervisor.ownership: DaemonSupervisor#ownership.
  DaemonSupervisor.isLiveWorker: DaemonSupervisor#isLiveWorker().
  DaemonSupervisor.queueCatchup: DaemonSupervisor#queueCatchup().
  DaemonSupervisor.getPromptAdmission: DaemonSupervisor#getPromptAdmission().
  DaemonSupervisor.writeSnapshotRecord: DaemonSupervisor#writeSnapshotRecord().
  DaemonSupervisor.cleanupSocket: DaemonSupervisor#cleanupSocket().
  DaemonSupervisor.snapshotGenerationsFor: DaemonSupervisor#snapshotGenerationsFor().
  DaemonSupervisor.snapshotGeneration: DaemonSupervisor#snapshotGeneration().
  DaemonSupervisor.assertTelemetryAttachAllowed: DaemonSupervisor#assertTelemetryAttachAllowed().
  ResidentWorker.heartbeatSnapshot: ResidentWorker#heartbeatSnapshot.
  DaemonSupervisor.assertCurrentOwnership: DaemonSupervisor#assertCurrentOwnership().
  SnapshotTranscriptGeneration.incoming: SnapshotTranscriptGeneration#incoming.
  DaemonSupervisor.promptAdmissions: DaemonSupervisor#promptAdmissions.
  DaemonSupervisor.cancelOwnedWorkerCleanup: DaemonSupervisor#cancelOwnedWorkerCleanup().
  DaemonSupervisor.createSnapshotDuplicateValidation: DaemonSupervisor#createSnapshotDuplicateValidation().
  DaemonSupervisor.isWorkerRecoveryEligible: DaemonSupervisor#isWorkerRecoveryEligible().
  DaemonSupervisor.isVisibleWorker: DaemonSupervisor#isVisibleWorker().
  DaemonSupervisor.writeSerialized: DaemonSupervisor#writeSerialized().
  DaemonSupervisor.reportCleanupFailure: DaemonSupervisor#reportCleanupFailure().
  ResidentWorker.stopRevision: ResidentWorker#stopRevision.
  DaemonSupervisor.broadcastHeartbeatsChanged: DaemonSupervisor#broadcastHeartbeatsChanged().
  ResidentWorker.updateRestartPrepareClient: ResidentWorker#updateRestartPrepareClient.
  SnapshotTranscriptGeneration.validation: SnapshotTranscriptGeneration#validation.
  WorkerMatch: WorkerMatch#
  throwIfAdmissionCancelled: throwIfAdmissionCancelled().
  DaemonSupervisor.socketLease: DaemonSupervisor#socketLease.
  DaemonSupervisor.deferWorkerRecovery: DaemonSupervisor#deferWorkerRecovery().
  DaemonSupervisor.assertWorkerAccessibleToClient: DaemonSupervisor#assertWorkerAccessibleToClient().
  DaemonSupervisor.writeSnapshotBuffer: DaemonSupervisor#writeSnapshotBuffer().
  DaemonSupervisor.scheduleWorkerStopFinalization: DaemonSupervisor#scheduleWorkerStopFinalization().
  SupervisorPromptAdmission: SupervisorPromptAdmission#
  isSupervisorRecoveryCancelled: isSupervisorRecoveryCancelled().
  DaemonSupervisor.server: DaemonSupervisor#server.
  DaemonSupervisor.processIdentity: DaemonSupervisor#processIdentity().
  SnapshotTranscriptGeneration.duplicateResult: SnapshotTranscriptGeneration#duplicateResult.
  SupervisorPromptAdmission.worker: SupervisorPromptAdmission#worker.
  isSessionSummary: isSessionSummary().
  sessionSummariesFromResponse: sessionSummariesFromResponse().
  DaemonSupervisor.commandJournal: DaemonSupervisor#commandJournal.
  DaemonSupervisor.streamReconstructor: DaemonSupervisor#streamReconstructor.
  DaemonSupervisor.promptAdmissionsFor: DaemonSupervisor#promptAdmissionsFor().
  DaemonSupervisor.reclaimStoppedWorkerCronLock: DaemonSupervisor#reclaimStoppedWorkerCronLock().
  DaemonSupervisor.registerSignalHandlers: DaemonSupervisor#registerSignalHandlers().
  ResidentWorker.launchEnv: ResidentWorker#launchEnv.
  DaemonSupervisor.snapshotCacheRoot: DaemonSupervisor#snapshotCacheRoot.
  DaemonSupervisor.attachClient: DaemonSupervisor#attachClient().
  PersistedSupervisorConfig.defaultSessionConfig: PersistedSupervisorConfig#defaultSessionConfig.
  DaemonSupervisor.mutationDrain: DaemonSupervisor#mutationDrain.
  DaemonSupervisor.openingWorkers: DaemonSupervisor#openingWorkers.
  DaemonCommandBody: DaemonCommandBody#
  ResidentWorker.descriptorPath: ResidentWorker#descriptorPath.
  ResidentWorker.recovery: ResidentWorker#recovery.
  SnapshotTranscriptGeneration: SnapshotTranscriptGeneration#
  withoutCommandId: withoutCommandId().
  withoutSupervisorCreateFields: withoutSupervisorCreateFields().
  cronJobsFromResponse: cronJobsFromResponse().
  DaemonSupervisor.idleEvictionTimer: DaemonSupervisor#idleEvictionTimer.
  WorkerAttachData.worker: WorkerAttachData#worker.
  DaemonSupervisor.socketIdentity: DaemonSupervisor#socketIdentity.
  DaemonSupervisor.workerStopCounts: DaemonSupervisor#workerStopCounts.
  DaemonSupervisor.settingsManager: DaemonSupervisor#settingsManager.
  SnapshotTranscriptGeneration.duplicateChunkIndex: SnapshotTranscriptGeneration#duplicateChunkIndex.
  SupervisorPromptAdmission.controller: SupervisorPromptAdmission#controller.
  heartbeatsFromResponse: heartbeatsFromResponse().
  sortCronJobs: sortCronJobs().
  workerSocketPath: workerSocketPath().
  normalizeCapabilities: normalizeCapabilities().
  DaemonSupervisor.generation: DaemonSupervisor#generation.
  DaemonSupervisor.idleEvictionSweep: DaemonSupervisor#idleEvictionSweep.
  DaemonSupervisor.hasPersistedWorkerDescriptors: DaemonSupervisor#hasPersistedWorkerDescriptors().
  DaemonSupervisor.handleList: DaemonSupervisor#handleList().
  DaemonSupervisor.handleSavedSessionList: DaemonSupervisor#handleSavedSessionList().
  DaemonSupervisor.cleanupSupervisorResources: DaemonSupervisor#cleanupSupervisorResources().
  WorkerAttachData.transcript: WorkerAttachData#transcript.
  DaemonSupervisor.summaryNameReservationInput: DaemonSupervisor#summaryNameReservationInput().
  SnapshotTranscriptGeneration.retired: SnapshotTranscriptGeneration#retired.
  SupervisorPromptAdmission.workerActiveSessionId: SupervisorPromptAdmission#workerActiveSessionId.
  isSupervisorGenerationStale: isSupervisorGenerationStale().
  DaemonSupervisor.supervisorConfigPath: DaemonSupervisor#supervisorConfigPath.
  DaemonSupervisor.idleEvictionFence: DaemonSupervisor#idleEvictionFence.
  DaemonSupervisor.stopWorker.directChild-typeLiteral2814.closed: DaemonSupervisor#stopWorker().(directChild)typeLiteral2814:closed.
  SupervisorPromptAdmission.client: SupervisorPromptAdmission#client.
  isSupervisorShutdownAdmissionCancelled: isSupervisorShutdownAdmissionCancelled().
  responseWithId: responseWithId().
  DaemonSupervisor.protocolClientIds: DaemonSupervisor#protocolClientIds.
  DaemonSupervisor.clearIdleEvictionTimer: DaemonSupervisor#clearIdleEvictionTimer().
  DaemonSupervisor.parseCommandAndRegisterPromptAdmission: DaemonSupervisor#parseCommandAndRegisterPromptAdmission().
  DaemonSupervisor.parseCommandAndRegisterPromptAdmission.typeLiteral846.command: DaemonSupervisor#parseCommandAndRegisterPromptAdmission().typeLiteral846:command.
  ResidentWorker.heartbeatSnapshotStale: ResidentWorker#heartbeatSnapshotStale.
  ResidentWorker.stopFinalization: ResidentWorker#stopFinalization.
  SnapshotTranscriptGeneration.end: SnapshotTranscriptGeneration#end.
  WorkerAttachData.releaseTranscript: WorkerAttachData#releaseTranscript.
  SupervisorPromptAdmission.workerAdmissionId: SupervisorPromptAdmission#workerAdmissionId.
  delay: delay().
  unrefDelay: unrefDelay().
  DaemonSupervisor.ready: DaemonSupervisor#ready.
  DaemonSupervisor.cleanupPromise: DaemonSupervisor#cleanupPromise.
  DaemonSupervisor.signalCleanupHandlers: DaemonSupervisor#signalCleanupHandlers.
  DaemonSupervisor.stopWorkerUntracked.directChild-typeLiteral2821.child: DaemonSupervisor#stopWorkerUntracked().(directChild)typeLiteral2821:child.
  structuredLog: structuredLog.
  commitWorkerStartupGate: commitWorkerStartupGate().
  defaultWorkerDescriptorDir: defaultWorkerDescriptorDir().
  DaemonSupervisor.listen: DaemonSupervisor#listen().
  WORKER_REQUEST_TIMEOUT_MS: WORKER_REQUEST_TIMEOUT_MS.
  SUPERVISOR_CONFIG_FILE_NAME: SUPERVISOR_CONFIG_FILE_NAME.
  ResidentWorker.deferredRecovery: ResidentWorker#deferredRecovery.
  SnapshotDuplicateValidation.promise: SnapshotDuplicateValidation#promise.
  SupervisorRecoveryCancelledError: SupervisorRecoveryCancelledError#
  DaemonSupervisor.ownsSocketPath: DaemonSupervisor#ownsSocketPath.
  DaemonSupervisor.compactCatchupInProgress: DaemonSupervisor#compactCatchupInProgress.
  DaemonSupervisor.pendingSessionNames: DaemonSupervisor#pendingSessionNames.
  DaemonSupervisor.promptAdmissionKey: DaemonSupervisor#promptAdmissionKey().
  UPDATE_RESTART_WORKER_REQUEST_TIMEOUT_MS: UPDATE_RESTART_WORKER_REQUEST_TIMEOUT_MS.
  WORKER_RETRY_DELAYS_MS: WORKER_RETRY_DELAYS_MS.
  LIVENESS_IDENTITY_RECHECK_MS: LIVENESS_IDENTITY_RECHECK_MS.
  IDLE_EVICTION_MAX_SWEEP_INTERVAL_MS: IDLE_EVICTION_MAX_SWEEP_INTERVAL_MS.
  WORKER_STARTUP_GATE_FD: WORKER_STARTUP_GATE_FD.
  ResidentWorker.promotedOwnerClientId: ResidentWorker#promotedOwnerClientId.
  SnapshotDuplicateValidation: SnapshotDuplicateValidation#
  SnapshotDuplicateValidation.resolve: SnapshotDuplicateValidation#resolve.
  SnapshotDuplicateValidation.reject: SnapshotDuplicateValidation#reject.
  SnapshotTranscriptGeneration.begin: SnapshotTranscriptGeneration#begin.
  DaemonSupervisorOptions: DaemonSupervisorOptions#
  DaemonSupervisorOptions.socketPath: DaemonSupervisorOptions#socketPath.
  PersistedSupervisorConfig: PersistedSupervisorConfig#
  PersistedSupervisorConfig.version: PersistedSupervisorConfig#version.
  PersistedSupervisorConfig.socketPath: PersistedSupervisorConfig#socketPath.
  SnapshotLoadInvalidatedError: SnapshotLoadInvalidatedError#
  WorkerStopTimeoutError: WorkerStopTimeoutError#
  descriptorKey: descriptorKey().
  looksLikeSessionPath: looksLikeSessionPath().
  DaemonSupervisor.markReady: DaemonSupervisor#markReady.
  DaemonSupervisor.rejectReady: DaemonSupervisor#rejectReady.
  DaemonSupervisor.agentPeerSyncQueue: DaemonSupervisor#agentPeerSyncQueue.
  DaemonSupervisor.parseCommandAndRegisterPromptAdmission.typeLiteral846.envelopeClientId: DaemonSupervisor#parseCommandAndRegisterPromptAdmission().typeLiteral846:envelopeClientId.
  DaemonSupervisor.parseCommandAndRegisterPromptAdmission.typeLiteral846.protocolVersion: DaemonSupervisor#parseCommandAndRegisterPromptAdmission().typeLiteral846:protocolVersion.
  DaemonSupervisor.summaryNameReservationInput.typeLiteral1414.name: DaemonSupervisor#summaryNameReservationInput().typeLiteral1414:name.
  DistributiveOmit: DistributiveOmit#
  WORKER_CONNECT_TIMEOUT_MS: WORKER_CONNECT_TIMEOUT_MS.
  UPDATE_RESTART_MUTATION_DRAIN_TIMEOUT_MS: UPDATE_RESTART_MUTATION_DRAIN_TIMEOUT_MS.
  UPDATE_RESTART_PREPARE_DEADLINE_MS: UPDATE_RESTART_PREPARE_DEADLINE_MS.
  DEFERRED_RECOVERY_RECHECK_MS: DEFERRED_RECOVERY_RECHECK_MS.
  STOP_FINALIZATION_RECHECK_MS: STOP_FINALIZATION_RECHECK_MS.
  STOP_FINALIZATION_SIGKILL_GRACE_MS: STOP_FINALIZATION_SIGKILL_GRACE_MS.
  STOP_FINALIZATION_RETRY_MS: STOP_FINALIZATION_RETRY_MS.
  STALE_RECLAIM_WAIT_MS: STALE_RECLAIM_WAIT_MS.
  OWNED_WORKER_DISCONNECT_GRACE_MS: OWNED_WORKER_DISCONNECT_GRACE_MS.
  IDLE_EVICTION_MIN_SWEEP_INTERVAL_MS: IDLE_EVICTION_MIN_SWEEP_INTERVAL_MS.
  IDLE_EVICTION_DRAIN_TIMEOUT_MS: IDLE_EVICTION_DRAIN_TIMEOUT_MS.
  CHILD_PASSIVATION_PER_WORKER_CAP: CHILD_PASSIVATION_PER_WORKER_CAP.
  DAEMON_COMMAND_TYPES: DAEMON_COMMAND_TYPES.
  WorkerAttachData: WorkerAttachData#
  SupervisorPromptAdmission.activeSessionId: SupervisorPromptAdmission#activeSessionId.
  SupervisorPromptAdmission.publicAdmissionId: SupervisorPromptAdmission#publicAdmissionId.
  isFinalizedTranscriptEvent: isFinalizedTranscriptEvent().
  DaemonSupervisor.supervisorAuthenticationClaim: DaemonSupervisor#supervisorAuthenticationClaim().
  DaemonSupervisor.supervisorAuthenticationClaim.typeLiteral584.supervisorGeneration: DaemonSupervisor#supervisorAuthenticationClaim().typeLiteral584:supervisorGeneration.
  DaemonSupervisor.supervisorAuthenticationClaim.typeLiteral584.supervisorPid: DaemonSupervisor#supervisorAuthenticationClaim().typeLiteral584:supervisorPid.
  DaemonSupervisor.supervisorAuthenticationClaim.typeLiteral584.supervisorProcessStartId: DaemonSupervisor#supervisorAuthenticationClaim().typeLiteral584:supervisorProcessStartId.
  DaemonSupervisor.withSessionNameReservation.input-typeLiteral1984.name: DaemonSupervisor#withSessionNameReservation().(input)typeLiteral1984:name.
  DaemonSupervisor.withSessionNameReservation.input-typeLiteral1984.depth: DaemonSupervisor#withSessionNameReservation().(input)typeLiteral1984:depth.
  DaemonSupervisor.savedSessionNameReservationInput: DaemonSupervisor#savedSessionNameReservationInput().
  DaemonSupervisor.savedSessionNameReservationInput.Promise.typeLiteral1261.name: DaemonSupervisor#savedSessionNameReservationInput().Promise:typeLiteral1261:name.
  DaemonSupervisor.summaryNameReservationInput.typeLiteral1414.depth: DaemonSupervisor#summaryNameReservationInput().typeLiteral1414:depth.
  DaemonSupervisor.summaryNameReservationInput.typeLiteral1414.parentSessionId: DaemonSupervisor#summaryNameReservationInput().typeLiteral1414:parentSessionId.
  DaemonSupervisor.stopWorkerUntracked.directChild-typeLiteral2821.closed: DaemonSupervisor#stopWorkerUntracked().(directChild)typeLiteral2821:closed.
  SupervisorRecoveryCancelledError.code: SupervisorRecoveryCancelledError#code.
  DaemonSupervisor.withSessionNameReservation.input-typeLiteral1984.parentSessionId: DaemonSupervisor#withSessionNameReservation().(input)typeLiteral1984:parentSessionId.
  DaemonSupervisor.withSessionNameReservation.input-typeLiteral1984.parentSessionPath: DaemonSupervisor#withSessionNameReservation().(input)typeLiteral1984:parentSessionPath.
  DaemonSupervisor.savedSessionNameReservationInput.Promise.typeLiteral1261.depth: DaemonSupervisor#savedSessionNameReservationInput().Promise:typeLiteral1261:depth.
  DaemonSupervisor.savedSessionNameReservationInput.Promise.typeLiteral1261.parentSessionId: DaemonSupervisor#savedSessionNameReservationInput().Promise:typeLiteral1261:parentSessionId.
  DaemonSupervisor.stopWorker.directChild-typeLiteral2814.child: DaemonSupervisor#stopWorker().(directChild)typeLiteral2814:child.
---
# Module: [`packages/coding-agent/src/modes/daemon/daemon-supervisor.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts)

## Classes
### `DaemonCommandBody`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor.ts:126`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L126)
- signature: `type DaemonCommandBody`
- uses (calls/refs, reference-scoped): [`DaemonCommand`](daemon-protocol.ts.md#DaemonCommand), [`DistributiveOmit`](daemon-supervisor.ts.md#DistributiveOmit)
- used by: [`withoutCommandId`](daemon-supervisor.ts.md#withoutCommandId)

### `DaemonSupervisor`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor.ts:583`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L583)
- signature: `class DaemonSupervisor`
- members:
  - `<constructor>(socketPath: string, options: DaemonSupervisorOptions)` — [`L620`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L620)
  - `adoptOrRecoverWorker(method)` — [`L2424`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2424)
  - `agentPeerSummary(method)` — [`L3205`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3205)
  - `assertCurrentOwnership(method)` — [`L885`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L885)
  - `assertRecoveryAllowed(method)` — [`L895`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L895)
  - `assertSavedSiblingNameAvailable(method)` — [`L3098`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3098)
  - `assertSupervisorSavedSessionNameAvailable(method)` — [`L3082`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3082)
  - `assertSupervisorSessionNameAvailable(method)` — [`L3037`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3037)
  - `assertTelemetryAttachAllowed(method)` — [`L3528`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3528)
  - `assertWorkerAccessibleToClient(method)` — [`L3270`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3270)
  - `attachClient(method)` — [`L3351`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3351)
  - `broadcastHeartbeatsChanged(method)` — [`L4947`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4947)
  - `cacheLoadedSnapshot(method)` — [`L3536`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3536)
  - `cancelOwnedWorkerCleanup(method)` — [`L1075`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1075)
  - `cancelWaitingPromptAdmissionsForClient(method)` — [`L1154`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1154)
  - `catchUpClient(method)` — [`L4296`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4296)
  - `cleanupSocket(method)` — [`L4979`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4979)
  - `cleanupSupervisorResources(method)` — [`L4989`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4989)
  - `cleanupSupervisorResourcesOnce(method)` — [`L4997`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4997)
  - `clearIdleEvictionTimer(method)` — [`L746`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L746)
  - `connectWorker(method)` — [`L2372`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2372)
  - `createOrReuseWorker(method)` — [`L1997`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1997)
  - `createSnapshotDuplicateValidation(method)` — [`L2749`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2749)
  - `createStreamedAttachResult(method)` — [`L3638`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3638)
  - `currentSnapshotGeneration(method)` — [`L2685`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2685)
  - `deferWorkerRecovery(method)` — [`L2551`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2551)
  - `deletePromptAdmission(method)` — [`L1146`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1146)
  - `deleteSnapshotGeneration(method)` — [`L2714`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2714)
  - `deleteWorkerDescriptor(method)` — [`L997`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L997)
  - `detachClient(method)` — [`L3800`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3800)
  - `drainClientCatchupQueue(method)` — [`L4312`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4312)
  - `drainClientCatchups(method)` — [`L4323`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4323)
  - `effectiveWorkerState(method)` — [`L3169`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3169) — The lifecycle reported to clients. A stop intent always wins, and a worker
  - `failSnapshotGeneration(method)` — [`L2731`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2731)
  - `failWorkerSnapshotCache(method)` — [`L2592`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2592)
  - `familyCatalogEntries(method)` — [`L3006`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3006)
  - `familyCatalogEntry(method)` — [`L3190`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3190)
  - `finalizeArchivedWorkerStop(method)` — [`L4899`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4899)
  - `finalizeTimedOutWorkerStop(method)` — [`L4814`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4814)
  - `findSummaryInWorker(method)` — [`L3299`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3299)
  - `findWorker(method)` — [`L3239`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3239)
  - `findWorkerBySessionFile(method)` — [`L3322`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3322)
  - `findWorkerForClient(method)` — [`L3259`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3259)
  - `forwardToWorker(method)` — [`L3334`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3334)
  - `getOrCreateTranscriptCache(method)` — [`L3597`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3597)
  - `getPromptAdmission(method)` — [`L1138`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1138)
  - `handleCommand(method)` — [`L1380`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1380)
  - `handleConnection(method)` — [`L1009`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1009)
  - `handleLine(method)` — [`L1231`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1231)
  - `handleList(method)` — [`L1921`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1921)
  - `handleSavedSessionList(method)` — [`L1956`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1956)
  - `handleWorkerClose(method)` — [`L2483`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2483)
  - `handleWorkerFrame(method)` — [`L3825`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3825)
  - `hasPersistedWorkerDescriptors(method)` — [`L983`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L983)
  - `invalidateWorkerSnapshot(method)` — [`L4251`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4251)
  - `isLiveWorker(method)` — [`L3161`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3161) — Live workers are visible to all clients and not stopping.
  - `isVisibleWorker(method)` — [`L3151`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3151)
  - `isWorkerAccessibleToClient(method)` — [`L3263`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3263)
  - `isWorkerRecoveryCancelled(method)` — [`L2879`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2879)
  - `isWorkerRecoveryCandidate(method)` — [`L2541`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2541)
  - `isWorkerRecoveryEligible(method)` — [`L2537`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2537)
  - `isWorkerStopping(method)` — [`L3156`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3156) — A worker with a durable or in-memory stop intent is stopping, never live.
  - `launchWorker(method)` — [`L2137`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2137) — documented in [packages-coding-agent-src-modes-daemon-daemon-supervisor.ts](../../../../../../concepts/packages-coding-agent-src-modes-daemon-daemon-supervisor.ts.md)
  - `listen(method)` — [`L724`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L724)
  - `loadPersistedSupervisorConfig(method)` — [`L951`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L951)
  - `loadWorkerDescriptors(method)` — [`L920`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L920)
  - `log(method)` — [`L740`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L740)
  - `matchWorkers(method)` — [`L3276`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3276)
  - `parseCommandAndRegisterPromptAdmission(method)` — [`L1187`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1187) — Non-async by design: prompt registration completes before handleLine's first await.
  - `persistSupervisorConfig(method)` — [`L971`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L971)
  - `persistWorker(method)` — [`L989`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L989)
  - `persistWorkerStopTombstone(method)` — [`L4936`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4936)
  - `prepareUpdateRestart(method)` — [`L4409`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4409)
  - `prepareUpdateRestartFenced(method)` — [`L4427`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4427)
  - `processIdentity(method)` — [`L4610`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4610) — Verdict on whether a pid is still the process we launched. Callers must
  - `promoteOwnedWorker(method)` — [`L2112`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2112)
  - `promptAdmissionKey(method)` — [`L1125`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1125)
  - `promptAdmissionsFor(method)` — [`L1129`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1129)
  - `protocolClientId(method)` — [`L1085`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1085)
  - `publicSummary(method)` — [`L3228`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3228)
  - `queueCatchup(method)` — [`L4281`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4281)
  - `reclaimStaleWorkerRegistration(method)` — [`L2079`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2079) — A stopping worker whose process already died can strand its registration
  - `reclaimStoppedWorkerCronLock(method)` — [`L4915`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4915)
  - `recoverUncertainWorkerOperations(method)` — [`L2888`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2888)
  - `recoverWorker(method)` — [`L2773`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2773)
  - `refreshWorkerSummaries(method)` — [`L2968`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2968)
  - `registerSignalHandlers(method)` — [`L4964`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4964)
  - `reportCleanupFailure(method)` — [`L5078`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L5078)
  - `requireAvailableWorkerClient(method)` — [`L3179`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3179)
  - `reserveSnapshotStream(method)` — [`L3735`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3735)
  - `resumeDeferredWorkerRecovery(method)` — [`L2560`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2560)
  - `retireWorkerSnapshotCache(method)` — [`L2639`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2639)
  - `reuseWorkerForCreate(method)` — [`L2061`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2061)
  - `runCleanupStep(method)` — [`L5070`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L5070)
  - `runIdleEvictionSweep(method)` — [`L793`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L793)
  - `savedSessionNameReservationInput(method)` — [`L3050`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3050)
  - `scheduleCompactCatchup(method)` — [`L4264`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4264)
  - `scheduleIdleEvictionSweep(method)` — [`L752`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L752)
  - `scheduleOwnedWorkerCleanup(method)` — [`L1100`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1100)
  - `scheduleOwnedWorkerCleanupForClient(method)` — [`L1089`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1089)
  - `scheduleWorkerStopFinalization(method)` — [`L4805`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4805) — A stop that timed out leaves a tombstoned registration behind. Keep
  - `settleSnapshotDuplicateValidation(method)` — [`L2760`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2760)
  - `shutdown(method)` — [`L5087`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L5087)
  - `snapshotGeneration(method)` — [`L2677`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2677)
  - `snapshotGenerationsFor(method)` — [`L2664`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2664)
  - `start(method)` — [`L641`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L641)
  - `stopWorker(method)` — [`L4627`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4627)
  - `stopWorkerUntracked(method)` — [`L4647`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4647)
  - `streamSnapshot(method)` — [`L3654`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3654)
  - `subscribeWorker(method)` — [`L2404`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L2404)
  - `summaryNameReservationInput(method)` — [`L3069`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3069)
  - `supervisorAuthenticationClaim(method)` — [`L902`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L902)
  - `syncAgentPeers(method)` — [`L3122`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3122)
  - `syncWorkerExtensionUi(method)` — [`L3815`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3815)
  - `validateAndPersistUpdateManifest(method)` — [`L4561`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4561)
  - `withSessionNameReservation(method)` — [`L3021`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3021)
  - `workerEvictionSnapshot(method)` — [`L768`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L768)
  - `workerSessionArtifactContext(method)` — [`L4923`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4923)
  - `write(method)` — [`L4943`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4943)
  - `writeSerialized(method)` — [`L4953`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4953)
  - `writeSnapshotBuffer(method)` — [`L3773`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3773)
  - `writeSnapshotRecord(method)` — [`L3769`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3769)
  - `admission` — [`L1194`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1194)
  - `agentPeerSyncQueue` — [`L612`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L612)
  - `catalog` — [`L614`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L614)
  - `child` — [`L4633`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4633)
  - `child` — [`L4653`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4653)
  - `cleanupPromise` — [`L592`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L592)
  - `clients` — [`L596`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L596)
  - `closed` — [`L4633`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4633)
  - `closed` — [`L4653`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L4653)
  - `command` — [`L1191`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1191)
  - `commandJournal` — [`L609`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L609)
  - `compactCatchupInProgress` — [`L611`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L611)
  - `defaultSessionConfig` — [`L607`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L607)
  - `depth` — [`L3022`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3022)
  - `depth` — [`L3053`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3053)
  - `depth` — [`L3072`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3072)
  - `descriptorDir` — [`L604`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L604)
  - `envelopeClientId` — [`L1192`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1192)
  - `generation` — [`L605`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L605)
  - `idleEvictionFence` — [`L618`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L618)
  - `idleEvictionSweep` — [`L617`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L617)
  - `idleEvictionTimer` — [`L616`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L616)
  - `markReady` — [`L586`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L586)
  - `mutationDrain` — [`L595`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L595)
  - `name` — [`L3022`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3022)
  - `name` — [`L3053`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3053)
  - `name` — [`L3072`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3072)
  - `openingWorkers` — [`L600`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L600)
  - `ownership` — [`L591`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L591)
  - `ownsSocketPath` — [`L588`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L588)
  - `parentSessionId` — [`L3022`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3022)
  - `parentSessionId` — [`L3053`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3053)
  - `parentSessionId` — [`L3072`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3072)
  - `parentSessionPath` — [`L3022`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3022)
  - `parentSessionPath` — [`L3053`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3053)
  - `parentSessionPath` — [`L3072`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3072)
  - `pendingSessionNames` — [`L613`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L613)
  - `promptAdmissions` — [`L602`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L602) — Public admission ids are scoped to the socket that registered them.
  - `protocolClientIds` — [`L597`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L597)
  - `protocolVersion` — [`L1193`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1193)
  - `ready` — [`L585`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L585)
  - `rejectReady` — [`L587`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L587)
  - `server` — [`L584`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L584)
  - `settingsManager` — [`L615`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L615)
  - `shuttingDown` — [`L593`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L593)
  - `signalCleanupHandlers` — [`L603`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L603)
  - `snapshotCacheRoot` — [`L608`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L608)
  - `socketIdentity` — [`L589`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L589)
  - `socketLease` — [`L590`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L590)
  - `streamReconstructor` — [`L610`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L610)
  - `supervisorConfigPath` — [`L606`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L606)
  - `supervisorGeneration` — [`L903`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L903)
  - `supervisorPid` — [`L904`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L904)
  - `supervisorProcessStartId` — [`L905`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L905)
  - `supervisorSocketPath` — [`L906`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L906)
  - `type` — [`L1923`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1923)
  - `type` — [`L1958`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L1958)
  - `type` — [`L3353`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L3353)
  - `updateRestartPhase` — [`L594`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L594)
  - `workerStopCounts` — [`L599`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L599)
  - `workers` — [`L598`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L598)
- uses (calls/refs, reference-scoped): [`role`](../../../../ai/src/types.ts.md#AssistantMessage.role), [`role`](../../../../ai/src/types.ts.md#ToolResultMessage.role), [`role`](../../../../ai/src/types.ts.md#UserMessage.role), [`role`](../../core/messages.ts.md#CustomMessage.role), [`role`](../../core/messages.ts.md#BashExecutionMessage.role), [`role`](../../core/messages.ts.md#BranchSummaryMessage.role), [`role`](../../core/messages.ts.md#CompactionSummaryMessage.role), [`id`](../../core/cron-jobs.ts.md#AgentCronJob.id), [`DaemonCommand`](daemon-protocol.ts.md#DaemonCommand), [`DaemonSocketClient`](active-session-state.ts.md#DaemonSocketClient), [`SettingsManager`](../../core/settings-manager.ts.md#SettingsManager), [`activeSessionId`](daemon-session-list.ts.md#SessionSummary.activeSessionId), [`SessionSummary`](daemon-session-list.ts.md#SessionSummary), [`AgentCronJob`](../../core/cron-jobs.ts.md#AgentCronJob), [`cwd`](../../core/agent-session-config.ts.md#AgentSessionRuntimeConfig.cwd), [`descriptor`](daemon-supervisor.ts.md#ResidentWorker.descriptor), [`sessionId`](daemon-session-list.ts.md#SessionSummary.sessionId), [`id`](daemon-session-list.ts.md#SessionSummary.id), [`agentDir`](../../core/agent-session-config.ts.md#AgentSessionRuntimeConfig.agentDir), [`DaemonOutbound`](daemon-protocol.ts.md#DaemonOutbound), [`success`](daemon-protocol.ts.md#success), [`acquireDaemonSupervisorOwnership`](daemon-supervisor-ownership.ts.md#acquireDaemonSupervisorOwnership), [`summaryForInactiveSession`](daemon-session-list.ts.md#summaryForInactiveSession), [`sessionFile`](daemon-session-list.ts.md#SessionSummary.sessionFile), [`mergeAgentSessionRuntimeConfig`](../../core/agent-session-config.ts.md#mergeAgentSessionRuntimeConfig), [`status`](../../core/cron-jobs.ts.md#AgentCronJob.status), [`create`](../../core/settings-manager.ts.md#SettingsManager.create), [`DaemonAttachResult`](daemon-protocol.ts.md#DaemonAttachResult), [`snapshot`](daemon-protocol.ts.md#DaemonAttachResult.snapshot), [`socket`](active-session-state.ts.md#DaemonSocketClient.socket), [`sessionName`](daemon-session-list.ts.md#SessionSummary.sessionName), [`DaemonResponse`](daemon-protocol.ts.md#DaemonResponse), [`serializeSavedSessionInfo`](saved-session-info.ts.md#serializeSavedSessionInfo), [`workerPid`](daemon-session-list.ts.md#SessionSummary.workerPid), [`getProcessStartId`](../../core/session-lease.ts.md#getProcessStartId), [`ResidentWorker`](daemon-supervisor.ts.md#ResidentWorker), [`AgentConnectionHeartbeat`](../agent-connection/types.ts.md#AgentConnectionHeartbeat), [`SessionInfo`](../../core/session-manager.ts.md#SessionInfo), [`id`](../../core/session-manager.ts.md#SessionInfo.id), [`attachedActiveSessionIds`](active-session-state.ts.md#DaemonSocketClient.attachedActiveSessionIds)  (+407 more)
- used by: [`runDaemonSupervisorMode`](daemon-supervisor.ts.md#runDaemonSupervisorMode)  (17 test-only)

### `DaemonSupervisorOptions`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor.ts:296`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L296)
- signature: `interface DaemonSupervisorOptions`
- members:
  - `defaultSessionConfig` — [`L298`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L298)
  - `descriptorDir` — [`L299`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L299)
  - `socketPath` — [`L297`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L297)
- uses (calls/refs, reference-scoped): [`AgentSessionRuntimeConfig`](../../core/agent-session-config.ts.md#AgentSessionRuntimeConfig)
- used by: [`main`](../../main.ts.md#main), [`<constructor>`](daemon-supervisor.ts.md#DaemonSupervisor.-constructor), [`runDaemonSupervisorMode`](daemon-supervisor.ts.md#runDaemonSupervisorMode)  (8 test-only)

### `DistributiveOmit`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor.ts:125`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L125)
- signature: `type DistributiveOmit`
- used by: [`DaemonCommandBody`](daemon-supervisor.ts.md#DaemonCommandBody)

### `PersistedSupervisorConfig`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor.ts:302`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L302)
- signature: `interface PersistedSupervisorConfig`
- members:
  - `defaultSessionConfig` — [`L305`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L305)
  - `socketPath` — [`L304`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L304)
  - `version` — [`L303`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L303)
- uses (calls/refs, reference-scoped): [`AgentSessionRuntimeConfig`](../../core/agent-session-config.ts.md#AgentSessionRuntimeConfig)
- used by: [`loadPersistedSupervisorConfig`](daemon-supervisor.ts.md#DaemonSupervisor.loadPersistedSupervisorConfig), [`persistSupervisorConfig`](daemon-supervisor.ts.md#DaemonSupervisor.persistSupervisorConfig)

### `ResidentWorker`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor.ts:256`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L256)
- signature: `interface ResidentWorker`
- members:
  - `client` — [`L259`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L259)
  - `deferredRecovery` — [`L268`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L268)
  - `descriptor` — [`L257`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L257) — documented in [packages-coding-agent-src-modes-daemon-daemon-supervisor.ts](../../../../../../concepts/packages-coding-agent-src-modes-daemon-daemon-supervisor.ts.md)
  - `descriptorPath` — [`L258`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L258)
  - `heartbeatSnapshot` — [`L260`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L260)
  - `heartbeatSnapshotStale` — [`L261`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L261)
  - `intentionalStop` — [`L269`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L269)
  - `launchEnv` — [`L271`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L271)
  - `ownerCleanupTimer` — [`L273`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L273)
  - `promotedOwnerClientId` — [`L274`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L274)
  - `recovery` — [`L267`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L267)
  - `snapshotCache` — [`L263`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L263)
  - `snapshotGenerations` — [`L265`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L265)
  - `snapshotLoads` — [`L266`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L266)
  - `stopFinalization` — [`L272`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L272)
  - `stopRevision` — [`L270`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L270)
  - `summaries` — [`L262`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L262)
  - `transcriptCaches` — [`L264`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L264)
  - `updateRestartPrepareClient` — [`L275`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L275)
- uses (calls/refs, reference-scoped): [`SessionSummary`](daemon-session-list.ts.md#SessionSummary), [`DaemonAttachResult`](daemon-protocol.ts.md#DaemonAttachResult), [`AgentConnectionHeartbeat`](../agent-connection/types.ts.md#AgentConnectionHeartbeat), [`SnapshotTranscriptCache`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCache), [`DaemonWorkerDescriptor`](daemon-worker-protocol.ts.md#DaemonWorkerDescriptor), [`DaemonWorkerClient`](daemon-worker-client.ts.md#DaemonWorkerClient), [`SnapshotTranscriptGeneration`](daemon-supervisor.ts.md#SnapshotTranscriptGeneration)
- used by: [`handleCommand`](daemon-supervisor.ts.md#DaemonSupervisor.handleCommand), [`handleWorkerFrame`](daemon-supervisor.ts.md#DaemonSupervisor.handleWorkerFrame), [`launchWorker`](daemon-supervisor.ts.md#DaemonSupervisor.launchWorker), [`type`](daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type), [`start`](daemon-supervisor.ts.md#DaemonSupervisor.start), [`stopWorkerUntracked`](daemon-supervisor.ts.md#DaemonSupervisor.stopWorkerUntracked), [`shutdown`](daemon-supervisor.ts.md#DaemonSupervisor.shutdown), [`cleanupSupervisorResourcesOnce`](daemon-supervisor.ts.md#DaemonSupervisor.cleanupSupervisorResourcesOnce), [`refreshWorkerSummaries`](daemon-supervisor.ts.md#DaemonSupervisor.refreshWorkerSummaries), [`recoverWorker`](daemon-supervisor.ts.md#DaemonSupervisor.recoverWorker), [`getOrCreateTranscriptCache`](daemon-supervisor.ts.md#DaemonSupervisor.getOrCreateTranscriptCache), [`createOrReuseWorker`](daemon-supervisor.ts.md#DaemonSupervisor.createOrReuseWorker), [`runIdleEvictionSweep`](daemon-supervisor.ts.md#DaemonSupervisor.runIdleEvictionSweep), [`recoverUncertainWorkerOperations`](daemon-supervisor.ts.md#DaemonSupervisor.recoverUncertainWorkerOperations), [`workerEvictionSnapshot`](daemon-supervisor.ts.md#DaemonSupervisor.workerEvictionSnapshot), [`worker`](daemon-supervisor.ts.md#WorkerMatch.worker), [`prepareUpdateRestartFenced`](daemon-supervisor.ts.md#DaemonSupervisor.prepareUpdateRestartFenced), [`adoptOrRecoverWorker`](daemon-supervisor.ts.md#DaemonSupervisor.adoptOrRecoverWorker), [`handleWorkerClose`](daemon-supervisor.ts.md#DaemonSupervisor.handleWorkerClose), [`finalizeTimedOutWorkerStop`](daemon-supervisor.ts.md#DaemonSupervisor.finalizeTimedOutWorkerStop), [`cacheLoadedSnapshot`](daemon-supervisor.ts.md#DaemonSupervisor.cacheLoadedSnapshot), [`streamSnapshot`](daemon-supervisor.ts.md#DaemonSupervisor.streamSnapshot), [`connectWorker`](daemon-supervisor.ts.md#DaemonSupervisor.connectWorker), [`forwardToWorker`](daemon-supervisor.ts.md#DaemonSupervisor.forwardToWorker), [`loadWorkerDescriptors`](daemon-supervisor.ts.md#DaemonSupervisor.loadWorkerDescriptors), [`failWorkerSnapshotCache`](daemon-supervisor.ts.md#DaemonSupervisor.failWorkerSnapshotCache), [`workers`](daemon-supervisor.ts.md#DaemonSupervisor.workers), [`syncAgentPeers`](daemon-supervisor.ts.md#DaemonSupervisor.syncAgentPeers), [`type`](daemon-supervisor.ts.md#DaemonSupervisor.handleList.command-Extract.typeLiteral1418.type), [`reclaimStaleWorkerRegistration`](daemon-supervisor.ts.md#DaemonSupervisor.reclaimStaleWorkerRegistration), [`publicSummary`](daemon-supervisor.ts.md#DaemonSupervisor.publicSummary), [`retireWorkerSnapshotCache`](daemon-supervisor.ts.md#DaemonSupervisor.retireWorkerSnapshotCache), [`resumeDeferredWorkerRecovery`](daemon-supervisor.ts.md#DaemonSupervisor.resumeDeferredWorkerRecovery), [`failSnapshotGeneration`](daemon-supervisor.ts.md#DaemonSupervisor.failSnapshotGeneration), [`assertSupervisorSavedSessionNameAvailable`](daemon-supervisor.ts.md#DaemonSupervisor.assertSupervisorSavedSessionNameAvailable), [`familyCatalogEntries`](daemon-supervisor.ts.md#DaemonSupervisor.familyCatalogEntries), [`finalizeArchivedWorkerStop`](daemon-supervisor.ts.md#DaemonSupervisor.finalizeArchivedWorkerStop), [`promoteOwnedWorker`](daemon-supervisor.ts.md#DaemonSupervisor.promoteOwnedWorker), [`findSummaryInWorker`](daemon-supervisor.ts.md#DaemonSupervisor.findSummaryInWorker), [`scheduleOwnedWorkerCleanup`](daemon-supervisor.ts.md#DaemonSupervisor.scheduleOwnedWorkerCleanup)  (+38 more)

### `SnapshotDuplicateValidation`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor.ts:278`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L278)
- signature: `interface SnapshotDuplicateValidation`
- members:
  - `promise` — [`L279`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L279)
  - `reject` — [`L281`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L281)
  - `resolve` — [`L280`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L280)
- used by: [`type`](daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type), [`settleSnapshotDuplicateValidation`](daemon-supervisor.ts.md#DaemonSupervisor.settleSnapshotDuplicateValidation), [`createSnapshotDuplicateValidation`](daemon-supervisor.ts.md#DaemonSupervisor.createSnapshotDuplicateValidation), [`validation`](daemon-supervisor.ts.md#SnapshotTranscriptGeneration.validation)

### `SnapshotLoadInvalidatedError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor.ts:339`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L339)
- signature: `class SnapshotLoadInvalidatedError`
- used by: [`type`](daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type)

### `SnapshotTranscriptGeneration`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor.ts:284`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L284)
- signature: `interface SnapshotTranscriptGeneration`
- members:
  - `begin` — [`L287`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L287)
  - `duplicateChunkIndex` — [`L291`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L291)
  - `duplicateResult` — [`L292`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L292)
  - `end` — [`L288`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L288)
  - `incoming` — [`L289`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L289)
  - `result` — [`L286`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L286)
  - `retired` — [`L290`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L290)
  - `transcript` — [`L285`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L285)
  - `validation` — [`L293`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L293)
- uses (calls/refs, reference-scoped): [`DaemonAttachResult`](daemon-protocol.ts.md#DaemonAttachResult), [`SnapshotTranscriptCache`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCache), [`SnapshotDuplicateValidation`](daemon-supervisor.ts.md#SnapshotDuplicateValidation)
- used by: [`handleWorkerFrame`](daemon-supervisor.ts.md#DaemonSupervisor.handleWorkerFrame), [`type`](daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type), [`stopWorkerUntracked`](daemon-supervisor.ts.md#DaemonSupervisor.stopWorkerUntracked), [`cleanupSupervisorResourcesOnce`](daemon-supervisor.ts.md#DaemonSupervisor.cleanupSupervisorResourcesOnce), [`getOrCreateTranscriptCache`](daemon-supervisor.ts.md#DaemonSupervisor.getOrCreateTranscriptCache), [`handleWorkerClose`](daemon-supervisor.ts.md#DaemonSupervisor.handleWorkerClose), [`cacheLoadedSnapshot`](daemon-supervisor.ts.md#DaemonSupervisor.cacheLoadedSnapshot), [`failWorkerSnapshotCache`](daemon-supervisor.ts.md#DaemonSupervisor.failWorkerSnapshotCache), [`retireWorkerSnapshotCache`](daemon-supervisor.ts.md#DaemonSupervisor.retireWorkerSnapshotCache), [`failSnapshotGeneration`](daemon-supervisor.ts.md#DaemonSupervisor.failSnapshotGeneration), [`currentSnapshotGeneration`](daemon-supervisor.ts.md#DaemonSupervisor.currentSnapshotGeneration), [`deleteSnapshotGeneration`](daemon-supervisor.ts.md#DaemonSupervisor.deleteSnapshotGeneration), [`snapshotGenerations`](daemon-supervisor.ts.md#ResidentWorker.snapshotGenerations), [`settleSnapshotDuplicateValidation`](daemon-supervisor.ts.md#DaemonSupervisor.settleSnapshotDuplicateValidation), [`snapshotGeneration`](daemon-supervisor.ts.md#DaemonSupervisor.snapshotGeneration), [`snapshotGenerationsFor`](daemon-supervisor.ts.md#DaemonSupervisor.snapshotGenerationsFor)

### `SupervisorPromptAdmission`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor.ts:320`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L320)
- signature: `interface SupervisorPromptAdmission`
- members:
  - `activeSessionId` — [`L322`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L322)
  - `client` — [`L321`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L321)
  - `controller` — [`L326`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L326)
  - `publicAdmissionId` — [`L323`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L323)
  - `status` — [`L325`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L325)
  - `worker` — [`L327`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L327)
  - `workerActiveSessionId` — [`L328`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L328)
  - `workerAdmissionId` — [`L324`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L324)
- uses (calls/refs, reference-scoped): [`DaemonSocketClient`](active-session-state.ts.md#DaemonSocketClient), [`ResidentWorker`](daemon-supervisor.ts.md#ResidentWorker)
- used by: [`handleCommand`](daemon-supervisor.ts.md#DaemonSupervisor.handleCommand), [`handleLine`](daemon-supervisor.ts.md#DaemonSupervisor.handleLine), [`admission`](daemon-supervisor.ts.md#DaemonSupervisor.parseCommandAndRegisterPromptAdmission.typeLiteral846.admission), [`cancelWaitingPromptAdmissionsForClient`](daemon-supervisor.ts.md#DaemonSupervisor.cancelWaitingPromptAdmissionsForClient), [`deletePromptAdmission`](daemon-supervisor.ts.md#DaemonSupervisor.deletePromptAdmission), [`getPromptAdmission`](daemon-supervisor.ts.md#DaemonSupervisor.getPromptAdmission), [`promptAdmissions`](daemon-supervisor.ts.md#DaemonSupervisor.promptAdmissions), [`throwIfAdmissionCancelled`](daemon-supervisor.ts.md#throwIfAdmissionCancelled), [`promptAdmissionsFor`](daemon-supervisor.ts.md#DaemonSupervisor.promptAdmissionsFor)

### `SupervisorRecoveryCancelledError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor.ts:335`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L335)
- signature: `class SupervisorRecoveryCancelledError`
- members:
  - `code` — [`L336`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L336)
- used by: [`assertRecoveryAllowed`](daemon-supervisor.ts.md#DaemonSupervisor.assertRecoveryAllowed), [`supervisorSocketPath`](daemon-supervisor.ts.md#DaemonSupervisor.supervisorAuthenticationClaim.typeLiteral584.supervisorSocketPath), [`isSupervisorShutdownAdmissionCancelled`](daemon-supervisor.ts.md#isSupervisorShutdownAdmissionCancelled)

### `WorkerAttachData`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor.ts:313`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L313)
- signature: `interface WorkerAttachData`
- members:
  - `releaseTranscript` — [`L317`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L317)
  - `result` — [`L314`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L314)
  - `transcript` — [`L316`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L316)
  - `worker` — [`L315`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L315)
- uses (calls/refs, reference-scoped): [`DaemonAttachResult`](daemon-protocol.ts.md#DaemonAttachResult), [`ResidentWorker`](daemon-supervisor.ts.md#ResidentWorker), [`SnapshotTranscriptCache`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCache)
- used by: [`handleCommand`](daemon-supervisor.ts.md#DaemonSupervisor.handleCommand), [`type`](daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type), [`drainClientCatchups`](daemon-supervisor.ts.md#DaemonSupervisor.drainClientCatchups)

### `WorkerMatch`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor.ts:308`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L308)
- signature: `interface WorkerMatch`
- members:
  - `summary` — [`L310`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L310)
  - `worker` — [`L309`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L309)
- uses (calls/refs, reference-scoped): [`SessionSummary`](daemon-session-list.ts.md#SessionSummary), [`ResidentWorker`](daemon-supervisor.ts.md#ResidentWorker)
- used by: [`handleCommand`](daemon-supervisor.ts.md#DaemonSupervisor.handleCommand), [`type`](daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type), [`createOrReuseWorker`](daemon-supervisor.ts.md#DaemonSupervisor.createOrReuseWorker), [`type`](daemon-supervisor.ts.md#DaemonSupervisor.handleSavedSessionList.command-Extract.typeLiteral1475.type), [`findWorkerForClient`](daemon-supervisor.ts.md#DaemonSupervisor.findWorkerForClient), [`detachClient`](daemon-supervisor.ts.md#DaemonSupervisor.detachClient), [`matchWorkers`](daemon-supervisor.ts.md#DaemonSupervisor.matchWorkers), [`syncWorkerExtensionUi`](daemon-supervisor.ts.md#DaemonSupervisor.syncWorkerExtensionUi), [`findWorker`](daemon-supervisor.ts.md#DaemonSupervisor.findWorker), [`findWorkerBySessionFile`](daemon-supervisor.ts.md#DaemonSupervisor.findWorkerBySessionFile)

### `WorkerStopTimeoutError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor.ts:341`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L341)
- signature: `class WorkerStopTimeoutError`
- used by: [`stopWorkerUntracked`](daemon-supervisor.ts.md#DaemonSupervisor.stopWorkerUntracked), [`shutdown`](daemon-supervisor.ts.md#DaemonSupervisor.shutdown)

## Functions
- `attachResultFromResponse(response: DaemonResponse)` — [`L455`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L455)
- `commitWorkerStartupGate(gate: Writable)` — [`L374`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L374)
- `cronJobsFromResponse(response: DaemonResponse)` — [`L466`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L466)
- `defaultWorkerDescriptorDir(agentDir: string, socketPath: string)` — [`L501`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L501)
- `delay(ms: number)` — [`L366`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L366)
- `descriptorKey(socketPath: string)` — [`L497`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L497)
- `heartbeatsFromResponse(response: DaemonResponse)` — [`L474`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L474)
- `idleEvictionSweepIntervalMs(idleEvictionMinutes: IdleEvictionMinutes)` — [`L505`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L505)
- `isDaemonWorkerDescriptor(value: unknown, socketPath: string)` — [`L419`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L419)
- `isFinalizedTranscriptEvent(eventType: string | undefined)` — [`L525`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L525)
- `isSessionSummary(value: unknown)` — [`L409`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L409)
- `isSupervisorGenerationStale(error: unknown)` — [`L343`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L343)
- `isSupervisorRecoveryCancelled(error: unknown)` — [`L352`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L352)
- `isSupervisorShutdownAdmissionCancelled(error: unknown)` — [`L356`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L356)
- `looksLikeSessionPath(selector: string)` — [`L521`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L521)
- `mergeSessionLists(active: readonly SessionSummary[], saved: readonly SessionInfo[])` — [`L545`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L545)
- `normalizeCapabilities(capabilities: readonly DaemonClientCapability[] | undefined, supportsExtensionUi: boolean | undefined)` — [`L534`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L534)
- `responseWithId(response: DaemonResponse, id: string | undefined)` — [`L405`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L405)
- `runDaemonSupervisorMode(options: DaemonSupervisorOptions)` — [`L576`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L576)
- `sessionSummariesFromResponse(response: DaemonResponse)` — [`L444`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L444)
- `sortCronJobs(jobs: AgentCronJob[])` — [`L482`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L482)
- `throwIfAdmissionCancelled(admission: SupervisorPromptAdmission | undefined)` — [`L331`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L331)
- `unrefDelay(ms: number)` — [`L370`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L370)
- `withoutCommandId(command: DaemonCommand)` — [`L395`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L395)
- `withoutSupervisorCreateFields(command: { id?: string | undefined; type: "create"; sessionPath?: string | undefined; continueRecent?: boolean | undefined; noSession?: boolean | undefined; name?: string | undefined; config?: AgentSessionRuntimeConfig | undefined; runtimeMetadata?: AgentSessionRuntimeMetadata | undefined; lifecycle?: DaemonSessionLifecycle | undefined; } & DaemonClientEnv & DaemonLaunchEnv)` — [`L400`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L400)
- `workerSocketPath(supervisorSocketPath: string, workerId: string)` — [`L513`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L513)

## Module values
- `CHILD_PASSIVATION_PER_WORKER_CAP` — [`L151`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L151)
- `DAEMON_COMMAND_TYPES` — [`L155`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L155)
- `DEFERRED_RECOVERY_RECHECK_MS` — [`L138`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L138)
- `IDLE_EVICTION_DRAIN_TIMEOUT_MS` — [`L150`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L150)
- `IDLE_EVICTION_MAX_SWEEP_INTERVAL_MS` — [`L148`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L148)
- `IDLE_EVICTION_MIN_SWEEP_INTERVAL_MS` — [`L149`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L149)
- `LIVENESS_IDENTITY_RECHECK_MS` — [`L146`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L146)
- `OWNED_WORKER_DISCONNECT_GRACE_MS` — [`L147`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L147)
- `STALE_RECLAIM_WAIT_MS` — [`L142`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L142)
- `STOP_FINALIZATION_RECHECK_MS` — [`L139`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L139)
- `STOP_FINALIZATION_RETRY_MS` — [`L141`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L141)
- `STOP_FINALIZATION_SIGKILL_GRACE_MS` — [`L140`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L140)
- `SUPERVISOR_CONFIG_FILE_NAME` — [`L152`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L152)
- `UPDATE_RESTART_MUTATION_DRAIN_TIMEOUT_MS` — [`L131`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L131)
- `UPDATE_RESTART_PREPARE_DEADLINE_MS` — [`L136`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L136)
- `UPDATE_RESTART_WORKER_REQUEST_TIMEOUT_MS` — [`L132`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L132)
- `WORKER_CONNECT_TIMEOUT_MS` — [`L129`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L129)
- `WORKER_REQUEST_TIMEOUT_MS` — [`L130`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L130)
- `WORKER_RETRY_DELAYS_MS` — [`L137`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L137)
- `WORKER_STARTUP_GATE_FD` — [`L153`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L153)
- `structuredLog` — [`L128`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts#L128)


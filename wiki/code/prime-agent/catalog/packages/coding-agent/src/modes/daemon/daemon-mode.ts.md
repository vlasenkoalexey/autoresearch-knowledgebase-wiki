---
title: 'Module: packages/coding-agent/src/modes/daemon/daemon-mode.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/daemon-mode.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`daemon-mode.ts`/
symbols:
  AgentDaemon.handleCommand: AgentDaemon#handleCommand().
  AgentDaemon.-constructor: AgentDaemon#`<constructor>`().
  AgentDaemon.createRlmSubagentRuntime: AgentDaemon#createRlmSubagentRuntime().
  AgentDaemon.createRuntime: AgentDaemon#createRuntime().
  AgentDaemon.rehydrateCompletedRlmSubagentOnce: AgentDaemon#rehydrateCompletedRlmSubagentOnce().
  AgentDaemon.sendAgentSessionMessage.options-typeLiteral1160.origin: AgentDaemon#sendAgentSessionMessage().(options)typeLiteral1160:origin.
  DaemonModeOptions.defaultSessionConfig: DaemonModeOptions#defaultSessionConfig.
  DaemonModeOptions.createRuntime: DaemonModeOptions#createRuntime.
  AgentDaemon.createSubagentRuntimeHost: AgentDaemon#createSubagentRuntimeHost().
  AgentDaemon.createAgentObserveSummary: AgentDaemon#createAgentObserveSummary().
  AgentDaemon.createAgentMessageAgentSummary: AgentDaemon#createAgentMessageAgentSummary().
  AgentDaemon.createAgentFamilyCatalog: AgentDaemon#createAgentFamilyCatalog().
  AgentDaemon.addRuntime: AgentDaemon#addRuntime().
  AgentDaemon.createAgentMessageListResult: AgentDaemon#createAgentMessageListResult().
  AgentDaemon.handleWorkerCommand: AgentDaemon#handleWorkerCommand().
  AgentDaemon.createAgentObserveListResult: AgentDaemon#createAgentObserveListResult().
  AgentDaemon.handleConnection: AgentDaemon#handleConnection().
  AgentDaemon.handleLine: AgentDaemon#handleLine().
  AgentDaemon.getSessionState: AgentDaemon#getSessionState().
  AgentDaemon.drainBackpressuredClientCatchups: AgentDaemon#drainBackpressuredClientCatchups().
  AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.createdAt: AgentDaemon#recordRlmSubagentRegistryEntry().(input)typeLiteral250:createdAt.
  AgentDaemon.sessionPassivationSnapshot: AgentDaemon#sessionPassivationSnapshot().
  AgentDaemon.buildSessionListWithPassiveRlmSubagents: AgentDaemon#buildSessionListWithPassiveRlmSubagents().
  AgentDaemon.createRlmHeartbeatForState.input-typeLiteral666.deliveryMode: AgentDaemon#createRlmHeartbeatForState().(input)typeLiteral666:deliveryMode.
  AgentDaemon.sessions: AgentDaemon#sessions.
  AgentDaemon.closeSessionOnce: AgentDaemon#closeSessionOnce().
  AgentDaemon.buildRlmChildSnapshotsWithPassiveRlmSubagents: AgentDaemon#buildRlmChildSnapshotsWithPassiveRlmSubagents().
  AgentDaemon.createHeartbeatForState: AgentDaemon#createHeartbeatForState().
  AgentDaemon.hydratePassiveRlmSubagent: AgentDaemon#hydratePassiveRlmSubagent().
  AgentDaemon.createUpdateRestartSession: AgentDaemon#createUpdateRestartSession().
  AgentDaemon.streamWorkerSnapshot: AgentDaemon#streamWorkerSnapshot().
  AgentDaemon.broadcastToSession: AgentDaemon#broadcastToSession().
  AgentDaemon.runCronJob: AgentDaemon#runCronJob().
  AgentDaemon.getOrCreateCronJobSession: AgentDaemon#getOrCreateCronJobSession().
  AgentDaemon.restoreRlmHeartbeatSession: AgentDaemon#restoreRlmHeartbeatSession().
  AgentDaemon.passivateSession: AgentDaemon#passivateSession().
  AgentDaemon.acceptAgentSessionMessage.Promise.typeLiteral2954.status: AgentDaemon#acceptAgentSessionMessage().Promise:typeLiteral2954:status.
  AgentDaemon.agentFamilyEntry: AgentDaemon#agentFamilyEntry().
  AgentDaemon.passiveAgentFamilyEntry: AgentDaemon#passiveAgentFamilyEntry().
  AgentDaemon.prepareReplacementSnapshot.message-Extract.typeLiteral3411.type: AgentDaemon#prepareReplacementSnapshot().(message)Extract:typeLiteral3411:type.
  AgentDaemon.launchReplacementSupervisor: AgentDaemon#launchReplacementSupervisor().
  AgentDaemon.createCronJobForState: AgentDaemon#createCronJobForState().
  AgentDaemon.shutdown: AgentDaemon#shutdown().
  AgentDaemon.listPassiveRlmSubagents: AgentDaemon#listPassiveRlmSubagents().
  AgentDaemon.updateRlmHeartbeatForState.input-typeLiteral676.deliveryMode: AgentDaemon#updateRlmHeartbeatForState().(input)typeLiteral676:deliveryMode.
  AgentDaemon.cancelPreparedUpdateRestart: AgentDaemon#cancelPreparedUpdateRestart().
  AgentDaemon.recordWorkerRecoveryState: AgentDaemon#recordWorkerRecoveryState().
  AgentDaemon.rebindCronJobsToState: AgentDaemon#rebindCronJobsToState().
  AgentDaemon.prepareUpdateRestartCheckpoint: AgentDaemon#prepareUpdateRestartCheckpoint().
  AgentDaemon.createAgentMessageController: AgentDaemon#createAgentMessageController().
  AgentDaemon.write: AgentDaemon#write().
  AgentDaemon.setStateSessionName: AgentDaemon#setStateSessionName().
  AgentDaemon.start: AgentDaemon#start().
  AgentDaemon.rehydrateCompletedRlmSubagent: AgentDaemon#rehydrateCompletedRlmSubagent().
  AgentDaemon.createSessionSnapshot: AgentDaemon#createSessionSnapshot().
  AgentDaemon.isCronJobRunnableForState: AgentDaemon#isCronJobRunnableForState().
  AgentDaemon.refreshReplacedSessionState: AgentDaemon#refreshReplacedSessionState().
  AgentDaemon.closeSession: AgentDaemon#closeSession().
  AgentDaemon.getOrHydrateBoundSessionState: AgentDaemon#getOrHydrateBoundSessionState().
  AgentDaemon.cronStore: AgentDaemon#cronStore.
  AgentDaemon.createAgentObserveRecentMessages: AgentDaemon#createAgentObserveRecentMessages().
  AgentDaemon.assertStateSessionNameAvailable: AgentDaemon#assertStateSessionNameAvailable().
  AgentDaemon.appendUpdateRestartMarker: AgentDaemon#appendUpdateRestartMarker().
  AgentDaemon.createAttachResult.command-Extract.typeLiteral2508.type: AgentDaemon#createAttachResult().(command)Extract:typeLiteral2508:type.
  AgentDaemon.log: AgentDaemon#log().
  AgentDaemon.getOrHydrateAuthorizedAgentFamilyTarget: AgentDaemon#getOrHydrateAuthorizedAgentFamilyTarget().
  AgentDaemon.createAgentSessionMessageEndpoint: AgentDaemon#createAgentSessionMessageEndpoint().
  AgentDaemon.summarizer: AgentDaemon#summarizer.
  AgentDaemon.beginUpdateRestartTransaction: AgentDaemon#beginUpdateRestartTransaction().
  AgentDaemon.promptWithAgentMessagePreparingGuard: AgentDaemon#promptWithAgentMessagePreparingGuard().
  AgentDaemon.beginReplacementSnapshot.message-Extract.typeLiteral3394.type: AgentDaemon#beginReplacementSnapshot().(message)Extract:typeLiteral3394:type.
  AgentDaemon.registerCronStoreForState: AgentDaemon#registerCronStoreForState().
  AgentDaemon.runUpdateRestartPreparation: AgentDaemon#runUpdateRestartPreparation().
  AgentDaemon.setStateSessionNameViaSupervisor: AgentDaemon#setStateSessionNameViaSupervisor().
  AgentDaemon.adoptClientEnv: AgentDaemon#adoptClientEnv().
  AgentDaemon.assertFamilySessionNameAvailable.input-typeLiteral482.ignoreSessionId: AgentDaemon#assertFamilySessionNameAvailable().(input)typeLiteral482:ignoreSessionId.
  DaemonModeOptions.worker: DaemonModeOptions#worker.
  AgentDaemon.cancelScheduledJobsForSession: AgentDaemon#cancelScheduledJobsForSession().
  AgentDaemon.commitPreparedUpdateRestart: AgentDaemon#commitPreparedUpdateRestart().
  AgentDaemon.scheduleClientCatchupRetry: AgentDaemon#scheduleClientCatchupRetry().
  AgentDaemon.waitForHydratingChild: AgentDaemon#waitForHydratingChild().
  AgentDaemon.updateHeartbeatForState: AgentDaemon#updateHeartbeatForState().
  AgentDaemon.sendRemoteAgentSessionMessage: AgentDaemon#sendRemoteAgentSessionMessage().
  AgentDaemon.readLatestRlmSubagentRegistryPath: AgentDaemon#readLatestRlmSubagentRegistryPath().
  AgentDaemon.createConnectionState: AgentDaemon#createConnectionState().
  AgentDaemon.detachClientFromSession: AgentDaemon#detachClientFromSession().
  AgentDaemon.isDiscardableDraft: AgentDaemon#isDiscardableDraft().
  AgentDaemon.withAgentMessagePreparingGuard: AgentDaemon#withAgentMessagePreparingGuard().
  DaemonModeOptions.worker.typeLiteral0.restoreActiveSessionId: DaemonModeOptions#worker.typeLiteral0:restoreActiveSessionId.
  PersistedRlmSubagentRegistryEntry.sessionFile: PersistedRlmSubagentRegistryEntry#sessionFile.
  AgentDaemon.updateRestart: AgentDaemon#updateRestart.
  AgentDaemon.listHeartbeats: AgentDaemon#listHeartbeats().
  AgentDaemon.cancelSubagentRlmHeartbeats: AgentDaemon#cancelSubagentRlmHeartbeats().
  AgentDaemon.prepareUpdateRestart: AgentDaemon#prepareUpdateRestart().
  finishClientSnapshotStreaming: finishClientSnapshotStreaming().
  AgentDaemon.removeQueuedHeartbeatFollowUp: AgentDaemon#removeQueuedHeartbeatFollowUp().
  markClientSnapshotStreaming: markClientSnapshotStreaming().
  AgentDaemon: AgentDaemon#
  AgentDaemon.revokeSupervisorClaim: AgentDaemon#revokeSupervisorClaim().
  AgentDaemon.findPassiveRlmSubagent: AgentDaemon#findPassiveRlmSubagent().
  AgentDaemon.waitForBoundSession: AgentDaemon#waitForBoundSession().
  AgentDaemon.resolveAgentFamilySessionName: AgentDaemon#resolveAgentFamilySessionName().
  AgentDaemon.passivateIdleChildren: AgentDaemon#passivateIdleChildren().
  PersistedRlmSubagentRegistryEntry.childId: PersistedRlmSubagentRegistryEntry#childId.
  AgentDaemon.deleteRlmHeartbeatForState: AgentDaemon#deleteRlmHeartbeatForState().
  AgentDaemon.getBoundSessionState: AgentDaemon#getBoundSessionState().
  AgentDaemon.createAgentObserveController: AgentDaemon#createAgentObserveController().
  AgentDaemon.isEmptyDraftContent: AgentDaemon#isEmptyDraftContent().
  AgentDaemon.writeSerialized: AgentDaemon#writeSerialized().
  AgentDaemon.isPersistedCronJobRunnable: AgentDaemon#isPersistedCronJobRunnable().
  AgentDaemon.cronScheduler: AgentDaemon#cronScheduler.
  AgentDaemon.findSessionBySessionFile: AgentDaemon#findSessionBySessionFile().
  AgentDaemon.getUpdateRestartSessionDepth: AgentDaemon#getUpdateRestartSessionDepth().
  detachClientFromActiveSession: detachClientFromActiveSession().
  AgentDaemon.getRunnableCronJob: AgentDaemon#getRunnableCronJob().
  AgentDaemon.manageHeartbeat: AgentDaemon#manageHeartbeat().
  AgentDaemon.parseCommandAndRegisterPromptAdmission: AgentDaemon#parseCommandAndRegisterPromptAdmission().
  AgentDaemon.createAgentFamilyRoster: AgentDaemon#createAgentFamilyRoster().
  AgentDaemon.reserveAgentMessageQueueSlot: AgentDaemon#reserveAgentMessageQueueSlot().
  AgentDaemon.catchUpBackpressuredClient: AgentDaemon#catchUpBackpressuredClient().
  AgentDaemon.stampRlmChildActiveSessionId: AgentDaemon#stampRlmChildActiveSessionId().
  AgentDaemon.addSessionEventMeta: AgentDaemon#addSessionEventMeta().
  AgentDaemon.resolveHeaderParentSessionPath: AgentDaemon#resolveHeaderParentSessionPath().
  AgentDaemon.closingSessions: AgentDaemon#closingSessions.
  AgentDaemon.openingSessions: AgentDaemon#openingSessions.
  AgentDaemon.checkSupervisorFences: AgentDaemon#checkSupervisorFences().
  AgentDaemon.promptHeartbeatWithAgentMessagePreparingGuard: AgentDaemon#promptHeartbeatWithAgentMessagePreparingGuard().
  AgentDaemon.clearQueuedAgentSessionMessagesForState: AgentDaemon#clearQueuedAgentSessionMessagesForState().
  AgentDaemon.sendAgentSessionMessage.options-typeLiteral1160.fromState: AgentDaemon#sendAgentSessionMessage().(options)typeLiteral1160:fromState.
  AgentDaemon.abortBashForClose: AgentDaemon#abortBashForClose().
  AgentDaemon.assertSupervisorClaimCurrent: AgentDaemon#assertSupervisorClaimCurrent().
  AgentDaemon.readLatestRlmSubagentRegistry: AgentDaemon#readLatestRlmSubagentRegistry().
  setDaemonClientSessionCapabilities: setDaemonClientSessionCapabilities().
  AgentDaemon.scheduleSupervisorAvailabilityCheck: AgentDaemon#scheduleSupervisorAvailabilityCheck().
  AgentDaemon.appendRlmSubagentRegistryEntry: AgentDaemon#appendRlmSubagentRegistryEntry().
  AgentDaemon.recordRlmSubagentDeletion: AgentDaemon#recordRlmSubagentDeletion().
  AgentDaemon.archiveSession: AgentDaemon#archiveSession().
  shouldSendDaemonOutboundToClient: shouldSendDaemonOutboundToClient().
  getChildActiveSessionStates: getChildActiveSessionStates().
  AgentDaemon.updateRestart.typeLiteral28.phase: AgentDaemon#updateRestart.typeLiteral28:phase.
  AgentDaemon.supervisorClaims: AgentDaemon#supervisorClaims.
  AgentDaemon.checkSupervisorAvailability: AgentDaemon#checkSupervisorAvailability().
  AgentDaemon.drainBackpressuredClientCatchupQueue: AgentDaemon#drainBackpressuredClientCatchupQueue().
  runDaemonMode: runDaemonMode().
  AgentDaemon.cancelScheduledJobsForSessionFile: AgentDaemon#cancelScheduledJobsForSessionFile().
  AgentDaemon.getAgentMessageSafetyStatus: AgentDaemon#getAgentMessageSafetyStatus().
  AgentDaemon.assertAgentFamilyReachable: AgentDaemon#assertAgentFamilyReachable().
  AgentDaemon.assertUpdateRestartNotCancelled: AgentDaemon#assertUpdateRestartNotCancelled().
  PassiveRlmSubagent: PassiveRlmSubagent#
  AgentDaemon.scheduleSupervisorFenceCheck: AgentDaemon#scheduleSupervisorFenceCheck().
  AgentDaemon.writeWorkerSuccess: AgentDaemon#writeWorkerSuccess().
  AgentDaemon.withSessionNameReservation: AgentDaemon#withSessionNameReservation().
  AgentDaemon.listTargetableSessionStates: AgentDaemon#listTargetableSessionStates().
  AgentDaemon.detachClient: AgentDaemon#detachClient().
  AgentDaemon.findActiveSessionByFile: AgentDaemon#findActiveSessionByFile().
  AgentDaemon.closeChildSessions: AgentDaemon#closeChildSessions().
  PersistedRlmSubagentRegistryEntry: PersistedRlmSubagentRegistryEntry#
  RuntimeOpenCancelledError: RuntimeOpenCancelledError#
  AgentDaemon.shuttingDown: AgentDaemon#shuttingDown.
  AgentDaemon.writeWorkerSnapshotRecord: AgentDaemon#writeWorkerSnapshotRecord().
  daemonClientCapabilitiesForSession: daemonClientCapabilitiesForSession().
  AgentDaemon.rlmSubagentRegistryPathForEntry: AgentDaemon#rlmSubagentRegistryPathForEntry().
  AgentDaemon.createAgentObserveAgentSnapshot: AgentDaemon#createAgentObserveAgentSnapshot().
  AgentDaemon.applyReasonUpgrade: AgentDaemon#applyReasonUpgrade().
  AgentDaemon.registerSignalHandlers: AgentDaemon#registerSignalHandlers().
  BoundSessionUnavailableError: BoundSessionUnavailableError#
  AgentDaemon.updateRestart.typeLiteral28.id: AgentDaemon#updateRestart.typeLiteral28:id.
  AgentDaemon.sideQuestionRuns: AgentDaemon#sideQuestionRuns.
  AgentDaemon.queueClientCatchup: AgentDaemon#queueClientCatchup().
  AgentDaemon.rlmSubagentRegistryPath: AgentDaemon#rlmSubagentRegistryPath().
  AgentDaemon.passiveRlmSubagentsByPath: AgentDaemon#passiveRlmSubagentsByPath().
  AgentDaemon.cancelRlmHeartbeat: AgentDaemon#cancelRlmHeartbeat().
  AgentDaemon.writeWorkerSnapshotBuffer: AgentDaemon#writeWorkerSnapshotBuffer().
  AgentDaemon.isAgentFamilyReachable: AgentDaemon#isAgentFamilyReachable().
  removeDaemonClientSessionCapabilities: removeDaemonClientSessionCapabilities().
  cancelPendingExtensionUiRequests: cancelPendingExtensionUiRequests().
  AgentDaemon.updateRestart.typeLiteral28.deadline: AgentDaemon#updateRestart.typeLiteral28:deadline.
  AgentDaemon.promptAdmissions: AgentDaemon#promptAdmissions.
  AgentDaemon.rlmSubagentRegistryPathForInfo: AgentDaemon#rlmSubagentRegistryPathForInfo().
  AgentDaemon.createAgentSessionMessageSender: AgentDaemon#createAgentSessionMessageSender().
  AgentDaemon.agentMessageRelationship: AgentDaemon#agentMessageRelationship().
  AgentDaemon.hasScheduledJobsForSession: AgentDaemon#hasScheduledJobsForSession().
  AgentDaemon.mutationDrain: AgentDaemon#mutationDrain.
  AgentDaemon.cleanupSocketPath: AgentDaemon#cleanupSocketPath().
  AgentDaemon.createAttachResult: AgentDaemon#createAttachResult().
  AgentDaemon.abortSideQuestionsFor: AgentDaemon#abortSideQuestionsFor().
  PersistedRlmSubagentRegistryEntry.status: PersistedRlmSubagentRegistryEntry#status.
  AgentDaemon.supervisorMonitorTimer: AgentDaemon#supervisorMonitorTimer.
  normalizeClientCapabilities: normalizeClientCapabilities().
  PersistedRlmSubagentRegistryEntry.rlmDepth: PersistedRlmSubagentRegistryEntry#rlmDepth.
  AgentDaemon.server: AgentDaemon#server.
  AgentDaemon.bindingSessions: AgentDaemon#bindingSessions.
  AgentDaemon.supervisorFenceTimer: AgentDaemon#supervisorFenceTimer.
  abortClientSnapshotStreaming: abortClientSnapshotStreaming().
  AgentDaemon.updateRestart.typeLiteral28.deferredClientEnv.Array.typeLiteral29.state: AgentDaemon#updateRestart.typeLiteral28:deferredClientEnv.Array:typeLiteral29:state.
  AgentDaemon.startSupervisorMonitor: AgentDaemon#startSupervisorMonitor().
  AgentDaemon.writeUpdateRestartManifest: AgentDaemon#writeUpdateRestartManifest().
  AgentDaemon.beginReplacementSnapshot: AgentDaemon#beginReplacementSnapshot().
  AgentDaemon.prepareReplacementSnapshot: AgentDaemon#prepareReplacementSnapshot().
  AgentDaemon.broadcastGlobal: AgentDaemon#broadcastGlobal().
  AgentDaemon.getShutdownClosingReason: AgentDaemon#getShutdownClosingReason().
  daemonClientSupportsExtensionUi: daemonClientSupportsExtensionUi().
  resolveDaemonSessionPath: resolveDaemonSessionPath().
  PersistedRlmSubagentRegistryEntry.sessionDir: PersistedRlmSubagentRegistryEntry#sessionDir.
  AgentDaemon.agentMessagePreparingTargets: AgentDaemon#agentMessagePreparingTargets.
  AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.status: AgentDaemon#recordRlmSubagentRegistryEntry().(input)typeLiteral250:status.
  AgentDaemon.clients: AgentDaemon#clients.
  AgentDaemon.remoteAgentPeers: AgentDaemon#remoteAgentPeers.
  AgentDaemon.waitForPassivation: AgentDaemon#waitForPassivation().
  PersistedRlmSubagentRegistryEntry.sessionName: PersistedRlmSubagentRegistryEntry#sessionName.
  PersistedRlmSubagentRegistryEntry.parentSessionId: PersistedRlmSubagentRegistryEntry#parentSessionId.
  PersistedRlmSubagentRegistryEntry.model: PersistedRlmSubagentRegistryEntry#model.
  PassiveRlmRoot: PassiveRlmRoot#
  AgentDaemon.updateRestart.typeLiteral28.abort: AgentDaemon#updateRestart.typeLiteral28:abort.
  AgentDaemon.isStrongerCloseReason: AgentDaemon#isStrongerCloseReason().
  AgentDaemon.clearClientCatchupRetry: AgentDaemon#clearClientCatchupRetry().
  AgentDaemon.updateRestart.typeLiteral28.owner: AgentDaemon#updateRestart.typeLiteral28:owner.
  AgentDaemon.agentMessageRateLimiter: AgentDaemon#agentMessageRateLimiter.
  AgentDaemon.hasAuthenticatedSupervisorConnection: AgentDaemon#hasAuthenticatedSupervisorConnection().
  AgentDaemon.findPassivationBySessionFile: AgentDaemon#findPassivationBySessionFile().
  PersistedRlmSubagentRegistryEntry.rlmParentNodeId: PersistedRlmSubagentRegistryEntry#rlmParentNodeId.
  AgentDaemon.agentMessagePendingReservations: AgentDaemon#agentMessagePendingReservations.
  AgentDaemon.agentMessageTargetLocks: AgentDaemon#agentMessageTargetLocks.
  AgentDaemon.clearSupervisorAvailabilityCheck: AgentDaemon#clearSupervisorAvailabilityCheck().
  AgentDaemon.clearQueuedAgentSessionMessagesForAllStates: AgentDaemon#clearQueuedAgentSessionMessagesForAllStates().
  AgentDaemon.acceptAgentSessionMessage: AgentDaemon#acceptAgentSessionMessage().
  AgentDaemon.hasActiveSideQuestionFor: AgentDaemon#hasActiveSideQuestionFor().
  isSequencedSessionOutbound: isSequencedSessionOutbound().
  SupervisorGenerationClaim: SupervisorGenerationClaim#
  BoundSupervisorGenerationClaim.claim: BoundSupervisorGenerationClaim#claim.
  AgentDaemon.updateRestart.typeLiteral28.manifest: AgentDaemon#updateRestart.typeLiteral28:manifest.
  AgentDaemon.updateRestart.typeLiteral28.deferredClientEnv.Array.typeLiteral29.client: AgentDaemon#updateRestart.typeLiteral28:deferredClientEnv.Array:typeLiteral29:client.
  AgentDaemon.socketIdentity: AgentDaemon#socketIdentity.
  AgentDaemon.recoveryJournal: AgentDaemon#recoveryJournal.
  AgentDaemon.createRlmHeartbeatForState: AgentDaemon#createRlmHeartbeatForState().
  AgentDaemon.updateRlmHeartbeatForState: AgentDaemon#updateRlmHeartbeatForState().
  AgentDaemon.withAgentMessageTargetLock: AgentDaemon#withAgentMessageTargetLock().
  BoundSupervisorGenerationClaim.ownerFingerprint: BoundSupervisorGenerationClaim#ownerFingerprint.
  PersistedRlmSubagentRegistryEntry.parentSessionFile: PersistedRlmSubagentRegistryEntry#parentSessionFile.
  PersistedRlmSubagentRegistryEntry.rlmMaxDepth: PersistedRlmSubagentRegistryEntry#rlmMaxDepth.
  AgentDaemon.reservingSessionOpens: AgentDaemon#reservingSessionOpens.
  AgentDaemon.passivatingSessions: AgentDaemon#passivatingSessions.
  AgentDaemon.agentMessageAcceptingTargets: AgentDaemon#agentMessageAcceptingTargets.
  AgentDaemon.agentMessagesPaused: AgentDaemon#agentMessagesPaused.
  AgentDaemon.promptAdmissionKey: AgentDaemon#promptAdmissionKey().
  AgentDaemon.assertFamilySessionNameAvailable.input-typeLiteral482.parentSessionPath: AgentDaemon#assertFamilySessionNameAvailable().(input)typeLiteral482:parentSessionPath.
  AgentDaemon.recordRlmSubagentRegistryEntry: AgentDaemon#recordRlmSubagentRegistryEntry().
  AgentDaemon.sendAgentSessionMessage.options-typeLiteral1160.sender: AgentDaemon#sendAgentSessionMessage().(options)typeLiteral1160:sender.
  AgentDaemon.closeReasonStrength: AgentDaemon#closeReasonStrength().
  AgentDaemon.closeKeepsResumeEntry: AgentDaemon#closeKeepsResumeEntry().
  DaemonModeOptions: DaemonModeOptions#
  PersistedRlmSubagentRegistryEntry.prompt: PersistedRlmSubagentRegistryEntry#prompt.
  PersistedRlmSubagentRegistryEntry.spawnCode: PersistedRlmSubagentRegistryEntry#spawnCode.
  AgentDaemon.updateRestartQueuePauses: AgentDaemon#updateRestartQueuePauses.
  AgentDaemon.updateRestart.typeLiteral28.deferredClientEnv: AgentDaemon#updateRestart.typeLiteral28:deferredClientEnv.
  AgentDaemon.pendingSessionNames: AgentDaemon#pendingSessionNames.
  AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.rlmParentNodeId: AgentDaemon#recordRlmSubagentRegistryEntry().(input)typeLiteral250:rlmParentNodeId.
  AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.prompt: AgentDaemon#recordRlmSubagentRegistryEntry().(input)typeLiteral250:prompt.
  AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.spawnCode: AgentDaemon#recordRlmSubagentRegistryEntry().(input)typeLiteral250:spawnCode.
  AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.model: AgentDaemon#recordRlmSubagentRegistryEntry().(input)typeLiteral250:model.
  AgentDaemon.assertFamilySessionNameAvailable: AgentDaemon#assertFamilySessionNameAvailable().
  AgentDaemon.assertFamilySessionNameAvailable.input-typeLiteral482.name: AgentDaemon#assertFamilySessionNameAvailable().(input)typeLiteral482:name.
  AgentDaemon.assertFamilySessionNameAvailable.input-typeLiteral482.depth: AgentDaemon#assertFamilySessionNameAvailable().(input)typeLiteral482:depth.
  AgentDaemon.sendAgentSessionMessage.options-typeLiteral1160.targetSelector: AgentDaemon#sendAgentSessionMessage().(options)typeLiteral1160:targetSelector.
  AgentDaemon.sendAgentSessionMessage.options-typeLiteral1160.message: AgentDaemon#sendAgentSessionMessage().(options)typeLiteral1160:message.
  structuredLog: structuredLog.
  DAEMON_CLIENT_CAPABILITY_SET: DAEMON_CLIENT_CAPABILITY_SET.
  AgentDaemon.installCrashHandlers: AgentDaemon#installCrashHandlers().
  AgentDaemon.deleteSavedSessionFile: AgentDaemon#deleteSavedSessionFile().
  AgentDaemon.abortWaitingPromptAdmissionsForSession: AgentDaemon#abortWaitingPromptAdmissionsForSession().
  hasDaemonOutboundActiveSessionId: hasDaemonOutboundActiveSessionId().
  SequencedDaemonOutbound: SequencedDaemonOutbound#
  RLM_SUBAGENT_REGISTRY_FILE: RLM_SUBAGENT_REGISTRY_FILE.
  AgentDaemon.ownsSocketPath: AgentDaemon#ownsSocketPath.
  AgentDaemon.bindingCompletions: AgentDaemon#bindingCompletions.
  AgentDaemon.signalCleanupHandlers: AgentDaemon#signalCleanupHandlers.
  AgentDaemon.agentDir: AgentDaemon#agentDir.
  AgentDaemon.restoreActiveSessionId: AgentDaemon#restoreActiveSessionId.
  AgentDaemon.supervisorLaunchInProgress: AgentDaemon#supervisorLaunchInProgress.
  AgentDaemon.canConnectToSupervisor: AgentDaemon#canConnectToSupervisor().
  AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.childId: AgentDaemon#recordRlmSubagentRegistryEntry().(input)typeLiteral250:childId.
  AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.sessionName: AgentDaemon#recordRlmSubagentRegistryEntry().(input)typeLiteral250:sessionName.
  AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.sessionDir: AgentDaemon#recordRlmSubagentRegistryEntry().(input)typeLiteral250:sessionDir.
  AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.sessionFile: AgentDaemon#recordRlmSubagentRegistryEntry().(input)typeLiteral250:sessionFile.
  AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.rlmDepth: AgentDaemon#recordRlmSubagentRegistryEntry().(input)typeLiteral250:rlmDepth.
  AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.rlmMaxDepth: AgentDaemon#recordRlmSubagentRegistryEntry().(input)typeLiteral250:rlmMaxDepth.
  AgentDaemon.updateRlmHeartbeatForState.input-typeLiteral676.interval: AgentDaemon#updateRlmHeartbeatForState().(input)typeLiteral676:interval.
  AgentDaemon.withSessionNameReservation.input-typeLiteral1919.name: AgentDaemon#withSessionNameReservation().(input)typeLiteral1919:name.
  AgentDaemon.withSessionNameReservation.input-typeLiteral1919.depth: AgentDaemon#withSessionNameReservation().(input)typeLiteral1919:depth.
  AgentDaemon.sendAgentSessionMessage: AgentDaemon#sendAgentSessionMessage().
  AgentDaemon.sendAgentSessionMessage.options-typeLiteral1160.clientId: AgentDaemon#sendAgentSessionMessage().(options)typeLiteral1160:clientId.
  AgentDaemon.sendAgentSessionMessage.options-typeLiteral1160.senderKey: AgentDaemon#sendAgentSessionMessage().(options)typeLiteral1160:senderKey.
  isTerminalRemoteAgentMessageError: isTerminalRemoteAgentMessageError().
  DaemonModeOptions.socketPath: DaemonModeOptions#socketPath.
  DaemonModeOptions.worker.typeLiteral0.authenticationToken: DaemonModeOptions#worker.typeLiteral0:authenticationToken.
  WORKER_SNAPSHOT_TERMINAL_DRAIN_TIMEOUT_MS: WORKER_SNAPSHOT_TERMINAL_DRAIN_TIMEOUT_MS.
  delay: delay().
  RuntimeOpenGuard: RuntimeOpenGuard#
  BoundSupervisorGenerationClaim: BoundSupervisorGenerationClaim#
  PersistedRlmSubagentRegistryEntry.type: PersistedRlmSubagentRegistryEntry#type.
  PersistedRlmSubagentRegistryEntry.model.typeLiteral6.provider: PersistedRlmSubagentRegistryEntry#model.typeLiteral6:provider.
  PersistedRlmSubagentRegistryEntry.model.typeLiteral6.modelId: PersistedRlmSubagentRegistryEntry#model.typeLiteral6:modelId.
  PersistedRlmSubagentRegistryEntry.createdAt: PersistedRlmSubagentRegistryEntry#createdAt.
  PersistedRlmSubagentRegistryEntry.updatedAt: PersistedRlmSubagentRegistryEntry#updatedAt.
  AgentDaemon.updateRestart.typeLiteral28.deferredClientEnv.Array.typeLiteral29.env: AgentDaemon#updateRestart.typeLiteral28:deferredClientEnv.Array:typeLiteral29:env.
  AgentDaemon.updateRlmHeartbeatForState.input-typeLiteral676.instruction: AgentDaemon#updateRlmHeartbeatForState().(input)typeLiteral676:instruction.
  AgentDaemon.updateRlmHeartbeatForState.input-typeLiteral676.status: AgentDaemon#updateRlmHeartbeatForState().(input)typeLiteral676:status.
  AgentDaemon.assertFamilySessionNameAvailable.input-typeLiteral482.parentSessionId: AgentDaemon#assertFamilySessionNameAvailable().(input)typeLiteral482:parentSessionId.
  AgentDaemon.withSessionNameReservation.input-typeLiteral1919.parentSessionPath: AgentDaemon#withSessionNameReservation().(input)typeLiteral1919:parentSessionPath.
  UPDATE_RESTART_PREPARE_TIMEOUT_MS: UPDATE_RESTART_PREPARE_TIMEOUT_MS.
  MAX_SESSION_SNAPSHOT_STABILIZATION_RETRIES: MAX_SESSION_SNAPSHOT_STABILIZATION_RETRIES.
  DAEMON_COMMAND_TYPES: DAEMON_COMMAND_TYPES.
  CLIENT_CATCHUP_RETRY_MS: CLIENT_CATCHUP_RETRY_MS.
  UPDATE_RESTART_ABORT_BASH_TIMEOUT_MS: UPDATE_RESTART_ABORT_BASH_TIMEOUT_MS.
  SUPERVISOR_FENCE_POLL_MS: SUPERVISOR_FENCE_POLL_MS.
  UPDATE_RESTART_MARKER: UPDATE_RESTART_MARKER.
  RECOVERY_CHECKPOINT_EVENTS: RECOVERY_CHECKPOINT_EVENTS.
  AgentDaemon.isProcessAlive: AgentDaemon#isProcessAlive().
  AgentDaemon.createRlmHeartbeatForState.input-typeLiteral666.instruction: AgentDaemon#createRlmHeartbeatForState().(input)typeLiteral666:instruction.
  AgentDaemon.createRlmHeartbeatForState.input-typeLiteral666.interval: AgentDaemon#createRlmHeartbeatForState().(input)typeLiteral666:interval.
  AgentDaemon.createRlmHeartbeatForState.input-typeLiteral666.label: AgentDaemon#createRlmHeartbeatForState().(input)typeLiteral666:label.
  AgentDaemon.updateRlmHeartbeatForState.input-typeLiteral676.id: AgentDaemon#updateRlmHeartbeatForState().(input)typeLiteral676:id.
  AgentDaemon.updateRlmHeartbeatForState.input-typeLiteral676.label: AgentDaemon#updateRlmHeartbeatForState().(input)typeLiteral676:label.
  AgentDaemon.withSessionNameReservation.input-typeLiteral1919.parentSessionId: AgentDaemon#withSessionNameReservation().(input)typeLiteral1919:parentSessionId.
  AgentDaemon.createCliAgentMessageSenderKey: AgentDaemon#createCliAgentMessageSenderKey().
  AgentDaemon.assertUpdateRestartNotCancelled.transaction-typeLiteral3072.id: AgentDaemon#assertUpdateRestartNotCancelled().(transaction)typeLiteral3072:id.
  AgentDaemon.assertUpdateRestartNotCancelled.transaction-typeLiteral3072.abort: AgentDaemon#assertUpdateRestartNotCancelled().(transaction)typeLiteral3072:abort.
  SupervisorGenerationClaim.Omit.Extract.typeLiteral5.type: SupervisorGenerationClaim#Omit:Extract:typeLiteral5:type.
  AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.model.typeLiteral251.provider: AgentDaemon#recordRlmSubagentRegistryEntry().(input)typeLiteral250:model.typeLiteral251:provider.
  AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.model.typeLiteral251.modelId: AgentDaemon#recordRlmSubagentRegistryEntry().(input)typeLiteral250:model.typeLiteral251:modelId.
  AgentDaemon.createRuntime.command-Extract.typeLiteral438.type: AgentDaemon#createRuntime().(command)Extract:typeLiteral438:type.
  SequencedDaemonOutbound.Extract.typeLiteral3634.type: SequencedDaemonOutbound#Extract:typeLiteral3634:type.
---
# Module: [`packages/coding-agent/src/modes/daemon/daemon-mode.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts)

## Classes
### `AgentDaemon`
- def: [`packages/coding-agent/src/modes/daemon/daemon-mode.ts:426`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L426)
- signature: `class AgentDaemon`
- members:
  - `<constructor>(socketPath: string, options: DaemonModeOptions)` — [`L525`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L525)
  - `abortBashForClose(method)` — [`L6017`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6017)
  - `abortSideQuestionsFor(method)` — [`L6560`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6560)
  - `abortWaitingPromptAdmissionsForSession(method)` — [`L5906`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5906)
  - `acceptAgentSessionMessage(method)` — [`L5503`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5503)
  - `addRuntime(method)` — [`L1193`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1193)
  - `addSessionEventMeta(method)` — [`L6501`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6501)
  - `adoptClientEnv(method)` — [`L868`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L868) — Adopt env for a session that has none, propagating to subagents spawned
  - `agentFamilyEntry(method)` — [`L5238`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5238)
  - `agentMessageRelationship(method)` — [`L5339`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5339)
  - `appendRlmSubagentRegistryEntry(method)` — [`L889`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L889)
  - `appendUpdateRestartMarker(method)` — [`L5676`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5676)
  - `applyReasonUpgrade(method)` — [`L5984`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5984)
  - `archiveSession(method)` — [`L6013`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6013)
  - `assertAgentFamilyReachable(method)` — [`L5334`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5334)
  - `assertFamilySessionNameAvailable(method)` — [`L5044`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5044)
  - `assertStateSessionNameAvailable(method)` — [`L5071`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5071)
  - `assertSupervisorClaimCurrent(method)` — [`L719`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L719)
  - `assertUpdateRestartNotCancelled(method)` — [`L5718`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5718)
  - `beginReplacementSnapshot(method)` — [`L6197`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6197)
  - `beginUpdateRestartTransaction(method)` — [`L5724`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5724)
  - `broadcastGlobal(method)` — [`L6274`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6274)
  - `broadcastToSession(method)` — [`L6131`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6131)
  - `buildRlmChildSnapshotsWithPassiveRlmSubagents(method)` — [`L1109`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1109) — Add saved-only descendants discovered by the shared passive-registry walk.
  - `buildSessionListWithPassiveRlmSubagents(method)` — [`L1142`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1142)
  - `canConnectToSupervisor(method)` — [`L734`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L734)
  - `cancelPreparedUpdateRestart(method)` — [`L5835`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5835)
  - `cancelRlmHeartbeat(method)` — [`L2084`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2084)
  - `cancelScheduledJobsForSession(method)` — [`L1939`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1939)
  - `cancelScheduledJobsForSessionFile(method)` — [`L1963`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1963)
  - `cancelSubagentRlmHeartbeats(method)` — [`L1926`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1926)
  - `catchUpBackpressuredClient(method)` — [`L6300`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6300)
  - `checkSupervisorAvailability(method)` — [`L654`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L654)
  - `checkSupervisorFences(method)` — [`L705`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L705)
  - `cleanupSocketPath(method)` — [`L853`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L853)
  - `clearClientCatchupRetry(method)` — [`L6317`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6317)
  - `clearQueuedAgentSessionMessagesForAllStates(method)` — [`L5190`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5190)
  - `clearQueuedAgentSessionMessagesForState(method)` — [`L5184`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5184)
  - `clearSupervisorAvailabilityCheck(method)` — [`L684`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L684)
  - `closeChildSessions(method)` — [`L6113`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6113)
  - `closeKeepsResumeEntry(method)` — [`L6009`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6009)
  - `closeReasonStrength(method)` — [`L5974`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5974)
  - `closeSession(method)` — [`L5915`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5915)
  - `closeSessionOnce(method)` — [`L6028`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6028)
  - `commitPreparedUpdateRestart(method)` — [`L5812`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5812)
  - `createAgentFamilyCatalog(method)` — [`L4975`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L4975)
  - `createAgentFamilyRoster(method)` — [`L5037`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5037)
  - `createAgentMessageAgentSummary(method)` — [`L4899`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L4899)
  - `createAgentMessageController(method)` — [`L2822`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2822)
  - `createAgentMessageListResult(method)` — [`L4928`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L4928)
  - `createAgentObserveAgentSnapshot(method)` — [`L2909`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2909)
  - `createAgentObserveController(method)` — [`L2847`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2847)
  - `createAgentObserveListResult(method)` — [`L2862`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2862)
  - `createAgentObserveRecentMessages(method)` — [`L2920`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2920)
  - `createAgentObserveSummary(method)` — [`L2941`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2941)
  - `createAgentSessionMessageEndpoint(method)` — [`L4876`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L4876)
  - `createAgentSessionMessageSender(method)` — [`L4886`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L4886)
  - `createAttachResult(method)` — [`L4560`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L4560)
  - `createCliAgentMessageSenderKey(method)` — [`L5180`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5180)
  - `createConnectionState(method)` — [`L4867`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L4867)
  - `createCronJobForState(method)` — [`L1744`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1744)
  - `createHeartbeatForState(method)` — [`L1763`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1763)
  - `createRlmHeartbeatForState(method)` — [`L1809`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1809)
  - `createRlmSubagentRuntime(method)` — [`L2304`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2304)
  - `createRuntime(method)` — [`L1307`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1307)
  - `createSessionSnapshot(method)` — [`L4604`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L4604)
  - `createSubagentRuntimeHost(method)` — [`L2211`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2211)
  - `createUpdateRestartSession(method)` — [`L5623`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5623)
  - `deleteRlmHeartbeatForState(method)` — [`L1870`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1870)
  - `deleteSavedSessionFile(method)` — [`L1970`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1970)
  - `detachClient(method)` — [`L5885`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5885)
  - `detachClientFromSession(method)` — [`L5571`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5571)
  - `drainBackpressuredClientCatchupQueue(method)` — [`L6344`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6344)
  - `drainBackpressuredClientCatchups(method)` — [`L6357`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6357)
  - `findActiveSessionByFile(method)` — [`L5895`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5895)
  - `findPassivationBySessionFile(method)` — [`L2558`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2558)
  - `findPassiveRlmSubagent(method)` — [`L1176`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1176)
  - `findSessionBySessionFile(method)` — [`L2136`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2136)
  - `getAgentMessageSafetyStatus(method)` — [`L5170`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5170)
  - `getBoundSessionState(method)` — [`L2156`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2156)
  - `getOrCreateCronJobSession(method)` — [`L1984`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1984)
  - `getOrHydrateAuthorizedAgentFamilyTarget(method)` — [`L5279`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5279)
  - `getOrHydrateBoundSessionState(method)` — [`L2167`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2167)
  - `getRunnableCronJob(method)` — [`L1627`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1627)
  - `getSessionState(method)` — [`L2150`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2150)
  - `getShutdownClosingReason(method)` — [`L6598`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6598)
  - `getUpdateRestartSessionDepth(method)` — [`L5702`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5702)
  - `handleCommand(method)` — [`L3438`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L3438) — documented in [packages-coding-agent-src-modes-daemon-daemon-mode.ts](../../../../../../concepts/packages-coding-agent-src-modes-daemon-daemon-mode.ts.md)
  - `handleConnection(method)` — [`L2987`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2987)
  - `handleLine(method)` — [`L3113`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L3113)
  - `handleWorkerCommand(method)` — [`L3332`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L3332)
  - `hasActiveSideQuestionFor(method)` — [`L6570`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6570)
  - `hasAuthenticatedSupervisorConnection(method)` — [`L671`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L671)
  - `hasScheduledJobsForSession(method)` — [`L5876`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5876)
  - `hydratePassiveRlmSubagent(method)` — [`L2567`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2567)
  - `installCrashHandlers(method)` — [`L565`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L565)
  - `isAgentFamilyReachable(method)` — [`L5324`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5324)
  - `isCronJobRunnableForState(method)` — [`L2114`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2114)
  - `isDiscardableDraft(method)` — [`L5592`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5592)
  - `isEmptyDraftContent(method)` — [`L5615`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5615) — True when a session holds nothing worth persisting: no messages, no user
  - `isPersistedCronJobRunnable(method)` — [`L2090`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2090)
  - `isProcessAlive(method)` — [`L844`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L844)
  - `isStrongerCloseReason(method)` — [`L5980`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5980)
  - `launchReplacementSupervisor(method)` — [`L754`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L754)
  - `listHeartbeats(method)` — [`L1879`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1879)
  - `listPassiveRlmSubagents(method)` — [`L1042`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1042) — Walk each supplied parent's persisted child tree once, without creating runtimes.
  - `listTargetableSessionStates(method)` — [`L5162`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5162)
  - `log(method)` — [`L557`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L557)
  - `manageHeartbeat(method)` — [`L1894`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1894)
  - `parseCommandAndRegisterPromptAdmission(method)` — [`L3084`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L3084) — Parse and synchronously register prompt admission before returning a promise.
  - `passivateIdleChildren(method)` — [`L2534`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2534)
  - `passivateSession(method)` — [`L2459`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2459)
  - `passiveAgentFamilyEntry(method)` — [`L5258`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5258)
  - `passiveRlmSubagentsByPath(method)` — [`L1096`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1096)
  - `prepareReplacementSnapshot(method)` — [`L6219`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6219)
  - `prepareUpdateRestart(method)` — [`L5858`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5858)
  - `prepareUpdateRestartCheckpoint(method)` — [`L5763`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5763)
  - `promptAdmissionKey(method)` — [`L3076`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L3076)
  - `promptHeartbeatWithAgentMessagePreparingGuard(method)` — [`L1666`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1666)
  - `promptWithAgentMessagePreparingGuard(method)` — [`L1635`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1635)
  - `queueClientCatchup(method)` — [`L6468`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6468)
  - `readLatestRlmSubagentRegistry(method)` — [`L973`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L973)
  - `readLatestRlmSubagentRegistryPath(method)` — [`L983`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L983)
  - `rebindCronJobsToState(method)` — [`L1910`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1910)
  - `recordRlmSubagentDeletion(method)` — [`L955`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L955)
  - `recordRlmSubagentRegistryEntry(method)` — [`L917`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L917)
  - `recordWorkerRecoveryState(method)` — [`L6280`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6280)
  - `refreshReplacedSessionState(method)` — [`L1276`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1276)
  - `registerCronStoreForState(method)` — [`L1292`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1292)
  - `registerSignalHandlers(method)` — [`L6579`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6579)
  - `rehydrateCompletedRlmSubagent(method)` — [`L2631`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2631)
  - `rehydrateCompletedRlmSubagentOnce(method)` — [`L2691`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2691)
  - `removeQueuedHeartbeatFollowUp(method)` — [`L1977`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1977)
  - `reserveAgentMessageQueueSlot(method)` — [`L5196`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5196)
  - `resolveAgentFamilySessionName(method)` — [`L5302`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5302)
  - `resolveHeaderParentSessionPath(method)` — [`L5064`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5064)
  - `restoreRlmHeartbeatSession(method)` — [`L2035`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2035)
  - `revokeSupervisorClaim(method)` — [`L675`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L675)
  - `rlmSubagentRegistryPath(method)` — [`L881`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L881)
  - `rlmSubagentRegistryPathForEntry(method)` — [`L1033`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1033)
  - `rlmSubagentRegistryPathForInfo(method)` — [`L1037`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1037)
  - `runCronJob(method)` — [`L1558`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1558)
  - `runUpdateRestartPreparation(method)` — [`L5743`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5743)
  - `scheduleClientCatchupRetry(method)` — [`L6325`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6325)
  - `scheduleSupervisorAvailabilityCheck(method)` — [`L637`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L637)
  - `scheduleSupervisorFenceCheck(method)` — [`L695`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L695)
  - `sendAgentSessionMessage(method)` — [`L5347`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5347)
  - `sendRemoteAgentSessionMessage(method)` — [`L5455`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5455)
  - `sessionPassivationSnapshot(method)` — [`L2417`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2417)
  - `setStateSessionName(method)` — [`L5133`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5133)
  - `setStateSessionNameViaSupervisor(method)` — [`L5109`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5109)
  - `shutdown(method)` — [`L6602`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6602)
  - `stampRlmChildActiveSessionId(method)` — [`L6484`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6484)
  - `start(method)` — [`L578`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L578)
  - `startSupervisorMonitor(method)` — [`L629`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L629)
  - `streamWorkerSnapshot(method)` — [`L4645`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L4645)
  - `updateHeartbeatForState(method)` — [`L1792`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1792)
  - `updateRlmHeartbeatForState(method)` — [`L1838`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1838)
  - `waitForBoundSession(method)` — [`L2677`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2677)
  - `waitForHydratingChild(method)` — [`L2201`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2201)
  - `waitForPassivation(method)` — [`L2562`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L2562)
  - `withAgentMessagePreparingGuard(method)` — [`L1699`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1699)
  - `withAgentMessageTargetLock(method)` — [`L5219`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5219)
  - `withSessionNameReservation(method)` — [`L5093`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5093)
  - `write(method)` — [`L6515`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6515)
  - `writeSerialized(method)` — [`L6525`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6525)
  - `writeUpdateRestartManifest(method)` — [`L5696`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5696)
  - `writeWorkerSnapshotBuffer(method)` — [`L4819`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L4819)
  - `writeWorkerSnapshotRecord(method)` — [`L4802`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L4802)
  - `writeWorkerSuccess(method)` — [`L3322`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L3322)
  - `abort` — [`L434`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L434)
  - `abort` — [`L5718`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5718)
  - `agentDir` — [`L488`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L488)
  - `agentMessageAcceptingTargets` — [`L494`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L494)
  - `agentMessagePendingReservations` — [`L492`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L492)
  - `agentMessagePreparingTargets` — [`L497`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L497)
  - `agentMessageRateLimiter` — [`L490`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L490)
  - `agentMessageTargetLocks` — [`L493`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L493)
  - `agentMessagesPaused` — [`L507`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L507)
  - `bindingCompletions` — [`L451`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L451)
  - `bindingSessions` — [`L500`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L500)
  - `childId` — [`L920`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L920)
  - `client` — [`L439`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L439)
  - `clientId` — [`L5352`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5352)
  - `clients` — [`L446`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L446)
  - `closingSessions` — [`L459`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L459)
  - `createdAt` — [`L931`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L931)
  - `cronScheduler` — [`L489`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L489)
  - `cronStore` — [`L487`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L487)
  - `deadline` — [`L435`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L435)
  - `deferredClientEnv` — [`L438`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L438)
  - `deliveryMode` — [`L1815`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1815)
  - `deliveryMode` — [`L1846`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1846)
  - `depth` — [`L5047`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5047)
  - `depth` — [`L5094`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5094)
  - `env` — [`L441`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L441)
  - `fromState` — [`L5350`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5350)
  - `id` — [`L432`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L432)
  - `id` — [`L1841`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1841)
  - `id` — [`L5718`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5718)
  - `ignoreSessionId` — [`L5050`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5050)
  - `instruction` — [`L1812`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1812)
  - `instruction` — [`L1842`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1842)
  - `interval` — [`L1813`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1813)
  - `interval` — [`L1843`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1843)
  - `label` — [`L1814`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1814)
  - `label` — [`L1844`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1844)
  - `manifest` — [`L437`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L437)
  - `message` — [`L5349`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5349)
  - `model` — [`L929`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L929)
  - `modelId` — [`L929`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L929)
  - `mutationDrain` — [`L430`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L430)
  - `name` — [`L5046`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5046)
  - `name` — [`L5094`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5094)
  - `openingSessions` — [`L448`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L448)
  - `origin` — [`L5354`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5354)
  - `owner` — [`L433`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L433)
  - `ownsSocketPath` — [`L444`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L444)
  - `parentSessionId` — [`L5048`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5048)
  - `parentSessionId` — [`L5094`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5094)
  - `parentSessionPath` — [`L5049`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5049)
  - `parentSessionPath` — [`L5094`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5094)
  - `passivatingSessions` — [`L458`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L458) — Resolved-session-file keyed passivations let wake paths join after closeSessionOnce
  - `pendingSessionNames` — [`L501`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L501)
  - `phase` — [`L436`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L436)
  - `prompt` — [`L927`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L927)
  - `promptAdmissions` — [`L477`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L477) — Live prompt admissions, keyed by session and caller-generated admission id.
  - `provider` — [`L929`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L929)
  - `recoveryJournal` — [`L523`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L523)
  - `remoteAgentPeers` — [`L491`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L491)
  - `reservingSessionOpens` — [`L450`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L450) — Covers path resolution through publication in openingSessions, before the runtime promise exists.
  - `restoreActiveSessionId` — [`L502`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L502)
  - `rlmDepth` — [`L924`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L924)
  - `rlmMaxDepth` — [`L925`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L925)
  - `rlmParentNodeId` — [`L926`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L926)
  - `sender` — [`L5351`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5351)
  - `senderKey` — [`L5353`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5353)
  - `server` — [`L427`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L427)
  - `sessionDir` — [`L922`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L922)
  - `sessionFile` — [`L923`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L923)
  - `sessionName` — [`L921`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L921)
  - `sessions` — [`L447`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L447)
  - `shuttingDown` — [`L428`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L428)
  - `sideQuestionRuns` — [`L468`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L468)
  - `signalCleanupHandlers` — [`L486`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L486)
  - `socketIdentity` — [`L445`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L445)
  - `spawnCode` — [`L928`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L928)
  - `state` — [`L440`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L440)
  - `status` — [`L930`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L930)
  - `status` — [`L1845`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1845)
  - `status` — [`L5507`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5507)
  - `summarizer` — [`L508`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L508)
  - `supervisorClaims` — [`L506`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L506)
  - `supervisorFenceTimer` — [`L504`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L504)
  - `supervisorLaunchInProgress` — [`L505`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L505)
  - `supervisorMonitorTimer` — [`L503`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L503)
  - `targetSelector` — [`L5348`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L5348)
  - `type` — [`L1308`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L1308)
  - `type` — [`L4563`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L4563)
  - `type` — [`L6200`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6200)
  - `type` — [`L6222`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6222)
  - `updateRestart` — [`L431`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L431)
  - `updateRestartQueuePauses` — [`L429`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L429)
- uses (calls/refs, reference-scoped): [`Model`](../../../../ai/src/types.ts.md#Model), [`id`](../../../../ai/src/types.ts.md#Model.id), [`provider`](../../../../ai/src/types.ts.md#Model.provider), [`activeSessionId`](active-session-state.ts.md#ActiveSessionState.activeSessionId), [`runtime`](active-session-state.ts.md#ActiveSessionState.runtime), [`ActiveSessionState`](active-session-state.ts.md#ActiveSessionState), [`SessionManager`](../../core/session-manager.ts.md#SessionManager), [`<get>session`](../../core/agent-session-runtime.ts.md#AgentSessionRuntime.-get-session), [`prompt`](../../core/agent-session.ts.md#AgentSession.prompt), [`agent`](../../core/agent-session.ts.md#AgentSession.agent), [`id`](../../core/cron-jobs.ts.md#AgentCronJob.id), [`DaemonCommand`](daemon-protocol.ts.md#DaemonCommand), [`DaemonSocketClient`](active-session-state.ts.md#DaemonSocketClient), [`Api`](../../../../ai/src/types.ts.md#Api), [`summaryForActiveSession`](daemon-session-list.ts.md#summaryForActiveSession), [`activeSessionId`](daemon-session-list.ts.md#SessionSummary.activeSessionId), [`SessionSummary`](daemon-session-list.ts.md#SessionSummary), [`AgentCronJob`](../../core/cron-jobs.ts.md#AgentCronJob), [`cwd`](../../core/agent-session-config.ts.md#AgentSessionRuntimeConfig.cwd), [`request`](daemon-client.ts.md#DaemonClient.request), [`sessionId`](daemon-session-list.ts.md#SessionSummary.sessionId), [`agentDir`](../../core/agent-session-config.ts.md#AgentSessionRuntimeConfig.agentDir), [`createAgentConnectionState`](../agent-connection/snapshot.ts.md#createAgentConnectionState), [`startSideQuestion`](../../core/side-question.ts.md#startSideQuestion), [`<get>messages`](../../core/agent-session.ts.md#AgentSession.-get-messages), [`sessionManager`](../../core/agent-session.ts.md#AgentSession.sessionManager), [`DaemonOutbound`](daemon-protocol.ts.md#DaemonOutbound), [`success`](daemon-protocol.ts.md#success), [`defaultSessionConfig`](daemon-mode.ts.md#DaemonModeOptions.defaultSessionConfig), [`fork`](../../core/agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`createRuntime`](daemon-mode.ts.md#DaemonModeOptions.createRuntime), [`newSession`](../../core/session-manager.ts.md#SessionManager.newSession), [`getSessionFile`](../../core/session-manager.ts.md#SessionManager.getSessionFile), [`<get>sessionFile`](../../core/agent-session.ts.md#AgentSession.-get-sessionFile), [`create`](../../core/session-manager.ts.md#SessionManager.create), [`createHeartbeat`](../../core/cron-jobs.ts.md#AgentCronJobStore.createHeartbeat), [`createRlmHeartbeat`](../../core/cron-jobs.ts.md#AgentCronJobStore.createRlmHeartbeat), [`sendCustomMessage`](../../core/agent-session.ts.md#AgentSession.sendCustomMessage), [`createAgentConnectionResourceSnapshot`](../agent-connection/snapshot.ts.md#createAgentConnectionResourceSnapshot), [`inMemory`](../../core/session-manager.ts.md#SessionManager.inMemory)  (+661 more; 2 test-only)
- used by: [`runDaemonMode`](daemon-mode.ts.md#runDaemonMode)  (18 test-only)

### `BoundSessionUnavailableError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/modes/daemon/daemon-mode.ts:408`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L408)
- signature: `class BoundSessionUnavailableError`
- used by: [`handleCommand`](daemon-mode.ts.md#AgentDaemon.handleCommand), [`origin`](daemon-mode.ts.md#AgentDaemon.sendAgentSessionMessage.options-typeLiteral1160.origin), [`hydratePassiveRlmSubagent`](daemon-mode.ts.md#AgentDaemon.hydratePassiveRlmSubagent), [`restoreRlmHeartbeatSession`](daemon-mode.ts.md#AgentDaemon.restoreRlmHeartbeatSession), [`rehydrateCompletedRlmSubagent`](daemon-mode.ts.md#AgentDaemon.rehydrateCompletedRlmSubagent), [`getOrHydrateBoundSessionState`](daemon-mode.ts.md#AgentDaemon.getOrHydrateBoundSessionState), [`getOrHydrateAuthorizedAgentFamilyTarget`](daemon-mode.ts.md#AgentDaemon.getOrHydrateAuthorizedAgentFamilyTarget), [`waitForBoundSession`](daemon-mode.ts.md#AgentDaemon.waitForBoundSession), [`getBoundSessionState`](daemon-mode.ts.md#AgentDaemon.getBoundSessionState)

### `BoundSupervisorGenerationClaim`
- def: [`packages/coding-agent/src/modes/daemon/daemon-mode.ts:371`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L371)
- signature: `interface BoundSupervisorGenerationClaim`
- members:
  - `claim` — [`L372`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L372)
  - `ownerFingerprint` — [`L373`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L373)
- uses (calls/refs, reference-scoped): [`SupervisorGenerationClaim`](daemon-mode.ts.md#SupervisorGenerationClaim)
- used by: [`handleLine`](daemon-mode.ts.md#AgentDaemon.handleLine), [`revokeSupervisorClaim`](daemon-mode.ts.md#AgentDaemon.revokeSupervisorClaim), [`checkSupervisorFences`](daemon-mode.ts.md#AgentDaemon.checkSupervisorFences), [`supervisorClaims`](daemon-mode.ts.md#AgentDaemon.supervisorClaims)

### `DaemonModeOptions`
- def: [`packages/coding-agent/src/modes/daemon/daemon-mode.ts:212`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L212)
- signature: `interface DaemonModeOptions`
- members:
  - `authenticationToken` — [`L217`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L217)
  - `createRuntime` — [`L215`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L215)
  - `defaultSessionConfig` — [`L214`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L214)
  - `restoreActiveSessionId` — [`L218`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L218)
  - `socketPath` — [`L213`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L213)
  - `worker` — [`L216`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L216)
- uses (calls/refs, reference-scoped): [`DaemonCommand`](daemon-protocol.ts.md#DaemonCommand), [`SessionSummary`](daemon-session-list.ts.md#SessionSummary), [`daemon-protocol.ts`](daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`DaemonOutbound`](daemon-protocol.ts.md#DaemonOutbound), [`CreateAgentSessionRuntimeFactory`](../../core/agent-session-runtime.ts.md#CreateAgentSessionRuntimeFactory), [`daemon-session-list.ts`](daemon-session-list.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-session-list.ts), [`DaemonResponse`](daemon-protocol.ts.md#DaemonResponse), [`AgentSessionRuntimeConfig`](../../core/agent-session-config.ts.md#AgentSessionRuntimeConfig), [`defaultDaemonSocketPath`](daemon-socket.ts.md#defaultDaemonSocketPath), [`daemon-socket.ts`](daemon-socket.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-socket.ts), [`SessionLifecycle`](daemon-session-list.ts.md#SessionLifecycle), [`SessionActivity`](daemon-session-list.ts.md#SessionActivity)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`main`](../../main.ts.md#main), [`handleCommand`](daemon-mode.ts.md#AgentDaemon.handleCommand), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`<constructor>`](daemon-mode.ts.md#AgentDaemon.-constructor), [`createRlmSubagentRuntime`](daemon-mode.ts.md#AgentDaemon.createRlmSubagentRuntime), [`createRuntime`](daemon-mode.ts.md#AgentDaemon.createRuntime), [`rehydrateCompletedRlmSubagentOnce`](daemon-mode.ts.md#AgentDaemon.rehydrateCompletedRlmSubagentOnce), [`origin`](daemon-mode.ts.md#AgentDaemon.sendAgentSessionMessage.options-typeLiteral1160.origin), [`createAgentFamilyCatalog`](daemon-mode.ts.md#AgentDaemon.createAgentFamilyCatalog), [`handleConnection`](daemon-mode.ts.md#AgentDaemon.handleConnection), [`handleLine`](daemon-mode.ts.md#AgentDaemon.handleLine), [`createUpdateRestartSession`](daemon-mode.ts.md#AgentDaemon.createUpdateRestartSession), [`launchReplacementSupervisor`](daemon-mode.ts.md#AgentDaemon.launchReplacementSupervisor), [`start`](daemon-mode.ts.md#AgentDaemon.start), [`registerCronStoreForState`](daemon-mode.ts.md#AgentDaemon.registerCronStoreForState), [`setStateSessionNameViaSupervisor`](daemon-mode.ts.md#AgentDaemon.setStateSessionNameViaSupervisor), [`isDiscardableDraft`](daemon-mode.ts.md#AgentDaemon.isDiscardableDraft), [`revokeSupervisorClaim`](daemon-mode.ts.md#AgentDaemon.revokeSupervisorClaim), [`runDaemonMode`](daemon-mode.ts.md#runDaemonMode), [`startSupervisorMonitor`](daemon-mode.ts.md#AgentDaemon.startSupervisorMonitor)  (14 test-only)

### `PassiveRlmRoot`
- def: [`packages/coding-agent/src/modes/daemon/daemon-mode.ts:397`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L397)
- signature: `type PassiveRlmRoot`
- uses (calls/refs, reference-scoped): [`ActiveSessionState`](active-session-state.ts.md#ActiveSessionState), [`SessionInfo`](../../core/session-manager.ts.md#SessionInfo)
- used by: [`listPassiveRlmSubagents`](daemon-mode.ts.md#AgentDaemon.listPassiveRlmSubagents), [`PassiveRlmSubagent`](daemon-mode.ts.md#PassiveRlmSubagent)

### `PassiveRlmSubagent`
- def: [`packages/coding-agent/src/modes/daemon/daemon-mode.ts:401`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L401)
- signature: `type PassiveRlmSubagent`
- uses (calls/refs, reference-scoped): [`SessionInfo`](../../core/session-manager.ts.md#SessionInfo), [`PersistedRlmSubagentRegistryEntry`](daemon-mode.ts.md#PersistedRlmSubagentRegistryEntry), [`PassiveRlmRoot`](daemon-mode.ts.md#PassiveRlmRoot)
- used by: [`sessionPassivationSnapshot`](daemon-mode.ts.md#AgentDaemon.sessionPassivationSnapshot), [`hydratePassiveRlmSubagent`](daemon-mode.ts.md#AgentDaemon.hydratePassiveRlmSubagent), [`passiveAgentFamilyEntry`](daemon-mode.ts.md#AgentDaemon.passiveAgentFamilyEntry), [`listPassiveRlmSubagents`](daemon-mode.ts.md#AgentDaemon.listPassiveRlmSubagents), [`findPassiveRlmSubagent`](daemon-mode.ts.md#AgentDaemon.findPassiveRlmSubagent), [`passiveRlmSubagentsByPath`](daemon-mode.ts.md#AgentDaemon.passiveRlmSubagentsByPath)

### `PersistedRlmSubagentRegistryEntry`
- def: [`packages/coding-agent/src/modes/daemon/daemon-mode.ts:378`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L378)
- signature: `interface PersistedRlmSubagentRegistryEntry`
- members:
  - `childId` — [`L380`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L380)
  - `createdAt` — [`L393`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L393)
  - `model` — [`L391`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L391)
  - `modelId` — [`L391`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L391)
  - `parentSessionFile` — [`L385`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L385)
  - `parentSessionId` — [`L384`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L384)
  - `prompt` — [`L389`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L389)
  - `provider` — [`L391`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L391)
  - `rlmDepth` — [`L386`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L386)
  - `rlmMaxDepth` — [`L387`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L387)
  - `rlmParentNodeId` — [`L388`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L388)
  - `sessionDir` — [`L382`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L382)
  - `sessionFile` — [`L383`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L383)
  - `sessionName` — [`L381`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L381)
  - `spawnCode` — [`L390`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L390)
  - `status` — [`L392`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L392)
  - `type` — [`L379`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L379)
  - `updatedAt` — [`L394`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L394)
- used by: [`createRuntime`](daemon-mode.ts.md#AgentDaemon.createRuntime), [`rehydrateCompletedRlmSubagentOnce`](daemon-mode.ts.md#AgentDaemon.rehydrateCompletedRlmSubagentOnce), [`createSubagentRuntimeHost`](daemon-mode.ts.md#AgentDaemon.createSubagentRuntimeHost), [`createAgentFamilyCatalog`](daemon-mode.ts.md#AgentDaemon.createAgentFamilyCatalog), [`createAgentMessageListResult`](daemon-mode.ts.md#AgentDaemon.createAgentMessageListResult), [`createAgentObserveListResult`](daemon-mode.ts.md#AgentDaemon.createAgentObserveListResult), [`createdAt`](daemon-mode.ts.md#AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.createdAt), [`sessionPassivationSnapshot`](daemon-mode.ts.md#AgentDaemon.sessionPassivationSnapshot), [`buildSessionListWithPassiveRlmSubagents`](daemon-mode.ts.md#AgentDaemon.buildSessionListWithPassiveRlmSubagents), [`buildRlmChildSnapshotsWithPassiveRlmSubagents`](daemon-mode.ts.md#AgentDaemon.buildRlmChildSnapshotsWithPassiveRlmSubagents), [`hydratePassiveRlmSubagent`](daemon-mode.ts.md#AgentDaemon.hydratePassiveRlmSubagent), [`passiveAgentFamilyEntry`](daemon-mode.ts.md#AgentDaemon.passiveAgentFamilyEntry), [`listPassiveRlmSubagents`](daemon-mode.ts.md#AgentDaemon.listPassiveRlmSubagents), [`rehydrateCompletedRlmSubagent`](daemon-mode.ts.md#AgentDaemon.rehydrateCompletedRlmSubagent), [`readLatestRlmSubagentRegistryPath`](daemon-mode.ts.md#AgentDaemon.readLatestRlmSubagentRegistryPath), [`findPassiveRlmSubagent`](daemon-mode.ts.md#AgentDaemon.findPassiveRlmSubagent), [`readLatestRlmSubagentRegistry`](daemon-mode.ts.md#AgentDaemon.readLatestRlmSubagentRegistry), [`appendRlmSubagentRegistryEntry`](daemon-mode.ts.md#AgentDaemon.appendRlmSubagentRegistryEntry), [`recordRlmSubagentDeletion`](daemon-mode.ts.md#AgentDaemon.recordRlmSubagentDeletion), [`PassiveRlmSubagent`](daemon-mode.ts.md#PassiveRlmSubagent), [`rlmSubagentRegistryPathForEntry`](daemon-mode.ts.md#AgentDaemon.rlmSubagentRegistryPathForEntry), [`passiveRlmSubagentsByPath`](daemon-mode.ts.md#AgentDaemon.passiveRlmSubagentsByPath), [`status`](daemon-mode.ts.md#AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.status)

### `RuntimeOpenCancelledError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/modes/daemon/daemon-mode.ts:407`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L407)
- signature: `class RuntimeOpenCancelledError`
- used by: [`createRuntime`](daemon-mode.ts.md#AgentDaemon.createRuntime), [`rehydrateCompletedRlmSubagentOnce`](daemon-mode.ts.md#AgentDaemon.rehydrateCompletedRlmSubagentOnce), [`addRuntime`](daemon-mode.ts.md#AgentDaemon.addRuntime), [`hydratePassiveRlmSubagent`](daemon-mode.ts.md#AgentDaemon.hydratePassiveRlmSubagent), [`getOrCreateCronJobSession`](daemon-mode.ts.md#AgentDaemon.getOrCreateCronJobSession), [`restoreRlmHeartbeatSession`](daemon-mode.ts.md#AgentDaemon.restoreRlmHeartbeatSession)

### `RuntimeOpenGuard`
- def: [`packages/coding-agent/src/modes/daemon/daemon-mode.ts:368`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L368)
- signature: `type RuntimeOpenGuard`
- used by: [`createRuntime`](daemon-mode.ts.md#AgentDaemon.createRuntime), [`addRuntime`](daemon-mode.ts.md#AgentDaemon.addRuntime)

### `SequencedDaemonOutbound`
- def: [`packages/coding-agent/src/modes/daemon/daemon-mode.ts:6769`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6769)
- signature: `type SequencedDaemonOutbound`
- members:
  - `type` — [`L6772`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6772)
- uses (calls/refs, reference-scoped): [`DaemonOutbound`](daemon-protocol.ts.md#DaemonOutbound)
- used by: [`isSequencedSessionOutbound`](daemon-mode.ts.md#isSequencedSessionOutbound)

### `SupervisorGenerationClaim`
- def: [`packages/coding-agent/src/modes/daemon/daemon-mode.ts:369`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L369)
- signature: `type SupervisorGenerationClaim`
- members:
  - `type` — [`L369`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L369)
- uses (calls/refs, reference-scoped): [`DaemonWorkerCommand`](daemon-worker-protocol.ts.md#DaemonWorkerCommand)
- used by: [`handleLine`](daemon-mode.ts.md#AgentDaemon.handleLine), [`assertSupervisorClaimCurrent`](daemon-mode.ts.md#AgentDaemon.assertSupervisorClaimCurrent), [`claim`](daemon-mode.ts.md#BoundSupervisorGenerationClaim.claim)

## Functions
- `abortClientSnapshotStreaming(client: DaemonSocketClient, activeSessionId?: string | undefined)` — [`L6720`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6720)
- `cancelPendingExtensionUiRequests(state: ActiveSessionState)` — [`L6745`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6745)
- `daemonClientCapabilitiesForSession(client: DaemonSocketClient, activeSessionId: string)` — [`L6691`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6691)
- `daemonClientSupportsExtensionUi(client: DaemonSocketClient, activeSessionId: string)` — [`L6698`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6698)
- `delay(ms: number)` — [`L364`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L364)
- `detachClientFromActiveSession(client: DaemonSocketClient, state: ActiveSessionState)` — [`L6663`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6663)
- `finishClientSnapshotStreaming(client: DaemonSocketClient, activeSessionId: string)` — [`L6730`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6730)
- `getChildActiveSessionStates(sessions: ReadonlyMap<string, ActiveSessionState>, parentState: ActiveSessionState)` — [`L6652`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6652)
- `hasDaemonOutboundActiveSessionId(message: DaemonOutbound)` — [`L6646`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6646)
- `isSequencedSessionOutbound(message: DaemonOutbound)` — [`L6783`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6783)
- `isTerminalRemoteAgentMessageError(error: unknown)` — [`L417`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L417)
- `markClientSnapshotStreaming(client: DaemonSocketClient, activeSessionId: string)` — [`L6702`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6702)
- `normalizeClientCapabilities(capabilities: readonly DaemonClientCapability[] | undefined, supportsExtensionUi: boolean | undefined)` — [`L6753`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6753)
- `removeDaemonClientSessionCapabilities(client: DaemonSocketClient, activeSessionId: string)` — [`L6684`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6684)
- `resolveDaemonSessionPath(selector: string, cwd: string, sessionDir?: string | undefined)` — [`L6803`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6803)
- `runDaemonMode(options: DaemonModeOptions)` — [`L410`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L410)
- `setDaemonClientSessionCapabilities(client: DaemonSocketClient, activeSessionId: string, capabilities: ReadonlySet<DaemonClientCapability>)` — [`L6672`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6672)
- `shouldSendDaemonOutboundToClient(client: DaemonSocketClient, message: DaemonOutbound)` — [`L6795`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L6795)

## Module values
- `CLIENT_CATCHUP_RETRY_MS` — [`L338`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L338)
- `DAEMON_CLIENT_CAPABILITY_SET` — [`L337`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L337)
- `DAEMON_COMMAND_TYPES` — [`L239`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L239)
- `MAX_SESSION_SNAPSHOT_STABILIZATION_RETRIES` — [`L237`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L237)
- `RECOVERY_CHECKPOINT_EVENTS` — [`L345`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L345)
- `RLM_SUBAGENT_REGISTRY_FILE` — [`L376`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L376)
- `SUPERVISOR_FENCE_POLL_MS` — [`L340`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L340)
- `UPDATE_RESTART_ABORT_BASH_TIMEOUT_MS` — [`L339`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L339)
- `UPDATE_RESTART_MARKER` — [`L341`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L341)
- `UPDATE_RESTART_PREPARE_TIMEOUT_MS` — [`L236`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L236)
- `WORKER_SNAPSHOT_TERMINAL_DRAIN_TIMEOUT_MS` — [`L235`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L235)
- `structuredLog` — [`L234`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-mode.ts#L234)


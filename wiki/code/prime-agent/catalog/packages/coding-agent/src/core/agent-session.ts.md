---
title: 'Module: packages/coding-agent/src/core/agent-session.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/agent-session.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`agent-session.ts`/
symbols:
  AgentSession.prompt: AgentSession#prompt().
  AgentSession._startRlmChildRun: AgentSession#_startRlmChildRun().
  AgentSession.agent: AgentSession#agent.
  AgentSession.-constructor: AgentSession#`<constructor>`().
  AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry: AgentSession#_navigateTreeUnderPause().Promise:typeLiteral4237:summaryEntry.
  AgentSession._prompt: AgentSession#_prompt().
  AgentSession._bindExtensionCore: AgentSession#_bindExtensionCore().
  AgentSession._createInlineRlmSubagentRuntime: AgentSession#_createInlineRlmSubagentRuntime().
  AgentSession.-get-messages: AgentSession#`<get>messages`().
  AgentSession.sessionManager: AgentSession#sessionManager.
  AgentSession._processAgentEvent: AgentSession#_processAgentEvent().
  AgentSession._startPreparedTurnActions: AgentSession#_startPreparedTurnActions().
  AgentSession._createKernelHostHandlers: AgentSession#_createKernelHostHandlers().
  AgentSession.dispose: AgentSession#dispose().
  AgentSession.-get-sessionFile: AgentSession#`<get>sessionFile`().
  AgentSession._pumpSessionInputs: AgentSession#_pumpSessionInputs().
  AgentSession._performCompaction.options-typeLiteral2765.signal: AgentSession#_performCompaction().(options)typeLiteral2765:signal.
  AgentSession._buildRuntime: AgentSession#_buildRuntime().
  AgentSession.sendCustomMessage: AgentSession#sendCustomMessage().
  AgentSession.getSessionActionRecoverySnapshot: AgentSession#getSessionActionRecoverySnapshot().
  AgentSession._createPreparedTurnAction.options-typeLiteral696.acceptedBeforeCompletion: AgentSession#_createPreparedTurnAction().(options)typeLiteral696:acceptedBeforeCompletion.
  AgentSession.-get-sessionId: AgentSession#`<get>sessionId`().
  AgentSession._installAgentToolHooks: AgentSession#_installAgentToolHooks().
  AgentSession._emitExtensionEvent: AgentSession#_emitExtensionEvent().
  AgentSession._applyRefine: AgentSession#_applyRefine().
  AgentSession.getSessionStats: AgentSession#getSessionStats().
  AgentSession: AgentSession#
  AgentSession._promptInjectedMessage: AgentSession#_promptInjectedMessage().
  AgentSession._checkCompaction: AgentSession#_checkCompaction().
  AgentSession.restoreSessionActions: AgentSession#restoreSessionActions().
  AgentSession.compact: AgentSession#compact().
  AgentSession._createRlmSubagentRuntimeOptions.options-typeLiteral3607.model: AgentSession#_createRlmSubagentRuntimeOptions().(options)typeLiteral3607:model.
  AgentSession.waitForIdle: AgentSession#waitForIdle().
  AgentSession._cancelSessionActions: AgentSession#_cancelSessionActions().
  AgentSession.mutateQueuedMessage: AgentSession#mutateQueuedMessage().
  AgentSession._handleAgentEvent: AgentSession#_handleAgentEvent.
  AgentSession.-get-model: AgentSession#`<get>model`().
  AgentSession._admitSessionInput.typeLiteral1523.ticket: AgentSession#_admitSessionInput().typeLiteral1523:ticket.
  AgentSession.runRlmChild: AgentSession#runRlmChild().
  AgentSession.getContextUsage: AgentSession#getContextUsage().
  AgentSession._runAutoCompaction: AgentSession#_runAutoCompaction().
  AgentSession._buildRlmSubagentList: AgentSession#_buildRlmSubagentList().
  AgentSession.getContextTree: AgentSession#getContextTree().
  AgentSession.handleCompactHostRequest: AgentSession#handleCompactHostRequest().
  AgentSession._rebuildSystemPrompt: AgentSession#_rebuildSystemPrompt().
  AgentSession._assertRlmSubagentSessionNameAvailable: AgentSession#_assertRlmSubagentSessionNameAvailable().
  AgentSession._executeSelectedSessionCommand: AgentSession#_executeSelectedSessionCommand().
  AgentSession.deleteRlmSubagent: AgentSession#deleteRlmSubagent().
  AgentSession.setModel: AgentSession#setModel().
  AgentSession.refine: AgentSession#refine().
  AgentSession._handleRetryableError: AgentSession#_handleRetryableError().
  AgentSession.getUserMessagesForForking: AgentSession#getUserMessagesForForking().
  AgentSession._actionStore: AgentSession#_actionStore.
  AgentSession.clearQueue: AgentSession#clearQueue().
  AgentSession._maybeAutoRefine: AgentSession#_maybeAutoRefine().
  AgentSession._refreshToolRegistry: AgentSession#_refreshToolRegistry().
  AgentSession.reload: AgentSession#reload().
  AgentSession.subscribe: AgentSession#subscribe().
  AgentSession.clearQueuedUserMessagesMatching: AgentSession#clearQueuedUserMessagesMatching().
  AgentSession.recordBashResult: AgentSession#recordBashResult().
  AgentSession.setRlmMaxDepth: AgentSession#setRlmMaxDepth().
  AgentSession.bindExtensions: AgentSession#bindExtensions().
  AgentSession._cycleScopedModel: AgentSession#_cycleScopedModel().
  AgentSession.requestAbort: AgentSession#requestAbort().
  AgentSession._drainPendingRefinementForDisposal: AgentSession#_drainPendingRefinementForDisposal().
  AgentSession.-get-isStreaming: AgentSession#`<get>isStreaming`().
  AgentSession.disposeAsync: AgentSession#disposeAsync().
  AgentSession._notifyKernelStateAfterCompaction: AgentSession#_notifyKernelStateAfterCompaction().
  AgentSession._restoreLateIpythonSentAgentMessages: AgentSession#_restoreLateIpythonSentAgentMessages().
  AgentSession.handleRefineHostRequest: AgentSession#handleRefineHostRequest().
  AgentSession._cycleAvailableModel: AgentSession#_cycleAvailableModel().
  AgentSession._planRefine: AgentSession#_planRefine().
  AgentSession.getFollowUpMessages: AgentSession#getFollowUpMessages().
  AgentSession._loadPersistedGoalState: AgentSession#_loadPersistedGoalState().
  AgentSession.-get-goalState: AgentSession#`<get>goalState`().
  AgentSession._deleteResolvedRlmSubagent: AgentSession#_deleteResolvedRlmSubagent().
  AgentSession._appendBeforeAgentStartMessages: AgentSession#_appendBeforeAgentStartMessages().
  AgentSession.abort: AgentSession#abort().
  AgentSession.waitForSessionInputCheckpoint: AgentSession#waitForSessionInputCheckpoint().
  AgentSession._loadRefinementHistory: AgentSession#_loadRefinementHistory().
  AgentSession.acquireQueuedWorkPause: AgentSession#acquireQueuedWorkPause().
  AgentSession._queueAutonomousContinuationForThresholdCompaction: AgentSession#_queueAutonomousContinuationForThresholdCompaction().
  AgentSession._loadPersistedRlmMaxDepthState: AgentSession#_loadPersistedRlmMaxDepthState().
  AgentSession._executeQueuedSessionCommand: AgentSession#_executeQueuedSessionCommand().
  AgentSession.runUserBashLocked: AgentSession#runUserBashLocked().
  AgentSession._goalState: AgentSession#_goalState.
  AgentSession.acceptAgentMessagePrompt: AgentSession#acceptAgentMessagePrompt().
  AgentSession.listRlmSubagents: AgentSession#listRlmSubagents().
  AgentSession._extensionRunner: AgentSession#_extensionRunner.
  AgentSession._clearQueuedAutonomousContinuations: AgentSession#_clearQueuedAutonomousContinuations().
  AgentSession.extendResourcesFromExtensions: AgentSession#extendResourcesFromExtensions().
  AgentSessionEvent: AgentSessionEvent#
  AgentSession.followUp: AgentSession#followUp().
  AgentSession._runtimeActivity: AgentSession#_runtimeActivity().
  AgentSession.promptAndWait: AgentSession#promptAndWait().
  AgentSession.settingsManager: AgentSession#settingsManager.
  AgentSession._appendDurableSessionCommandMessage: AgentSession#_appendDurableSessionCommandMessage().
  AgentSession.getPendingNextTurnMessageSnapshots: AgentSession#getPendingNextTurnMessageSnapshots().
  AgentSession._maybeStartSerializedBackgroundPlan: AgentSession#_maybeStartSerializedBackgroundPlan().
  AgentSession.getSessionActionSnapshot: AgentSession#getSessionActionSnapshot().
  AgentSession._getThresholdContextTokens: AgentSession#_getThresholdContextTokens().
  AgentSession._clearQueuedGoalContexts: AgentSession#_clearQueuedGoalContexts().
  AgentSession._prepareForCommit: AgentSession#_prepareForCommit().
  AgentSession._findAssistantEntryForMessage: AgentSession#_findAssistantEntryForMessage().
  AgentSession.-get-modelRegistry: AgentSession#`<get>modelRegistry`().
  AgentSession._emit: AgentSession#_emit().
  AgentSession.handleRlmHeartbeatHostRequest: AgentSession#handleRlmHeartbeatHostRequest().
  AgentSession.setThinkingLevel: AgentSession#setThinkingLevel().
  AgentSession._isBranchSeedable: AgentSession#_isBranchSeedable().
  AgentSession._createSessionCommandAction.options-typeLiteral1777.source: AgentSession#_createSessionCommandAction().(options)typeLiteral1777:source.
  AgentSession._runScheduledPostCompactionContinue: AgentSession#_runScheduledPostCompactionContinue().
  AgentSession._modelVisibleSkills: AgentSession#_modelVisibleSkills().
  AgentSession.getLastAssistantText: AgentSession#getLastAssistantText().
  AgentSession.steer: AgentSession#steer().
  SessionActionRecoveryAction.payload: SessionActionRecoveryAction#payload.
  AgentSession._emitAutonomousStatus: AgentSession#_emitAutonomousStatus().
  AgentSession._getContinuationMessages: AgentSession#_getContinuationMessages().
  AgentSession.-get-queuedActionCount: AgentSession#`<get>queuedActionCount`().
  AgentSession.setServiceTier: AgentSession#setServiceTier().
  AgentSession._persistCompactionOutcome: AgentSession#_persistCompactionOutcome().
  AgentSession._startGoal: AgentSession#_startGoal().
  AgentSession.-get-systemPrompt: AgentSession#`<get>systemPrompt`().
  AgentSession.queueAgentMessagePrompt: AgentSession#queueAgentMessagePrompt().
  AgentSession._accountGoalUsageForAssistantMessage: AgentSession#_accountGoalUsageForAssistantMessage().
  AgentSession.getActiveToolNames: AgentSession#getActiveToolNames().
  AgentSession._disposed: AgentSession#_disposed.
  AgentSession._shouldStopAfterTurn: AgentSession#_shouldStopAfterTurn().
  AgentSession._thresholdCompactionNeeded: AgentSession#_thresholdCompactionNeeded().
  AgentSession.executeBash: AgentSession#executeBash().
  AgentSession._runSerializedAutoRefineReview: AgentSession#_runSerializedAutoRefineReview().
  AgentSession.getAutonomousStatus: AgentSession#getAutonomousStatus().
  AgentSession._reviewAutoRefine: AgentSession#_reviewAutoRefine().
  AgentSession.getRlmChildSession: AgentSession#getRlmChildSession().
  AgentSession.handleAgentObserveHostRequest: AgentSession#handleAgentObserveHostRequest().
  AgentSession.-get-sessionName: AgentSession#`<get>sessionName`().
  AgentSession._emitRlmSubagentRemoval: AgentSession#_emitRlmSubagentRemoval().
  AgentSession.deleteInactiveRlmSubagent: AgentSession#deleteInactiveRlmSubagent().
  AgentSession._shouldStopForThresholdCompaction: AgentSession#_shouldStopForThresholdCompaction().
  AgentSession._expandSkillCommand: AgentSession#_expandSkillCommand().
  AgentSession.restoreSteeringMessage.options-typeLiteral1729.prefixMessages: AgentSession#restoreSteeringMessage().(options)typeLiteral1729:prefixMessages.
  AgentSession.restoreFollowUpMessage.options-typeLiteral1730.prefixMessages: AgentSession#restoreFollowUpMessage().(options)typeLiteral1730:prefixMessages.
  AgentSession._scheduleSessionInputPump: AgentSession#_scheduleSessionInputPump().
  AgentSession.abortForUpdateRestart: AgentSession#abortForUpdateRestart().
  SessionActionRecoverySnapshot.actions: SessionActionRecoverySnapshot#actions.
  appendSentAgentMessageToToolResult: appendSentAgentMessageToToolResult().
  AgentSession._runSerializedRefineCheckpointAfterBackground: AgentSession#_runSerializedRefineCheckpointAfterBackground().
  AgentSession._turnExecutionPolicy.options-typeLiteral1740.skipPrePromptWork: AgentSession#_turnExecutionPolicy().(options)typeLiteral1740:skipPrePromptWork.
  AgentSession.removeQueuedFollowUp: AgentSession#removeQueuedFollowUp().
  rlmHeartbeatHostResponse: rlmHeartbeatHostResponse().
  AgentSession._handleGoalSlashCommand: AgentSession#_handleGoalSlashCommand().
  AgentSession.handleGoalHostRequest: AgentSession#handleGoalHostRequest().
  AgentSession._addLoginGuidanceToAuthError: AgentSession#_addLoginGuidanceToAuthError().
  AgentSession.setSessionName: AgentSession#setSessionName().
  AgentSession._normalizeSubmission: AgentSession#_normalizeSubmission().
  primaryDeliveryRecord: primaryDeliveryRecord().
  queuedAgentMessagePreview: queuedAgentMessagePreview().
  AgentSession.registerRlmChildSession: AgentSession#registerRlmChildSession().
  AgentSession._runOrQueueGoalContext: AgentSession#_runOrQueueGoalContext().
  AgentSession._runBackgroundPlan: AgentSession#_runBackgroundPlan().
  AgentSession._getGoalContinuationMessages: AgentSession#_getGoalContinuationMessages().
  AgentSession._addWebsearchKeyEnv: AgentSession#_addWebsearchKeyEnv().
  AgentSession._findLastAssistantMessage: AgentSession#_findLastAssistantMessage().
  AgentSession.acquireQueuedWorkPause.typeLiteral2422.release: AgentSession#acquireQueuedWorkPause().typeLiteral2422:release().
  RlmChildRun.status: RlmChildRun#status.
  AgentSession._setGoalState: AgentSession#_setGoalState().
  AgentSession._navigateTree.Promise.typeLiteral4222.summaryEntry: AgentSession#_navigateTree().Promise:typeLiteral4222:summaryEntry.
  AgentSession._applyLateIpythonSentAgentMessages: AgentSession#_applyLateIpythonSentAgentMessages().
  AgentSession.exportToHtml: AgentSession#exportToHtml().
  AgentSession.exportToJsonl: AgentSession#exportToJsonl().
  AgentSession.promptHeartbeat: AgentSession#promptHeartbeat().
  turnExecutionPoliciesEqual: turnExecutionPoliciesEqual().
  AgentSession._resumeGoal: AgentSession#_resumeGoal().
  AgentSession.navigateTree: AgentSession#navigateTree().
  AgentSession._settleAgentMessage: AgentSession#_settleAgentMessage().
  AgentSession._removeRlmSubagentTracking: AgentSession#_removeRlmSubagentTracking().
  AgentSession.waitForAgentMessagePromptDelivery: AgentSession#waitForAgentMessagePromptDelivery().
  AgentSession._isBusyForSessionInput: AgentSession#_isBusyForSessionInput().
  AgentSession.setActiveToolsByName: AgentSession#setActiveToolsByName().
  AgentSession._runApprovedRefine: AgentSession#_runApprovedRefine().
  AgentSession.setRlmHeartbeatController: AgentSession#setRlmHeartbeatController().
  AgentSession._reloadRlmMaxDepthFromBranch: AgentSession#_reloadRlmMaxDepthFromBranch().
  AgentSession._isPromptTurnStartMessage: AgentSession#_isPromptTurnStartMessage().
  AgentSession._disposeAsyncOnce: AgentSession#_disposeAsyncOnce().
  AgentSession.getAllTools: AgentSession#getAllTools().
  AgentSession._executeExtensionCommand: AgentSession#_executeExtensionCommand().
  RlmChildRun.id: RlmChildRun#id.
  AgentSession._disposing: AgentSession#_disposing.
  AgentSession._lastAutoRefineReviewAt: AgentSession#_lastAutoRefineReviewAt.
  AgentSession.handleAgentMessageHostRequest: AgentSession#handleAgentMessageHostRequest().
  AgentSession._captureRetryAuthFailureSource: AgentSession#_captureRetryAuthFailureSource().
  QueuedSessionAction: QueuedSessionAction#
  AgentSession._activeRlmChildRuns: AgentSession#_activeRlmChildRuns.
  AgentSession._modelRegistry: AgentSession#_modelRegistry.
  AgentSession._runSerializedRefine.options-typeLiteral770.global: AgentSession#_runSerializedRefine().(options)typeLiteral770:global.
  AgentSession.abortRetry: AgentSession#abortRetry().
  AgentSession._refineInFlight: AgentSession#_refineInFlight.
  AgentSession._resolveRlmMaxDepth: AgentSession#_resolveRlmMaxDepth().
  AgentSession._runSerializedRefineCheckpoint: AgentSession#_runSerializedRefineCheckpoint().
  AgentSession.-get-thinkingLevel: AgentSession#`<get>thinkingLevel`().
  AgentSession._restoreSessionCommand: AgentSession#_restoreSessionCommand().
  AgentSession._restorePromptInput: AgentSession#_restorePromptInput().
  AgentSession.runUserBash.options-typeLiteral4141.runId: AgentSession#runUserBash().(options)typeLiteral4141:runId.
  AgentSession._emitQueueUpdate: AgentSession#_emitQueueUpdate().
  AgentSession.-get-isSessionActive: AgentSession#`<get>isSessionActive`().
  AgentSession.-get-isRetrying: AgentSession#`<get>isRetrying`().
  AgentSession._autoRefineBranchVersion: AgentSession#_autoRefineBranchVersion.
  AgentSession._completeGoalFromHost: AgentSession#_completeGoalFromHost().
  AgentSession._createRetryPromiseForAgentEnd: AgentSession#_createRetryPromiseForAgentEnd().
  AgentSession.-get-serviceTier: AgentSession#`<get>serviceTier`().
  AgentSession.resumeQueuedWork: AgentSession#resumeQueuedWork().
  AgentSession._serializedPlanInFlight: AgentSession#_serializedPlanInFlight.
  AgentSession._findLastAssistantInMessages: AgentSession#_findLastAssistantInMessages().
  AgentSession._mergeUnpersistedCompactionOutcomes: AgentSession#_mergeUnpersistedCompactionOutcomes().
  AgentSession.restoreFollowUpMessage: AgentSession#restoreFollowUpMessage().
  AgentSession._acquireDirectTurnAdmissionFence: AgentSession#_acquireDirectTurnAdmissionFence().
  AgentSession.getSteeringMessages: AgentSession#getSteeringMessages().
  AgentSession.-get-isBashRunning: AgentSession#`<get>isBashRunning`().
  AgentSessionConfig.agent: AgentSessionConfig#agent.
  AgentSession._capturingCancelledAction: AgentSession#_capturingCancelledAction().
  AgentSession.-get-isCompacting: AgentSession#`<get>isCompacting`().
  AgentSession.setFollowUpMode: AgentSession#setFollowUpMode().
  AgentSession._isRetryableError: AgentSession#_isRetryableError().
  AgentSession.navigateTree.Promise.typeLiteral134.summaryEntry: AgentSession#navigateTree().Promise:typeLiteral134:summaryEntry.
  visibleSessionActionProjection: visibleSessionActionProjection().
  AgentSession._pendingRequestedRefine: AgentSession#_pendingRequestedRefine.
  AgentSession.-get-hasPendingSessionWork: AgentSession#`<get>hasPendingSessionWork`().
  AgentSession.releaseRlmChildSession: AgentSession#releaseRlmChildSession().
  AgentSessionConfig.sessionManager: AgentSessionConfig#sessionManager.
  AgentSessionConfig.settingsManager: AgentSessionConfig#settingsManager.
  AgentSessionConfig.resourceLoader: AgentSessionConfig#resourceLoader.
  AgentSessionConfig.modelRegistry: AgentSessionConfig#modelRegistry.
  parsePersistedIpythonSentAgentMessage: parsePersistedIpythonSentAgentMessage().
  AgentSession._pauseGoal: AgentSession#_pauseGoal().
  AgentSession._formatAutonomousStatus: AgentSession#_formatAutonomousStatus().
  AgentSession.-get-state: AgentSession#`<get>state`().
  AgentSession._applyPreparedSystemPrompt: AgentSession#_applyPreparedSystemPrompt().
  AgentSession.followUp.options-typeLiteral1689.resumeIfIdle: AgentSession#followUp().(options)typeLiteral1689:resumeIfIdle.
  AgentSession._coalescedFollowUpOwner: AgentSession#_coalescedFollowUpOwner().
  AgentSession._onIpythonStateRestored: AgentSession#_onIpythonStateRestored().
  AgentSession._invalidatePendingAutoRefineForBranchChange: AgentSession#_invalidatePendingAutoRefineForBranchChange().
  AgentSession._awaitPendingRlmChildPublication: AgentSession#_awaitPendingRlmChildPublication().
  AgentSession._finishSubmissionNormalization: AgentSession#_finishSubmissionNormalization().
  AgentSession._canStartSessionActionImmediately: AgentSession#_canStartSessionActionImmediately().
  AgentSession._createDeliveryRecord: AgentSession#_createDeliveryRecord().
  AgentSession.waitForSessionInputIdle: AgentSession#waitForSessionInputIdle().
  TurnExecutionPolicy.preparation: TurnExecutionPolicy#preparation.
  normalizeMessageContent: normalizeMessageContent().
  AgentSession.cycleModel: AgentSession#cycleModel().
  AgentSession.-get-hasAcceptedPromptInFlight: AgentSession#`<get>hasAcceptedPromptInFlight`().
  AgentSession.getRlmMaxDepthStatus: AgentSession#getRlmMaxDepthStatus().
  AgentSession._assistantTurnsSinceAutoRefine: AgentSession#_assistantTurnsSinceAutoRefine.
  AgentSession._rememberLateIpythonSentAgentMessage: AgentSession#_rememberLateIpythonSentAgentMessage().
  AgentSession._finishGoalWithError: AgentSession#_finishGoalWithError().
  AgentSession._validateCanStartAgentRun: AgentSession#_validateCanStartAgentRun().
  AgentSession.-get-unfinishedActionCount: AgentSession#`<get>unfinishedActionCount`().
  AgentSession._applyExtensionBindings: AgentSession#_applyExtensionBindings().
  AgentSession._refreshCurrentModelFromRegistry: AgentSession#_refreshCurrentModelFromRegistry().
  AgentSession._authenticatedRlmModels: AgentSession#_authenticatedRlmModels().
  RlmChildRun.session: RlmChildRun#session.
  AgentSession._autonomousState: AgentSession#_autonomousState.
  AgentSession._rlmChildSessions: AgentSession#_rlmChildSessions.
  AgentSession._getRequiredRequestAuth: AgentSession#_getRequiredRequestAuth().
  AgentSession.cancelRlmChildRun: AgentSession#cancelRlmChildRun().
  AgentSessionConfig.cwd: AgentSessionConfig#cwd.
  AgentSession._recordLateIpythonSentAgentMessage: AgentSession#_recordLateIpythonSentAgentMessage().
  AgentSession.buildSessionContext: AgentSession#buildSessionContext().
  AgentSession._acquireSessionActionCommitFence: AgentSession#_acquireSessionActionCommitFence().
  AgentSession._resolveRlmSubagentModel: AgentSession#_resolveRlmSubagentModel().
  AgentSession._ensureGoalRuntimeActive: AgentSession#_ensureGoalRuntimeActive().
  AgentSession.-get-rlmDepth: AgentSession#`<get>rlmDepth`().
  AgentSession.sendUserMessage: AgentSession#sendUserMessage().
  AgentSession._clampServiceTierForModel: AgentSession#_clampServiceTierForModel().
  AgentSession._cancelRlmChildRun: AgentSession#_cancelRlmChildRun().
  AgentSession._retryAttempt: AgentSession#_retryAttempt.
  AgentSession._refineAbortController: AgentSession#_refineAbortController.
  AgentSession._queuePreparedPrompt.options-typeLiteral1804.source: AgentSession#_queuePreparedPrompt().(options)typeLiteral1804:source.
  AgentSession._finishGoalForTerminalAssistantMessage: AgentSession#_finishGoalForTerminalAssistantMessage().
  AgentSession.-get-_steeringStopPending: AgentSession#`<get>_steeringStopPending`().
  AgentSession._hasCancelledDispatchCapture: AgentSession#_hasCancelledDispatchCapture().
  AgentSession._surfaceSessionInputError: AgentSession#_surfaceSessionInputError().
  AgentSession._schedulePostCompactionContinue: AgentSession#_schedulePostCompactionContinue().
  AgentSession.hasRunningRlmChildren: AgentSession#hasRunningRlmChildren().
  AgentSession._flushPendingBashMessages: AgentSession#_flushPendingBashMessages().
  AgentSession._refinePlanInFlight: AgentSession#_refinePlanInFlight.
  AgentSession.-get-resourceLoader: AgentSession#`<get>resourceLoader`().
  PreparedTurnPayload.captureRunMessages: PreparedTurnPayload#captureRunMessages.
  attributeChildUsage: attributeChildUsage().
  AgentSession._agentMessageController: AgentSession#_agentMessageController.
  AgentSession._discardPendingAutoRefine: AgentSession#_discardPendingAutoRefine().
  AgentSession._rlmKernelEnv: AgentSession#_rlmKernelEnv().
  AgentSession._markProviderAuthStale: AgentSession#_markProviderAuthStale().
  AgentSession._markProviderAuthStaleForRetryFailure.options-typeLiteral4097.authSourceTokens: AgentSession#_markProviderAuthStaleForRetryFailure().(options)typeLiteral4097:authSourceTokens.
  AgentSession.createReplacedSessionContext: AgentSession#createReplacedSessionContext().
  AgentSession._agentEventQueue: AgentSession#_agentEventQueue.
  AgentSession._subagentRuntimeHost: AgentSession#_subagentRuntimeHost.
  AgentSession._compactAutoRefinePending: AgentSession#_compactAutoRefinePending.
  AgentSession._restoreAutonomousRuntimeSnapshot: AgentSession#_restoreAutonomousRuntimeSnapshot().
  AgentSession.getFollowUpMessagePreviews: AgentSession#getFollowUpMessagePreviews().
  AgentSession._trackModelSelectEmitError: AgentSession#_trackModelSelectEmitError().
  AgentSession._getThinkingLevelForModelSwitch: AgentSession#_getThinkingLevelForModelSwitch().
  AgentSession._scheduleAutoRefine: AgentSession#_scheduleAutoRefine().
  AgentSession._rlmSubagentMatchesTarget: AgentSession#_rlmSubagentMatchesTarget().
  cloneQueuedAgentMessage: cloneQueuedAgentMessage().
  readAssistantText: readAssistantText().
  AgentSession._baseSystemPrompt: AgentSession#_baseSystemPrompt.
  AgentSession._snapshotAutonomousRuntimeState: AgentSession#_snapshotAutonomousRuntimeState().
  AgentSession.promptUntilAccepted: AgentSession#promptUntilAccepted().
  AgentSession._forgetConsumedPostCompactionContinuations: AgentSession#_forgetConsumedPostCompactionContinuations().
  AgentSession._pendingNextTurnMessages: AgentSession#_pendingNextTurnMessages.
  AgentSession._resourceLoader: AgentSession#_resourceLoader.
  AgentSession._rlmChildCleanupFailures: AgentSession#_rlmChildCleanupFailures.
  PromptOptions: PromptOptions#
  SessionActionRecoveryPayload: SessionActionRecoveryPayload#
  injectedMessagePreviewLabel: injectedMessagePreviewLabel().
  AgentSession._parseGoalSlashCommand: AgentSession#_parseGoalSlashCommand().
  AgentSession._handleAutonomousSlashCommand: AgentSession#_handleAutonomousSlashCommand().
  AgentSession._invalidateQueuedPromptPreparation: AgentSession#_invalidateQueuedPromptPreparation().
  AgentSession._finishActiveRetryWithFailure: AgentSession#_finishActiveRetryWithFailure().
  AgentSession._notifySessionInputCheckpointChange: AgentSession#_notifySessionInputCheckpointChange().
  AgentSession._queueModelSelectEmit: AgentSession#_queueModelSelectEmit().
  AgentSession.cycleThinkingLevel: AgentSession#cycleThinkingLevel().
  AgentSession._scheduleAutoRefineAfterAgentEnd: AgentSession#_scheduleAutoRefineAfterAgentEnd().
  AgentSession.findRlmModels: AgentSession#findRlmModels().
  cloneCustomMessage: cloneCustomMessage().
  AgentSession._rlmDepth: AgentSession#_rlmDepth.
  AgentSession.-get-promptTemplates: AgentSession#`<get>promptTemplates`().
  AgentSession._localHarnessStateDir: AgentSession#_localHarnessStateDir().
  AgentSession.-get-extensionRunner: AgentSession#`<get>extensionRunner`().
  AgentSession._goalWithCurrentWallClock: AgentSession#_goalWithCurrentWallClock().
  AgentSession._resolveRetry: AgentSession#_resolveRetry().
  AgentSession.setSteeringMode: AgentSession#setSteeringMode().
  AgentSession._scheduleDeferredAutoRefineIfIdle: AgentSession#_scheduleDeferredAutoRefineIfIdle().
  AgentSession._loadMergedHarnessState: AgentSession#_loadMergedHarnessState().
  AgentSession._deletingRlmChildren: AgentSession#_deletingRlmChildren.
  AgentSession._goalWithAccountedWallClock: AgentSession#_goalWithAccountedWallClock().
  AgentSession._consumeSerializedBackgroundPlan: AgentSession#_consumeSerializedBackgroundPlan().
  AgentSession._assertSessionActionAdmissionAvailable: AgentSession#_assertSessionActionAdmissionAvailable().
  AgentSession._queuePreparedPrompt: AgentSession#_queuePreparedPrompt().
  AgentSession._hasSelectableSessionInput: AgentSession#_hasSelectableSessionInput().
  AgentSession.getSteeringMessagePreviews: AgentSession#getSteeringMessagePreviews().
  AgentSession._autoRefineAllowedForSession: AgentSession#_autoRefineAllowedForSession().
  AgentSession._scheduleAutoRefineAfterCompaction: AgentSession#_scheduleAutoRefineAfterCompaction().
  RlmChildRun.detachedDeletion: RlmChildRun#detachedDeletion.
  AgentSession._retryAuthFailureSources: AgentSession#_retryAuthFailureSources.
  AgentSession._installAgentTurnHook: AgentSession#_installAgentTurnHook().
  AgentSession._reloadGoalStateFromBranch: AgentSession#_reloadGoalStateFromBranch().
  AgentSession._persistGoalState: AgentSession#_persistGoalState().
  AgentSession._observeSessionActionDeferral: AgentSession#_observeSessionActionDeferral().
  AgentSession._cancelPostCompactionContinue: AgentSession#_cancelPostCompactionContinue().
  AgentSession._endCompactionUnsuccessfully.options-typeLiteral3110.customInstructions: AgentSession#_endCompactionUnsuccessfully().(options)typeLiteral3110:customInstructions.
  AgentSession.setExecEnvProvider: AgentSession#setExecEnvProvider().
  AgentSession.-get-repliedToParentSinceTask: AgentSession#`<get>repliedToParentSinceTask`().
  AgentSession._createRlmSubagentRuntime: AgentSession#_createRlmSubagentRuntime().
  AgentSession._resolveDirectRlmSubagent: AgentSession#_resolveDirectRlmSubagent().
  AgentSession.abortBash: AgentSession#abortBash().
  PreparedTurnPayload.content: PreparedTurnPayload#content.
  createAgentMessageDeferred: createAgentMessageDeferred().
  RlmChildRun.unsubscribe: RlmChildRun#unsubscribe.
  autoRefineInstructions: autoRefineInstructions().
  AgentSession._sessionInputPumpSuspended: AgentSession#_sessionInputPumpSuspended.
  AgentSession._cwd: AgentSession#_cwd.
  AgentSession.getAvailableThinkingLevels: AgentSession#getAvailableThinkingLevels().
  AgentSession._trackRlmSubagentDeletion: AgentSession#_trackRlmSubagentDeletion().
  AgentSession._deleteRlmSubagentSession: AgentSession#_deleteRlmSubagentSession().
  AgentSession._isConcreteProviderAuthFailure: AgentSession#_isConcreteProviderAuthFailure().
  AgentSession.runUserBash: AgentSession#runUserBash().
  SessionActionRecoverySnapshot: SessionActionRecoverySnapshot#
  AgentSession._postCompactionContinuationMessages: AgentSession#_postCompactionContinuationMessages.
  AgentSession.getToolDefinition: AgentSession#getToolDefinition().
  AgentSession.-get-rlmMaxDepth: AgentSession#`<get>rlmMaxDepth`().
  AgentSession.getRlmChildRunStatus: AgentSession#getRlmChildRunStatus().
  AgentSession._lastSessionActionSnapshot: AgentSession#_lastSessionActionSnapshot.
  AgentSession._sessionInputPumpEpoch: AgentSession#_sessionInputPumpEpoch.
  AgentSession._pendingAutoRefineReview: AgentSession#_pendingAutoRefineReview.
  AgentSession._applySerializedPlan: AgentSession#_applySerializedPlan().
  AgentSession._reconnectToAgent: AgentSession#_reconnectToAgent().
  AgentSession._buildPromptContent: AgentSession#_buildPromptContent().
  AgentSession._isSessionInputHandoffDeferred: AgentSession#_isSessionInputHandoffDeferred().
  AgentSession._getProviderStreamFailureDetails: AgentSession#_getProviderStreamFailureDetails().
  AgentSession._scopedModels.Array.typeLiteral301.model: AgentSession#_scopedModels.Array:typeLiteral301:model.
  AgentSession._admitSessionInput: AgentSession#_admitSessionInput().
  AgentSession.-get-hasPendingAdmissionWaiters: AgentSession#`<get>hasPendingAdmissionWaiters`().
  QueuedAgentMessage: QueuedAgentMessage#
  AgentSession._sessionInputCheckpointWaiters: AgentSession#_sessionInputCheckpointWaiters.
  AgentSession._rlmMaxDepth: AgentSession#_rlmMaxDepth.
  AgentSession._rlmSessionDir: AgentSession#_rlmSessionDir.
  AgentSession._rlmChildUnsubscribes: AgentSession#_rlmChildUnsubscribes.
  AgentSession._emitGoalUpdate: AgentSession#_emitGoalUpdate().
  AgentSession._parseAutonomousSlashCommand: AgentSession#_parseAutonomousSlashCommand().
  AgentSession._createGoalFromHost: AgentSession#_createGoalFromHost().
  AgentSession._rejectQueuedAgentMessageDeliveries: AgentSession#_rejectQueuedAgentMessageDeliveries().
  AgentSession._createPreparedTurnAction: AgentSession#_createPreparedTurnAction().
  AgentSession._isDeferredSessionInputError: AgentSession#_isDeferredSessionInputError().
  AgentSession._throwIfExtensionCommand: AgentSession#_throwIfExtensionCommand().
  AgentSession._emitModelSelect: AgentSession#_emitModelSelect().
  AgentSession._reapDeletedRlmSubagentRuntimesAfterCompaction: AgentSession#_reapDeletedRlmSubagentRuntimesAfterCompaction().
  AgentSession._currentActiveSessionId: AgentSession#_currentActiveSessionId().
  AgentSession.navigateTree.Promise.typeLiteral134.cancelled: AgentSession#navigateTree().Promise:typeLiteral134:cancelled.
  AgentSession._contextWindowResolver: AgentSession#_contextWindowResolver().
  ExtensionBindings.commandContextActions: ExtensionBindings#commandContextActions.
  ExtensionBindings.onError: ExtensionBindings#onError.
  CommitPreparationPolicy.initialRefineBarrier: CommitPreparationPolicy#initialRefineBarrier.
  CommitPreparationPolicy.preTurnCompaction: CommitPreparationPolicy#preTurnCompaction.
  CommitPreparationPolicy.finalRefineBarrier: CommitPreparationPolicy#finalRefineBarrier.
  PreparedTurnPayload.images: PreparedTurnPayload#images.
  AgentSession._createPreparedTurnAction.options-typeLiteral696.message: AgentSession#_createPreparedTurnAction().(options)typeLiteral696:message.
  AgentSession._shouldWaitForModelSelectEmit: AgentSession#_shouldWaitForModelSelectEmit().
  PromptOptions.streamingBehavior: PromptOptions#streamingBehavior.
  AgentSession._queuedWorkPauses: AgentSession#_queuedWorkPauses.
  AgentSession._goalAccountingStartedAt: AgentSession#_goalAccountingStartedAt.
  AgentSession._deletedRlmChildIds: AgentSession#_deletedRlmChildIds.
  AgentSession._postCompactionContinuationScheduled: AgentSession#_postCompactionContinuationScheduled.
  AgentSession._admitSessionInput.typeLiteral1523.disposition: AgentSession#_admitSessionInput().typeLiteral1523:disposition.
  AgentSession._endCompactionUnsuccessfully: AgentSession#_endCompactionUnsuccessfully().
  AgentSessionEventListener: AgentSessionEventListener#
  PreparedTurnPayload.customMessage: PreparedTurnPayload#customMessage.
  AgentSession._toolRegistry: AgentSession#_toolRegistry.
  AgentSession._stopGoalContinuationForTerminalMessage: AgentSession#_stopGoalContinuationForTerminalMessage().
  AgentSession.-get-steeringMode: AgentSession#`<get>steeringMode`().
  AgentSession.-get-followUpMode: AgentSession#`<get>followUpMode`().
  AgentSession._createSessionCommandAction: AgentSession#_createSessionCommandAction().
  AgentSession.restorePendingNextTurnMessages: AgentSession#restorePendingNextTurnMessages().
  AgentSession._getEffectiveServiceTier: AgentSession#_getEffectiveServiceTier().
  AgentSession._ensureRlmSessionDir: AgentSession#_ensureRlmSessionDir().
  AgentSession._contextTokensForCurrentMessages: AgentSession#_contextTokensForCurrentMessages().
  AgentSession._isStructuredPermanentProviderRetryExhausted: AgentSession#_isStructuredPermanentProviderRetryExhausted().
  AgentSessionConfig.subagentRuntimeHost: AgentSessionConfig#subagentRuntimeHost.
  AutoRefineReviewer: AutoRefineReviewer#
  PromptOptions.signal: PromptOptions#signal.
  TurnExecutionPolicy.nextTurnContextTiming: TurnExecutionPolicy#nextTurnContextTiming.
  PreparedTurnPayload.acceptedAgentMessage: PreparedTurnPayload#acceptedAgentMessage.
  SessionActionRecoveryAction.id: SessionActionRecoveryAction#id.
  RlmChildRun.error: RlmChildRun#error.
  AgentSession._sessionInputPumpRequested: AgentSession#_sessionInputPumpRequested.
  AgentSession._pendingRequestedCompaction: AgentSession#_pendingRequestedCompaction.
  AgentSession._branchSummaryOperation: AgentSession#_branchSummaryOperation.
  AgentSession._retryPromise: AgentSession#_retryPromise.
  AgentSession._queuedAutonomousContinuationSnapshots: AgentSession#_queuedAutonomousContinuationSnapshots.
  AgentSession._autoRefineReviewAbort: AgentSession#_autoRefineReviewAbort.
  AgentSession.setScopedModels: AgentSession#setScopedModels().
  AgentSession._takePendingNextTurnMessages: AgentSession#_takePendingNextTurnMessages().
  AgentSession._acquireDirectTurnAdmissionFence.Promise.typeLiteral1522.release: AgentSession#_acquireDirectTurnAdmissionFence().Promise:typeLiteral1522:release().
  AgentSession.abortCompaction: AgentSession#abortCompaction().
  AgentSession.setCurrentRecap: AgentSession#setCurrentRecap().
  RlmChildAgentSnapshot.status: RlmChildAgentSnapshot#status.
  ExtensionBindings.shutdownHandler: ExtensionBindings#shutdownHandler.
  PreparedTurnPayload.prepared: PreparedTurnPayload#prepared.
  PreparedTurnPayload.executionPolicy: PreparedTurnPayload#executionPolicy.
  isPersistedRlmMaxDepthState: isPersistedRlmMaxDepthState().
  AgentSession._agentMessageOutcomes: AgentSession#_agentMessageOutcomes.
  AgentSession._rlmHeartbeatController: AgentSession#_rlmHeartbeatController.
  AgentSession._ipythonKernelProvisioner: AgentSession#_ipythonKernelProvisioner.
  AgentSession.setSubagentRuntimeHost: AgentSession#setSubagentRuntimeHost().
  AgentSession._installAgentContinuationHook: AgentSession#_installAgentContinuationHook().
  AgentSession._clearGoal: AgentSession#_clearGoal().
  AgentSession._rejectAgentMessage: AgentSession#_rejectAgentMessage().
  AgentSession.refreshAutonomousGates: AgentSession#refreshAutonomousGates().
  AgentSession._pendingModelSelectEmit: AgentSession#_pendingModelSelectEmit().
  AgentSession._clampThinkingLevel: AgentSession#_clampThinkingLevel().
  AgentSession._consumePendingRequestedRefine: AgentSession#_consumePendingRequestedRefine().
  AgentSession._waitForRefineIdle: AgentSession#_waitForRefineIdle().
  AgentSession._isFauxProviderQueueExhausted: AgentSession#_isFauxProviderQueueExhausted().
  AgentSession._isAgentLifecycleFailure: AgentSession#_isAgentLifecycleFailure().
  AgentSession.waitForRetry: AgentSession#waitForRetry().
  AgentSession._drainQueuedMessagesAfterBash: AgentSession#_drainQueuedMessagesAfterBash().
  AgentSession.-get-hasPendingBashMessages: AgentSession#`<get>hasPendingBashMessages`().
  AgentSession._rlmSessionDirForReading: AgentSession#_rlmSessionDirForReading().
  PromptOptions.content: PromptOptions#content.
  NormalizedSubmission: NormalizedSubmission#
  CommitPreparationPolicy.flushPendingBashBeforeValidation: CommitPreparationPolicy#flushPendingBashBeforeValidation.
  TurnExecutionPolicy.runBeforeAgentStart: TurnExecutionPolicy#runBeforeAgentStart.
  PreparedTurnPayload.queueVisible: PreparedTurnPayload#queueVisible.
  RestoredPromptInput.content: RestoredPromptInput#content.
  SessionActionRecoveryRecord.role: SessionActionRecoveryRecord#role.
  normalizeMessageContent.typeLiteral184.text: normalizeMessageContent().typeLiteral184:text.
  compactRlmText: compactRlmText().
  AgentSession._sessionInputPump: AgentSession#_sessionInputPump.
  AgentSession._goalAbortInProgress: AgentSession#_goalAbortInProgress.
  AgentSession._autoRefineInProgress: AgentSession#_autoRefineInProgress.
  AgentSession._scheduledAutoRefineTimers: AgentSession#_scheduledAutoRefineTimers.
  AgentSession._turnIntervalAutoRefinePending: AgentSession#_turnIntervalAutoRefinePending.
  AgentSession._serializedRefine: AgentSession#_serializedRefine.
  AgentSession._resolveRlmMaxDepth.typeLiteral325.maxDepth: AgentSession#_resolveRlmMaxDepth().typeLiteral325:maxDepth.
  AgentSession.registerDisposeCallback: AgentSession#registerDisposeCallback().
  AgentSession._markAutonomousContinuationSuppressed: AgentSession#_markAutonomousContinuationSuppressed().
  AgentSession.-get-scopedModels.ReadonlyArray.typeLiteral18.thinkingLevel: AgentSession#`<get>scopedModels`().ReadonlyArray:typeLiteral18:thinkingLevel.
  AgentSession._admitSessionInput.typeLiteral1523.accepted: AgentSession#_admitSessionInput().typeLiteral1523:accepted.
  AgentSession._getServiceTierForModelSwitch: AgentSession#_getServiceTierForModelSwitch().
  AgentSession.supportsThinking: AgentSession#supportsThinking().
  AgentSession._shouldSkipAutoRefineForActiveAgent: AgentSession#_shouldSkipAutoRefineForActiveAgent().
  AgentSession._cancelActiveRlmChildRuns: AgentSession#_cancelActiveRlmChildRuns().
  AgentSessionConfig.customTools: AgentSessionConfig#customTools.
  ExtensionBindings.uiContext: ExtensionBindings#uiContext.
  PromptOptions.source: PromptOptions#source.
  SubmissionNormalizationPolicy.extensionCommands: SubmissionNormalizationPolicy#extensionCommands.
  PreparedTurnPayload: PreparedTurnPayload#
  SessionActionRecoverySnapshot.formatVersion: SessionActionRecoverySnapshot#formatVersion.
  ModelCycleResult.model: ModelCycleResult#model.
  ToolDefinitionEntry.definition: ToolDefinitionEntry#definition.
  RlmChildRun.publication: RlmChildRun#publication.
  AgentSession._eventListeners: AgentSession#_eventListeners.
  AgentSession._pendingBashMessages: AgentSession#_pendingBashMessages.
  AgentSession._agentObserveController: AgentSession#_agentObserveController.
  AgentSession._baseToolsOverride: AgentSession#_baseToolsOverride.
  AgentSession.restoreSteeringMessage: AgentSession#restoreSteeringMessage().
  AgentSession._emitRefineFailed: AgentSession#_emitRefineFailed().
  AgentSession.buildExtensionResourcePaths.Array.typeLiteral3179.metadata.typeLiteral3180.baseDir: AgentSession#buildExtensionResourcePaths().Array:typeLiteral3179:metadata.typeLiteral3180:baseDir.
  PromptOptions.queueIfBusy: PromptOptions#queueIfBusy.
  InternalPromptOptions.returnAfterAccepted: InternalPromptOptions#returnAfterAccepted.
  CommitPreparationPolicy.validateModelAndAuth: CommitPreparationPolicy#validateModelAndAuth.
  CommitPreparationPolicy.awaitPendingModelSelection: CommitPreparationPolicy#awaitPendingModelSelection.
  TurnExecutionPolicy: TurnExecutionPolicy#
  TurnExecutionPolicy.preserveEmptyExtensionPrompt: TurnExecutionPolicy#preserveEmptyExtensionPrompt.
  TurnExecutionPolicy.completionIncludesRetryChain: TurnExecutionPolicy#completionIncludesRetryChain.
  PreparedCommandPayload: PreparedCommandPayload#
  PreparedCommandPayload.images: PreparedCommandPayload#images.
  PreparedPromptPreparation.result: PreparedPromptPreparation#result.
  normalizeMessageContent.typeLiteral184.images: normalizeMessageContent().typeLiteral184:images.
  RlmChildRun.abort: RlmChildRun#abort.
  RlmSubagentModelSelection: RlmSubagentModelSelection#
  AgentSession._continueAfterThresholdCompaction: AgentSession#_continueAfterThresholdCompaction.
  AgentSession._includeGoals: AgentSession#_includeGoals.
  AgentSession._disposeCallbacksPromise: AgentSession#_disposeCallbacksPromise.
  AgentSession._repliedToParentSinceTask: AgentSession#_repliedToParentSinceTask.
  AgentSession._queuedAutonomousThresholdContinuations: AgentSession#_queuedAutonomousThresholdContinuations.
  AgentSession._resolveRlmMaxDepth.typeLiteral325.source: AgentSession#_resolveRlmMaxDepth().typeLiteral325:source.
  AgentSession._clearQueuedAutonomousContinuationsAfterSkippedThresholdCompaction: AgentSession#_clearQueuedAutonomousContinuationsAfterSkippedThresholdCompaction().
  AgentSession._agentMessageOutcome: AgentSession#_agentMessageOutcome().
  AgentSession.recordHostAutonomousContinuation: AgentSession#recordHostAutonomousContinuation().
  AgentSession._runPreTurnCompaction: AgentSession#_runPreTurnCompaction().
  AgentSession._deliveryPolicy: AgentSession#_deliveryPolicy().
  AgentSession._createPreparedTurnAction.options-typeLiteral696.content: AgentSession#_createPreparedTurnAction().(options)typeLiteral696:content.
  AgentSession._sessionOwnsScheduledContinuations: AgentSession#_sessionOwnsScheduledContinuations().
  AgentSession.setAutoCompactionEnabled: AgentSession#setAutoCompactionEnabled().
  AgentSession.setAutoRetryEnabled: AgentSession#setAutoRetryEnabled().
  AgentSessionConfig.agentMessageController: AgentSessionConfig#agentMessageController.
  AgentSessionConfig.baseToolsOverride: AgentSessionConfig#baseToolsOverride.
  SerializedBackgroundPlanResult: SerializedBackgroundPlanResult#
  PromptOptions.customMessage: PromptOptions#customMessage.
  SessionActionRecoveryAction.delivery: SessionActionRecoveryAction#delivery.
  AgentMessageOutcome.delivery: AgentMessageOutcome#delivery.
  AgentSession._serviceTierPreference: AgentSession#_serviceTierPreference.
  AgentSession._lateIpythonSentAgentMessages: AgentSession#_lateIpythonSentAgentMessages.
  AgentSession._mcpManager: AgentSession#_mcpManager.
  AgentSession._extensionErrorListener: AgentSession#_extensionErrorListener.
  AgentSession._rlmMaxDepthSource: AgentSession#_rlmMaxDepthSource.
  AgentSession._scheduledPostCompactionContinuationMessages: AgentSession#_scheduledPostCompactionContinuationMessages.
  AgentSession._pendingThresholdCompactionAutonomousMessages: AgentSession#_pendingThresholdCompactionAutonomousMessages.
  AgentSession._lastAssistantMessage: AgentSession#_lastAssistantMessage.
  AgentSession._createPreparedTurnAction.options-typeLiteral696.executionPolicy: AgentSession#_createPreparedTurnAction().(options)typeLiteral696:executionPolicy.
  AgentSession.-get-isQueuedWorkSuspended: AgentSession#`<get>isQueuedWorkSuspended`().
  AgentSession.abortBranchSummary: AgentSession#abortBranchSummary().
  AgentSession._markProviderAuthStaleForRetryFailure: AgentSession#_markProviderAuthStaleForRetryFailure().
  AgentSessionConfig.rlmDepth: AgentSessionConfig#rlmDepth.
  AgentSessionConfig.initialGoal: AgentSessionConfig#initialGoal.
  PromptOptions.preflightResult: PromptOptions#preflightResult.
  SessionInputSchedule: SessionInputSchedule#
  DeferredSessionInputError: DeferredSessionInputError#
  SESSION_ACTION_RECOVERY_FORMAT_VERSION: SESSION_ACTION_RECOVERY_FORMAT_VERSION.
  isNonNegativeInteger: isNonNegativeInteger().
  rlmChildLabel: rlmChildLabel().
  AgentSession._scopedModels: AgentSession#_scopedModels.
  AgentSession._unsubscribeAgent: AgentSession#_unsubscribeAgent.
  AgentSession._sessionInputArrivalEpoch: AgentSession#_sessionInputArrivalEpoch.
  AgentSession._sessionActionCommitOwner: AgentSession#_sessionActionCommitOwner.
  AgentSession._sessionActionCommitContext: AgentSession#_sessionActionCommitContext.
  AgentSession._autoCompactionAbortController: AgentSession#_autoCompactionAbortController.
  AgentSession._compactionOperation: AgentSession#_compactionOperation.
  AgentSession._overflowRecovery: AgentSession#_overflowRecovery.
  AgentSession._branchSummaryAbortController: AgentSession#_branchSummaryAbortController.
  AgentSession._retryAbortController: AgentSession#_retryAbortController.
  AgentSession._bashAbortController: AgentSession#_bashAbortController.
  AgentSession._serializedExplicitRefineOptions: AgentSession#_serializedExplicitRefineOptions.
  AgentSession._startDisposeCallbacks: AgentSession#_startDisposeCallbacks().
  AgentSession.restoreSteeringMessage.options-typeLiteral1729.content: AgentSession#restoreSteeringMessage().(options)typeLiteral1729:content.
  AgentSession.restoreFollowUpMessage.options-typeLiteral1730.content: AgentSession#restoreFollowUpMessage().(options)typeLiteral1730:content.
  AgentSession._turnExecutionPolicy: AgentSession#_turnExecutionPolicy().
  AgentSession.-get-autoCompactionEnabled: AgentSession#`<get>autoCompactionEnabled`().
  AgentSession._createChildRlmSessionDir: AgentSession#_createChildRlmSessionDir().
  AgentSession._getProviderStreamFailureKind: AgentSession#_getProviderStreamFailureKind().
  AgentSession._isStructuredPermanentProviderFailure: AgentSession#_isStructuredPermanentProviderFailure().
  AgentSession._getProviderStreamFailureAuthStatus: AgentSession#_getProviderStreamFailureAuthStatus().
  AgentSession.navigateTree.Promise.typeLiteral134.editorText: AgentSession#navigateTree().Promise:typeLiteral134:editorText.
  AgentSession._navigateTreeUnderPause: AgentSession#_navigateTreeUnderPause().
  AgentSession.getUserMessagesForForking.Array.typeLiteral4333.entryId: AgentSession#getUserMessagesForForking().Array:typeLiteral4333:entryId.
  AgentSessionConfig.agentObserveController: AgentSessionConfig#agentObserveController.
  AgentSessionConfig.sessionStartEvent: AgentSessionConfig#sessionStartEvent.
  AgentSessionConfig.autonomous: AgentSessionConfig#autonomous.
  AutoRefineReviewRequest.reason: AutoRefineReviewRequest#reason.
  SubmissionNormalizationPolicy.inputSource: SubmissionNormalizationPolicy#inputSource.
  RestoredPromptInput.images: RestoredPromptInput#images.
  RestoredPromptInput.customMessage: RestoredPromptInput#customMessage.
  RestoredPromptInput.prefixMessages: RestoredPromptInput#prefixMessages.
  SessionActionRecoveryRecord.message: SessionActionRecoveryRecord#message.
  AutonomousRuntimeSnapshot: AutonomousRuntimeSnapshot#
  AgentSession._customTools: AgentSession#_customTools.
  AgentSession._baseToolDefinitions: AgentSession#_baseToolDefinitions.
  AgentSession._sessionStartEvent: AgentSession#_sessionStartEvent.
  AgentSession._extensionUIContext: AgentSession#_extensionUIContext.
  AgentSession._extensionCommandContextActions: AgentSession#_extensionCommandContextActions.
  AgentSession._extensionShutdownHandler: AgentSession#_extensionShutdownHandler.
  AgentSession._toolDefinitions: AgentSession#_toolDefinitions.
  AgentSession._baseSystemPromptOptions: AgentSession#_baseSystemPromptOptions.
  AgentSession._autoRefineReviewer: AgentSession#_autoRefineReviewer.
  AgentSession._disconnectFromAgent: AgentSession#_disconnectFromAgent().
  AgentSession._createPreparedTurnAction.options-typeLiteral696.prefixMessages: AgentSession#_createPreparedTurnAction().(options)typeLiteral696:prefixMessages.
  AgentSession._createPreparedTurnAction.options-typeLiteral696.source: AgentSession#_createPreparedTurnAction().(options)typeLiteral696:source.
  AgentSession._performCompaction.options-typeLiteral2765.model: AgentSession#_performCompaction().(options)typeLiteral2765:model.
  RlmChildAgentStatus: RlmChildAgentStatus#
  CompactionSkippedError: CompactionSkippedError#
  AgentSessionConfig.rlmMaxDepth: AgentSessionConfig#rlmMaxDepth.
  AgentSessionConfig.rlmSessionDir: AgentSessionConfig#rlmSessionDir.
  InternalPromptOptions.agentMessageId: InternalPromptOptions#agentMessageId.
  isObjectRecord: isObjectRecord().
  AgentMessageDeferred: AgentMessageDeferred#
  AgentMessageDeferred.promise: AgentMessageDeferred#promise.
  AgentMessageOutcome.completion: AgentMessageOutcome#completion.
  ModelCycleResult: ModelCycleResult#
  ModelSelectOptions: ModelSelectOptions#
  noopRlmChildAbort: noopRlmChildAbort().
  AgentSession._compactionAbortController: AgentSession#_compactionAbortController.
  AgentSession._retryResolve: AgentSession#_retryResolve.
  AgentSession._includeCompactSkill: AgentSession#_includeCompactSkill.
  AgentSession._configuredRlmMaxDepth: AgentSession#_configuredRlmMaxDepth.
  AgentSession._postCompactionContinuationTimer: AgentSession#_postCompactionContinuationTimer.
  AgentSession._serializedPlanClaim: AgentSession#_serializedPlanClaim.
  AgentSession._createPreparedTurnAction.options-typeLiteral696.resumeIfIdle: AgentSession#_createPreparedTurnAction().(options)typeLiteral696:resumeIfIdle.
  AgentSession._queuePreparedPrompt.options-typeLiteral1804.content: AgentSession#_queuePreparedPrompt().(options)typeLiteral1804:content.
  AgentSession.clearQueue.typeLiteral2126.followUp: AgentSession#clearQueue().typeLiteral2126:followUp.
  AgentSession._acquireSessionActionCommitFence.Promise.typeLiteral1917.release: AgentSession#_acquireSessionActionCommitFence().Promise:typeLiteral1917:release().
  AgentSession.-get-autoRetryEnabled: AgentSession#`<get>autoRetryEnabled`().
  AgentSession.hasExtensionHandlers: AgentSession#hasExtensionHandlers().
  RlmChildAgentSnapshot.activity: RlmChildAgentSnapshot#activity.
  AgentSessionConfig.serviceTierPreference: AgentSessionConfig#serviceTierPreference.
  AgentSessionConfig.rlmHeartbeatController: AgentSessionConfig#rlmHeartbeatController.
  AgentSessionConfig.mcpManager: AgentSessionConfig#mcpManager.
  AgentSessionConfig.autoRefineReviewer: AgentSessionConfig#autoRefineReviewer.
  PromptOptions.images: PromptOptions#images.
  InternalPromptOptions: InternalPromptOptions#
  SessionActionRecoveryAction.wake: SessionActionRecoveryAction#wake.
  AgentMessageOutcome: AgentMessageOutcome#
  ModelCycleResult.serviceTier: ModelCycleResult#serviceTier.
  ToolDefinitionEntry: ToolDefinitionEntry#
  parseDepth: parseDepth().
  AgentSession._goalAccountedAssistantMessages: AgentSession#_goalAccountedAssistantMessages.
  AgentSession._autonomousContinuationSuppressedMessages: AgentSession#_autonomousContinuationSuppressedMessages.
  AgentSession._unpersistedCompactionOutcomes: AgentSession#_unpersistedCompactionOutcomes.
  AgentSession.-get-scopedModels.ReadonlyArray.typeLiteral18.model: AgentSession#`<get>scopedModels`().ReadonlyArray:typeLiteral18:model.
  AgentSession.setScopedModels.scopedModels-Array.typeLiteral1372.model: AgentSession#setScopedModels().(scopedModels)Array:typeLiteral1372:model.
  AgentSession._refreshExtensionSystemPrompt: AgentSession#_refreshExtensionSystemPrompt().
  AgentSession.restoreSteeringMessage.options-typeLiteral1729.customMessage: AgentSession#restoreSteeringMessage().(options)typeLiteral1729:customMessage.
  AgentSession.restoreFollowUpMessage.options-typeLiteral1730.customMessage: AgentSession#restoreFollowUpMessage().(options)typeLiteral1730:customMessage.
  AgentSession.getCurrentRecap: AgentSession#getCurrentRecap().
  AgentSessionConfig.agentDir: AgentSessionConfig#agentDir.
  AgentSessionConfig.allowedToolNames: AgentSessionConfig#allowedToolNames.
  PromptOptions.expandPromptTemplates: PromptOptions#expandPromptTemplates.
  PromptOptions.resumeIfIdle: PromptOptions#resumeIfIdle.
  SubmissionNormalizationPolicy.parseSessionCommands: SubmissionNormalizationPolicy#parseSessionCommands.
  SubmissionNormalizationPolicy.expandSkills: SubmissionNormalizationPolicy#expandSkills.
  SubmissionNormalizationPolicy.expandPromptTemplates: SubmissionNormalizationPolicy#expandPromptTemplates.
  AgentMessageDeferred.reject: AgentMessageDeferred#reject.
  RlmChildRun: RlmChildRun#
  RlmChildRun.sessionName: RlmChildRun#sessionName.
  RlmSubagentModelSelection.model: RlmSubagentModelSelection#model.
  AgentSession._pendingSessionActionFenceWaiters: AgentSession#_pendingSessionActionFenceWaiters.
  AgentSession._sessionActionCommitDisposeAbortController: AgentSession#_sessionActionCommitDisposeAbortController.
  AgentSession._userBashRunning: AgentSession#_userBashRunning.
  AgentSession._turnIndex: AgentSession#_turnIndex.
  AgentSession._modelSelectEmitQueue: AgentSession#_modelSelectEmitQueue.
  AgentSession._agentDir: AgentSession#_agentDir.
  AgentSession._allowedToolNames: AgentSession#_allowedToolNames.
  AgentSession._disposeAsyncPromise: AgentSession#_disposeAsyncPromise.
  AgentSession._ipythonKernelSnapshotDir: AgentSession#_ipythonKernelSnapshotDir.
  AgentSession._pendingRlmSubagentSessionNames: AgentSession#_pendingRlmSubagentSessionNames.
  AgentSession._getRequiredRequestAuth.Promise.typeLiteral334.apiKey: AgentSession#_getRequiredRequestAuth().Promise:typeLiteral334:apiKey.
  AgentSession._getRequiredRequestAuth.Promise.typeLiteral334.headers: AgentSession#_getRequiredRequestAuth().Promise:typeLiteral334:headers.
  AgentSession._createPreparedTurnAction.options-typeLiteral696.queueVisible: AgentSession#_createPreparedTurnAction().(options)typeLiteral696:queueVisible.
  AgentSession._asError: AgentSession#_asError().
  AgentSession._buildRuntime.options-typeLiteral333.activeToolNames: AgentSession#_buildRuntime().(options)typeLiteral333:activeToolNames.
  AgentSession._buildRuntime.options-typeLiteral333.includeAllExtensionTools: AgentSession#_buildRuntime().(options)typeLiteral333:includeAllExtensionTools.
  SessionActionRecoveryAction.source: SessionActionRecoveryAction#source.
  PersistedIpythonSentAgentMessage: PersistedIpythonSentAgentMessage#
  THINKING_LEVELS: THINKING_LEVELS.
  parseGoalBudgetValue: parseGoalBudgetValue().
  AgentSession._scopedModels.Array.typeLiteral301.thinkingLevel: AgentSession#_scopedModels.Array:typeLiteral301:thinkingLevel.
  AgentSession._extensionRunnerRef.typeLiteral309.current: AgentSession#_extensionRunnerRef.typeLiteral309:current.
  AgentSession._shouldStopBeforeTurn: AgentSession#_shouldStopBeforeTurn().
  AgentSession._replaceMessageInPlace: AgentSession#_replaceMessageInPlace().
  AgentSession.-get-retryAttempt: AgentSession#`<get>retryAttempt`().
  AgentSession._runWithAutonomousContinuationSuppressed: AgentSession#_runWithAutonomousContinuationSuppressed().
  AgentSession._createEphemeralRlmSessionDir: AgentSession#_createEphemeralRlmSessionDir().
  AgentSession.executeBash.options-typeLiteral4128.operations: AgentSession#executeBash().(options)typeLiteral4128:operations.
  isRlmHeartbeatStatusUpdate: isRlmHeartbeatStatusUpdate().
  RlmChildAgentSnapshot.id: RlmChildAgentSnapshot#id.
  RlmChildAgentSnapshot.label: RlmChildAgentSnapshot#label.
  AgentSessionConfig: AgentSessionConfig#
  AgentSessionConfig.scopedModels: AgentSessionConfig#scopedModels.
  AgentSessionConfig.initialActiveToolNames: AgentSessionConfig#initialActiveToolNames.
  AgentSessionConfig.includeGoals: AgentSessionConfig#includeGoals.
  AgentSessionConfig.includeCompactSkill: AgentSessionConfig#includeCompactSkill.
  AgentSessionConfig.extensionRunnerRef: AgentSessionConfig#extensionRunnerRef.
  AgentSessionConfig.rlmParentNodeId: AgentSessionConfig#rlmParentNodeId.
  AgentSessionConfig.rlmParentAgent: AgentSessionConfig#rlmParentAgent.
  AgentSessionConfig.serializedRefine: AgentSessionConfig#serializedRefine.
  ExtensionBindings: ExtensionBindings#
  AutoRefineReviewRequest.turnsSinceLastReview: AutoRefineReviewRequest#turnsSinceLastReview.
  PromptOptions.followUpQueueKey: PromptOptions#followUpQueueKey.
  PromptOptions.admissionCommitted: PromptOptions#admissionCommitted.
  PromptOptions.agentMessageId: PromptOptions#agentMessageId.
  InternalPromptOptions.skipPrePromptWork: InternalPromptOptions#skipPrePromptWork.
  CommitPreparationSteps.shouldCommit: CommitPreparationSteps#shouldCommit.
  PreparedTurnPayload.acceptedBeforeCompletion: PreparedTurnPayload#acceptedBeforeCompletion.
  RestoredPromptInput.text: RestoredPromptInput#text.
  RestoredPromptInput.queueKey: RestoredPromptInput#queueKey.
  RestoredPromptInput.agentMessageId: RestoredPromptInput#agentMessageId.
  AgentMessageDeferred.resolve: AgentMessageDeferred#resolve.
  PersistedRlmMaxDepthState: PersistedRlmMaxDepthState#
  RlmChildRun.sessionDir: RlmChildRun#sessionDir.
  RlmChildRun.settled: RlmChildRun#settled.
  waitForPromiseOrAbort: waitForPromiseOrAbort().
  AgentSession._autonomousContinuationSuppressionDepth: AgentSession#_autonomousContinuationSuppressionDepth.
  AgentSession._userBashAbortRequested: AgentSession#_userBashAbortRequested.
  AgentSession._execEnvProvider: AgentSession#_execEnvProvider.
  AgentSession._modelSelectEmitQueueIdle: AgentSession#_modelSelectEmitQueueIdle.
  AgentSession._modelSelectEmitContext: AgentSession#_modelSelectEmitContext.
  AgentSession._extensionRunnerRef: AgentSession#_extensionRunnerRef.
  AgentSession._disposeCallbacks: AgentSession#_disposeCallbacks.
  AgentSession._rlmParentNodeId: AgentSession#_rlmParentNodeId.
  AgentSession._parentReplyCount: AgentSession#_parentReplyCount.
  AgentSession._currentRecap: AgentSession#_currentRecap.
  AgentSession._autoRefineOperations: AgentSession#_autoRefineOperations.
  AgentSession._runSerializedRefine: AgentSession#_runSerializedRefine().
  AgentSession._createPreparedTurnAction.options-typeLiteral696.queueKey: AgentSession#_createPreparedTurnAction().(options)typeLiteral696:queueKey.
  AgentSession._createPreparedTurnAction.options-typeLiteral696.previewLabel: AgentSession#_createPreparedTurnAction().(options)typeLiteral696:previewLabel.
  AgentSession._createPreparedTurnAction.options-typeLiteral696.suppressAutonomousContinuation: AgentSession#_createPreparedTurnAction().(options)typeLiteral696:suppressAutonomousContinuation.
  AgentSession._performCompaction.options-typeLiteral2765.apiKey: AgentSession#_performCompaction().(options)typeLiteral2765:apiKey.
  AgentSession._performCompaction.options-typeLiteral2765.headers: AgentSession#_performCompaction().(options)typeLiteral2765:headers.
  AgentSession._performCompaction.options-typeLiteral2765.customInstructions: AgentSession#_performCompaction().(options)typeLiteral2765:customInstructions.
  AgentSession._planRefine.options-typeLiteral2976.rollbackId: AgentSession#_planRefine().(options)typeLiteral2976:rollbackId.
  AgentSession.buildExtensionResourcePaths: AgentSession#buildExtensionResourcePaths().
  AgentSession.buildExtensionResourcePaths.entries-Array.typeLiteral3178.extensionPath: AgentSession#buildExtensionResourcePaths().(entries)Array:typeLiteral3178:extensionPath.
  AgentSession._refreshToolRegistry.options-typeLiteral3268.activeToolNames: AgentSession#_refreshToolRegistry().(options)typeLiteral3268:activeToolNames.
  AgentSession._buildRuntime.options-typeLiteral333.flagValues: AgentSession#_buildRuntime().(options)typeLiteral333:flagValues.
  AgentSession._createRlmSubagentRuntimeOptions.options-typeLiteral3607.id: AgentSession#_createRlmSubagentRuntimeOptions().(options)typeLiteral3607:id.
  AgentSession._navigateTreeUnderPause.options-typeLiteral4236.summarize: AgentSession#_navigateTreeUnderPause().(options)typeLiteral4236:summarize.
  AgentSessionConfig.scopedModels.Array.typeLiteral81.model: AgentSessionConfig#scopedModels.Array:typeLiteral81:model.
  AgentSessionConfig.scopedModels.Array.typeLiteral81.thinkingLevel: AgentSessionConfig#scopedModels.Array:typeLiteral81:thinkingLevel.
  AgentSessionConfig.extensionRunnerRef.typeLiteral82.current: AgentSessionConfig#extensionRunnerRef.typeLiteral82:current.
  ModelCycleResult.thinkingLevel: ModelCycleResult#thinkingLevel.
  AgentSession._queuePreparedPrompt.options-typeLiteral1804.message: AgentSession#_queuePreparedPrompt().(options)typeLiteral1804:message.
  AgentSession._queuePreparedPrompt.options-typeLiteral1804.prefixMessages: AgentSession#_queuePreparedPrompt().(options)typeLiteral1804:prefixMessages.
  RlmChildAgentActivity: RlmChildAgentActivity#
  RlmChildAgentSnapshot.parentId: RlmChildAgentSnapshot#parentId.
  RlmChildAgentSnapshot.sessionName: RlmChildAgentSnapshot#sessionName.
  RlmChildAgentSnapshot.recap: RlmChildAgentSnapshot#recap.
  RlmChildAgentSnapshot.sessionDir: RlmChildAgentSnapshot#sessionDir.
  RlmChildAgentSnapshot.error: RlmChildAgentSnapshot#error.
  CompactionReason: CompactionReason#
  UserBashEndDetails: UserBashEndDetails#
  AgentSessionConfig.prewarmIpythonKernel: AgentSessionConfig#prewarmIpythonKernel.
  AutoRefineReviewRequest: AutoRefineReviewRequest#
  PromptOptions.suppressAutonomousContinuation: PromptOptions#suppressAutonomousContinuation.
  PromptOptions.skipInputHandlers: PromptOptions#skipInputHandlers.
  SubmissionNormalizationPolicy: SubmissionNormalizationPolicy#
  RefineBarrierPolicy: RefineBarrierPolicy#
  CommitPreparationPolicy: CommitPreparationPolicy#
  CommitPreparationSteps.afterValidation: CommitPreparationSteps#afterValidation.
  CommitPreparationSteps.prepare: CommitPreparationSteps#prepare.
  CommitPreparationSteps.commit: CommitPreparationSteps#commit.
  PreparedTurnPayload.cancelledDispatchEnded: PreparedTurnPayload#cancelledDispatchEnded.
  PreparedPromptPreparation: PreparedPromptPreparation#
  oncePreflight: oncePreflight().
  SessionActionRecoveryRecord.ownerActionId: SessionActionRecoveryRecord#ownerActionId.
  SessionActionRecoveryAction.queueKey: SessionActionRecoveryAction#queueKey.
  SessionActionRecoveryAction.agentMessageId: SessionActionRecoveryAction#agentMessageId.
  IPYTHON_SENT_AGENT_MESSAGE_CUSTOM_ENTRY: IPYTHON_SENT_AGENT_MESSAGE_CUSTOM_ENTRY.
  ToolDefinitionEntry.sourceInfo: ToolDefinitionEntry#sourceInfo.
  PersistedRlmMaxDepthState.maxDepth: PersistedRlmMaxDepthState#maxDepth.
  RlmChildRun.prompt: RlmChildRun#prompt.
  RlmChildRun.emitUpdate: RlmChildRun#emitUpdate.
  RLM_MAX_DEPTH_STATE_CUSTOM_TYPE: RLM_MAX_DEPTH_STATE_CUSTOM_TYPE.
  noopRlmChildEventUnsubscribe: noopRlmChildEventUnsubscribe().
  AgentSession._sessionActionCommitTail: AgentSession#_sessionActionCommitTail.
  AgentSession._initialActiveToolNames: AgentSession#_initialActiveToolNames.
  AgentSession._extensionErrorUnsubscriber: AgentSession#_extensionErrorUnsubscriber.
  AgentSession._ipythonRuntimeBuilt: AgentSession#_ipythonRuntimeBuilt.
  AgentSession._prewarmIpythonKernel: AgentSession#_prewarmIpythonKernel.
  AgentSession._rlmParentAgent: AgentSession#_rlmParentAgent.
  AgentSession._toolPromptSnippets: AgentSession#_toolPromptSnippets.
  AgentSession._toolPromptGuidelines: AgentSession#_toolPromptGuidelines.
  AgentSession._clearQueuedAutonomousContinuations.options-typeLiteral895.messages: AgentSession#_clearQueuedAutonomousContinuations().(options)typeLiteral895:messages.
  AgentSession.-get-scopedModels: AgentSession#`<get>scopedModels`().
  AgentSession.restoreSteeringMessage.options-typeLiteral1729.agentMessageId: AgentSession#restoreSteeringMessage().(options)typeLiteral1729:agentMessageId.
  AgentSession.restoreFollowUpMessage.options-typeLiteral1730.agentMessageId: AgentSession#restoreFollowUpMessage().(options)typeLiteral1730:agentMessageId.
  AgentSession._createPreparedTurnAction.options-typeLiteral696.agentMessageId: AgentSession#_createPreparedTurnAction().(options)typeLiteral696:agentMessageId.
  AgentSession._createPreparedTurnAction.options-typeLiteral696.acceptedAgentMessage: AgentSession#_createPreparedTurnAction().(options)typeLiteral696:acceptedAgentMessage.
  AgentSession._admitSessionInput.options-typeLiteral1782.restore: AgentSession#_admitSessionInput().(options)typeLiteral1782:restore.
  AgentSession._admitSessionInput.options-typeLiteral1782.front: AgentSession#_admitSessionInput().(options)typeLiteral1782:front.
  AgentSession.sendCustomMessage.options-typeLiteral2091.deliverAs: AgentSession#sendCustomMessage().(options)typeLiteral2091:deliverAs.
  AgentSession.clearQueuedUserMessagesMatching.typeLiteral2185.steering: AgentSession#clearQueuedUserMessagesMatching().typeLiteral2185:steering.
  AgentSession.clearQueuedUserMessagesMatching.typeLiteral2185.followUp: AgentSession#clearQueuedUserMessagesMatching().typeLiteral2185:followUp.
  AgentSession._observeSessionActionDeferral.typeLiteral1625.deferred: AgentSession#_observeSessionActionDeferral().typeLiteral1625:deferred.
  AgentSession._observeSessionActionDeferral.typeLiteral1625.stop: AgentSession#_observeSessionActionDeferral().typeLiteral1625:stop().
  AgentSession._acquireSessionActionCommitFence.Promise.typeLiteral1917.owner: AgentSession#_acquireSessionActionCommitFence().Promise:typeLiteral1917:owner.
  AgentSession.compact.options-typeLiteral2740.skipAbort: AgentSession#compact().(options)typeLiteral2740:skipAbort.
  AgentSession._performCompaction: AgentSession#_performCompaction().
  AgentSession._applyRefine.options-typeLiteral3026.rollbackId: AgentSession#_applyRefine().(options)typeLiteral3026:rollbackId.
  AgentSession._endCompactionUnsuccessfully.options-typeLiteral3110.aborted: AgentSession#_endCompactionUnsuccessfully().(options)typeLiteral3110:aborted.
  AgentSession._createRlmSubagentRuntimeOptions.options-typeLiteral3607.prompt: AgentSession#_createRlmSubagentRuntimeOptions().(options)typeLiteral3607:prompt.
  AgentSession._createRlmSubagentRuntimeOptions.options-typeLiteral3607.sessionName: AgentSession#_createRlmSubagentRuntimeOptions().(options)typeLiteral3607:sessionName.
  AgentSession._createRlmSubagentRuntimeOptions.options-typeLiteral3607.spawnCode: AgentSession#_createRlmSubagentRuntimeOptions().(options)typeLiteral3607:spawnCode.
  AgentSession._createRlmSubagentRuntimeOptions.options-typeLiteral3607.sessionDir: AgentSession#_createRlmSubagentRuntimeOptions().(options)typeLiteral3607:sessionDir.
  AgentSession.runUserBash.options-typeLiteral4141.transient: AgentSession#runUserBash().(options)typeLiteral4141:transient.
  AgentSession.setRlmMaxDepth.options-typeLiteral4181.global: AgentSession#setRlmMaxDepth().(options)typeLiteral4181:global.
  AgentSession._branchNavigationQueue: AgentSession#_branchNavigationQueue.
  AgentSession._extractUserMessageText: AgentSession#_extractUserMessageText().
  RlmChildAgentSnapshot: RlmChildAgentSnapshot#
  RlmChildAgentSnapshot.activeSessionId: RlmChildAgentSnapshot#activeSessionId.
  RlmChildAgentSnapshot.model: RlmChildAgentSnapshot#model.
  RlmChildAgentSnapshot.durationMs: RlmChildAgentSnapshot#durationMs.
  RlmChildAgentSnapshot.answerPreview: RlmChildAgentSnapshot#answerPreview.
  RlmChildAgentSnapshot.toolUseCount: RlmChildAgentSnapshot#toolUseCount.
  RlmChildAgentSnapshot.tokenCount: RlmChildAgentSnapshot#tokenCount.
  RlmChildAgentSnapshot.repliedSinceTask: RlmChildAgentSnapshot#repliedSinceTask.
  AgentSessionConfig.initialGoal.typeLiteral83.objective: AgentSessionConfig#initialGoal.typeLiteral83:objective.
  AgentSessionConfig.initialGoal.typeLiteral83.tokenBudget: AgentSessionConfig#initialGoal.typeLiteral83:tokenBudget.
  PromptOptions.internalPrompt: PromptOptions#internalPrompt.
  SubmissionExtensionCommandPolicy: SubmissionExtensionCommandPolicy#
  PreTurnCompactionTiming: PreTurnCompactionTiming#
  CommitPreparationSteps: CommitPreparationSteps#
  CommitPreparationSteps.beforeFinalRefineBarrier: CommitPreparationSteps#beforeFinalRefineBarrier.
  PreparedPromptPreparation.basePromptSnapshot: PreparedPromptPreparation#basePromptSnapshot.
  RestoredPromptInput: RestoredPromptInput#
  SessionActionRecoveryRecord: SessionActionRecoveryRecord#
  SessionActionRecoveryRecord.id: SessionActionRecoveryRecord#id.
  SessionActionRecoveryAction: SessionActionRecoveryAction#
  SessionActionRecoveryAction.suppressAutonomousContinuation: SessionActionRecoveryAction#suppressAutonomousContinuation.
  PersistedIpythonSentAgentMessage.toolCallId: PersistedIpythonSentAgentMessage#toolCallId.
  PersistedIpythonSentAgentMessage.message: PersistedIpythonSentAgentMessage#message.
  ModelSelectOptions.waitForExtensions: ModelSelectOptions#waitForExtensions.
  GoalSlashCommand: GoalSlashCommand#
  AutonomousSlashCommand: AutonomousSlashCommand#
  KERNEL_STATE_LISTING_TIMEOUT_MS: KERNEL_STATE_LISTING_TIMEOUT_MS.
  AgentSession._setGoalState.options-typeLiteral477.persist: AgentSession#_setGoalState().(options)typeLiteral477:persist.
  AgentSession._runBackgroundPlan.options-typeLiteral825.instructions: AgentSession#_runBackgroundPlan().(options)typeLiteral825:instructions.
  AgentSession._runSerializedRefine.options-typeLiteral770.instructions: AgentSession#_runSerializedRefine().(options)typeLiteral770:instructions.
  AgentSession._clearQueuedAutonomousContinuations.options-typeLiteral895.restoreAutonomousState: AgentSession#_clearQueuedAutonomousContinuations().(options)typeLiteral895:restoreAutonomousState.
  AgentSession._normalizePromptSnippet: AgentSession#_normalizePromptSnippet().
  AgentSession._normalizePromptGuidelines: AgentSession#_normalizePromptGuidelines().
  AgentSession.steer.options-typeLiteral1685.queueKey: AgentSession#steer().(options)typeLiteral1685:queueKey.
  AgentSession.steer.options-typeLiteral1685.agentMessageId: AgentSession#steer().(options)typeLiteral1685:agentMessageId.
  AgentSession.steer.options-typeLiteral1685.resumeIfIdle: AgentSession#steer().(options)typeLiteral1685:resumeIfIdle.
  AgentSession.followUp.options-typeLiteral1689.queueKey: AgentSession#followUp().(options)typeLiteral1689:queueKey.
  AgentSession.followUp.options-typeLiteral1689.agentMessageId: AgentSession#followUp().(options)typeLiteral1689:agentMessageId.
  AgentSession.restoreSteeringMessage.options-typeLiteral1729.queueKey: AgentSession#restoreSteeringMessage().(options)typeLiteral1729:queueKey.
  AgentSession.restoreFollowUpMessage.options-typeLiteral1730.queueKey: AgentSession#restoreFollowUpMessage().(options)typeLiteral1730:queueKey.
  AgentSession._turnExecutionPolicy.options-typeLiteral1740.returnAfterAccepted: AgentSession#_turnExecutionPolicy().(options)typeLiteral1740:returnAfterAccepted.
  AgentSession._createSessionCommandAction.options-typeLiteral1777.agentMessageId: AgentSession#_createSessionCommandAction().(options)typeLiteral1777:agentMessageId.
  AgentSession._admitSessionInput.options-typeLiteral1782.wake: AgentSession#_admitSessionInput().(options)typeLiteral1782:wake.
  AgentSession._admitSessionInput.options-typeLiteral1782.immediatelyEligible: AgentSession#_admitSessionInput().(options)typeLiteral1782:immediatelyEligible.
  AgentSession.sendCustomMessage.options-typeLiteral2091.triggerTurn: AgentSession#sendCustomMessage().(options)typeLiteral2091:triggerTurn.
  AgentSession.sendUserMessage.options-typeLiteral2113.deliverAs: AgentSession#sendUserMessage().(options)typeLiteral2113:deliverAs.
  AgentSession.clearQueue.typeLiteral2126.steering: AgentSession#clearQueue().typeLiteral2126:steering.
  AgentSession._acquireDirectTurnAdmissionFence.Promise.typeLiteral1522.owner: AgentSession#_acquireDirectTurnAdmissionFence().Promise:typeLiteral1522:owner.
  AgentSession._discardPendingAutoRefine.options-typeLiteral2838.cancelPostCompactionContinue: AgentSession#_discardPendingAutoRefine().(options)typeLiteral2838:cancelPostCompactionContinue.
  AgentSession.refine.internal-typeLiteral2939.skipAbort: AgentSession#refine().(internal)typeLiteral2939:skipAbort.
  AgentSession._planRefine.options-typeLiteral2976.global: AgentSession#_planRefine().(options)typeLiteral2976:global.
  AgentSession._applyRefine.options-typeLiteral3026.global: AgentSession#_applyRefine().(options)typeLiteral3026:global.
  AgentSession._endCompactionUnsuccessfully.options-typeLiteral3110.errorSeverity: AgentSession#_endCompactionUnsuccessfully().(options)typeLiteral3110:errorSeverity.
  AgentSession.buildExtensionResourcePaths.entries-Array.typeLiteral3178.path: AgentSession#buildExtensionResourcePaths().(entries)Array:typeLiteral3178:path.
  AgentSession.getExtensionSourceLabel: AgentSession#getExtensionSourceLabel().
  AgentSession._refreshToolRegistry.options-typeLiteral3268.includeAllExtensionTools: AgentSession#_refreshToolRegistry().(options)typeLiteral3268:includeAllExtensionTools.
  AgentSession._createRlmSubagentRuntimeOptions: AgentSession#_createRlmSubagentRuntimeOptions().
  AgentSession._markProviderAuthStaleForRetryFailure.options-typeLiteral4097.markAuthStaleOnFailure: AgentSession#_markProviderAuthStaleForRetryFailure().(options)typeLiteral4097:markAuthStaleOnFailure.
  AgentSession.executeBash.options-typeLiteral4128.transient: AgentSession#executeBash().(options)typeLiteral4128:transient.
  AgentSession.runUserBash.options-typeLiteral4141.excludeFromContext: AgentSession#runUserBash().(options)typeLiteral4141:excludeFromContext.
  AgentSession.recordBashResult.options-typeLiteral4174.excludeFromContext: AgentSession#recordBashResult().(options)typeLiteral4174:excludeFromContext.
  AgentSession.navigateTree.Promise.typeLiteral134.aborted: AgentSession#navigateTree().Promise:typeLiteral134:aborted.
  AgentSession._navigateTree: AgentSession#_navigateTree().
  AgentSession._navigateTree.options-typeLiteral4221.summarize: AgentSession#_navigateTree().(options)typeLiteral4221:summarize.
  AgentSession._navigateTreeUnderPause.options-typeLiteral4236.customInstructions: AgentSession#_navigateTreeUnderPause().(options)typeLiteral4236:customInstructions.
  AgentSession._navigateTreeUnderPause.options-typeLiteral4236.replaceInstructions: AgentSession#_navigateTreeUnderPause().(options)typeLiteral4236:replaceInstructions.
  AgentSession._navigateTreeUnderPause.options-typeLiteral4236.label: AgentSession#_navigateTreeUnderPause().(options)typeLiteral4236:label.
  AgentSession.getUserMessagesForForking.Array.typeLiteral4333.text: AgentSession#getUserMessagesForForking().Array:typeLiteral4333:text.
  RlmChildAgentActivity.kind: RlmChildAgentActivity#kind.
  RlmChildAgentActivity.toolName: RlmChildAgentActivity#toolName.
  UserBashEndDetails.typeLiteral80.exitCode: UserBashEndDetails#typeLiteral80:exitCode.
  UserBashEndDetails.typeLiteral80.cancelled: UserBashEndDetails#typeLiteral80:cancelled.
  UserBashEndDetails.typeLiteral80.truncated: UserBashEndDetails#typeLiteral80:truncated.
  UserBashEndDetails.typeLiteral80.fullOutputPath: UserBashEndDetails#typeLiteral80:fullOutputPath.
  UserBashEndDetails.typeLiteral80.errorMessage: UserBashEndDetails#typeLiteral80:errorMessage.
  ModelCycleResult.isScoped: ModelCycleResult#isScoped.
  AgentSession._serializedExplicitRefineOptions.typeLiteral318.instructions: AgentSession#_serializedExplicitRefineOptions.typeLiteral318:instructions.
  AgentSession._serializedExplicitRefineOptions.typeLiteral318.global: AgentSession#_serializedExplicitRefineOptions.typeLiteral318:global.
  AgentSession._applySerializedPlan.bgResult-Extract.typeLiteral791.status: AgentSession#_applySerializedPlan().(bgResult)Extract:typeLiteral791:status.
  AgentSession._runBackgroundPlan.options-typeLiteral825.rollbackId: AgentSession#_runBackgroundPlan().(options)typeLiteral825:rollbackId.
  AgentSession._runBackgroundPlan.options-typeLiteral825.global: AgentSession#_runBackgroundPlan().(options)typeLiteral825:global.
  AgentSession._runSerializedRefine.options-typeLiteral770.rollbackId: AgentSession#_runSerializedRefine().(options)typeLiteral770:rollbackId.
  AgentSession.setScopedModels.scopedModels-Array.typeLiteral1372.thinkingLevel: AgentSession#setScopedModels().(scopedModels)Array:typeLiteral1372:thinkingLevel.
  AgentSession._queuePreparedPrompt.options-typeLiteral1804.agentMessageId: AgentSession#_queuePreparedPrompt().(options)typeLiteral1804:agentMessageId.
  AgentSession._queuePreparedPrompt.options-typeLiteral1804.queueKey: AgentSession#_queuePreparedPrompt().(options)typeLiteral1804:queueKey.
  AgentSession._queuePreparedPrompt.options-typeLiteral1804.previewLabel: AgentSession#_queuePreparedPrompt().(options)typeLiteral1804:previewLabel.
  AgentSession._queuePreparedPrompt.options-typeLiteral1804.suppressAutonomousContinuation: AgentSession#_queuePreparedPrompt().(options)typeLiteral1804:suppressAutonomousContinuation.
  AgentSession._queuePreparedPrompt.options-typeLiteral1804.resumeIfIdle: AgentSession#_queuePreparedPrompt().(options)typeLiteral1804:resumeIfIdle.
  AgentSession.refine.options-typeLiteral2938.instructions: AgentSession#refine().(options)typeLiteral2938:instructions.
  AgentSession.refine.options-typeLiteral2938.rollbackId: AgentSession#refine().(options)typeLiteral2938:rollbackId.
  AgentSession.refine.options-typeLiteral2938.global: AgentSession#refine().(options)typeLiteral2938:global.
  AgentSession._planRefine.options-typeLiteral2976.instructions: AgentSession#_planRefine().(options)typeLiteral2976:instructions.
  AgentSession._applyRefine.options-typeLiteral3026.instructions: AgentSession#_applyRefine().(options)typeLiteral3026:instructions.
  AgentSession.buildExtensionResourcePaths.Array.typeLiteral3179.path: AgentSession#buildExtensionResourcePaths().Array:typeLiteral3179:path.
  AgentSession.buildExtensionResourcePaths.Array.typeLiteral3179.metadata: AgentSession#buildExtensionResourcePaths().Array:typeLiteral3179:metadata.
  AgentSession.buildExtensionResourcePaths.Array.typeLiteral3179.metadata.typeLiteral3180.source: AgentSession#buildExtensionResourcePaths().Array:typeLiteral3179:metadata.typeLiteral3180:source.
  AgentSession.buildExtensionResourcePaths.Array.typeLiteral3179.metadata.typeLiteral3180.scope: AgentSession#buildExtensionResourcePaths().Array:typeLiteral3179:metadata.typeLiteral3180:scope.
  AgentSession.buildExtensionResourcePaths.Array.typeLiteral3179.metadata.typeLiteral3180.origin: AgentSession#buildExtensionResourcePaths().Array:typeLiteral3179:metadata.typeLiteral3180:origin.
  AgentSession._handleRetryableError.options-typeLiteral4104.markAuthStaleOnFailure: AgentSession#_handleRetryableError().(options)typeLiteral4104:markAuthStaleOnFailure.
  AgentSession._handleRetryableError.options-typeLiteral4104.authSourceTokens: AgentSession#_handleRetryableError().(options)typeLiteral4104:authSourceTokens.
  AgentSession.executeBash.options-typeLiteral4128.excludeFromContext: AgentSession#executeBash().(options)typeLiteral4128:excludeFromContext.
  AgentSession.runUserBashLocked.identity-typeLiteral4148.transient: AgentSession#runUserBashLocked().(identity)typeLiteral4148:transient.
  AgentSession.runUserBashLocked.identity-typeLiteral4148.runId: AgentSession#runUserBashLocked().(identity)typeLiteral4148:runId.
  AgentSession.navigateTree.options-typeLiteral4209.summarize: AgentSession#navigateTree().(options)typeLiteral4209:summarize.
  AgentSession.navigateTree.options-typeLiteral4209.customInstructions: AgentSession#navigateTree().(options)typeLiteral4209:customInstructions.
  AgentSession.navigateTree.options-typeLiteral4209.replaceInstructions: AgentSession#navigateTree().(options)typeLiteral4209:replaceInstructions.
  AgentSession.navigateTree.options-typeLiteral4209.label: AgentSession#navigateTree().(options)typeLiteral4209:label.
  AgentSession._navigateTree.options-typeLiteral4221.customInstructions: AgentSession#_navigateTree().(options)typeLiteral4221:customInstructions.
  AgentSession._navigateTree.options-typeLiteral4221.replaceInstructions: AgentSession#_navigateTree().(options)typeLiteral4221:replaceInstructions.
  AgentSession._navigateTree.options-typeLiteral4221.label: AgentSession#_navigateTree().(options)typeLiteral4221:label.
  AgentSession._navigateTree.Promise.typeLiteral4222.editorText: AgentSession#_navigateTree().Promise:typeLiteral4222:editorText.
  AgentSession._navigateTree.Promise.typeLiteral4222.cancelled: AgentSession#_navigateTree().Promise:typeLiteral4222:cancelled.
  AgentSession._navigateTree.Promise.typeLiteral4222.aborted: AgentSession#_navigateTree().Promise:typeLiteral4222:aborted.
  AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.editorText: AgentSession#_navigateTreeUnderPause().Promise:typeLiteral4237:editorText.
  AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.cancelled: AgentSession#_navigateTreeUnderPause().Promise:typeLiteral4237:cancelled.
  AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.aborted: AgentSession#_navigateTreeUnderPause().Promise:typeLiteral4237:aborted.
---
# Module: [`packages/coding-agent/src/core/agent-session.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts)

## Classes
### `AgentMessageDeferred`
- def: [`packages/coding-agent/src/core/agent-session.ts:871`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L871)
- signature: `interface AgentMessageDeferred`
- members:
  - `promise` — [`L872`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L872)
  - `reject` — [`L874`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L874)
  - `resolve` — [`L873`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L873)
- used by: [`_startRlmChildRun`](agent-session.ts.md#AgentSession._startRlmChildRun), [`promptAndWait`](agent-session.ts.md#AgentSession.promptAndWait), [`_settleAgentMessage`](agent-session.ts.md#AgentSession._settleAgentMessage), [`waitForAgentMessagePromptDelivery`](agent-session.ts.md#AgentSession.waitForAgentMessagePromptDelivery), [`_awaitPendingRlmChildPublication`](agent-session.ts.md#AgentSession._awaitPendingRlmChildPublication), [`_cancelRlmChildRun`](agent-session.ts.md#AgentSession._cancelRlmChildRun), [`createAgentMessageDeferred`](agent-session.ts.md#createAgentMessageDeferred), [`publication`](agent-session.ts.md#RlmChildRun.publication), [`delivery`](agent-session.ts.md#AgentMessageOutcome.delivery), [`AgentMessageOutcome`](agent-session.ts.md#AgentMessageOutcome)

### `AgentMessageOutcome`
- def: [`packages/coding-agent/src/core/agent-session.ts:881`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L881)
- doc: Per-agent-message settlement record: `delivery` settles when the prompt reaches agent state,
- signature: `interface AgentMessageOutcome`
- members:
  - `completion` — [`L883`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L883)
  - `delivery` — [`L882`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L882)
- uses (calls/refs, reference-scoped): [`AgentMessageDeferred`](agent-session.ts.md#AgentMessageDeferred)
- used by: [`dispose`](agent-session.ts.md#AgentSession.dispose), [`promptAndWait`](agent-session.ts.md#AgentSession.promptAndWait), [`_settleAgentMessage`](agent-session.ts.md#AgentSession._settleAgentMessage), [`waitForAgentMessagePromptDelivery`](agent-session.ts.md#AgentSession.waitForAgentMessagePromptDelivery), [`_agentMessageOutcomes`](agent-session.ts.md#AgentSession._agentMessageOutcomes), [`_agentMessageOutcome`](agent-session.ts.md#AgentSession._agentMessageOutcome)

### `AgentSession`
- def: [`packages/coding-agent/src/core/agent-session.ts:1084`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1084)
- signature: `class AgentSession`
- members:
  - `<constructor>(config: AgentSessionConfig)` — [`L1289`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1289) — documented in [packages-coding-agent-src-core-agent-session.ts](../../../../../concepts/packages-coding-agent-src-core-agent-session.ts.md)
  - `<get>_steeringStopPending` — [`L2152`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2152)
  - `<get>autoCompactionEnabled` — [`L8309`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8309) — Whether auto-compaction is enabled
  - `<get>autoRetryEnabled` — [`L10365`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10365) — Whether auto-retry is enabled
  - `<get>extensionRunner` — [`L11264`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L11264) — Get the extension runner (for setting UI context and error handlers).
  - `<get>followUpMode` — [`L4174`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4174) — Current follow-up mode
  - `<get>goalState` — [`L4203`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4203)
  - `<get>hasAcceptedPromptInFlight` — [`L10353`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10353) — Whether an accepted prompt is still running or waiting for retry completion.
  - `<get>hasPendingAdmissionWaiters` — [`L5403`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5403)
  - `<get>hasPendingBashMessages` — [`L10608`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10608) — Whether there are pending bash messages waiting to be flushed
  - `<get>hasPendingSessionWork` — [`L5391`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5391)
  - `<get>isBashRunning` — [`L10603`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10603) — Whether a bash command is currently running
  - `<get>isCompacting` — [`L4132`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4132) — Whether compaction or branch summarization is currently running
  - `<get>isQueuedWorkSuspended` — [`L6190`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6190)
  - `<get>isRetrying` — [`L10348`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10348) — Whether auto-retry is currently in progress
  - `<get>isSessionActive` — [`L6194`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6194)
  - `<get>isStreaming` — [`L4065`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4065) — Whether agent is currently streaming a response
  - `<get>messages` — [`L4141`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4141) — All messages including custom types like BashExecutionMessage
  - `<get>model` — [`L4051`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4051) — Current model (may be undefined if not yet selected)
  - `<get>modelRegistry` — [`L1387`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1387) — Model registry for API key resolution and model discovery
  - `<get>promptTemplates` — [`L4248`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4248) — File-based prompt templates
  - `<get>queuedActionCount` — [`L6182`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6182)
  - `<get>repliedToParentSinceTask` — [`L8995`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8995)
  - `<get>resourceLoader` — [`L6582`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6582)
  - `<get>retryAttempt` — [`L4075`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4075) — Current retry attempt (0 if not retrying)
  - `<get>rlmDepth` — [`L4189`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4189) — Current RLM spawn depth for this session.
  - `<get>rlmMaxDepth` — [`L4194`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4194) — Current absolute RLM spawn-depth cap.
  - `<get>scopedModels` — [`L4235`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4235) — Scoped models for cycling (from --models flag)
  - `<get>serviceTier` — [`L4060`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4060)
  - `<get>sessionFile` — [`L4179`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4179) — Current session file path, or undefined if sessions are disabled
  - `<get>sessionId` — [`L4184`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4184) — Current session ID
  - `<get>sessionName` — [`L4199`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4199) — Current session display name, if set
  - `<get>state` — [`L4046`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4046) — Full agent state
  - `<get>steeringMode` — [`L4169`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4169) — Current steering mode
  - `<get>systemPrompt` — [`L4070`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4070) — Current effective system prompt (includes any per-turn extension modifications)
  - `<get>thinkingLevel` — [`L4056`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4056) — Current thinking level
  - `<get>unfinishedActionCount` — [`L6186`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6186)
  - `_appendBeforeAgentStartMessages(method)` — [`L2006`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2006) — Append custom messages returned by before_agent_start extension handlers.
  - `_applyRefine(method)` — [`L7867`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7867) — Synchronous application phase: disconnects from the agent, aborts any
  - `_applySerializedPlan(method)` — [`L2461`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2461) — Apply an exact background plan directly via _applyRefine without
  - `_consumeSerializedBackgroundPlan(method)` — [`L2425`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2425) — Claim and process the serialized background plan if one is in flight.
  - `_contextTokensForCurrentMessages(method)` — [`L8984`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8984) — Context size (tokens) of this session's latest assistant turn, for live subagent display.
  - `_createKernelHostHandlers(method)` — [`L8761`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8761) — Typed handlers for host requests arriving from the IPython kernel comm bridge.
  - `_disconnectFromAgent(method)` — [`L3750`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3750) — Temporarily disconnect from agent events.
  - `_drainPendingRefinementForDisposal(method)` — [`L3804`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3804) — Await any in-flight refinement (planning or application) and run a
  - `_emit(method)` — [`L1491`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1491) — Emit an event to all listeners
  - `_emitExtensionEvent(method)` — [`L3649`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3649) — Emit extension events based on agent events
  - `_emitRefineFailed(method)` — [`L7324`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7324) — Consume a refine request that was scheduled by the agent-callable refine
  - `_endCompactionUnsuccessfully(method)` — [`L8113`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8113) — Emit an unsuccessful compaction_end and durably record the outcome.
  - `_ensureGoalRuntimeActive(method)` — [`L2041`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2041) — Goals are pursued through the IPython goal skill, so the only tool the
  - `_expandSkillCommand(method)` — [`L4815`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4815) — Expand skill commands (/skill:name args) to their full content.
  - `_findLastAssistantMessage(method)` — [`L3621`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3621) — Find the last assistant message in agent state (including aborted ones)
  - `_flushPendingBashMessages(method)` — [`L10616`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10616) — Flush pending bash messages to agent state and session.
  - `_getThresholdContextTokens(method)` — [`L7984`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7984) — Check if compaction is needed and run it.
  - `_handleRetryableError(method)` — [`L10223`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10223) — Handle retryable errors with exponential backoff.
  - `_installAgentToolHooks(method)` — [`L1425`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1425) — Install tool hooks once on the Agent instance.
  - `_isBranchSeedable(method)` — [`L1622`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1622) — Whether the session branch is seedable for an initial goal. Returns true
  - `_isRetryableError(method)` — [`L10051`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10051) — Check if an error is retryable (overloaded, rate limit, server errors).
  - `_loadMergedHarnessState(method)` — [`L7648`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7648) — Global harness state overlaid with this session's local state, when persisted.
  - `_maybeStartSerializedBackgroundPlan(method)` — [`L2486`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2486) — Start background refinement planning at assistant message_end, while
  - `_mergeUnpersistedCompactionOutcomes(method)` — [`L4158`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4158) — Merge disclosures whose session-file append failed into a rebuilt message
  - `_modelVisibleSkills(method)` — [`L8737`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8737) — Skills exposed to the model (system prompt + kernel). The bundled goal
  - `_onIpythonStateRestored(method)` — [`L7022`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7022) — Tell the model when a resumed session revived its IPython kernel state, so it
  - `_performCompaction(method)` — [`L7170`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7170) — Shared compaction core behind /compact, auto-compaction, and the compact
  - `_planRefine(method)` — [`L7801`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7801) — Background planning phase: runs the LLM planning call via `planRefinement`.
  - `_reconnectToAgent(method)` — [`L3761`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3761) — Reconnect to agent events after _disconnectFromAgent().
  - `_rejectAgentMessage(method)` — [`L3277`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3277) — Reject both currently registered legs of an agent message outcome.
  - `_resolveRetry(method)` — [`L3611`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3611) — Resolve the pending retry promise
  - `_rlmSessionDirForReading(method)` — [`L11096`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L11096) — RLM session dir holding sub-* child sessions, without creating directories.
  - `_runBackgroundPlan(method)` — [`L2542`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2542) — Shared background planning coroutine. Runs review + planRefine and
  - `_runSerializedAutoRefineReview(method)` — [`L2379`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2379) — Run automatic review and, when approved, refinement at a serialized turn boundary.
  - `_runSerializedRefine(method)` — [`L2607`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2607) — Direct serialized plan+apply. Calls _planRefine and _applyRefine with
  - `_runSerializedRefineCheckpoint(method)` — [`L2226`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2226) — Serialized-mode auto-refine checkpoint called from _shouldStopAfterTurn.
  - `_sessionOwnsScheduledContinuations(method)` — [`L7389`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7389) — Whether any snapshot of scheduled continuation messages is still session-owned.
  - `_settleAgentMessage(method)` — [`L3258`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3258) — Resolve (no error) or reject an existing leg of an agent message outcome.
  - `_throwIfExtensionCommand(method)` — [`L5887`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5887) — Throw an error if the text is an extension command.
  - `_waitForRefineIdle(method)` — [`L7790`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7790) — Block a new agent turn until any in-flight refine application phase has
  - `abort(method)` — [`L6609`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6609) — Abort current operation and wait for agent to become idle.
  - `abortBash(method)` — [`L10593`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10593) — Cancel running bash command.
  - `abortBranchSummary(method)` — [`L7969`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7969) — Cancel in-progress branch summarization.
  - `abortCompaction(method)` — [`L7260`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7260) — Cancel in-progress compaction (manual or auto).
  - `abortForUpdateRestart(method)` — [`L6627`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6627)
  - `abortRetry(method)` — [`L10314`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10314) — Cancel in-progress retry.
  - `acceptAgentMessagePrompt(method)` — [`L4479`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4479)
  - `acquireQueuedWorkPause(method)` — [`L6401`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6401)
  - `bindExtensions(method)` — [`L8324`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8324)
  - `buildExtensionResourcePaths(method)` — [`L8368`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8368)
  - `buildSessionContext(method)` — [`L4145`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4145)
  - `cancelRlmChildRun(method)` — [`L9584`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9584) — Cancel a single RLM child run by id, searching nested child sessions.
  - `clearQueue(method)` — [`L6017`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6017) — Clear all queued messages and return them.
  - `clearQueuedUserMessagesMatching(method)` — [`L6051`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6051)
  - `compact(method)` — [`L7081`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7081) — Manually compact the session context.
  - `createReplacedSessionContext(method)` — [`L11244`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L11244)
  - `cycleModel(method)` — [`L6746`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6746) — Cycle to next/previous model.
  - `cycleThinkingLevel(method)` — [`L6923`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6923) — Cycle to next thinking level.
  - `deleteInactiveRlmSubagent(method)` — [`L9268`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9268) — Delete an inactive direct or nested child by its registry child id without affecting active runs.
  - `deleteRlmSubagent(method)` — [`L9310`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9310) — Delete a running, retained, or passive direct child selected from this parent session's registry.
  - `dispose(method)` — [`L3976`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3976)
  - `disposeAsync(method)` — [`L3775`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3775) — Async teardown for graceful quit/switch: await the IPython kernel's dispose
  - `executeBash(method)` — [`L10388`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10388) — Execute a bash command.
  - `exportToHtml(method)` — [`L11154`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L11154) — Export session to HTML.
  - `exportToJsonl(method)` — [`L11177`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L11177) — Export the current session branch to a JSONL file.
  - `extendResourcesFromExtensions(method)` — [`L8343`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8343)
  - `findRlmModels(method)` — [`L9651`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9651)
  - `followUp(method)` — [`L4883`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4883) — Queue a follow-up message to be processed after the agent finishes.
  - `getActiveToolNames(method)` — [`L4083`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4083) — Get the names of currently active tools.
  - `getAllTools(method)` — [`L4090`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4090) — Get all configured tools with name, description, parameter schema, and source metadata.
  - `getAutonomousStatus(method)` — [`L4207`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4207)
  - `getAvailableThinkingLevels(method)` — [`L6939`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6939) — Get available thinking levels for current model.
  - `getContextTree(method)` — [`L11110`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L11110) — Build the agent context overview for /context: this session as the root
  - `getContextUsage(method)` — [`L11049`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L11049)
  - `getCurrentRecap(method)` — [`L8999`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8999)
  - `getExtensionSourceLabel(method)` — [`L8392`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8392)
  - `getFollowUpMessagePreviews(method)` — [`L6255`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6255)
  - `getFollowUpMessages(method)` — [`L6249`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6249)
  - `getLastAssistantText(method)` — [`L11216`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L11216) — Get text content of last assistant message.
  - `getPendingNextTurnMessageSnapshots(method)` — [`L6541`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6541)
  - `getRlmChildRunStatus(method)` — [`L9139`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9139) — Status of a direct RLM child run, while the run is still tracked.
  - `getRlmChildSession(method)` — [`L9558`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9558)
  - `getRlmMaxDepthStatus(method)` — [`L10635`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10635) — Current RLM max-depth value and the source that supplied it.
  - `getSessionActionRecoverySnapshot(method)` — [`L6261`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6261)
  - `getSessionActionSnapshot(method)` — [`L6206`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6206)
  - `getSessionStats(method)` — [`L11004`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L11004) — Get session statistics.
  - `getSteeringMessagePreviews(method)` — [`L6243`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6243)
  - `getSteeringMessages(method)` — [`L6237`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6237)
  - `getToolDefinition(method)` — [`L4099`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4099)
  - `getUserMessagesForForking(method)` — [`L10973`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10973) — Get all user messages from session for fork selector.
  - `handleAgentMessageHostRequest(method)` — [`L3060`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3060)
  - `handleAgentObserveHostRequest(method)` — [`L3092`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3092)
  - `handleCompactHostRequest(method)` — [`L2851`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2851) — Handle a compact.* request from the kernel host bridge. Compaction would
  - `handleGoalHostRequest(method)` — [`L2823`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2823) — Handle a goal.* request from the IPython kernel host bridge (the bundled
  - `handleRefineHostRequest(method)` — [`L2906`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2906) — Handle a refine.* request from the kernel host bridge. Like compact,
  - `handleRlmHeartbeatHostRequest(method)` — [`L2971`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2971) — Handle an rlm_heartbeat.* request from the bundled rlm-heartbeat skill.
  - `hasExtensionHandlers(method)` — [`L11257`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L11257) — Check if extensions have handlers for a specific event type.
  - `hasRunningRlmChildren(method)` — [`L9539`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9539) — True when any direct or nested subagent is still running or queued.
  - `listRlmSubagents(method)` — [`L9164`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9164) — Current direct-child registry for the model-facing rlm.list_subagents API.
  - `mutateQueuedMessage(method)` — [`L6115`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6115) — Mutate a single visible queued message, addressed by its position in the same
  - `navigateTree(method)` — [`L10698`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10698)
  - `prompt(method)` — [`L4453`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4453) — Send a prompt to the agent. — documented in [packages-coding-agent-src-core-agent-session.ts](../../../../../concepts/packages-coding-agent-src-core-agent-session.ts.md)
  - `promptAndWait(method)` — [`L4462`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4462)
  - `promptHeartbeat(method)` — [`L4516`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4516)
  - `promptUntilAccepted(method)` — [`L4458`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4458) — Resolve once the session has accepted ownership, before queued or active execution completes.
  - `queueAgentMessagePrompt(method)` — [`L4494`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4494)
  - `recordBashResult(method)` — [`L10564`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10564) — Record a bash execution result in session history.
  - `recordHostAutonomousContinuation(method)` — [`L4211`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4211)
  - `refine(method)` — [`L7671`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7671) — Refine editable continual harness state: prompt notes, memory, skills, and subagent specs.
  - `refreshAutonomousGates(method)` — [`L4215`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4215)
  - `registerDisposeCallback(method)` — [`L4028`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4028)
  - `registerRlmChildSession(method)` — [`L9502`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9502) — Retain a finished child session for the parent lifetime so inspectors and
  - `release(method)` — [`L6401`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6401)
  - `release(method)` — [`L6418`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6418)
  - `release(method)` — [`L6460`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6460)
  - `releaseRlmChildSession(method)` — [`L9523`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9523) — Stop retaining an idle daemon child without deleting its durable registry row.
  - `reload(method)` — [`L8865`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8865)
  - `removeQueuedFollowUp(method)` — [`L6569`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6569)
  - `requestAbort(method)` — [`L6586`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6586)
  - `restoreFollowUpMessage(method)` — [`L5051`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5051)
  - `restorePendingNextTurnMessages(method)` — [`L6565`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6565)
  - `restoreSessionActions(method)` — [`L4909`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4909)
  - `restoreSteeringMessage(method)` — [`L5024`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5024)
  - `resumeQueuedWork(method)` — [`L6500`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6500) — Resume the scheduler after requestAbort/abortForUpdateRestart suspended it; owned pause leases are unaffected.
  - `runRlmChild(method)` — [`L10035`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10035)
  - `runUserBash(method)` — [`L10433`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10433) — Run a user-initiated bash command (! / !! prefix), emitting bash_start,
  - `runUserBashLocked(method)` — [`L10477`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10477)
  - `sendCustomMessage(method)` — [`L5910`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5910) — Send a custom message to the session. Creates a CustomMessageEntry.
  - `sendUserMessage(method)` — [`L5978`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5978) — Send a user message to the agent. Always triggers a turn.
  - `setActiveToolsByName(method)` — [`L4109`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4109) — Set active tools by name.
  - `setAutoCompactionEnabled(method)` — [`L8304`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8304) — Toggle auto-compaction setting.
  - `setAutoRetryEnabled(method)` — [`L10372`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10372) — Toggle auto-retry setting.
  - `setCurrentRecap(method)` — [`L8989`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8989)
  - `setExecEnvProvider(method)` — [`L8318`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8318) — Set the provider for extra env vars merged over process.env in extension
  - `setFollowUpMode(method)` — [`L7067`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7067) — Set follow-up message mode.
  - `setModel(method)` — [`L6691`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6691) — Set model directly.
  - `setRlmHeartbeatController(method)` — [`L1373`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1373) — Set the RLM heartbeat controller after construction. Used by
  - `setRlmMaxDepth(method)` — [`L10640`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10640) — Persist and immediately apply a per-chat RLM max-depth override.
  - `setScopedModels(method)` — [`L4243`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4243) — Update scoped models for cycling
  - `setServiceTier(method)` — [`L6876`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6876)
  - `setSessionName(method)` — [`L10673`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10673) — Set a display name for the current session.
  - `setSteeringMode(method)` — [`L7058`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7058) — Set steering message mode.
  - `setSubagentRuntimeHost(method)` — [`L1391`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1391)
  - `setThinkingLevel(method)` — [`L6852`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6852) — Set thinking level.
  - `steer(method)` — [`L4850`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4850) — Queue a steering message while the agent is running.
  - `stop(method)` — [`L6337`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6337)
  - `subscribe(method)` — [`L3733`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3733) — Subscribe to agent events.
  - `supportsThinking(method)` — [`L6947`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6947) — Check if current model supports thinking/reasoning.
  - `waitForAgentMessagePromptDelivery(method)` — [`L3251`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3251) — Register a delivery waiter before submitting the prompt. Delivery outcomes are not retained
  - `waitForIdle(method)` — [`L6515`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6515)
  - `waitForRetry(method)` — [`L10338`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10338) — Wait for any in-progress retry to complete.
  - `waitForSessionInputCheckpoint(method)` — [`L6354`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6354)
  - `waitForSessionInputIdle(method)` — [`L6507`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6507)
  - `_actionStore` — [`L1106`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1106) — Session-owned actions. Items are never fed into Agent.steer/followUp.
  - `_branchNavigationQueue` — [`L10696`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10696) — Navigate to a different node in the session tree.
  - `_currentRecap` — [`L1238`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1238) — Latest recap for this session, written by the daemon summarizer; read by a parent to label its child snapshots.
  - `_handleAgentEvent` — [`L3313`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3313) — Internal handler for agent events - shared by subscribe and reconnect
  - `_ipythonKernelSnapshotDir` — [`L1204`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1204) — Artifact dir backing the current provisioner's kernel snapshot, if any.
  - `_ipythonRuntimeBuilt` — [`L1206`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1206) — True once the runtime has been built once; later builds are in-process rebuilds (/reload).
  - `_overflowRecovery` — [`L1140`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1140) — One recovery attempt per overflow; "reported" dedups the failure notice.
  - `_pendingNextTurnMessages` — [`L1125`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1125) — Messages queued to be included with the next user prompt as context ("asides").
  - `_refineInFlight` — [`L1274`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1274) — Settles (never rejects) after a planned refine waits for idle and finishes applying.
  - `_refinePlanInFlight` — [`L1276`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1276) — Settles when the background planning LLM pass completes. Planning does not block turn entry points.
  - `_serializedPlanInFlight` — [`L1282`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1282) — Settles when a serialized-mode background planning pass completes.
  - `_serializedRefine` — [`L1272`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1272) — When true, auto-refine runs synchronously between turns (serialized mode).
  - `_unpersistedCompactionOutcomes` — [`L1158`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1158) — Outcome disclosures whose session-file append failed; retained for context rebuilds.
  - `aborted` — [`L8118`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8118)
  - `aborted` — [`L10709`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10709)
  - `aborted` — [`L10736`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10736)
  - `aborted` — [`L10777`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10777)
  - `accepted` — [`L5302`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5302)
  - `acceptedAgentMessage` — [`L5201`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5201)
  - `acceptedBeforeCompletion` — [`L5202`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5202)
  - `activeToolNames` — [`L8536`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8536)
  - `activeToolNames` — [`L8634`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8634)
  - `agent` — [`L1085`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1085) — documented in [packages-coding-agent-src-core-agent-session.ts](../../../../../concepts/packages-coding-agent-src-core-agent-session.ts.md)
  - `agentMessageId` — [`L4855`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4855)
  - `agentMessageId` — [`L4888`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4888)
  - `agentMessageId` — [`L5029`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5029)
  - `agentMessageId` — [`L5056`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5056)
  - `agentMessageId` — [`L5190`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5190)
  - `agentMessageId` — [`L5256`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5256)
  - `agentMessageId` — [`L5353`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5353)
  - `apiKey` — [`L1396`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1396)
  - `apiKey` — [`L7172`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7172)
  - `authSourceTokens` — [`L10189`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10189)
  - `authSourceTokens` — [`L10227`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10227)
  - `baseDir` — [`L8374`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8374)
  - `cancelPostCompactionContinue` — [`L7285`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7285)
  - `cancelled` — [`L10708`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10708)
  - `cancelled` — [`L10735`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10735)
  - `cancelled` — [`L10776`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10776)
  - `content` — [`L5030`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5030)
  - `content` — [`L5057`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5057)
  - `content` — [`L5192`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5192)
  - `content` — [`L5355`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5355)
  - `current` — [`L1179`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1179)
  - `customInstructions` — [`L7174`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7174)
  - `customInstructions` — [`L8120`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8120)
  - `customInstructions` — [`L10702`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10702)
  - `customInstructions` — [`L10729`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10729)
  - `customInstructions` — [`L10770`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10770)
  - `customMessage` — [`L5031`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5031)
  - `customMessage` — [`L5058`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5058)
  - `deferred` — [`L6336`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6336)
  - `deliverAs` — [`L5914`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5914)
  - `deliverAs` — [`L5980`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5980)
  - `disposition` — [`L5303`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5303)
  - `editorText` — [`L10707`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10707)
  - `editorText` — [`L10734`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10734)
  - `editorText` — [`L10775`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10775)
  - `entryId` — [`L10973`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10973)
  - `errorSeverity` — [`L8119`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8119)
  - `excludeFromContext` — [`L10392`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10392)
  - `excludeFromContext` — [`L10436`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10436)
  - `excludeFromContext` — [`L10564`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10564)
  - `executionPolicy` — [`L5199`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5199)
  - `extensionPath` — [`L8368`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8368)
  - `flagValues` — [`L8635`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8635)
  - `followUp` — [`L6017`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6017)
  - `followUp` — [`L6051`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6051)
  - `front` — [`L5297`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5297)
  - `global` — [`L1286`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1286)
  - `global` — [`L2543`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2543)
  - `global` — [`L2610`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2610)
  - `global` — [`L7675`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7675)
  - `global` — [`L7802`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7802)
  - `global` — [`L7869`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7869)
  - `global` — [`L10640`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10640)
  - `headers` — [`L1397`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1397)
  - `headers` — [`L7173`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7173)
  - `id` — [`L9010`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9010)
  - `immediatelyEligible` — [`L5299`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5299)
  - `includeAllExtensionTools` — [`L8536`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8536)
  - `includeAllExtensionTools` — [`L8636`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8636)
  - `instructions` — [`L1285`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1285)
  - `instructions` — [`L2543`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2543)
  - `instructions` — [`L2608`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2608)
  - `instructions` — [`L7673`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7673)
  - `instructions` — [`L7802`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7802)
  - `instructions` — [`L7869`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7869)
  - `label` — [`L10704`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10704)
  - `label` — [`L10731`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10731)
  - `label` — [`L10772`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10772)
  - `markAuthStaleOnFailure` — [`L10188`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10188)
  - `markAuthStaleOnFailure` — [`L10226`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10226)
  - `maxDepth` — [`L1578`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1578)
  - `message` — [`L5193`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5193)
  - `message` — [`L5356`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5356)
  - `messages` — [`L2763`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2763)
  - `metadata` — [`L8370`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8370)
  - `model` — [`L1091`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1091)
  - `model` — [`L4236`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4236)
  - `model` — [`L4243`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4243)
  - `model` — [`L7171`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7171)
  - `model` — [`L9015`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9015)
  - `operations` — [`L10393`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10393)
  - `origin` — [`L8373`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8373)
  - `owner` — [`L6418`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6418)
  - `owner` — [`L6460`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6460)
  - `path` — [`L8368`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8368)
  - `path` — [`L8369`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8369)
  - `persist` — [`L1667`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1667)
  - `prefixMessages` — [`L5032`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5032)
  - `prefixMessages` — [`L5059`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5059)
  - `prefixMessages` — [`L5194`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5194)
  - `prefixMessages` — [`L5357`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5357)
  - `previewLabel` — [`L5195`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5195)
  - `previewLabel` — [`L5358`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5358)
  - `prompt` — [`L9011`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9011)
  - `queueKey` — [`L4854`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4854)
  - `queueKey` — [`L4887`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4887)
  - `queueKey` — [`L5028`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5028)
  - `queueKey` — [`L5055`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5055)
  - `queueKey` — [`L5191`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5191)
  - `queueKey` — [`L5354`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5354)
  - `queueVisible` — [`L5200`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5200)
  - `replaceInstructions` — [`L10703`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10703)
  - `replaceInstructions` — [`L10730`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10730)
  - `replaceInstructions` — [`L10771`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10771)
  - `restore` — [`L5296`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5296)
  - `restoreAutonomousState` — [`L2763`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2763)
  - `resumeIfIdle` — [`L4856`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4856)
  - `resumeIfIdle` — [`L4889`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4889)
  - `resumeIfIdle` — [`L5197`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5197)
  - `resumeIfIdle` — [`L5360`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5360)
  - `returnAfterAccepted` — [`L5117`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5117)
  - `rollbackId` — [`L2543`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2543)
  - `rollbackId` — [`L2609`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2609)
  - `rollbackId` — [`L7674`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7674)
  - `rollbackId` — [`L7802`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7802)
  - `rollbackId` — [`L7869`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7869)
  - `runId` — [`L10438`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10438)
  - `runId` — [`L10481`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10481)
  - `scope` — [`L8372`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8372)
  - `sessionDir` — [`L9014`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9014)
  - `sessionManager` — [`L1086`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1086)
  - `sessionName` — [`L9012`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9012)
  - `settingsManager` — [`L1087`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1087)
  - `signal` — [`L7175`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7175)
  - `skipAbort` — [`L7081`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7081)
  - `skipAbort` — [`L7677`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7677)
  - `skipPrePromptWork` — [`L5118`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5118)
  - `source` — [`L1579`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1579)
  - `source` — [`L5198`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5198)
  - `source` — [`L5257`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5257)
  - `source` — [`L5361`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5361)
  - `source` — [`L8371`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8371)
  - `spawnCode` — [`L9013`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9013)
  - `status` — [`L2462`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2462)
  - `steering` — [`L6017`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6017)
  - `steering` — [`L6051`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6051)
  - `summarize` — [`L10701`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10701)
  - `summarize` — [`L10728`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10728)
  - `summarize` — [`L10769`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10769)
  - `summaryEntry` — [`L10710`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10710)
  - `summaryEntry` — [`L10737`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10737)
  - `summaryEntry` — [`L10778`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10778)
  - `suppressAutonomousContinuation` — [`L5196`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5196)
  - `suppressAutonomousContinuation` — [`L5359`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5359)
  - `text` — [`L10973`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10973)
  - `thinkingLevel` — [`L1092`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1092)
  - `thinkingLevel` — [`L4237`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4237)
  - `thinkingLevel` — [`L4243`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4243)
  - `ticket` — [`L5304`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5304)
  - `transient` — [`L10394`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10394)
  - `transient` — [`L10437`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10437)
  - `transient` — [`L10481`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10481)
  - `triggerTurn` — [`L5913`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5913)
  - `wake` — [`L5298`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5298)
- protocol/private: `_accountGoalUsageForAssistantMessage`[`L2112`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2112), `_acquireDirectTurnAdmissionFence`[`L6418`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6418), `_acquireSessionActionCommitFence`[`L6460`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6460), `_activeRlmChildRuns`[`L1218`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1218), `_addLoginGuidanceToAuthError`[`L3411`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3411), `_addWebsearchKeyEnv`[`L8919`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8919), `_admitSessionInput`[`L5293`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5293), `_agentDir`[`L1178`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1178), `_agentEventQueue`[`L1103`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1103), `_agentMessageController`[`L1185`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1185), `_agentMessageOutcome`[`L3238`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3238), `_agentMessageOutcomes`[`L1155`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1155), `_agentObserveController`[`L1186`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1186), `_allowedToolNames`[`L1181`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1181), `_appendDurableSessionCommandMessage`[`L5857`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5857), `_applyExtensionBindings`[`L8401`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8401), `_applyLateIpythonSentAgentMessages`[`L1537`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1537), `_applyPreparedSystemPrompt`[`L4417`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4417), `_asError`[`L5649`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5649), `_assertRlmSubagentSessionNameAvailable`[`L9603`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9603), `_assertSessionActionAdmissionAvailable`[`L5284`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5284), `_assistantTurnsSinceAutoRefine`[`L1252`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1252), `_authenticatedRlmModels`[`L9644`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9644), `_autoCompactionAbortController`[`L1137`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1137), `_autoRefineAllowedForSession`[`L7272`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7272), `_autoRefineBranchVersion`[`L1267`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1267), `_autoRefineInProgress`[`L1254`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1254), `_autoRefineOperations`[`L1255`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1255), `_autoRefineReviewAbort`[`L1268`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1268), `_autoRefineReviewer`[`L1270`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1270), `_autonomousContinuationSuppressedMessages`[`L1133`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1133), `_autonomousContinuationSuppressionDepth`[`L1132`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1132), `_autonomousState`[`L1131`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1131), `_awaitPendingRlmChildPublication`[`L9151`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9151), `_baseSystemPrompt`[`L1250`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1250), `_baseSystemPromptOptions`[`L1251`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1251), `_baseToolDefinitions`[`L1176`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1176), `_baseToolsOverride`[`L1188`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1188), `_bashAbortController`[`L1161`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1161), `_bindExtensionCore`[`L8425`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8425), `_branchSummaryAbortController`[`L1146`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1146), `_branchSummaryOperation`[`L1147`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1147), `_buildPromptContent`[`L5082`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5082), `_buildRlmSubagentList`[`L9168`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9168), `_buildRuntime`[`L8633`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8633), `_canStartSessionActionImmediately`[`L4431`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4431), `_cancelActiveRlmChildRuns`[`L9117`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9117), `_cancelPostCompactionContinue`[`L7276`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7276), `_cancelRlmChildRun`[`L9123`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9123), `_cancelSessionActions`[`L1707`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1707), `_captureRetryAuthFailureSource`[`L10144`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10144), `_capturingCancelledAction`[`L3290`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3290), `_checkCompaction`[`L8008`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8008), `_clampServiceTierForModel`[`L6907`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6907), `_clampThinkingLevel`[`L6961`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6961), `_clearGoal`[`L1806`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1806), `_clearQueuedAutonomousContinuations`[`L2762`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2762), `_clearQueuedAutonomousContinuationsAfterSkippedThresholdCompaction`[`L2806`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2806), `_clearQueuedGoalContexts`[`L1770`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1770), `_coalescedFollowUpOwner`[`L5271`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5271), `_compactAutoRefinePending`[`L1257`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1257), `_compactionAbortController`[`L1136`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1136), `_compactionOperation`[`L1138`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1138), `_completeGoalFromHost`[`L3148`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3148), `_configuredRlmMaxDepth`[`L1209`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1209), `_consumePendingRequestedRefine`[`L7331`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7331), `_contextWindowResolver`[`L11100`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L11100), `_continueAfterThresholdCompaction`[`L1141`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1141), `_createChildRlmSessionDir`[`L8961`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8961), `_createDeliveryRecord`[`L5099`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5099), `_createEphemeralRlmSessionDir`[`L8978`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8978), `_createGoalFromHost`[`L3128`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3128), `_createInlineRlmSubagentRuntime`[`L9048`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9048), `_createPreparedTurnAction`[`L5185`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5185), `_createRetryPromiseForAgentEnd`[`L3377`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3377), `_createRlmSubagentRuntime`[`L9040`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9040), `_createRlmSubagentRuntimeOptions`[`L9009`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9009), `_createSessionCommandAction`[`L5250`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5250), `_currentActiveSessionId`[`L9143`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9143), `_customTools`[`L1175`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1175), `_cwd`[`L1177`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1177), `_cycleAvailableModel`[`L6803`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6803), `_cycleScopedModel`[`L6756`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6756), `_deleteResolvedRlmSubagent`[`L9434`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9434), `_deleteRlmSubagentSession`[`L9395`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9395), `_deletedRlmChildIds`[`L1223`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1223), `_deletingRlmChildren`[`L1227`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1227), `_deliveryPolicy`[`L5095`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5095), `_discardPendingAutoRefine`[`L7285`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7285), `_disposeAsyncOnce`[`L3929`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3929), `_disposeAsyncPromise`[`L1201`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1201), `_disposeCallbacks`[`L1196`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1196), `_disposeCallbacksPromise`[`L1197`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1197), `_disposed`[`L1195`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1195), `_disposing`[`L1200`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1200), `_drainQueuedMessagesAfterBash`[`L10472`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10472), `_emitAutonomousStatus`[`L1970`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1970), `_emitGoalUpdate`[`L1558`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1558), `_emitModelSelect`[`L6653`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6653), `_emitQueueUpdate`[`L1502`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1502), `_emitRlmSubagentRemoval`[`L9418`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9418), `_ensureRlmSessionDir`[`L8945`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8945), `_eventListeners`[`L1097`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1097), `_execEnvProvider`[`L1168`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1168), `_executeExtensionCommand`[`L4787`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4787), `_executeQueuedSessionCommand`[`L5809`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5809), `_executeSelectedSessionCommand`[`L5579`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5579), `_extensionCommandContextActions`[`L1191`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1191), `_extensionErrorListener`[`L1193`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1193), `_extensionErrorUnsubscriber`[`L1194`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1194), `_extensionRunner`[`L1167`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1167), `_extensionRunnerRef`[`L1179`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1179), `_extensionShutdownHandler`[`L1192`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1192), `_extensionUIContext`[`L1190`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1190), `_extractUserMessageText`[`L10990`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10990), `_findAssistantEntryForMessage`[`L9003`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9003), `_findLastAssistantInMessages`[`L3401`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3401), `_finishActiveRetryWithFailure`[`L10204`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10204), `_finishGoalForTerminalAssistantMessage`[`L1865`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1865), `_finishGoalWithError`[`L1851`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1851), `_finishSubmissionNormalization`[`L4331`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4331), `_forgetConsumedPostCompactionContinuations`[`L7442`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7442), `_formatAutonomousStatus`[`L1964`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1964), `_getContinuationMessages`[`L3198`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3198), `_getEffectiveServiceTier`[`L6899`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6899), `_getGoalContinuationMessages`[`L3167`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3167), `_getProviderStreamFailureAuthStatus`[`L10104`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10104), `_getProviderStreamFailureDetails`[`L10081`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10081), `_getProviderStreamFailureKind`[`L10090`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10090), `_getRequiredRequestAuth`[`L1395`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1395), `_getServiceTierForModelSwitch`[`L6903`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6903), `_getThinkingLevelForModelSwitch`[`L6951`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6951), `_goalAbortInProgress`[`L1130`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1130), `_goalAccountedAssistantMessages`[`L1129`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1129), `_goalAccountingStartedAt`[`L1128`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1128), `_goalState`[`L1127`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1127), `_goalWithAccountedWallClock`[`L1698`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1698), `_goalWithCurrentWallClock`[`L1684`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1684), `_handleAutonomousSlashCommand`[`L1990`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1990), `_handleGoalSlashCommand`[`L2075`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2075), `_hasCancelledDispatchCapture`[`L3301`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3301), `_hasSelectableSessionInput`[`L5384`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5384), `_includeCompactSkill`[`L1183`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1183), `_includeGoals`[`L1182`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1182), `_initialActiveToolNames`[`L1180`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1180), `_installAgentContinuationHook`[`L1477`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1477), `_installAgentTurnHook`[`L1481`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1481), `_invalidatePendingAutoRefineForBranchChange`[`L7294`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7294), `_invalidateQueuedPromptPreparation`[`L6045`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6045), `_ipythonKernelProvisioner`[`L1202`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1202), `_isAgentLifecycleFailure`[`L10077`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10077), `_isBusyForSessionInput`[`L5630`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5630), `_isConcreteProviderAuthFailure`[`L10126`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10126), `_isDeferredSessionInputError`[`L5653`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5653), `_isFauxProviderQueueExhausted`[`L10073`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10073), `_isPromptTurnStartMessage`[`L3602`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3602), `_isSessionInputHandoffDeferred`[`L5645`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5645), `_isStructuredPermanentProviderFailure`[`L10095`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10095), `_isStructuredPermanentProviderRetryExhausted`[`L10100`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10100), `_lastAssistantMessage`[`L3236`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3236), `_lastAutoRefineReviewAt`[`L1253`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1253), `_lastSessionActionSnapshot`[`L1098`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1098), `_lateIpythonSentAgentMessages`[`L1156`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1156), `_loadPersistedGoalState`[`L1599`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1599), `_loadPersistedRlmMaxDepthState`[`L1562`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1562), `_loadRefinementHistory`[`L7656`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7656), `_localHarnessStateDir`[`L7265`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7265), `_markAutonomousContinuationSuppressed`[`L4230`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4230), `_markProviderAuthStale`[`L10163`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10163), `_markProviderAuthStaleForRetryFailure`[`L10185`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10185), `_maybeAutoRefine`[`L7488`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7488), `_mcpManager`[`L1187`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1187), `_modelRegistry`[`L1241`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1241), `_modelSelectEmitContext`[`L1172`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1172), `_modelSelectEmitQueue`[`L1170`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1170), `_modelSelectEmitQueueIdle`[`L1171`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1171), `_navigateTree`[`L10725`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10725), `_navigateTreeUnderPause`[`L10765`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L10765), `_normalizePromptGuidelines`[`L4261`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4261), `_normalizePromptSnippet`[`L4252`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4252), `_normalizeSubmission`[`L4344`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4344), `_notifyKernelStateAfterCompaction`[`L6967`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6967), `_notifySessionInputCheckpointChange`[`L6329`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6329), `_observeSessionActionDeferral`[`L6335`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6335), `_parentReplyCount`[`L1216`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1216), `_parseAutonomousSlashCommand`[`L1948`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1948), `_parseGoalSlashCommand`[`L1896`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1896), `_pauseGoal`[`L1811`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1811), `_pendingAutoRefineReview`[`L1266`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1266), `_pendingBashMessages`[`L1164`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1164), `_pendingModelSelectEmit`[`L6733`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6733), `_pendingRequestedCompaction`[`L1142`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1142), `_pendingRequestedRefine`[`L1143`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1143), `_pendingRlmSubagentSessionNames`[`L1219`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1219), `_pendingSessionActionFenceWaiters`[`L1119`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1119), `_pendingThresholdCompactionAutonomousMessages`[`L1265`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1265), `_persistCompactionOutcome`[`L8137`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8137), `_persistGoalState`[`L1659`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1659), `_postCompactionContinuationMessages`[`L1261`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1261), `_postCompactionContinuationScheduled`[`L1259`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1259), `_postCompactionContinuationTimer`[`L1260`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1260), `_prepareForCommit`[`L4381`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4381), `_prewarmIpythonKernel`[`L1207`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1207), `_processAgentEvent`[`L3427`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3427), `_prompt`[`L4597`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4597), `_promptInjectedMessage`[`L4525`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4525), `_pumpSessionInputs`[`L5426`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5426), `_queueAutonomousContinuationForThresholdCompaction`[`L2726`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2726), `_queueModelSelectEmit`[`L6667`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6667), `_queuePreparedPrompt`[`L5348`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5348), `_queuedAutonomousContinuationSnapshots`[`L1264`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1264), `_queuedAutonomousThresholdContinuations`[`L1263`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1263), `_queuedWorkPauses`[`L1116`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1116), `_reapDeletedRlmSubagentRuntimesAfterCompaction`[`L7250`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7250), `_rebuildSystemPrompt`[`L4276`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4276), `_recordLateIpythonSentAgentMessage`[`L1546`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1546), `_refineAbortController`[`L1269`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1269), `_refreshCurrentModelFromRegistry`[`L8411`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8411), `_refreshExtensionSystemPrompt`[`L4321`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4321), `_refreshToolRegistry`[`L8536`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8536), `_rejectQueuedAgentMessageDeliveries`[`L3283`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3283), `_reloadGoalStateFromBranch`[`L1642`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1642), `_reloadRlmMaxDepthFromBranch`[`L1648`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1648), `_rememberLateIpythonSentAgentMessage`[`L1522`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1522), `_removeRlmSubagentTracking`[`L9402`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9402), `_replaceMessageInPlace`[`L3632`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3632), `_repliedToParentSinceTask`[`L1215`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1215), `_resolveDirectRlmSubagent`[`L9255`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9255), `_resolveRlmMaxDepth`[`L1577`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1577), `_resolveRlmSubagentModel`[`L9657`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9657), `_resourceLoader`[`L1174`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1174), `_restoreAutonomousRuntimeSnapshot`[`L2717`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2717), `_restoreLateIpythonSentAgentMessages`[`L1509`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1509), `_restorePromptInput`[`L5013`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5013), `_restoreSessionCommand`[`L4994`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4994), `_resumeGoal`[`L1827`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1827), `_retryAbortController`[`L1150`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1150), `_retryAttempt`[`L1151`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1151), `_retryAuthFailureSources`[`L1154`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1154), `_retryPromise`[`L1152`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1152), `_retryResolve`[`L1153`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1153), `_reviewAutoRefine`[`L7625`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7625), `_rlmChildCleanupFailures`[`L1226`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1226), `_rlmChildSessions`[`L1222`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1222), `_rlmChildUnsubscribes`[`L1236`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1236), `_rlmDepth`[`L1208`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1208), `_rlmHeartbeatController`[`L1184`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1184), `_rlmKernelEnv`[`L8899`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8899), `_rlmMaxDepth`[`L1210`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1210), `_rlmMaxDepthSource`[`L1211`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1211), `_rlmParentAgent`[`L1214`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1214), `_rlmParentNodeId`[`L1213`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1213), `_rlmSessionDir`[`L1212`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1212), `_rlmSubagentMatchesTarget`[`L9246`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9246), `_runApprovedRefine`[`L7601`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7601), `_runAutoCompaction`[`L8167`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L8167), `_runOrQueueGoalContext`[`L2063`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2063), `_runPreTurnCompaction`[`L4376`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4376), `_runScheduledPostCompactionContinue`[`L7393`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7393), `_runSerializedRefineCheckpointAfterBackground`[`L2315`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2315), `_runWithAutonomousContinuationSuppressed`[`L4221`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L4221), `_runtimeActivity`[`L5371`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5371), `_scheduleAutoRefine`[`L7475`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7475), `_scheduleAutoRefineAfterAgentEnd`[`L7339`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7339), `_scheduleAutoRefineAfterCompaction`[`L7358`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7358), `_scheduleDeferredAutoRefineIfIdle`[`L7465`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7465), `_schedulePostCompactionContinue`[`L7376`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7376), `_scheduleSessionInputPump`[`L5411`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5411), `_scheduledAutoRefineTimers`[`L1256`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1256), `_scheduledPostCompactionContinuationMessages`[`L1262`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1262), `_scopedModels`[`L1090`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1090), `_serializedExplicitRefineOptions`[`L1284`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1284), `_serializedPlanClaim`[`L1283`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1283), `_serviceTierPreference`[`L1088`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1088), `_sessionActionCommitContext`[`L1120`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1120), `_sessionActionCommitDisposeAbortController`[`L1121`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1121), `_sessionActionCommitOwner`[`L1118`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1118), `_sessionActionCommitTail`[`L1117`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1117), `_sessionInputArrivalEpoch`[`L1112`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1112), `_sessionInputCheckpointWaiters`[`L1123`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1123), `_sessionInputPump`[`L1107`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1107), `_sessionInputPumpEpoch`[`L1111`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1111), `_sessionInputPumpRequested`[`L1109`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1109), `_sessionInputPumpSuspended`[`L1114`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1114), `_sessionStartEvent`[`L1189`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1189), `_setGoalState`[`L1667`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1667), `_shouldSkipAutoRefineForActiveAgent`[`L7461`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L7461), `_shouldStopAfterTurn`[`L2169`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2169), `_shouldStopBeforeTurn`[`L2165`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2165), `_shouldStopForThresholdCompaction`[`L2205`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2205), `_shouldWaitForModelSelectEmit`[`L6729`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6729), `_snapshotAutonomousRuntimeState`[`L2704`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2704), `_startDisposeCallbacks`[`L3956`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L3956), `_startGoal`[`L1785`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1785), `_startPreparedTurnActions`[`L5677`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5677), `_startRlmChildRun`[`L9684`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9684), `_stopGoalContinuationForTerminalMessage`[`L1884`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1884), `_subagentRuntimeHost`[`L1217`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1217), `_surfaceSessionInputError`[`L5663`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5663), `_takePendingNextTurnMessages`[`L5089`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5089), `_thresholdCompactionNeeded`[`L2682`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2682), `_toolDefinitions`[`L1245`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1245), `_toolPromptGuidelines`[`L1247`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1247), `_toolPromptSnippets`[`L1246`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1246), `_toolRegistry`[`L1244`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1244), `_trackModelSelectEmitError`[`L6718`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L6718), `_trackRlmSubagentDeletion`[`L9375`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L9375), `_turnExecutionPolicy`[`L5114`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L5114), `_turnIndex`[`L1169`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1169), `_turnIntervalAutoRefinePending`[`L1258`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1258), `_unsubscribeAgent`[`L1096`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1096), `_userBashAbortRequested`[`L1163`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1163), `_userBashRunning`[`L1162`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1162), `_validateCanStartAgentRun`[`L2023`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L2023)
- uses (calls/refs, reference-scoped): [`Model`](../../../ai/src/types.ts.md#Model), [`id`](../../../ai/src/types.ts.md#Model.id), [`provider`](../../../ai/src/types.ts.md#Model.provider), [`contextWindow`](../../../ai/src/types.ts.md#Model.contextWindow), [`reasoning`](../../../ai/src/types.ts.md#Model.reasoning), [`input`](../../../ai/src/types.ts.md#Model.input), [`role`](../../../ai/src/types.ts.md#AssistantMessage.role), [`role`](../../../ai/src/types.ts.md#ToolResultMessage.role), [`role`](../../../ai/src/types.ts.md#UserMessage.role), [`type`](../../../ai/src/types.ts.md#TextContent.type), [`content`](../../../ai/src/types.ts.md#AssistantMessage.content), [`role`](messages.ts.md#CustomMessage.role), [`role`](messages.ts.md#BashExecutionMessage.role), [`SessionManager`](session-manager.ts.md#SessionManager), [`role`](messages.ts.md#BranchSummaryMessage.role), [`role`](messages.ts.md#CompactionSummaryMessage.role), [`type`](../../../ai/src/types.ts.md#ToolCall.type), [`type`](../../../ai/src/types.ts.md#ThinkingContent.type), [`timestamp`](../../../ai/src/types.ts.md#AssistantMessage.timestamp), [`AgentMessage`](../../../agent/src/types.ts.md#AgentMessage), [`timestamp`](../../../ai/src/types.ts.md#ToolResultMessage.timestamp), [`timestamp`](../../../ai/src/types.ts.md#UserMessage.timestamp), [`AssistantMessage`](../../../ai/src/types.ts.md#AssistantMessage), [`content`](../../../ai/src/types.ts.md#UserMessage.content), [`stopReason`](../../../ai/src/types.ts.md#AssistantMessage.stopReason), [`usage`](../../../ai/src/types.ts.md#AssistantMessage.usage), [`id`](cron-jobs.ts.md#AgentCronJob.id), [`Api`](../../../ai/src/types.ts.md#Api), [`type`](../../../ai/src/types.ts.md#ImageContent.type), [`SettingsManager`](settings-manager.ts.md#SettingsManager), [`appendMessage`](session-manager.ts.md#SessionManager.appendMessage), [`<get>state`](../../../agent/src/agent.ts.md#Agent.-get-state), [`AgentCronJob`](cron-jobs.ts.md#AgentCronJob), [`cost`](../../../ai/src/types.ts.md#Usage.cost), [`type`](session-manager.ts.md#CompactionEntry.type), [`type`](session-manager.ts.md#CustomEntry.type), [`type`](session-manager.ts.md#LabelEntry.type), [`type`](session-manager.ts.md#ChildUsageAttributionEntry.type), [`type`](session-manager.ts.md#ModelChangeEntry.type), [`type`](session-manager.ts.md#AgentStatusEntry.type)  (+1117 more; 2 test-only)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`main`](../main.ts.md#main), [`handleCommand`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.handleCommand), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`createAgentSession`](sdk.ts.md#createAgentSession), [`<get>session`](agent-session-runtime.ts.md#AgentSessionRuntime.-get-session), [`summaryForActiveSession`](../modes/daemon/daemon-session-list.ts.md#summaryForActiveSession), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`installAgentTelemetry`](telemetry.ts.md#installAgentTelemetry), [`createRlmSubagentRuntime`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRlmSubagentRuntime), [`createRuntime`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRuntime), [`rehydrateCompletedRlmSubagentOnce`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.rehydrateCompletedRlmSubagentOnce), [`origin`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.sendAgentSessionMessage.options-typeLiteral1160.origin), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`createAgentSessionFromServices`](agent-session-services.ts.md#createAgentSessionFromServices), [`sdk.ts`](sdk.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-sdk.ts), [`agent-session-runtime.ts`](agent-session-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-runtime.ts), [`createSubagentRuntimeHost`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createSubagentRuntimeHost), [`createAgentObserveSummary`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentObserveSummary), [`rlmChildSnapshotForActiveSession`](../modes/daemon/daemon-session-list.ts.md#rlmChildSnapshotForActiveSession), [`createRlmSubagentRuntime`](agent-session-runtime.ts.md#AgentSessionRuntime.createRlmSubagentRuntime), [`createAgentConnectionResourceSnapshot`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionResourceSnapshot), [`createAgentFamilyCatalog`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentFamilyCatalog), [`createAgentMessageAgentSummary`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentMessageAgentSummary), [`addRuntime`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.addRuntime), [`createAgentMessageListResult`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentMessageListResult), [`bindActiveSessionState`](../modes/daemon/daemon-extension-binding.ts.md#bindActiveSessionState), [`createdAt`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.createdAt), [`sessionPassivationSnapshot`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.sessionPassivationSnapshot), [`cancelled`](agent-session-runtime.ts.md#AgentSessionRuntime.newSession.Promise.typeLiteral136.cancelled), [`buildSessionListWithPassiveRlmSubagents`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.buildSessionListWithPassiveRlmSubagents), [`createInteractiveModeLocalSessionHost`](../modes/interactive/interactive-mode-services.ts.md#createInteractiveModeLocalSessionHost), [`deliveryMode`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRlmHeartbeatForState.input-typeLiteral666.deliveryMode), [`closeSessionOnce`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.closeSessionOnce), [`createHeartbeatForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createHeartbeatForState), [`hydratePassiveRlmSubagent`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.hydratePassiveRlmSubagent), [`createUpdateRestartSession`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createUpdateRestartSession), [`summarize`](../modes/daemon/daemon-session-summarizer.ts.md#DaemonSessionSummarizer.summarize), [`runCronJob`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.runCronJob)  (+140 more; 124 test-only)

### `AgentSessionConfig`
- def: [`packages/coding-agent/src/core/agent-session.ts:410`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L410)
- signature: `interface AgentSessionConfig`
- members:
  - `agent` — [`L411`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L411)
  - `agentDir` — [`L417`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L417) — Config dir backing credentials (auth.json); exported to the kernel for skills.
  - `agentMessageController` — [`L437`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L437) — Daemon-backed agent-to-agent messaging bridge. Omitted for local-only sessions.
  - `agentObserveController` — [`L439`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L439) — Daemon-backed read-only active-session observation bridge. Omitted for local-only sessions.
  - `allowedToolNames` — [`L429`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L429) — Optional allowlist of tool names. When provided, only these tool names are exposed.
  - `autoRefineReviewer` — [`L488`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L488) — Test/extension hook for automatic refine review decisions. Defaults to the model-backed review gate.
  - `autonomous` — [`L479`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L479) — Host-side autonomous continuation policy.
  - `baseToolsOverride` — [`L461`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L461) — Override base tools (useful for custom runtimes).
  - `current` — [`L463`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L463)
  - `customTools` — [`L423`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L423) — SDK custom tools registered outside extensions
  - `cwd` — [`L415`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L415)
  - `extensionRunnerRef` — [`L463`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L463) — Mutable ref used by Agent to access the current ExtensionRunner
  - `includeCompactSkill` — [`L444`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L444) — Whether the bundled compact skill and its compact.* host handlers are
  - `includeGoals` — [`L435`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L435) — Whether the built-in long-running goals feature is available: the bundled
  - `initialActiveToolNames` — [`L427`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L427) — Initial active built-in tool names. Default: [ipython]
  - `initialGoal` — [`L500`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L500) — Initial goal to seed at session creation. Only applied when rlmDepth
  - `mcpManager` — [`L454`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L454) — Optional MCP integration manager. When present, its mcp.* host requests
  - `model` — [`L419`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L419)
  - `modelRegistry` — [`L425`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L425) — Model registry for API key resolution and model discovery
  - `objective` — [`L500`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L500)
  - `prewarmIpythonKernel` — [`L486`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L486) — Boot the IPython kernel in the background as soon as the session is created,
  - `resourceLoader` — [`L421`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L421) — Resource loader for skills, prompts, themes, context files, system prompt
  - `rlmDepth` — [`L467`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L467) — Current RLM recursion depth. Root sessions default to RLM_DEPTH or 0.
  - `rlmHeartbeatController` — [`L449`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L449) — Optional host-side controller for the bundled rlm-heartbeat Python skill.
  - `rlmMaxDepth` — [`L469`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L469) — Maximum RLM recursion depth. Defaults to RLM_MAX_DEPTH or 1.
  - `rlmParentAgent` — [`L475`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L475) — Parent agent name/id shown in child communication doctrine.
  - `rlmParentNodeId` — [`L473`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L473) — Node id for this session when it is itself an RLM child.
  - `rlmSessionDir` — [`L471`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L471) — Directory exposed to the kernel as RLM_SESSION_DIR.
  - `scopedModels` — [`L419`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L419) — Models to cycle through with Ctrl+P (from --models flag)
  - `serializedRefine` — [`L495`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L495) — When true, auto-refine runs synchronously between turns at the
  - `serviceTierPreference` — [`L414`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L414)
  - `sessionManager` — [`L412`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L412)
  - `sessionStartEvent` — [`L465`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L465) — Session start event metadata emitted when extensions bind to this runtime.
  - `settingsManager` — [`L413`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L413)
  - `subagentRuntimeHost` — [`L477`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L477) — Host responsible for creating RLM subagent runtimes.
  - `thinkingLevel` — [`L419`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L419)
  - `tokenBudget` — [`L500`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L500)
- uses (calls/refs, reference-scoped): [`Model`](../../../ai/src/types.ts.md#Model), [`SessionManager`](session-manager.ts.md#SessionManager), [`SettingsManager`](settings-manager.ts.md#SettingsManager), [`ModelRegistry`](model-registry.ts.md#ModelRegistry), [`ThinkingLevel`](../../../agent/src/types.ts.md#ThinkingLevel), [`AgentTool`](../../../agent/src/types.ts.md#AgentTool), [`ToolDefinition`](extensions/types.ts.md#ToolDefinition), [`ServiceTier`](../../../ai/src/types.ts.md#ServiceTier), [`AgentSessionMessageController`](agent-messages.ts.md#AgentSessionMessageController), [`ExtensionRunner`](extensions/runner.ts.md#ExtensionRunner), [`SubagentRuntimeHost`](rlm-runtime.ts.md#SubagentRuntimeHost), [`ResourceLoader`](resource-loader.ts.md#ResourceLoader), [`AgentObserveController`](agent-observe.ts.md#AgentObserveController), [`Agent`](../../../agent/src/agent.ts.md#Agent), [`AgentAutonomousConfig`](autonomous.ts.md#AgentAutonomousConfig), [`SessionStartEvent`](extensions/types.ts.md#SessionStartEvent), [`AutoRefineReviewer`](agent-session.ts.md#AutoRefineReviewer), [`AgentRlmHeartbeatController`](cron-jobs.ts.md#AgentRlmHeartbeatController), [`McpManager`](mcp/mcp-manager.ts.md#McpManager)  (1 test-only)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`createAgentSession`](sdk.ts.md#createAgentSession), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`_createInlineRlmSubagentRuntime`](agent-session.ts.md#AgentSession._createInlineRlmSubagentRuntime)  (11 test-only)

### `AgentSessionEvent`
- def: [`packages/coding-agent/src/core/agent-session.ts:319`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L319)
- doc: Session-specific events that extend the core AgentEvent
- signature: `type AgentSessionEvent`
- uses (calls/refs, reference-scoped): [`ThinkingLevel`](../../../agent/src/types.ts.md#ThinkingLevel), [`AgentEvent`](../../../agent/src/types.ts.md#AgentEvent), [`GoalState`](goals.ts.md#GoalState), [`ServiceTier`](../../../ai/src/types.ts.md#ServiceTier), [`RefinementResult`](refinement/refinement.ts.md#RefinementResult), [`KernelSentAgentMessage`](kernel/index.ts.md#KernelSentAgentMessage), [`AuthSourceToken`](auth-storage.ts.md#AuthSourceToken), [`CompactionResult`](compaction/compaction.ts.md#CompactionResult), [`SessionActionSnapshot`](session-action-store.ts.md#SessionActionSnapshot), [`CompactionReason`](agent-session.ts.md#CompactionReason), [`RlmChildAgentSnapshot`](agent-session.ts.md#RlmChildAgentSnapshot)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`daemon-agent-connection.ts`](../modes/agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`daemon-command.ts`](../cli/daemon-command.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-daemon-command.ts), [`telemetry.ts`](telemetry.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-telemetry.ts), [`_emit`](agent-session.ts.md#AgentSession._emit), [`handleSessionEvent`](../cli/daemon-command.ts.md#DaemonAttachTerminal.handleSessionEvent), [`observeStreamingMessage`](../modes/agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.observeStreamingMessage), [`assistantMessage`](telemetry.ts.md#assistantMessage), [`AgentSessionEventListener`](agent-session.ts.md#AgentSessionEventListener)  (11 test-only)

### `AgentSessionEventListener`
- def: [`packages/coding-agent/src/core/agent-session.ts:392`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L392)
- doc: Listener function for agent session events
- signature: `type AgentSessionEventListener`
- uses (calls/refs, reference-scoped): [`AgentSessionEvent`](agent-session.ts.md#AgentSessionEvent)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`subscribe`](agent-session.ts.md#AgentSession.subscribe), [`_eventListeners`](agent-session.ts.md#AgentSession._eventListeners)  (2 test-only)

### `AutoRefineReviewRequest`
- def: [`packages/coding-agent/src/core/agent-session.ts:510`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L510)
- signature: `interface AutoRefineReviewRequest`
- members:
  - `reason` — [`L511`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L511)
  - `turnsSinceLastReview` — [`L512`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L512)
- uses (calls/refs, reference-scoped): [`AutoRefineReason`](refinement/refinement.ts.md#AutoRefineReason)
- used by: [`_maybeAutoRefine`](agent-session.ts.md#AgentSession._maybeAutoRefine), [`_reviewAutoRefine`](agent-session.ts.md#AgentSession._reviewAutoRefine), [`_runSerializedAutoRefineReview`](agent-session.ts.md#AgentSession._runSerializedAutoRefineReview), [`_runBackgroundPlan`](agent-session.ts.md#AgentSession._runBackgroundPlan), [`AutoRefineReviewer`](agent-session.ts.md#AutoRefineReviewer)

### `AutoRefineReviewer`
- def: [`packages/coding-agent/src/core/agent-session.ts:542`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L542)
- signature: `type AutoRefineReviewer`
- uses (calls/refs, reference-scoped): [`AutoRefineReview`](refinement/refinement.ts.md#AutoRefineReview), [`AutoRefineReviewRequest`](agent-session.ts.md#AutoRefineReviewRequest)
- used by: [`_autoRefineReviewer`](agent-session.ts.md#AgentSession._autoRefineReviewer), [`autoRefineReviewer`](agent-session.ts.md#AgentSessionConfig.autoRefineReviewer)  (2 test-only)

### `AutonomousRuntimeSnapshot`
- def: [`packages/coding-agent/src/core/agent-session.ts:931`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L931)
- signature: `type AutonomousRuntimeSnapshot`
- uses (calls/refs, reference-scoped): [`AutonomousRuntimeState`](autonomous.ts.md#AutonomousRuntimeState)
- used by: [`_restoreAutonomousRuntimeSnapshot`](agent-session.ts.md#AgentSession._restoreAutonomousRuntimeSnapshot), [`_snapshotAutonomousRuntimeState`](agent-session.ts.md#AgentSession._snapshotAutonomousRuntimeState), [`_queuedAutonomousContinuationSnapshots`](agent-session.ts.md#AgentSession._queuedAutonomousContinuationSnapshots)

### `AutonomousSlashCommand`
- def: [`packages/coding-agent/src/core/agent-session.ts:921`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L921)
- signature: `type AutonomousSlashCommand`
- used by: [`_parseAutonomousSlashCommand`](agent-session.ts.md#AgentSession._parseAutonomousSlashCommand)

### `CommitPreparationPolicy`
- def: [`packages/coding-agent/src/core/agent-session.ts:607`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L607)
- signature: `interface CommitPreparationPolicy`
- members:
  - `awaitPendingModelSelection` — [`L611`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L611)
  - `finalRefineBarrier` — [`L613`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L613)
  - `flushPendingBashBeforeValidation` — [`L609`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L609)
  - `initialRefineBarrier` — [`L608`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L608)
  - `preTurnCompaction` — [`L612`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L612)
  - `validateModelAndAuth` — [`L610`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L610)
- uses (calls/refs, reference-scoped): [`RefineBarrierPolicy`](agent-session.ts.md#RefineBarrierPolicy), [`PreTurnCompactionTiming`](agent-session.ts.md#PreTurnCompactionTiming)
- used by: [`_prepareForCommit`](agent-session.ts.md#AgentSession._prepareForCommit), [`skipPrePromptWork`](agent-session.ts.md#AgentSession._turnExecutionPolicy.options-typeLiteral1740.skipPrePromptWork), [`turnExecutionPoliciesEqual`](agent-session.ts.md#turnExecutionPoliciesEqual), [`preparation`](agent-session.ts.md#TurnExecutionPolicy.preparation)

### `CommitPreparationSteps`
- def: [`packages/coding-agent/src/core/agent-session.ts:616`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L616)
- signature: `interface CommitPreparationSteps`
- members:
  - `afterValidation` — [`L617`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L617)
  - `beforeFinalRefineBarrier` — [`L620`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L620)
  - `commit` — [`L621`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L621)
  - `prepare` — [`L618`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L618)
  - `shouldCommit` — [`L619`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L619)
- used by: [`_startPreparedTurnActions`](agent-session.ts.md#AgentSession._startPreparedTurnActions), [`_prepareForCommit`](agent-session.ts.md#AgentSession._prepareForCommit)

### `CompactionReason`
- def: [`packages/coding-agent/src/core/agent-session.ts:316`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L316)
- signature: `type CompactionReason`
- used by: [`AgentSessionEvent`](agent-session.ts.md#AgentSessionEvent)

### `CompactionSkippedError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/core/agent-session.ts:404`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L404)
- doc: Thrown when compaction is skipped for a benign reason (surfaced as a warning, not an error)
- signature: `class CompactionSkippedError`
- used by: [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`compact`](agent-session.ts.md#AgentSession.compact), [`_runAutoCompaction`](agent-session.ts.md#AgentSession._runAutoCompaction), [`_executeQueuedSessionCommand`](agent-session.ts.md#AgentSession._executeQueuedSessionCommand)

### `DeferredSessionInputError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/core/agent-session.ts:675`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L675)
- signature: `class DeferredSessionInputError`
- used by: [`_startPreparedTurnActions`](agent-session.ts.md#AgentSession._startPreparedTurnActions), [`_isDeferredSessionInputError`](agent-session.ts.md#AgentSession._isDeferredSessionInputError)

### `ExtensionBindings`
- def: [`packages/coding-agent/src/core/agent-session.ts:503`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L503)
- signature: `interface ExtensionBindings`
- members:
  - `commandContextActions` — [`L505`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L505)
  - `onError` — [`L507`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L507)
  - `shutdownHandler` — [`L506`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L506)
  - `uiContext` — [`L504`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L504)
- uses (calls/refs, reference-scoped): [`ExtensionUIContext`](extensions/types.ts.md#ExtensionUIContext), [`ExtensionCommandContextActions`](extensions/types.ts.md#ExtensionCommandContextActions), [`ExtensionErrorListener`](extensions/runner.ts.md#ExtensionErrorListener), [`ShutdownHandler`](extensions/runner.ts.md#ShutdownHandler)
- used by: [`bindCurrentSessionExtensions`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.bindCurrentSessionExtensions), [`bindActiveSessionState`](../modes/daemon/daemon-extension-binding.ts.md#bindActiveSessionState), [`bindExtensions`](agent-session.ts.md#AgentSession.bindExtensions), [`bindCurrentSessionExtensions`](../modes/agent-connection/in-process-agent-connection.ts.md#InProcessAgentConnection.bindCurrentSessionExtensions), [`interactive-mode-services.ts`](../modes/interactive/interactive-mode-services.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode-services.ts), [`bindExtensions`](../modes/interactive/interactive-mode-services.ts.md#InteractiveModeLocalSessionHost.bindExtensions)  (4 test-only)

### `GoalSlashCommand`
- def: [`packages/coding-agent/src/core/agent-session.ts:914`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L914)
- signature: `type GoalSlashCommand`
- used by: [`_parseGoalSlashCommand`](agent-session.ts.md#AgentSession._parseGoalSlashCommand)

### `InternalPromptOptions`
- def: [`packages/coding-agent/src/core/agent-session.ts:577`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L577)
- signature: `interface InternalPromptOptions`
- members:
  - `agentMessageId` — [`L580`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L580)
  - `returnAfterAccepted` — [`L579`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L579)
  - `skipPrePromptWork` — [`L578`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L578)
- uses (calls/refs, reference-scoped): [`PromptOptions`](agent-session.ts.md#PromptOptions)
- used by: [`_prompt`](agent-session.ts.md#AgentSession._prompt), [`_promptInjectedMessage`](agent-session.ts.md#AgentSession._promptInjectedMessage)

### `ModelCycleResult`
- def: [`packages/coding-agent/src/core/agent-session.ts:897`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L897)
- doc: Result from cycleModel()
- signature: `interface ModelCycleResult`
- members:
  - `isScoped` — [`L902`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L902) — Whether cycling through scoped models (--models flag) or all available
  - `model` — [`L898`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L898)
  - `serviceTier` — [`L900`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L900)
  - `thinkingLevel` — [`L899`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L899)
- uses (calls/refs, reference-scoped): [`Model`](../../../ai/src/types.ts.md#Model), [`ThinkingLevel`](../../../agent/src/types.ts.md#ThinkingLevel), [`ServiceTier`](../../../ai/src/types.ts.md#ServiceTier)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`_cycleScopedModel`](agent-session.ts.md#AgentSession._cycleScopedModel), [`_cycleAvailableModel`](agent-session.ts.md#AgentSession._cycleAvailableModel), [`cycleModel`](agent-session.ts.md#AgentSession.cycleModel)  (3 test-only)

### `ModelSelectOptions`
- def: [`packages/coding-agent/src/core/agent-session.ts:905`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L905)
- signature: `interface ModelSelectOptions`
- members:
  - `waitForExtensions` — [`L906`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L906)
- used by: [`setModel`](agent-session.ts.md#AgentSession.setModel), [`_cycleScopedModel`](agent-session.ts.md#AgentSession._cycleScopedModel), [`_cycleAvailableModel`](agent-session.ts.md#AgentSession._cycleAvailableModel), [`cycleModel`](agent-session.ts.md#AgentSession.cycleModel), [`_shouldWaitForModelSelectEmit`](agent-session.ts.md#AgentSession._shouldWaitForModelSelectEmit)

### `NormalizedSubmission`
- def: [`packages/coding-agent/src/core/agent-session.ts:593`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L593)
- signature: `type NormalizedSubmission`
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../ai/src/types.ts.md#ImageContent), [`SessionSlashCommand`](slash-commands.ts.md#SessionSlashCommand)
- used by: [`_normalizeSubmission`](agent-session.ts.md#AgentSession._normalizeSubmission), [`_finishSubmissionNormalization`](agent-session.ts.md#AgentSession._finishSubmissionNormalization)

### `PersistedIpythonSentAgentMessage`
- def: [`packages/coding-agent/src/core/agent-session.ts:801`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L801)
- signature: `interface PersistedIpythonSentAgentMessage`
- members:
  - `message` — [`L803`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L803)
  - `toolCallId` — [`L802`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L802)
- uses (calls/refs, reference-scoped): [`KernelSentAgentMessage`](kernel/index.ts.md#KernelSentAgentMessage)
- used by: [`_restoreLateIpythonSentAgentMessages`](agent-session.ts.md#AgentSession._restoreLateIpythonSentAgentMessages), [`parsePersistedIpythonSentAgentMessage`](agent-session.ts.md#parsePersistedIpythonSentAgentMessage)

### `PersistedRlmMaxDepthState`
- def: [`packages/coding-agent/src/core/agent-session.ts:927`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L927)
- signature: `interface PersistedRlmMaxDepthState`
- members:
  - `maxDepth` — [`L928`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L928)
- used by: [`_loadPersistedRlmMaxDepthState`](agent-session.ts.md#AgentSession._loadPersistedRlmMaxDepthState), [`_resolveRlmMaxDepth`](agent-session.ts.md#AgentSession._resolveRlmMaxDepth), [`isPersistedRlmMaxDepthState`](agent-session.ts.md#isPersistedRlmMaxDepthState)

### `PreTurnCompactionTiming`
- def: [`packages/coding-agent/src/core/agent-session.ts:604`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L604)
- signature: `type PreTurnCompactionTiming`
- used by: [`preTurnCompaction`](agent-session.ts.md#CommitPreparationPolicy.preTurnCompaction)

### `PreparedCommandPayload`
- def: [`packages/coding-agent/src/core/agent-session.ts:663`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L663)
- signature: `interface PreparedCommandPayload`
- members:
  - `images` — [`L664`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L664)
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../ai/src/types.ts.md#ImageContent), [`SessionCommandPayload`](session-action-store.ts.md#SessionCommandPayload)
- used by: [`getSessionActionRecoverySnapshot`](agent-session.ts.md#AgentSession.getSessionActionRecoverySnapshot), [`restoreSessionActions`](agent-session.ts.md#AgentSession.restoreSessionActions), [`mutateQueuedMessage`](agent-session.ts.md#AgentSession.mutateQueuedMessage), [`_executeQueuedSessionCommand`](agent-session.ts.md#AgentSession._executeQueuedSessionCommand), [`source`](agent-session.ts.md#AgentSession._createSessionCommandAction.options-typeLiteral1777.source), [`QueuedSessionAction`](agent-session.ts.md#QueuedSessionAction)

### `PreparedPromptPreparation`
- def: [`packages/coding-agent/src/core/agent-session.ts:669`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L669)
- signature: `interface PreparedPromptPreparation`
- members:
  - `basePromptSnapshot` — [`L672`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L672) — Base system prompt captured at emitBeforeAgentStart, for stale-base refresh at handoff.
  - `result` — [`L670`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L670)
- uses (calls/refs, reference-scoped): [`emitBeforeAgentStart`](extensions/runner.ts.md#ExtensionRunner.emitBeforeAgentStart), [`ExtensionRunner`](extensions/runner.ts.md#ExtensionRunner)
- used by: [`_startPreparedTurnActions`](agent-session.ts.md#AgentSession._startPreparedTurnActions), [`_applyPreparedSystemPrompt`](agent-session.ts.md#AgentSession._applyPreparedSystemPrompt), [`prepared`](agent-session.ts.md#PreparedTurnPayload.prepared)

### `PreparedTurnPayload`
- def: [`packages/coding-agent/src/core/agent-session.ts:650`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L650)
- signature: `interface PreparedTurnPayload`
- members:
  - `acceptedAgentMessage` — [`L657`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L657)
  - `acceptedBeforeCompletion` — [`L658`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L658)
  - `cancelledDispatchEnded` — [`L660`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L660)
  - `captureRunMessages` — [`L659`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L659)
  - `content` — [`L652`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L652)
  - `customMessage` — [`L653`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L653)
  - `executionPolicy` — [`L655`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L655)
  - `images` — [`L651`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L651)
  - `prepared` — [`L654`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L654)
  - `queueVisible` — [`L656`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L656)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../agent/src/types.ts.md#AgentMessage), [`ImageContent`](../../../ai/src/types.ts.md#ImageContent), [`TextContent`](../../../ai/src/types.ts.md#TextContent), [`CustomMessage`](messages.ts.md#CustomMessage), [`TurnExecutionPolicy`](agent-session.ts.md#TurnExecutionPolicy), [`SessionTurnPayload`](session-action-store.ts.md#SessionTurnPayload), [`PreparedPromptPreparation`](agent-session.ts.md#PreparedPromptPreparation)
- used by: [`_processAgentEvent`](agent-session.ts.md#AgentSession._processAgentEvent), [`_startPreparedTurnActions`](agent-session.ts.md#AgentSession._startPreparedTurnActions), [`_pumpSessionInputs`](agent-session.ts.md#AgentSession._pumpSessionInputs), [`getSessionActionRecoverySnapshot`](agent-session.ts.md#AgentSession.getSessionActionRecoverySnapshot), [`acceptedBeforeCompletion`](agent-session.ts.md#AgentSession._createPreparedTurnAction.options-typeLiteral696.acceptedBeforeCompletion), [`restoreSessionActions`](agent-session.ts.md#AgentSession.restoreSessionActions), [`_cancelSessionActions`](agent-session.ts.md#AgentSession._cancelSessionActions), [`mutateQueuedMessage`](agent-session.ts.md#AgentSession.mutateQueuedMessage), [`_handleAgentEvent`](agent-session.ts.md#AgentSession._handleAgentEvent), [`clearQueue`](agent-session.ts.md#AgentSession.clearQueue), [`clearQueuedUserMessagesMatching`](agent-session.ts.md#AgentSession.clearQueuedUserMessagesMatching), [`requestAbort`](agent-session.ts.md#AgentSession.requestAbort), [`getPendingNextTurnMessageSnapshots`](agent-session.ts.md#AgentSession.getPendingNextTurnMessageSnapshots), [`_clearQueuedGoalContexts`](agent-session.ts.md#AgentSession._clearQueuedGoalContexts), [`source`](agent-session.ts.md#AgentSession._createSessionCommandAction.options-typeLiteral1777.source), [`queuedAgentMessagePreview`](agent-session.ts.md#queuedAgentMessagePreview), [`QueuedSessionAction`](agent-session.ts.md#QueuedSessionAction), [`_capturingCancelledAction`](agent-session.ts.md#AgentSession._capturingCancelledAction), [`visibleSessionActionProjection`](agent-session.ts.md#visibleSessionActionProjection), [`<get>hasAcceptedPromptInFlight`](agent-session.ts.md#AgentSession.-get-hasAcceptedPromptInFlight), [`_hasCancelledDispatchCapture`](agent-session.ts.md#AgentSession._hasCancelledDispatchCapture), [`_invalidateQueuedPromptPreparation`](agent-session.ts.md#AgentSession._invalidateQueuedPromptPreparation)

### `PromptOptions`
- def: [`packages/coding-agent/src/core/agent-session.ts:545`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L545)
- doc: Options for AgentSession.prompt()
- signature: `interface PromptOptions`
- members:
  - `admissionCommitted` — [`L571`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L571) — Internal host hook fired at the direct-turn ownership commit point.
  - `agentMessageId` — [`L572`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L572)
  - `content` — [`L573`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L573)
  - `customMessage` — [`L574`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L574)
  - `expandPromptTemplates` — [`L547`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L547) — Whether to expand file-based prompt templates (default: true)
  - `followUpQueueKey` — [`L553`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L553) — Coalesce follow-up queueing so only one pending follow-up exists for this key.
  - `images` — [`L549`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L549) — Image attachments
  - `internalPrompt` — [`L563`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L563) — Host-generated prompt that must bypass extension/slash/template input interception.
  - `preflightResult` — [`L557`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L557) — Internal hook used by RPC mode to observe prompt preflight acceptance or rejection.
  - `queueIfBusy` — [`L559`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L559) — Queue instead of starting immediately when the session is idle but already has queued work.
  - `resumeIfIdle` — [`L561`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L561) — Start queued work when no agent turn is currently running.
  - `signal` — [`L569`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L569) — Cancel this prompt while it is waiting for direct-turn admission.
  - `skipInputHandlers` — [`L567`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L567) — Skip extension input handlers for replaying already-accepted input.
  - `source` — [`L555`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L555) — Source of input for extension input event handlers. Defaults to "interactive".
  - `streamingBehavior` — [`L551`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L551) — When streaming, how to queue the message: "steer" (interrupt) or "followUp" (wait). Required if streaming.
  - `suppressAutonomousContinuation` — [`L565`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L565) — Prevent host-driven prompts from causing autonomous continuation injection.
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../ai/src/types.ts.md#ImageContent), [`TextContent`](../../../ai/src/types.ts.md#TextContent), [`CustomMessage`](messages.ts.md#CustomMessage), [`InputSource`](extensions/types.ts.md#InputSource)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`handleCommand`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.handleCommand), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`prompt`](agent-session.ts.md#AgentSession.prompt), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`_prompt`](agent-session.ts.md#AgentSession._prompt), [`_promptInjectedMessage`](agent-session.ts.md#AgentSession._promptInjectedMessage), [`status`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.acceptAgentSessionMessage.Promise.typeLiteral2954.status), [`acceptAgentMessagePrompt`](agent-session.ts.md#AgentSession.acceptAgentMessagePrompt), [`promptAndWait`](agent-session.ts.md#AgentSession.promptAndWait), [`promptWithAgentMessagePreparingGuard`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.promptWithAgentMessagePreparingGuard), [`promptHeartbeat`](agent-session.ts.md#AgentSession.promptHeartbeat), [`promptHeartbeatWithAgentMessagePreparingGuard`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.promptHeartbeatWithAgentMessagePreparingGuard), [`promptUntilAccepted`](agent-session.ts.md#AgentSession.promptUntilAccepted), [`InternalPromptOptions`](agent-session.ts.md#InternalPromptOptions)  (1 test-only)

### `QueuedAgentMessage`
- def: [`packages/coding-agent/src/core/agent-session.ts:624`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L624)
- signature: `type QueuedAgentMessage`
- uses (calls/refs, reference-scoped): [`CustomMessage`](messages.ts.md#CustomMessage), [`UserMessage`](../../../ai/src/types.ts.md#UserMessage)
- used by: [`_createDeliveryRecord`](agent-session.ts.md#AgentSession._createDeliveryRecord), [`cloneQueuedAgentMessage`](agent-session.ts.md#cloneQueuedAgentMessage), [`message`](agent-session.ts.md#AgentSession._createPreparedTurnAction.options-typeLiteral696.message), [`message`](agent-session.ts.md#SessionActionRecoveryRecord.message), [`message`](agent-session.ts.md#AgentSession._queuePreparedPrompt.options-typeLiteral1804.message)

### `QueuedSessionAction`
- def: [`packages/coding-agent/src/core/agent-session.ts:667`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L667)
- signature: `type QueuedSessionAction`
- uses (calls/refs, reference-scoped): [`SessionAction`](session-action-store.ts.md#SessionAction), [`PreparedTurnPayload`](agent-session.ts.md#PreparedTurnPayload), [`PreparedCommandPayload`](agent-session.ts.md#PreparedCommandPayload)
- used by: [`_startPreparedTurnActions`](agent-session.ts.md#AgentSession._startPreparedTurnActions), [`_pumpSessionInputs`](agent-session.ts.md#AgentSession._pumpSessionInputs), [`acceptedBeforeCompletion`](agent-session.ts.md#AgentSession._createPreparedTurnAction.options-typeLiteral696.acceptedBeforeCompletion), [`restoreSessionActions`](agent-session.ts.md#AgentSession.restoreSessionActions), [`_cancelSessionActions`](agent-session.ts.md#AgentSession._cancelSessionActions), [`_executeSelectedSessionCommand`](agent-session.ts.md#AgentSession._executeSelectedSessionCommand), [`_actionStore`](agent-session.ts.md#AgentSession._actionStore), [`_executeQueuedSessionCommand`](agent-session.ts.md#AgentSession._executeQueuedSessionCommand), [`source`](agent-session.ts.md#AgentSession._createSessionCommandAction.options-typeLiteral1777.source), [`primaryDeliveryRecord`](agent-session.ts.md#primaryDeliveryRecord), [`queuedAgentMessagePreview`](agent-session.ts.md#queuedAgentMessagePreview), [`_capturingCancelledAction`](agent-session.ts.md#AgentSession._capturingCancelledAction), [`visibleSessionActionProjection`](agent-session.ts.md#visibleSessionActionProjection), [`_coalescedFollowUpOwner`](agent-session.ts.md#AgentSession._coalescedFollowUpOwner), [`_observeSessionActionDeferral`](agent-session.ts.md#AgentSession._observeSessionActionDeferral), [`_admitSessionInput`](agent-session.ts.md#AgentSession._admitSessionInput)

### `RefineBarrierPolicy`
- def: [`packages/coding-agent/src/core/agent-session.ts:605`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L605)
- signature: `type RefineBarrierPolicy`
- used by: [`finalRefineBarrier`](agent-session.ts.md#CommitPreparationPolicy.finalRefineBarrier), [`initialRefineBarrier`](agent-session.ts.md#CommitPreparationPolicy.initialRefineBarrier)

### `RestoredPromptInput`
- def: [`packages/coding-agent/src/core/agent-session.ts:690`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L690)
- signature: `interface RestoredPromptInput`
- members:
  - `agentMessageId` — [`L695`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L695)
  - `content` — [`L692`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L692)
  - `customMessage` — [`L696`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L696)
  - `images` — [`L693`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L693)
  - `prefixMessages` — [`L697`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L697)
  - `queueKey` — [`L694`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L694)
  - `text` — [`L691`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L691)
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../ai/src/types.ts.md#ImageContent), [`TextContent`](../../../ai/src/types.ts.md#TextContent), [`CustomMessage`](messages.ts.md#CustomMessage)
- used by: [`prefixMessages`](agent-session.ts.md#AgentSession.restoreFollowUpMessage.options-typeLiteral1730.prefixMessages), [`prefixMessages`](agent-session.ts.md#AgentSession.restoreSteeringMessage.options-typeLiteral1729.prefixMessages), [`_restorePromptInput`](agent-session.ts.md#AgentSession._restorePromptInput)

### `RlmChildAgentActivity`
- def: [`packages/coding-agent/src/core/agent-session.ts:285`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L285)
- signature: `interface RlmChildAgentActivity`
- members:
  - `kind` — [`L286`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L286)
  - `toolName` — [`L287`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L287)
- used by: [`_startRlmChildRun`](agent-session.ts.md#AgentSession._startRlmChildRun), [`activity`](agent-session.ts.md#RlmChildAgentSnapshot.activity)

### `RlmChildAgentSnapshot`
- def: [`packages/coding-agent/src/core/agent-session.ts:290`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L290)
- signature: `interface RlmChildAgentSnapshot`
- members:
  - `activeSessionId` — [`L293`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L293)
  - `activity` — [`L309`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L309)
  - `answerPreview` — [`L301`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L301)
  - `durationMs` — [`L300`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L300)
  - `error` — [`L313`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L313) — Failure reason when status is "error".
  - `id` — [`L291`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L291)
  - `label` — [`L298`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L298)
  - `model` — [`L297`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L297) — Exact provider/model selector used by the child.
  - `parentId` — [`L292`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L292)
  - `recap` — [`L307`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L307) — Latest recap of what the subagent is doing, from the summarizer.
  - `repliedSinceTask` — [`L311`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L311) — Child sent at least one explicit agent message since task admission.
  - `sessionDir` — [`L308`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L308)
  - `sessionName` — [`L295`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L295) — Stable daemon-visible session name for addressing/displaying the child.
  - `status` — [`L299`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L299)
  - `tokenCount` — [`L305`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L305) — Context size (tokens) of the subagent's latest turn.
  - `toolUseCount` — [`L303`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L303) — Number of tool executions the subagent has started so far.
- uses (calls/refs, reference-scoped): [`RlmChildAgentStatus`](agent-session.ts.md#RlmChildAgentStatus), [`RlmChildAgentActivity`](agent-session.ts.md#RlmChildAgentActivity)
- used by: [`_startRlmChildRun`](agent-session.ts.md#AgentSession._startRlmChildRun), [`AgentSessionEvent`](agent-session.ts.md#AgentSessionEvent), [`_emitRlmSubagentRemoval`](agent-session.ts.md#AgentSession._emitRlmSubagentRemoval), [`handleSessionEvent`](../cli/daemon-command.ts.md#DaemonAttachTerminal.handleSessionEvent)  (1 test-only)

### `RlmChildAgentStatus`
- def: [`packages/coding-agent/src/core/agent-session.ts:283`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L283)
- signature: `type RlmChildAgentStatus`
- used by: [`context-tree.ts`](context-tree.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-context-tree.ts), [`status`](agent-session.ts.md#RlmChildRun.status), [`status`](context-tree.ts.md#ContextTreeNode.status), [`getRlmChildRunStatus`](agent-session.ts.md#AgentSession.getRlmChildRunStatus), [`status`](agent-session.ts.md#RlmChildAgentSnapshot.status)

### `RlmChildRun`
- def: [`packages/coding-agent/src/core/agent-session.ts:936`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L936)
- signature: `interface RlmChildRun`
- members:
  - `abort` — [`L943`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L943)
  - `detachedDeletion` — [`L950`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L950) — Selector snapshot for a delete admitted while runtime startup was still pending.
  - `emitUpdate` — [`L952`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L952) — Re-emits the run's rlm_child_update snapshot with its current status.
  - `error` — [`L942`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L942)
  - `id` — [`L937`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L937)
  - `prompt` — [`L938`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L938)
  - `publication` — [`L944`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L944)
  - `session` — [`L946`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L946) — Child session, once its runtime exists. Used to cancel nested child runs.
  - `sessionDir` — [`L940`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L940)
  - `sessionName` — [`L939`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L939)
  - `settled` — [`L948`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L948) — True once the detached run task has finished its catch and cleanup paths.
  - `status` — [`L941`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L941)
  - `unsubscribe` — [`L954`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L954) — Idempotent child-event forwarder cleanup, once the child runtime exists.
- uses (calls/refs, reference-scoped): [`AgentSession`](agent-session.ts.md#AgentSession), [`RlmSubagentRegistryEntry`](rlm-runtime.ts.md#RlmSubagentRegistryEntry), [`AgentMessageDeferred`](agent-session.ts.md#AgentMessageDeferred), [`RlmChildAgentStatus`](agent-session.ts.md#RlmChildAgentStatus)
- used by: [`_startRlmChildRun`](agent-session.ts.md#AgentSession._startRlmChildRun), [`_buildRlmSubagentList`](agent-session.ts.md#AgentSession._buildRlmSubagentList), [`getContextTree`](agent-session.ts.md#AgentSession.getContextTree), [`_assertRlmSubagentSessionNameAvailable`](agent-session.ts.md#AgentSession._assertRlmSubagentSessionNameAvailable), [`_deleteResolvedRlmSubagent`](agent-session.ts.md#AgentSession._deleteResolvedRlmSubagent), [`getRlmChildSession`](agent-session.ts.md#AgentSession.getRlmChildSession), [`deleteInactiveRlmSubagent`](agent-session.ts.md#AgentSession.deleteInactiveRlmSubagent), [`_removeRlmSubagentTracking`](agent-session.ts.md#AgentSession._removeRlmSubagentTracking), [`_disposeAsyncOnce`](agent-session.ts.md#AgentSession._disposeAsyncOnce), [`_activeRlmChildRuns`](agent-session.ts.md#AgentSession._activeRlmChildRuns), [`releaseRlmChildSession`](agent-session.ts.md#AgentSession.releaseRlmChildSession), [`_awaitPendingRlmChildPublication`](agent-session.ts.md#AgentSession._awaitPendingRlmChildPublication), [`cancelRlmChildRun`](agent-session.ts.md#AgentSession.cancelRlmChildRun), [`_cancelRlmChildRun`](agent-session.ts.md#AgentSession._cancelRlmChildRun), [`hasRunningRlmChildren`](agent-session.ts.md#AgentSession.hasRunningRlmChildren), [`getRlmChildRunStatus`](agent-session.ts.md#AgentSession.getRlmChildRunStatus), [`_reapDeletedRlmSubagentRuntimesAfterCompaction`](agent-session.ts.md#AgentSession._reapDeletedRlmSubagentRuntimesAfterCompaction)

### `RlmSubagentModelSelection`
- def: [`packages/coding-agent/src/core/agent-session.ts:957`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L957)
- signature: `interface RlmSubagentModelSelection`
- members:
  - `model` — [`L958`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L958)
- uses (calls/refs, reference-scoped): [`Model`](../../../ai/src/types.ts.md#Model), [`Api`](../../../ai/src/types.ts.md#Api)
- used by: [`_startRlmChildRun`](agent-session.ts.md#AgentSession._startRlmChildRun), [`_resolveRlmSubagentModel`](agent-session.ts.md#AgentSession._resolveRlmSubagentModel)

### `SerializedBackgroundPlanResult`
- def: [`packages/coding-agent/src/core/agent-session.ts:523`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L523)
- doc: Discriminated result from a serialized-mode background planning pass.
- signature: `type SerializedBackgroundPlanResult`
- uses (calls/refs, reference-scoped): [`RefinementPlan`](refinement/refinement.ts.md#RefinementPlan)
- used by: [`_runBackgroundPlan`](agent-session.ts.md#AgentSession._runBackgroundPlan), [`_serializedPlanInFlight`](agent-session.ts.md#AgentSession._serializedPlanInFlight), [`_consumeSerializedBackgroundPlan`](agent-session.ts.md#AgentSession._consumeSerializedBackgroundPlan), [`_applySerializedPlan`](agent-session.ts.md#AgentSession._applySerializedPlan)

### `SessionActionRecoveryAction`
- def: [`packages/coding-agent/src/core/agent-session.ts:730`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L730)
- signature: `interface SessionActionRecoveryAction`
- members:
  - `agentMessageId` — [`L737`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L737)
  - `delivery` — [`L733`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L733)
  - `id` — [`L731`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L731)
  - `payload` — [`L735`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L735)
  - `queueKey` — [`L736`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L736)
  - `source` — [`L732`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L732)
  - `suppressAutonomousContinuation` — [`L738`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L738)
  - `wake` — [`L734`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L734)
- uses (calls/refs, reference-scoped): [`InputSource`](extensions/types.ts.md#InputSource), [`DeliveryPolicy`](session-action-store.ts.md#DeliveryPolicy), [`SessionActionRecoveryPayload`](agent-session.ts.md#SessionActionRecoveryPayload), [`WakePolicy`](session-action-store.ts.md#WakePolicy)
- used by: [`restoreSessionActions`](agent-session.ts.md#AgentSession.restoreSessionActions), [`restoreDaemonUpdateRestartSession`](../package-manager-cli.ts.md#restoreDaemonUpdateRestartSession), [`SessionActionRecoverySnapshot`](agent-session.ts.md#SessionActionRecoverySnapshot)  (5 test-only)

### `SessionActionRecoveryPayload`
- def: [`packages/coding-agent/src/core/agent-session.ts:709`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L709)
- signature: `type SessionActionRecoveryPayload`
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../ai/src/types.ts.md#ImageContent), [`TextContent`](../../../ai/src/types.ts.md#TextContent), [`CustomMessage`](messages.ts.md#CustomMessage), [`SessionSlashCommand`](slash-commands.ts.md#SessionSlashCommand), [`TurnExecutionPolicy`](agent-session.ts.md#TurnExecutionPolicy), [`SessionActionRecoveryRecord`](agent-session.ts.md#SessionActionRecoveryRecord)
- used by: [`payload`](agent-session.ts.md#SessionActionRecoveryAction.payload)

### `SessionActionRecoveryRecord`
- def: [`packages/coding-agent/src/core/agent-session.ts:702`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L702)
- signature: `interface SessionActionRecoveryRecord`
- members:
  - `id` — [`L703`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L703)
  - `message` — [`L705`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L705)
  - `ownerActionId` — [`L706`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L706)
  - `role` — [`L704`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L704)
- uses (calls/refs, reference-scoped): [`role`](session-action-store.ts.md#DeliveryRecord.role), [`QueuedAgentMessage`](agent-session.ts.md#QueuedAgentMessage), [`DeliveryRecord`](session-action-store.ts.md#DeliveryRecord)
- used by: [`restoreSessionActions`](agent-session.ts.md#AgentSession.restoreSessionActions), [`SessionActionRecoveryPayload`](agent-session.ts.md#SessionActionRecoveryPayload)  (2 test-only)

### `SessionActionRecoverySnapshot`
- def: [`packages/coding-agent/src/core/agent-session.ts:741`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L741)
- signature: `interface SessionActionRecoverySnapshot`
- members:
  - `actions` — [`L743`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L743)
  - `formatVersion` — [`L742`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L742)
- uses (calls/refs, reference-scoped): [`SESSION_ACTION_RECOVERY_FORMAT_VERSION`](agent-session.ts.md#SESSION_ACTION_RECOVERY_FORMAT_VERSION), [`SessionActionRecoveryAction`](agent-session.ts.md#SessionActionRecoveryAction)
- used by: [`DaemonCommand`](../modes/daemon/daemon-protocol.ts.md#DaemonCommand), [`package-manager-cli.ts`](../package-manager-cli.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-package-manager-cli.ts), [`daemon-protocol.ts`](../modes/daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`getSessionActionRecoverySnapshot`](agent-session.ts.md#AgentSession.getSessionActionRecoverySnapshot), [`restoreSessionActions`](agent-session.ts.md#AgentSession.restoreSessionActions), [`restoreDaemonUpdateRestartSession`](../package-manager-cli.ts.md#restoreDaemonUpdateRestartSession), [`createUpdateRestartSession`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createUpdateRestartSession), [`isSessionActionRecoveryAction`](../package-manager-cli.ts.md#isSessionActionRecoveryAction), [`parseSessionActionRecoverySnapshot`](../package-manager-cli.ts.md#parseSessionActionRecoverySnapshot), [`actions`](../modes/daemon/daemon-protocol.ts.md#DaemonUpdateRestartQueue.actions)  (8 test-only)

### `SessionInputSchedule`
- def: [`packages/coding-agent/src/core/agent-session.ts:625`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L625)
- signature: `type SessionInputSchedule`
- used by: [`_restorePromptInput`](agent-session.ts.md#AgentSession._restorePromptInput), [`_restoreSessionCommand`](agent-session.ts.md#AgentSession._restoreSessionCommand), [`_queuePreparedPrompt`](agent-session.ts.md#AgentSession._queuePreparedPrompt), [`_createPreparedTurnAction`](agent-session.ts.md#AgentSession._createPreparedTurnAction), [`_createSessionCommandAction`](agent-session.ts.md#AgentSession._createSessionCommandAction), [`_deliveryPolicy`](agent-session.ts.md#AgentSession._deliveryPolicy)

### `SubmissionExtensionCommandPolicy`
- def: [`packages/coding-agent/src/core/agent-session.ts:583`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L583)
- signature: `type SubmissionExtensionCommandPolicy`
- used by: [`extensionCommands`](agent-session.ts.md#SubmissionNormalizationPolicy.extensionCommands)

### `SubmissionNormalizationPolicy`
- def: [`packages/coding-agent/src/core/agent-session.ts:585`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L585)
- signature: `interface SubmissionNormalizationPolicy`
- members:
  - `expandPromptTemplates` — [`L590`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L590)
  - `expandSkills` — [`L589`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L589)
  - `extensionCommands` — [`L587`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L587)
  - `inputSource` — [`L588`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L588)
  - `parseSessionCommands` — [`L586`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L586)
- uses (calls/refs, reference-scoped): [`InputSource`](extensions/types.ts.md#InputSource), [`SubmissionExtensionCommandPolicy`](agent-session.ts.md#SubmissionExtensionCommandPolicy)
- used by: [`_prompt`](agent-session.ts.md#AgentSession._prompt), [`steer`](agent-session.ts.md#AgentSession.steer), [`_normalizeSubmission`](agent-session.ts.md#AgentSession._normalizeSubmission), [`resumeIfIdle`](agent-session.ts.md#AgentSession.followUp.options-typeLiteral1689.resumeIfIdle), [`_finishSubmissionNormalization`](agent-session.ts.md#AgentSession._finishSubmissionNormalization)

### `ToolDefinitionEntry`
- def: [`packages/coding-agent/src/core/agent-session.ts:909`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L909)
- signature: `interface ToolDefinitionEntry`
- members:
  - `definition` — [`L910`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L910)
  - `sourceInfo` — [`L911`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L911)
- uses (calls/refs, reference-scoped): [`ToolDefinition`](extensions/types.ts.md#ToolDefinition), [`SourceInfo`](source-info.ts.md#SourceInfo)
- used by: [`_refreshToolRegistry`](agent-session.ts.md#AgentSession._refreshToolRegistry), [`getAllTools`](agent-session.ts.md#AgentSession.getAllTools), [`getToolDefinition`](agent-session.ts.md#AgentSession.getToolDefinition), [`_toolDefinitions`](agent-session.ts.md#AgentSession._toolDefinitions)

### `TurnExecutionPolicy`
- def: [`packages/coding-agent/src/core/agent-session.ts:627`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L627)
- signature: `interface TurnExecutionPolicy`
- members:
  - `completionIncludesRetryChain` — [`L632`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L632)
  - `nextTurnContextTiming` — [`L630`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L630)
  - `preparation` — [`L628`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L628)
  - `preserveEmptyExtensionPrompt` — [`L631`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L631)
  - `runBeforeAgentStart` — [`L629`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L629)
- uses (calls/refs, reference-scoped): [`CommitPreparationPolicy`](agent-session.ts.md#CommitPreparationPolicy)
- used by: [`_startPreparedTurnActions`](agent-session.ts.md#AgentSession._startPreparedTurnActions), [`getSessionActionRecoverySnapshot`](agent-session.ts.md#AgentSession.getSessionActionRecoverySnapshot), [`_promptInjectedMessage`](agent-session.ts.md#AgentSession._promptInjectedMessage), [`restoreSessionActions`](agent-session.ts.md#AgentSession.restoreSessionActions), [`skipPrePromptWork`](agent-session.ts.md#AgentSession._turnExecutionPolicy.options-typeLiteral1740.skipPrePromptWork), [`turnExecutionPoliciesEqual`](agent-session.ts.md#turnExecutionPoliciesEqual), [`SessionActionRecoveryPayload`](agent-session.ts.md#SessionActionRecoveryPayload), [`executionPolicy`](agent-session.ts.md#PreparedTurnPayload.executionPolicy), [`executionPolicy`](agent-session.ts.md#AgentSession._createPreparedTurnAction.options-typeLiteral696.executionPolicy)

### `UserBashEndDetails`
- def: [`packages/coding-agent/src/core/agent-session.ts:395`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L395)
- doc: Payload of the bash_end event for a user-initiated bash command
- signature: `type UserBashEndDetails`
- members:
  - `cancelled` — [`L397`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L397)
  - `errorMessage` — [`L400`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L400)
  - `exitCode` — [`L396`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L396)
  - `fullOutputPath` — [`L399`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L399)
  - `truncated` — [`L398`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L398)
- used by: [`runUserBashLocked`](agent-session.ts.md#AgentSession.runUserBashLocked), [`runId`](agent-session.ts.md#AgentSession.runUserBash.options-typeLiteral4141.runId)

## Functions
- `appendSentAgentMessageToToolResult(message: AgentMessage, toolCallId: string, sentMessage: KernelSentAgentMessage)` — [`L840`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L840)
- `attributeChildUsage(parentUsage: Usage, childUsage: Usage)` — [`L1069`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1069)
- `autoRefineInstructions(reason: AutoRefineReason, review: AutoRefineReview)` — [`L975`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L975)
- `cloneCustomMessage(message: CustomMessage<unknown>)` — [`L746`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L746)
- `cloneQueuedAgentMessage(message: QueuedAgentMessage)` — [`L753`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L753)
- `compactRlmText(text: string, maxLength?: number)` — [`L1018`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1018)
- `createAgentMessageDeferred()` — [`L886`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L886)
- `injectedMessagePreviewLabel(message: CustomMessage<unknown>)` — [`L860`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L860)
- `isNonNegativeInteger(value: unknown)` — [`L983`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L983)
- `isObjectRecord(value: unknown)` — [`L806`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L806)
- `isPersistedRlmMaxDepthState(value: unknown)` — [`L1001`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1001)
- `isRlmHeartbeatStatusUpdate(value: unknown)` — [`L11269`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L11269)
- `noopRlmChildAbort()` — [`L972`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L972)
- `noopRlmChildEventUnsubscribe()` — [`L973`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L973)
- `normalizeMessageContent(content: string | (TextContent | ImageContent)[])` — [`L768`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L768)
- `oncePreflight(preflightResult: ((success: boolean, queued?: boolean | undefined) => void) | undefined)` — [`L678`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L678) — Wrap a preflight callback so only the first report wins.
- `parseDepth(value: string | undefined, fallback: number, name: string)` — [`L987`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L987)
- `parseGoalBudgetValue(value: string)` — [`L1007`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1007)
- `parsePersistedIpythonSentAgentMessage(value: unknown)` — [`L810`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L810)
- `primaryDeliveryRecord(action: QueuedSessionAction)` — [`L761`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L761)
- `queuedAgentMessagePreview(action: QueuedSessionAction)` — [`L781`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L781)
- `readAssistantText(message: AssistantMessage)` — [`L1033`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1033)
- `rlmChildLabel(prompt: string)` — [`L1029`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1029)
- `rlmHeartbeatHostResponse(job: AgentCronJob)` — [`L11273`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L11273)
- `turnExecutionPoliciesEqual(left: TurnExecutionPolicy, right: TurnExecutionPolicy)` — [`L635`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L635)
- `visibleSessionActionProjection(actions: readonly QueuedSessionAction[])` — [`L790`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L790)
- `waitForPromiseOrAbort(promise: Promise<T>, signal: AbortSignal | undefined, abortMessage: string)` — [`L1040`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L1040)

## Module values
- `IPYTHON_SENT_AGENT_MESSAGE_CUSTOM_ENTRY` — [`L799`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L799)
- `KERNEL_STATE_LISTING_TIMEOUT_MS` — [`L969`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L969) — Cap on the post-compaction kernel namespace probe so a wedged kernel can't stall recovery.
- `RLM_MAX_DEPTH_STATE_CUSTOM_TYPE` — [`L970`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L970)
- `SESSION_ACTION_RECOVERY_FORMAT_VERSION` — [`L700`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L700)
- `THINKING_LEVELS` — [`L966`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L966) — Standard thinking levels
- `images` — [`L770`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L770)
- `text` — [`L769`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-session.ts#L769)


---
title: 'Module: packages/coding-agent/src/modes/agent-connection/types.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/agent-connection/types.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/agent-connection/`types.ts`/AgentConnection
symbols:
  AgentConnectionModel: Model#
  AgentConnectionSessionTreeFlatNode.entry: SessionTreeFlatNode#entry.
  AgentConnectionSessionEntryBase.id: SessionEntryBase#id.
  AgentConnectionSessionEvent: SessionEvent#
  AgentConnectionHeartbeat: Heartbeat#
  AgentConnectionHeartbeat.job: Heartbeat#job.
  AgentConnectionState: State#
  AgentConnectionEvent: Event#
  AgentConnectionSourceInfo: SourceInfo#
  AgentConnectionRlmChildAgentSnapshot: RlmChildAgentSnapshot#
  AgentConnectionSessionEntry: SessionEntry#
  AgentConnectionSessionTreeNode: SessionTreeNode#
  AgentConnectionState.sessionId: State#sessionId.
  AgentConnectionSideQuestionEvent.id: SideQuestionEvent#id.
  AgentConnection: '#'
  AgentConnectionSavedSessionInfo: SavedSessionInfo#
  AgentConnectionSideQuestionEvent.status: SideQuestionEvent#status.
  AgentConnectionSnapshot: Snapshot#
  AgentConnectionQueueState: QueueState#
  AgentConnectionSnapshot.state: Snapshot#state.
  AgentConnectionSessionContext: SessionContext#
  AgentConnectionSideQuestionEvent.answer: SideQuestionEvent#answer.
  AgentConnectionRlmChildAgentSnapshot.status: RlmChildAgentSnapshot#status.
  AgentConnectionModelCatalog: ModelCatalog#
  AgentConnectionSideQuestionEvent.question: SideQuestionEvent#question.
  AgentConnectionRlmChildAgentSnapshot.id: RlmChildAgentSnapshot#id.
  AgentConnectionState.activeSessionId: State#activeSessionId.
  AgentConnectionExtensionUiResponse: ExtensionUiResponse#
  AgentConnection.getState: '#getState().'
  AgentConnectionState.thinkingLevel: State#thinkingLevel.
  AgentConnectionSessionMessageEntry.type: SessionMessageEntry#type.
  AgentConnectionState.sessionFile: State#sessionFile.
  AgentConnectionResourceSnapshot: ResourceSnapshot#
  AgentConnectionRlmChildAgentSnapshot.activeSessionId: RlmChildAgentSnapshot#activeSessionId.
  AgentConnectionState.serviceTier: State#serviceTier.
  AgentConnectionState.scopedModels: State#scopedModels.
  AgentConnectionResourceDiagnostic: ResourceDiagnostic#
  AgentConnectionSessionEntryBase.parentId: SessionEntryBase#parentId.
  AgentConnectionSideQuestionEvent: SideQuestionEvent#
  AgentConnectionQueueState.steering: QueueState#steering.
  AgentConnectionSnapshot.messages: Snapshot#messages.
  AgentConnectionState.model: State#model.
  AgentConnectionEventListener: EventListener#
  AgentConnectionSessionEntryBase: SessionEntryBase#
  AgentConnectionState.contextUsage: State#contextUsage.
  AgentConnectionSlashCommand: SlashCommand#
  AgentConnectionQueueState.followUp: QueueState#followUp.
  AgentConnection.mutateQueuedMessage: '#mutateQueuedMessage().'
  AgentConnectionQueueMode: QueueMode#
  AgentConnectionCompactionEntry.type: CompactionEntry#type.
  AgentConnectionBranchSummaryEntry.type: BranchSummaryEntry#type.
  AgentConnectionCustomMessageEntry.type: CustomMessageEntry#type.
  AgentConnectionSessionStateEntry.type: SessionStateEntry#type.
  AgentConnectionAgentStatusEntry.type: AgentStatusEntry#type.
  AgentConnectionGitStateEntry.type: GitStateEntry#type.
  AgentConnectionSlashCommand.name: SlashCommand#name.
  AgentConnectionToolDefinition: ToolDefinition#
  AgentConnection.updateHeartbeat: '#updateHeartbeat().'
  AgentConnectionSnapshot.streamingMessage: Snapshot#streamingMessage.
  AgentConnectionChildUsageAttributionEntry.type: ChildUsageAttributionEntry#type.
  AgentConnectionState.isStreaming: State#isStreaming.
  AgentConnectionSessionContext.messages: SessionContext#messages.
  AgentConnectionScopedModel.model: ScopedModel#model.
  AgentConnection.getMessages: '#getMessages().'
  AgentConnection.listSavedSessions: '#listSavedSessions().'
  AgentConnection.respondToExtensionUiRequest: '#respondToExtensionUiRequest().'
  AgentConnection.fork: '#fork().'
  AgentConnectionServiceTierChangeEntry.type: ServiceTierChangeEntry#type.
  AgentConnectionSessionInfoEntry.type: SessionInfoEntry#type.
  AgentConnectionState.isBashRunning: State#isBashRunning.
  AgentConnectionExtensionUiRequest: ExtensionUiRequest#
  AgentConnection.manageHeartbeat: '#manageHeartbeat().'
  AgentConnection.setHeartbeat: '#setHeartbeat().'
  AgentConnection.navigateTree: '#navigateTree().'
  AgentConnectionScopedModel: ScopedModel#
  AgentConnectionState.heartbeat: State#heartbeat.
  AgentConnectionQueuedMessageMutationStatus: QueuedMessageMutationStatus#
  AgentConnection.subscribe: '#subscribe().'
  AgentConnection.getSessionStats: '#getSessionStats().'
  AgentConnection.prompt: '#prompt().'
  AgentConnectionSavedSessionScope: SavedSessionScope#
  AgentConnectionSessionMessageEntry: SessionMessageEntry#
  AgentConnectionSessionMessageEntry.message: SessionMessageEntry#message.
  AgentConnectionCustomMessageEntry.content: CustomMessageEntry#content.
  AgentConnectionExtensionUiRequest.method: ExtensionUiRequest#method.
  AgentConnection.dispose: '#dispose().'
  AgentConnectionModelCatalog.models: ModelCatalog#models.
  AgentConnectionSessionListCallbacks: SessionListCallbacks#
  AgentConnectionState.availableThinkingLevels: State#availableThinkingLevels.
  AgentConnectionState.sessionActions: State#sessionActions.
  AgentConnection.getCommands: '#getCommands().'
  AgentConnection.promptAndWait: '#promptAndWait().'
  AgentConnection.setThinkingLevel: '#setThinkingLevel().'
  AgentConnection.newSession: '#newSession().'
  AgentConnection.switchSession: '#switchSession().'
  AgentConnectionThinkingLevelChangeEntry.type: ThinkingLevelChangeEntry#type.
  AgentConnectionModelChangeEntry.type: ModelChangeEntry#type.
  AgentConnectionArtifactReference: ArtifactReference#
  AgentConnectionPromptOptions: PromptOptions#
  AgentConnectionExtensionUiRequest.id: ExtensionUiRequest#id.
  AgentConnection.abort: '#abort().'
  AgentConnectionResourceDiagnostic.collision: ResourceDiagnostic#collision.
  AgentConnectionSnapshot.sessionContext: Snapshot#sessionContext.
  AgentConnectionState.steeringMode: State#steeringMode.
  AgentConnectionState.followUpMode: State#followUpMode.
  AgentConnectionState.goal: State#goal.
  AgentConnection.getModelCatalog: '#getModelCatalog().'
  AgentConnection.listHeartbeats: '#listHeartbeats().'
  AgentConnection.getHeartbeat: '#getHeartbeat().'
  AgentConnection.getUserMessagesForForking: '#getUserMessagesForForking().'
  AgentConnection.getToolDefinition: '#getToolDefinition().'
  AgentConnection.waitForHeadlessCompletion: '#waitForHeadlessCompletion().'
  AgentConnection.setModel: '#setModel().'
  AgentConnection.setScopedModels: '#setScopedModels().'
  AgentConnection.setSteeringMode: '#setSteeringMode().'
  AgentConnection.setFollowUpMode: '#setFollowUpMode().'
  AgentConnection.compact: '#compact().'
  AgentConnectionSessionTreeFlatNode.label: SessionTreeFlatNode#label.
  AgentConnectionSessionTreeNode.children: SessionTreeNode#children.
  AgentConnectionModelCycleResult: ModelCycleResult#
  AgentConnectionState.cwd: State#cwd.
  AgentConnectionState.sessionName: State#sessionName.
  AgentConnectionState.autoCompactionEnabled: State#autoCompactionEnabled.
  AgentConnection.abortBash: '#abortBash().'
  AgentConnectionSnapshot.lastEventCursor: Snapshot#lastEventCursor.
  AgentConnectionResourceSnapshot.diagnostics: ResourceSnapshot#diagnostics.
  AgentConnectionPromptAdmissionError.-constructor: PromptAdmissionError#`<constructor>`().
  AgentConnectionPromptOptions.images: PromptOptions#images.
  AgentConnectionPromptOptions.source: PromptOptions#source.
  AgentConnectionRlmChildAgentSnapshot.activity: RlmChildAgentSnapshot#activity.
  AgentConnection.onBeforeSessionInvalidate: '#onBeforeSessionInvalidate().'
  AgentConnection.getInitialSnapshot: '#getInitialSnapshot().'
  AgentConnection.getSessionHeader: '#getSessionHeader().'
  AgentConnection.getResourceSnapshot: '#getResourceSnapshot().'
  AgentConnection.getAvailableModels: '#getAvailableModels().'
  AgentConnection.getContextTree: '#getContextTree().'
  AgentConnection.getSessionContext: '#getSessionContext().'
  AgentConnection.getQueue: '#getQueue().'
  AgentConnection.addCronJob: '#addCronJob().'
  AgentConnection.cancelCronJob: '#cancelCronJob().'
  AgentConnection.sendAgentMessage: '#sendAgentMessage().'
  AgentConnection.getAgentMessageStatus: '#getAgentMessageStatus().'
  AgentConnection.pauseAgentMessages: '#pauseAgentMessages().'
  AgentConnection.resumeAgentMessages: '#resumeAgentMessages().'
  AgentConnection.startSideQuestion: '#startSideQuestion().'
  AgentConnection.steer: '#steer().'
  AgentConnection.followUp: '#followUp().'
  AgentConnection.executeBash: '#executeBash().'
  AgentConnection.executeBashAndWait: '#executeBashAndWait().'
  AgentConnection.cycleModel: '#cycleModel().'
  AgentConnection.setServiceTier: '#setServiceTier().'
  AgentConnection.cycleThinkingLevel: '#cycleThinkingLevel().'
  AgentConnection.setTransport: '#setTransport().'
  AgentConnection.getRlmMaxDepthStatus: '#getRlmMaxDepthStatus().'
  AgentConnection.watchSession: '#watchSession().'
  AgentConnectionSessionHeader: SessionHeader#
  AgentConnectionSourceInfo.source: SourceInfo#source.
  AgentConnectionResourceDiagnostic.type: ResourceDiagnostic#type.
  AgentConnectionSavedSessionInfo.path: SavedSessionInfo#path.
  AgentConnectionSavedSessionInfo.id: SavedSessionInfo#id.
  AgentConnectionSessionEntryBase.timestamp: SessionEntryBase#timestamp.
  AgentConnectionCustomEntry.type: CustomEntry#type.
  AgentConnectionState.isCompacting: State#isCompacting.
  AgentConnectionPromptAdmissionError: PromptAdmissionError#
  AgentConnectionSideQuestionTurn: SideQuestionTurn#
  AgentConnectionRlmChildAgentSnapshot.parentId: RlmChildAgentSnapshot#parentId.
  AgentConnection.getSessionTree: '#getSessionTree().'
  AgentConnection.exportToHtml: '#exportToHtml().'
  AgentConnection.setSessionName: '#setSessionName().'
  AgentConnectionSessionWatcher: SessionWatcher#
  AgentConnectionSourceInfo.scope: SourceInfo#scope.
  AgentConnectionSavedSessionState: SavedSessionState#
  AgentConnectionSessionContext.serviceTier: SessionContext#serviceTier.
  AgentConnectionSlashCommand.sourceInfo: SlashCommand#sourceInfo.
  AgentConnectionResourceSnapshot.extensions: ResourceSnapshot#extensions.
  AgentConnectionQueuedMessageLane: QueuedMessageLane#
  AgentConnectionQueuedMessageMutation: QueuedMessageMutation#
  AgentConnection.clearQueue: '#clearQueue().'
  AgentConnection.abortAndClearQueue: '#abortAndClearQueue().'
  AgentConnection.deleteSavedSession: '#deleteSavedSession().'
  AgentConnectionSavedSessionInfo.parentSessionPath: SavedSessionInfo#parentSessionPath.
  AgentConnectionLabelEntry.type: LabelEntry#type.
  AgentConnectionSessionStateEntry: SessionStateEntry#
  AgentConnectionState.retryAttempt: State#retryAttempt.
  AgentConnectionState.recap: State#recap.
  AgentConnectionNavigateTreeResult: NavigateTreeResult#
  AgentConnectionUserMessage: UserMessage#
  AgentConnectionBeforeSessionInvalidateListener: BeforeSessionInvalidateListener#
  AgentConnection.getLastAssistantText: '#getLastAssistantText().'
  AgentConnection.waitForIdle: '#waitForIdle().'
  AgentConnection.setAutoCompactionEnabled: '#setAutoCompactionEnabled().'
  AgentConnection.abortRetry: '#abortRetry().'
  AgentConnection.importFromJsonl: '#importFromJsonl().'
  AgentConnectionSavedSessionInfo.agentStatus: SavedSessionInfo#agentStatus.
  AgentConnectionModelChangeEntry: ModelChangeEntry#
  AgentConnectionChildUsageAttributionEntry.childUsage: ChildUsageAttributionEntry#childUsage.
  AgentConnectionSnapshot.children: Snapshot#children.
  AgentConnectionResourceTheme.sourceInfo: ResourceTheme#sourceInfo.
  AgentConnectionResourceSnapshot.contextFiles: ResourceSnapshot#contextFiles.
  AgentConnectionResourceSnapshot.skills: ResourceSnapshot#skills.
  AgentConnectionModelCatalog.configuredProviders: ModelCatalog#configuredProviders.
  AgentConnectionServiceTierChangeEntry: ServiceTierChangeEntry#
  AgentConnectionAgentStatusEntry: AgentStatusEntry#
  AgentConnectionState.activeToolNames: State#activeToolNames.
  AgentConnectionArtifactType: ArtifactType#
  AgentConnectionPromptOptions.streamingBehavior: PromptOptions#streamingBehavior.
  AgentConnectionPromptOptions.queueIfBusy: PromptOptions#queueIfBusy.
  AgentConnectionNewSessionOptions: NewSessionOptions#
  AgentConnectionForkOptions: ForkOptions#
  AgentConnectionSwitchSessionOptions: SwitchSessionOptions#
  AgentConnectionNavigateTreeOptions: NavigateTreeOptions#
  AgentConnection.listCronJobs: '#listCronJobs().'
  AgentConnection.clearAgentMessages: '#clearAgentMessages().'
  AgentConnection.getSystemPrompt: '#getSystemPrompt().'
  AgentConnection.setSessionEntryLabel: '#setSessionEntryLabel().'
  AgentConnection.abortSideQuestion: '#abortSideQuestion().'
  AgentConnection.setAutoRetryEnabled: '#setAutoRetryEnabled().'
  AgentConnection.refine: '#refine().'
  AgentConnection.abortCompaction: '#abortCompaction().'
  AgentConnection.abortBranchSummary: '#abortBranchSummary().'
  AgentConnection.reload: '#reload().'
  AgentConnection.fork.Promise.typeLiteral138.cancelled: '#fork().Promise:typeLiteral138:cancelled.'
  AgentConnection.exportToJsonl: '#exportToJsonl().'
  AgentConnection.setRlmMaxDepth: '#setRlmMaxDepth().'
  AgentConnectionSnapshot.parent: Snapshot#parent.
  AgentConnectionResourceSkill.sourceInfo: ResourceSkill#sourceInfo.
  AgentConnectionResourcePrompt.sourceInfo: ResourcePrompt#sourceInfo.
  AgentConnectionResourceDiagnostics.skills: ResourceDiagnostics#skills.
  AgentConnectionResourceDiagnostics.prompts: ResourceDiagnostics#prompts.
  AgentConnectionResourceDiagnostics.extensions: ResourceDiagnostics#extensions.
  AgentConnectionResourceDiagnostics.themes: ResourceDiagnostics#themes.
  AgentConnectionResourceSnapshot.prompts: ResourceSnapshot#prompts.
  AgentConnectionResourceSnapshot.themes: ResourceSnapshot#themes.
  AgentConnectionAgentStatus: AgentStatus#
  AgentConnectionSavedSessionInfo.created: SavedSessionInfo#created.
  AgentConnectionSavedSessionInfo.modified: SavedSessionInfo#modified.
  AgentConnectionSavedSessionInfo.firstMessage: SavedSessionInfo#firstMessage.
  AgentConnectionSessionContext.thinkingLevel: SessionContext#thinkingLevel.
  AgentConnectionSessionContext.model: SessionContext#model.
  AgentConnectionSnapshot.sessionTree: Snapshot#sessionTree.
  AgentConnectionSnapshot.lastEventSequence: Snapshot#lastEventSequence.
  AgentConnectionState.leafId: State#leafId.
  AgentConnectionState.messageCount: State#messageCount.
  AgentConnectionState.compactionCount: State#compactionCount.
  AgentConnectionSlashCommand.source: SlashCommand#source.
  AgentConnectionResourceTheme.sourcePath: ResourceTheme#sourcePath.
  AgentConnectionPromptOptions.signal: PromptOptions#signal.
  AgentConnectionExecuteBashOptions: ExecuteBashOptions#
  AgentConnectionExtensionUiRequest.payload: ExtensionUiRequest#payload.
  AgentConnection.cancelRlmChild: '#cancelRlmChild().'
  AgentConnection.renameSavedSession: '#renameSavedSession().'
  AgentConnectionThinkingLevelChangeEntry: ThinkingLevelChangeEntry#
  AgentConnectionCompactionEntry: CompactionEntry#
  AgentConnectionBranchSummaryEntry: BranchSummaryEntry#
  AgentConnectionCustomEntry: CustomEntry#
  AgentConnectionChildUsageAttributionEntry: ChildUsageAttributionEntry#
  AgentConnectionCustomMessageEntry: CustomMessageEntry#
  AgentConnectionLabelEntry: LabelEntry#
  AgentConnectionSessionInfoEntry: SessionInfoEntry#
  AgentConnectionResourceContextFile: ResourceContextFile#
  AgentConnectionToolDefinition.replayBuiltInToolName: ToolDefinition#replayBuiltInToolName.
  AgentConnectionSessionWatcher.getMessages: SessionWatcher#getMessages().
  AgentConnectionSavedSessionInfo.cwd: SavedSessionInfo#cwd.
  AgentConnectionSavedSessionInfo.name: SavedSessionInfo#name.
  AgentConnectionServiceTierChangeEntry.serviceTier: ServiceTierChangeEntry#serviceTier.
  AgentConnectionSessionInfoEntry.name: SessionInfoEntry#name.
  AgentConnectionSessionTreeFlatNode: SessionTreeFlatNode#
  AgentConnectionSessionTreeFlatNode.labelTimestamp: SessionTreeFlatNode#labelTimestamp.
  AgentConnectionState.sessionDir: State#sessionDir.
  AgentConnectionSlashCommand.description: SlashCommand#description.
  AgentConnectionSideQuestionEvent.errorMessage: SideQuestionEvent#errorMessage.
  AgentConnectionHeartbeat.sessionName: Heartbeat#sessionName.
  AgentConnectionRlmChildAgentSnapshot.sessionName: RlmChildAgentSnapshot#sessionName.
  AgentConnectionRlmChildAgentSnapshot.model: RlmChildAgentSnapshot#model.
  AgentConnectionRlmChildAgentSnapshot.label: RlmChildAgentSnapshot#label.
  AgentConnectionRlmChildAgentSnapshot.sessionDir: RlmChildAgentSnapshot#sessionDir.
  AgentConnectionSourceInfo.origin: SourceInfo#origin.
  AgentConnectionSavedSessionInfo.state: SavedSessionInfo#state.
  AgentConnectionSessionListCallbacks.onProgress: SessionListCallbacks#onProgress.
  AgentConnectionGitStateEntry: GitStateEntry#
  AgentConnectionSnapshot.replay: Snapshot#replay.
  AgentConnectionResourceSkill.artifact: ResourceSkill#artifact.
  AgentConnectionResourceExtension.artifact: ResourceExtension#artifact.
  AgentConnection.getSessionTree.Promise.typeLiteral133.tree: '#getSessionTree().Promise:typeLiteral133:tree.'
  AgentConnectionSessionWatcher.subscribe: SessionWatcher#subscribe().
  AgentConnectionResourceDiagnostic.message: ResourceDiagnostic#message.
  AgentConnectionResourceDiagnostic.path: ResourceDiagnostic#path.
  AgentConnectionSavedSessionInfo.rlmDepth: SavedSessionInfo#rlmDepth.
  AgentConnectionSavedSessionInfo.messageCount: SavedSessionInfo#messageCount.
  AgentConnectionSavedSessionInfo.allMessagesText: SavedSessionInfo#allMessagesText.
  AgentConnectionModelChangeEntry.modelId: ModelChangeEntry#modelId.
  AgentConnectionEventCursor: EventCursor#
  AgentConnectionSlashCommand.registeredName: SlashCommand#registeredName.
  AgentConnectionResourcePrompt.name: ResourcePrompt#name.
  AgentConnectionResourcePrompt.filePath: ResourcePrompt#filePath.
  AgentConnectionToolDefinition.renderShell: ToolDefinition#renderShell.
  AgentConnection.getSessionTree.Promise.typeLiteral133.leafId: '#getSessionTree().Promise:typeLiteral133:leafId.'
  AgentConnection.fork.Promise.typeLiteral138.selectedText: '#fork().Promise:typeLiteral138:selectedText.'
  AgentConnectionChildUsageAttributionEntry.aggregateUsage: ChildUsageAttributionEntry#aggregateUsage.
  AgentConnectionReplayInfo.status: ReplayInfo#status.
  AgentConnectionReplayInfo.fromCursor: ReplayInfo#fromCursor.
  AgentConnectionReplayInfo.toCursor: ReplayInfo#toCursor.
  AgentConnectionSnapshot.sessionTree.typeLiteral11.tree: Snapshot#sessionTree.typeLiteral11:tree.
  AgentConnectionModelCycleResult.model: ModelCycleResult#model.
  AgentConnectionModelCycleResult.thinkingLevel: ModelCycleResult#thinkingLevel.
  AgentConnectionModelCycleResult.serviceTier: ModelCycleResult#serviceTier.
  AgentConnectionArtifactReference.type: ArtifactReference#type.
  AgentConnectionResourcePrompt.artifact: ResourcePrompt#artifact.
  AgentConnectionResourceExtension.sourceInfo: ResourceExtension#sourceInfo.
  AgentConnectionResourceTheme.artifact: ResourceTheme#artifact.
  AgentConnection.listCronJobs.options-typeLiteral134.includeInactive: '#listCronJobs().(options)typeLiteral134:includeInactive.'
  AgentConnection.refine.options-typeLiteral135.global: '#refine().(options)typeLiteral135:global.'
  AgentConnection.setRlmMaxDepth.options-typeLiteral140.global: '#setRlmMaxDepth().(options)typeLiteral140:global.'
  AgentConnectionSessionWatcher.getCommands: SessionWatcher#getCommands().
  AgentConnectionSessionWatcher.getToolDefinition: SessionWatcher#getToolDefinition().
  AgentConnectionSavedSessionStateStatus: SavedSessionStateStatus#
  AgentConnectionSourceScope: SourceScope#
  AgentConnectionSourceOrigin: SourceOrigin#
  AgentConnectionSourceInfo.path: SourceInfo#path.
  AgentConnectionSourceInfo.baseDir: SourceInfo#baseDir.
  AgentConnectionResourceCollision: ResourceCollision#
  AgentConnectionResourceCollision.name: ResourceCollision#name.
  AgentConnectionResourceCollision.winnerPath: ResourceCollision#winnerPath.
  AgentConnectionResourceCollision.loserPath: ResourceCollision#loserPath.
  AgentConnectionAgentStatus.summary: AgentStatus#summary.
  AgentConnectionSessionListProgress: SessionListProgress#
  AgentConnectionThinkingLevelChangeEntry.thinkingLevel: ThinkingLevelChangeEntry#thinkingLevel.
  AgentConnectionBranchSummaryEntry.summary: BranchSummaryEntry#summary.
  AgentConnectionCustomEntry.customType: CustomEntry#customType.
  AgentConnectionCustomMessageEntry.customType: CustomMessageEntry#customType.
  AgentConnectionLabelEntry.label: LabelEntry#label.
  AgentConnectionReplayStatus: ReplayStatus#
  AgentConnectionReplayInfo: ReplayInfo#
  AgentConnectionParentMetadata: ParentMetadata#
  AgentConnectionParentMetadata.childId: ParentMetadata#childId.
  AgentConnectionScopedModel.thinkingLevel: ScopedModel#thinkingLevel.
  AgentConnectionSlashCommand.argumentHint: SlashCommand#argumentHint.
  AgentConnectionResourceContextFile.path: ResourceContextFile#path.
  AgentConnectionResourceSkill: ResourceSkill#
  AgentConnectionResourceSkill.filePath: ResourceSkill#filePath.
  AgentConnectionResourcePrompt: ResourcePrompt#
  AgentConnectionResourceExtension: ResourceExtension#
  AgentConnectionResourceTheme: ResourceTheme#
  AgentConnectionResourceDiagnostics: ResourceDiagnostics#
  AgentConnectionToolDefinition.label: ToolDefinition#label.
  AgentConnectionPromptAdmissionError.cancelled: PromptAdmissionError#cancelled.
  AgentConnectionSideQuestionTurn.question: SideQuestionTurn#question.
  AgentConnectionSideQuestionTurn.answer: SideQuestionTurn#answer.
  AgentConnectionExecuteBashOptions.transient: ExecuteBashOptions#transient.
  AgentConnectionNavigateTreeResult.cancelled: NavigateTreeResult#cancelled.
  AgentConnectionRlmChildAgentStatus: RlmChildAgentStatus#
  AgentConnectionRlmChildAgentActivity: RlmChildAgentActivity#
  AgentConnectionRlmChildAgentSnapshot.tokenCount: RlmChildAgentSnapshot#tokenCount.
  AgentConnection.newSession.Promise.typeLiteral136.cancelled: '#newSession().Promise:typeLiteral136:cancelled.'
  AgentConnection.switchSession.Promise.typeLiteral137.cancelled: '#switchSession().Promise:typeLiteral137:cancelled.'
  AgentConnection.importFromJsonl.Promise.typeLiteral139.cancelled: '#importFromJsonl().Promise:typeLiteral139:cancelled.'
  AgentConnectionAgentStatus.taskState: AgentStatus#taskState.
  AgentConnectionSessionListCallbacks.onSession: SessionListCallbacks#onSession.
  AgentConnectionModelChangeEntry.provider: ModelChangeEntry#provider.
  AgentConnectionCompactionEntry.tokensBefore: CompactionEntry#tokensBefore.
  AgentConnectionChildUsageAttributionEntry.targetId: ChildUsageAttributionEntry#targetId.
  AgentConnectionResourceSkill.name: ResourceSkill#name.
  AgentConnectionResourceTheme.name: ResourceTheme#name.
  AgentConnectionToolDefinition.name: ToolDefinition#name.
  AgentConnectionToolDefinition.description: ToolDefinition#description.
  AgentConnectionToolDefinition.parameters: ToolDefinition#parameters.
  AgentConnectionExecuteBashOptions.excludeFromContext: ExecuteBashOptions#excludeFromContext.
  AgentConnectionExecuteBashOptions.runId: ExecuteBashOptions#runId.
  AgentConnectionNewSessionOptions.parentSession: NewSessionOptions#parentSession.
  AgentConnectionForkOptions.position: ForkOptions#position.
  AgentConnectionSwitchSessionOptions.cwdOverride: SwitchSessionOptions#cwdOverride.
  AgentConnectionNavigateTreeOptions.summarize: NavigateTreeOptions#summarize.
  AgentConnectionNavigateTreeOptions.customInstructions: NavigateTreeOptions#customInstructions.
  AgentConnectionNavigateTreeOptions.replaceInstructions: NavigateTreeOptions#replaceInstructions.
  AgentConnectionNavigateTreeOptions.label: NavigateTreeOptions#label.
  AgentConnectionNavigateTreeResult.aborted: NavigateTreeResult#aborted.
  AgentConnectionHeartbeat.firstMessage: Heartbeat#firstMessage.
  AgentConnectionRlmChildAgentSnapshot.answerPreview: RlmChildAgentSnapshot#answerPreview.
  AgentConnectionRlmChildAgentSnapshot.toolUseCount: RlmChildAgentSnapshot#toolUseCount.
  AgentConnectionRlmChildAgentSnapshot.recap: RlmChildAgentSnapshot#recap.
  AgentConnectionRlmChildAgentSnapshot.error: RlmChildAgentSnapshot#error.
  AgentConnectionSessionWatcher.close: SessionWatcher#close().
  AgentConnectionSessionHeader.type: SessionHeader#type.
  AgentConnectionSessionHeader.version: SessionHeader#version.
  AgentConnectionSessionHeader.id: SessionHeader#id.
  AgentConnectionSessionHeader.timestamp: SessionHeader#timestamp.
  AgentConnectionSessionHeader.cwd: SessionHeader#cwd.
  AgentConnectionSessionHeader.parentSession: SessionHeader#parentSession.
  AgentConnectionSessionHeader.rlmDepth: SessionHeader#rlmDepth.
  AgentConnectionSessionHeader.git: SessionHeader#git.
  AgentConnectionSessionHeader.git.typeLiteral0.repoUrl: SessionHeader#git.typeLiteral0:repoUrl.
  AgentConnectionSessionHeader.git.typeLiteral0.commit: SessionHeader#git.typeLiteral0:commit.
  AgentConnectionSessionHeader.git.typeLiteral0.branch: SessionHeader#git.typeLiteral0:branch.
  AgentConnectionResourceCollision.resourceType: ResourceCollision#resourceType.
  AgentConnectionResourceCollision.winnerSource: ResourceCollision#winnerSource.
  AgentConnectionResourceCollision.loserSource: ResourceCollision#loserSource.
  AgentConnectionSavedSessionState.status: SavedSessionState#status.
  AgentConnectionAgentStatus.basedOnMessageCount: AgentStatus#basedOnMessageCount.
  AgentConnectionSessionEntryBase.type: SessionEntryBase#type.
  AgentConnectionCompactionEntry.summary: CompactionEntry#summary.
  AgentConnectionCompactionEntry.firstKeptEntryId: CompactionEntry#firstKeptEntryId.
  AgentConnectionCompactionEntry.details: CompactionEntry#details.
  AgentConnectionCompactionEntry.fromHook: CompactionEntry#fromHook.
  AgentConnectionBranchSummaryEntry.fromId: BranchSummaryEntry#fromId.
  AgentConnectionBranchSummaryEntry.details: BranchSummaryEntry#details.
  AgentConnectionBranchSummaryEntry.fromHook: BranchSummaryEntry#fromHook.
  AgentConnectionCustomEntry.data: CustomEntry#data.
  AgentConnectionChildUsageAttributionEntry.origin: ChildUsageAttributionEntry#origin.
  AgentConnectionCustomMessageEntry.details: CustomMessageEntry#details.
  AgentConnectionCustomMessageEntry.display: CustomMessageEntry#display.
  AgentConnectionLabelEntry.targetId: LabelEntry#targetId.
  AgentConnectionSessionStateEntry.state: SessionStateEntry#state.
  AgentConnectionAgentStatusEntry.status: AgentStatusEntry#status.
  AgentConnectionGitStateEntry.git: GitStateEntry#git.
  AgentConnectionGitStateEntry.git.typeLiteral6.repoUrl: GitStateEntry#git.typeLiteral6:repoUrl.
  AgentConnectionGitStateEntry.git.typeLiteral6.commit: GitStateEntry#git.typeLiteral6:commit.
  AgentConnectionGitStateEntry.git.typeLiteral6.branch: GitStateEntry#git.typeLiteral6:branch.
  AgentConnectionReplayInfo.fromSequence: ReplayInfo#fromSequence.
  AgentConnectionReplayInfo.toSequence: ReplayInfo#toSequence.
  AgentConnectionReplayInfo.reason: ReplayInfo#reason.
  AgentConnectionEventCursor.generation: EventCursor#generation.
  AgentConnectionEventCursor.sequence: EventCursor#sequence.
  AgentConnectionParentMetadata.activeSessionId: ParentMetadata#activeSessionId.
  AgentConnectionParentMetadata.sessionId: ParentMetadata#sessionId.
  AgentConnectionParentMetadata.nodeId: ParentMetadata#nodeId.
  AgentConnectionSnapshot.sessionTree.typeLiteral11.leafId: Snapshot#sessionTree.typeLiteral11:leafId.
  AgentConnectionModelCycleResult.isScoped: ModelCycleResult#isScoped.
  AgentConnectionArtifactReference.id: ArtifactReference#id.
  AgentConnectionArtifactReference.sessionId: ArtifactReference#sessionId.
  AgentConnectionArtifactReference.logicalPath: ArtifactReference#logicalPath.
  AgentConnectionArtifactReference.relativePath: ArtifactReference#relativePath.
  AgentConnectionArtifactReference.mimeType: ArtifactReference#mimeType.
  AgentConnectionResourceContextFile.artifact: ResourceContextFile#artifact.
  AgentConnectionResourceSkill.description: ResourceSkill#description.
  AgentConnectionResourcePrompt.description: ResourcePrompt#description.
  AgentConnectionResourcePrompt.argumentHint: ResourcePrompt#argumentHint.
  AgentConnectionResourceExtension.path: ResourceExtension#path.
  AgentConnectionToolDefinition.promptSnippet: ToolDefinition#promptSnippet.
  AgentConnectionToolDefinition.promptGuidelines: ToolDefinition#promptGuidelines.
  AgentConnectionNavigateTreeResult.editorText: NavigateTreeResult#editorText.
  AgentConnectionUserMessage.entryId: UserMessage#entryId.
  AgentConnectionUserMessage.text: UserMessage#text.
  AgentConnectionRlmChildAgentActivity.kind: RlmChildAgentActivity#kind.
  AgentConnectionRlmChildAgentActivity.toolName: RlmChildAgentActivity#toolName.
  AgentConnectionRlmChildAgentSnapshot.durationMs: RlmChildAgentSnapshot#durationMs.
  AgentConnectionRlmChildAgentSnapshot.repliedSinceTask: RlmChildAgentSnapshot#repliedSinceTask.
  AgentConnection.refine.options-typeLiteral135.instructions: '#refine().(options)typeLiteral135:instructions.'
  AgentConnection.refine.options-typeLiteral135.rollbackId: '#refine().(options)typeLiteral135:rollbackId.'
---
# Module: [`packages/coding-agent/src/modes/agent-connection/types.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts)

## Classes
### `AgentConnection`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:635`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L635)
- signature: `interface AgentConnection`
- members:
  - `abort(method)` — [`L700`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L700) — Request cancellation of the active turn and return once the request is accepted.
  - `abortAndClearQueue(method)` — [`L663`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L663)
  - `abortBash(method)` — [`L712`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L712)
  - `abortBranchSummary(method)` — [`L729`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L729)
  - `abortCompaction(method)` — [`L728`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L728)
  - `abortRetry(method)` — [`L730`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L730)
  - `abortSideQuestion(method)` — [`L696`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L696)
  - `addCronJob(method)` — [`L671`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L671)
  - `cancelCronJob(method)` — [`L672`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L672)
  - `cancelRlmChild(method)` — [`L701`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L701)
  - `clearAgentMessages(method)` — [`L684`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L684)
  - `clearQueue(method)` — [`L662`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L662)
  - `compact(method)` — [`L726`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L726)
  - `cycleModel(method)` — [`L715`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L715)
  - `cycleThinkingLevel(method)` — [`L719`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L719)
  - `deleteSavedSession(method)` — [`L747`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L747)
  - `dispose(method)` — [`L752`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L752)
  - `executeBash(method)` — [`L710`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L710) — Run a user-initiated bash command (! / !! prefix). Resolution timing is
  - `executeBashAndWait(method)` — [`L711`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L711)
  - `exportToHtml(method)` — [`L741`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L741)
  - `exportToJsonl(method)` — [`L742`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L742)
  - `followUp(method)` — [`L698`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L698)
  - `fork(method)` — [`L735`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L735)
  - `getAgentMessageStatus(method)` — [`L681`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L681)
  - `getAvailableModels(method)` — [`L646`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L646)
  - `getCommands(method)` — [`L643`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L643)
  - `getContextTree(method)` — [`L648`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L648)
  - `getHeartbeat(method)` — [`L673`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L673)
  - `getInitialSnapshot(method)` — [`L640`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L640)
  - `getLastAssistantText(method)` — [`L686`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L686)
  - `getMessages(method)` — [`L641`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L641)
  - `getModelCatalog(method)` — [`L645`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L645)
  - `getQueue(method)` — [`L655`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L655)
  - `getResourceSnapshot(method)` — [`L644`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L644)
  - `getRlmMaxDepthStatus(method)` — [`L744`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L744)
  - `getSessionContext(method)` — [`L649`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L649)
  - `getSessionHeader(method)` — [`L642`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L642)
  - `getSessionStats(method)` — [`L647`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L647)
  - `getSessionTree(method)` — [`L650`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L650)
  - `getState(method)` — [`L639`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L639)
  - `getSystemPrompt(method)` — [`L688`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L688) — The system prompt currently in effect for the model (with any per-turn extension changes).
  - `getToolDefinition(method)` — [`L689`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L689)
  - `getUserMessagesForForking(method)` — [`L685`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L685)
  - `importFromJsonl(method)` — [`L740`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L740)
  - `listCronJobs(method)` — [`L664`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L664)
  - `listHeartbeats(method)` — [`L665`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L665)
  - `listSavedSessions(method)` — [`L651`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L651)
  - `manageHeartbeat(method)` — [`L666`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L666)
  - `mutateQueuedMessage(method)` — [`L656`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L656)
  - `navigateTree(method)` — [`L736`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L736)
  - `newSession(method)` — [`L733`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L733)
  - `onBeforeSessionInvalidate(method)` — [`L637`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L637)
  - `pauseAgentMessages(method)` — [`L682`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L682)
  - `prompt(method)` — [`L693`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L693)
  - `promptAndWait(method)` — [`L694`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L694)
  - `refine(method)` — [`L727`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L727)
  - `reload(method)` — [`L732`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L732)
  - `renameSavedSession(method)` — [`L746`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L746)
  - `respondToExtensionUiRequest(method)` — [`L691`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L691)
  - `resumeAgentMessages(method)` — [`L683`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L683)
  - `sendAgentMessage(method)` — [`L680`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L680)
  - `setAutoCompactionEnabled(method)` — [`L723`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L723)
  - `setAutoRetryEnabled(method)` — [`L724`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L724)
  - `setFollowUpMode(method)` — [`L722`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L722)
  - `setHeartbeat(method)` — [`L674`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L674)
  - `setModel(method)` — [`L714`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L714)
  - `setRlmMaxDepth(method)` — [`L745`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L745)
  - `setScopedModels(method)` — [`L716`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L716)
  - `setServiceTier(method)` — [`L718`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L718)
  - `setSessionEntryLabel(method)` — [`L690`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L690)
  - `setSessionName(method)` — [`L743`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L743)
  - `setSteeringMode(method)` — [`L721`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L721)
  - `setThinkingLevel(method)` — [`L717`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L717)
  - `setTransport(method)` — [`L720`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L720)
  - `startSideQuestion(method)` — [`L695`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L695)
  - `steer(method)` — [`L697`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L697)
  - `subscribe(method)` — [`L636`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L636)
  - `switchSession(method)` — [`L734`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L734)
  - `updateHeartbeat(method)` — [`L679`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L679)
  - `waitForHeadlessCompletion(method)` — [`L703`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L703)
  - `waitForIdle(method)` — [`L702`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L702)
  - `watchSession(method)` — [`L750`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L750) — Read-only watcher on another live session (a subagent); undefined if the transport can't reach it.
  - `cancelled` — [`L733`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L733)
  - `cancelled` — [`L734`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L734)
  - `cancelled` — [`L735`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L735)
  - `cancelled` — [`L740`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L740)
  - `global` — [`L727`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L727)
  - `global` — [`L745`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L745)
  - `includeInactive` — [`L664`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L664)
  - `instructions` — [`L727`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L727)
  - `leafId` — [`L650`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L650)
  - `rollbackId` — [`L727`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L727)
  - `selectedText` — [`L735`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L735)
  - `tree` — [`L650`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L650)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage), [`AgentCronJob`](../../core/cron-jobs.ts.md#AgentCronJob), [`ImageContent`](../../../../ai/src/types.ts.md#ImageContent), [`AgentConnectionModel`](types.ts.md#AgentConnectionModel), [`ThinkingLevel`](../../../../agent/src/types.ts.md#ThinkingLevel), [`AgentConnectionHeartbeat`](types.ts.md#AgentConnectionHeartbeat), [`dispose`](daemon-agent-connection.ts.md#DaemonAgentConnection.dispose), [`AgentConnectionState`](types.ts.md#AgentConnectionState), [`getInitialSnapshot`](daemon-agent-connection.ts.md#DaemonAgentConnection.getInitialSnapshot), [`ServiceTier`](../../../../ai/src/types.ts.md#ServiceTier), [`RefinementResult`](../../core/refinement/refinement.ts.md#RefinementResult), [`AgentAutonomousStatus`](../../core/autonomous.ts.md#AgentAutonomousStatus), [`DaemonAgentConnection`](daemon-agent-connection.ts.md#DaemonAgentConnection), [`AgentConnectionSessionTreeNode`](types.ts.md#AgentConnectionSessionTreeNode), [`subscribe`](daemon-agent-connection.ts.md#DaemonAgentConnection.subscribe), [`AgentHeartbeatDeliveryMode`](../../core/cron-jobs.ts.md#AgentHeartbeatDeliveryMode), [`AgentHeartbeatManagementAction`](../../core/cron-jobs.ts.md#AgentHeartbeatManagementAction), [`AgentConnectionSavedSessionInfo`](types.ts.md#AgentConnectionSavedSessionInfo), [`ContextTreeNode`](../../core/context-tree.ts.md#ContextTreeNode), [`AgentConnectionSnapshot`](types.ts.md#AgentConnectionSnapshot), [`listSavedSessions`](in-process-agent-connection.ts.md#InProcessAgentConnection.listSavedSessions), [`AgentConnectionQueueState`](types.ts.md#AgentConnectionQueueState), [`SessionStats`](../../core/session-stats.ts.md#SessionStats), [`getState`](daemon-agent-connection.ts.md#DaemonAgentConnection.getState), [`AgentSessionMessageSafetyStatus`](../../core/agent-messages.ts.md#AgentSessionMessageSafetyStatus), [`BashResult`](../../core/bash-executor.ts.md#BashResult), [`CompactionResult`](../../core/compaction/compaction.ts.md#CompactionResult), [`executeBash`](daemon-agent-connection.ts.md#DaemonAgentConnection.executeBash), [`AgentConnectionSessionContext`](types.ts.md#AgentConnectionSessionContext), [`AgentSessionMessageReceipt`](../../core/agent-messages.ts.md#AgentSessionMessageReceipt), [`prompt`](in-process-agent-connection.ts.md#InProcessAgentConnection.prompt), [`Transport`](../../../../ai/src/types.ts.md#Transport), [`promptAndWait`](in-process-agent-connection.ts.md#InProcessAgentConnection.promptAndWait), [`AgentConnectionModelCatalog`](types.ts.md#AgentConnectionModelCatalog), [`watchSession`](daemon-agent-connection.ts.md#DaemonAgentConnection.watchSession), [`watchSession`](in-process-agent-connection.ts.md#InProcessAgentConnection.watchSession), [`getMessages`](daemon-agent-connection.ts.md#DaemonAgentConnection.getMessages), [`AgentConnectionExtensionUiResponse`](types.ts.md#AgentConnectionExtensionUiResponse), [`prompt`](daemon-agent-connection.ts.md#DaemonAgentConnection.prompt), [`InProcessAgentConnection`](in-process-agent-connection.ts.md#InProcessAgentConnection)  (+180 more)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`main`](../../main.ts.md#main), [`main.ts`](../../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`showSettingsSelector`](../interactive/interactive-mode.ts.md#InteractiveMode.showSettingsSelector), [`handleEvent`](../interactive/interactive-mode.ts.md#InteractiveMode.handleEvent), [`setupEditorSubmitHandler`](../interactive/interactive-mode.ts.md#InteractiveMode.setupEditorSubmitHandler), [`runRpcModeWithConnectionInternal`](../rpc/rpc-mode.ts.md#runRpcModeWithConnectionInternal), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`<constructor>`](../interactive/interactive-mode.ts.md#InteractiveMode.-constructor), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`handleReloadCommand`](../interactive/interactive-mode.ts.md#InteractiveMode.handleReloadCommand), [`run`](../interactive/interactive-mode.ts.md#InteractiveMode.run), [`bindCurrentSessionExtensions`](../interactive/interactive-mode.ts.md#InteractiveMode.bindCurrentSessionExtensions), [`runPrintModeWithConnectionInternal`](../print-mode.ts.md#runPrintModeWithConnectionInternal), [`setupExtensionShortcuts`](../interactive/interactive-mode.ts.md#InteractiveMode.setupExtensionShortcuts), [`runAcpModeWithConnection`](../acp/acp-mode.ts.md#runAcpModeWithConnection), [`agentConnection`](../interactive/interactive-mode.ts.md#InteractiveMode.agentConnection), [`handleTracesCommand`](../interactive/interactive-mode.ts.md#InteractiveMode.handleTracesCommand), [`handleUpdateCommand`](../interactive/interactive-mode.ts.md#InteractiveMode.handleUpdateCommand), [`showTreeSelector`](../interactive/interactive-mode.ts.md#InteractiveMode.showTreeSelector), [`acp-mode.ts`](../acp/acp-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-acp-acp-mode.ts), [`showModelsSelector`](../interactive/interactive-mode.ts.md#InteractiveMode.showModelsSelector), [`rpc-mode.ts`](../rpc/rpc-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-mode.ts), [`applyQueueSelection`](../interactive/interactive-mode.ts.md#InteractiveMode.applyQueueSelection), [`handleClearCommand`](../interactive/interactive-mode.ts.md#InteractiveMode.handleClearCommand), [`subscribeToAgent`](../interactive/interactive-mode.ts.md#InteractiveMode.subscribeToAgent), [`handleSideQuestion`](../interactive/interactive-mode.ts.md#InteractiveMode.handleSideQuestion), [`applySelectedModel`](../interactive/interactive-mode.ts.md#InteractiveMode.applySelectedModel), [`print-mode.ts`](../print-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-print-mode.ts), [`handleSessionCommand`](../interactive/interactive-mode.ts.md#InteractiveMode.handleSessionCommand), [`clearSideQuestion`](../interactive/interactive-mode.ts.md#InteractiveMode.clearSideQuestion), [`renderInitialMessages`](../interactive/interactive-mode.ts.md#InteractiveMode.renderInitialMessages), [`handleDebugCommand`](../interactive/interactive-mode.ts.md#InteractiveMode.handleDebugCommand), [`moveQueueSelection`](../interactive/interactive-mode.ts.md#InteractiveMode.moveQueueSelection), [`handleRlmMaxDepthCommand`](../interactive/interactive-mode.ts.md#InteractiveMode.handleRlmMaxDepthCommand), [`handleShareCommand`](../interactive/interactive-mode.ts.md#InteractiveMode.handleShareCommand), [`interruptOrClearInput`](../interactive/interactive-mode.ts.md#InteractiveMode.interruptOrClearInput)  (+35 more; 1 test-only)

### `AgentConnectionAgentStatus`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:106`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L106)
- signature: `interface AgentConnectionAgentStatus`
- members:
  - `basedOnMessageCount` — [`L109`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L109)
  - `summary` — [`L107`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L107)
  - `taskState` — [`L108`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L108)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`daemon-protocol.ts`](../daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`summaryForUnifiedRecord`](../agents-view/agents-view-state.ts.md#summaryForUnifiedRecord), [`createUnifiedSearchableText`](../agents-view/agents-view-state.ts.md#createUnifiedSearchableText), [`agentStatus`](types.ts.md#AgentConnectionSavedSessionInfo.agentStatus), [`agentStatus`](../daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.agentStatus), [`AgentConnectionAgentStatusEntry`](types.ts.md#AgentConnectionAgentStatusEntry)

### `AgentConnectionAgentStatusEntry`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:227`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L227)
- signature: `interface AgentConnectionAgentStatusEntry`
- members:
  - `status` — [`L229`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L229)
  - `type` — [`L228`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L228)
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionEntryBase`](types.ts.md#AgentConnectionSessionEntryBase), [`AgentConnectionAgentStatus`](types.ts.md#AgentConnectionAgentStatus)
- used by: [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`AgentConnectionSessionEntry`](types.ts.md#AgentConnectionSessionEntry)  (1 test-only)

### `AgentConnectionArtifactReference`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:366`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L366)
- signature: `interface AgentConnectionArtifactReference`
- members:
  - `id` — [`L367`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L367)
  - `logicalPath` — [`L370`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L370)
  - `mimeType` — [`L372`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L372)
  - `relativePath` — [`L371`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L371)
  - `sessionId` — [`L368`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L368)
  - `type` — [`L369`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L369)
- uses (calls/refs, reference-scoped): [`AgentConnectionArtifactType`](types.ts.md#AgentConnectionArtifactType)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`snapshot.ts`](snapshot.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-snapshot.ts), [`createArtifactReference`](snapshot.ts.md#createArtifactReference), [`AgentConnectionResourceContextFile`](types.ts.md#AgentConnectionResourceContextFile), [`artifact`](types.ts.md#AgentConnectionResourceExtension.artifact), [`artifact`](types.ts.md#AgentConnectionResourceSkill.artifact), [`artifact`](types.ts.md#AgentConnectionResourcePrompt.artifact), [`artifact`](types.ts.md#AgentConnectionResourceTheme.artifact)

### `AgentConnectionArtifactType`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:364`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L364)
- signature: `type AgentConnectionArtifactType`
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`snapshot.ts`](snapshot.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-snapshot.ts), [`createArtifactReference`](snapshot.ts.md#createArtifactReference), [`type`](types.ts.md#AgentConnectionArtifactReference.type)

### `AgentConnectionBeforeSessionInvalidateListener`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:633`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L633)
- signature: `type AgentConnectionBeforeSessionInvalidateListener`
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`onBeforeSessionInvalidate`](types.ts.md#AgentConnection.onBeforeSessionInvalidate), [`onBeforeSessionInvalidate`](in-process-agent-connection.ts.md#InProcessAgentConnection.onBeforeSessionInvalidate), [`beforeSessionInvalidateListeners`](in-process-agent-connection.ts.md#InProcessAgentConnection.beforeSessionInvalidateListeners), [`onBeforeSessionInvalidate`](daemon-agent-connection.ts.md#DaemonAgentConnection.onBeforeSessionInvalidate)

### `AgentConnectionBranchSummaryEntry`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:181`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L181)
- signature: `interface AgentConnectionBranchSummaryEntry`
- members:
  - `details` — [`L185`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L185)
  - `fromHook` — [`L186`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L186)
  - `fromId` — [`L183`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L183)
  - `summary` — [`L184`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L184)
  - `type` — [`L182`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L182)
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionEntryBase`](types.ts.md#AgentConnectionSessionEntryBase)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`AgentConnectionSessionEntry`](types.ts.md#AgentConnectionSessionEntry)  (1 test-only)

### `AgentConnectionChildUsageAttributionEntry`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:195`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L195)
- signature: `interface AgentConnectionChildUsageAttributionEntry`
- members:
  - `aggregateUsage` — [`L199`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L199)
  - `childUsage` — [`L198`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L198)
  - `origin` — [`L200`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L200)
  - `targetId` — [`L197`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L197)
  - `type` — [`L196`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L196)
- uses (calls/refs, reference-scoped): [`Usage`](../../../../ai/src/types.ts.md#Usage), [`AgentConnectionSessionEntryBase`](types.ts.md#AgentConnectionSessionEntryBase)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`AgentConnectionSessionEntry`](types.ts.md#AgentConnectionSessionEntry)  (1 test-only)

### `AgentConnectionCompactionEntry`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:172`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L172)
- signature: `interface AgentConnectionCompactionEntry`
- members:
  - `details` — [`L177`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L177)
  - `firstKeptEntryId` — [`L175`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L175)
  - `fromHook` — [`L178`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L178)
  - `summary` — [`L174`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L174)
  - `tokensBefore` — [`L176`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L176)
  - `type` — [`L173`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L173)
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionEntryBase`](types.ts.md#AgentConnectionSessionEntryBase)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`AgentConnectionSessionEntry`](types.ts.md#AgentConnectionSessionEntry)  (1 test-only)

### `AgentConnectionCustomEntry`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:189`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L189)
- signature: `interface AgentConnectionCustomEntry`
- members:
  - `customType` — [`L191`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L191)
  - `data` — [`L192`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L192)
  - `type` — [`L190`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L190)
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionEntryBase`](types.ts.md#AgentConnectionSessionEntryBase)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`AgentConnectionSessionEntry`](types.ts.md#AgentConnectionSessionEntry)  (1 test-only)

### `AgentConnectionCustomMessageEntry`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:203`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L203)
- signature: `interface AgentConnectionCustomMessageEntry`
- members:
  - `content` — [`L206`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L206)
  - `customType` — [`L205`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L205)
  - `details` — [`L207`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L207)
  - `display` — [`L208`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L208)
  - `type` — [`L204`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L204)
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../../ai/src/types.ts.md#ImageContent), [`TextContent`](../../../../ai/src/types.ts.md#TextContent), [`AgentConnectionSessionEntryBase`](types.ts.md#AgentConnectionSessionEntryBase)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`AgentConnectionSessionEntry`](types.ts.md#AgentConnectionSessionEntry)  (1 test-only)

### `AgentConnectionEvent`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:620`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L620)
- signature: `type AgentConnectionEvent`
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage), [`AgentConnectionSessionEvent`](types.ts.md#AgentConnectionSessionEvent), [`AgentConnectionState`](types.ts.md#AgentConnectionState), [`AgentConnectionSnapshot`](types.ts.md#AgentConnectionSnapshot), [`AgentConnectionSideQuestionEvent`](types.ts.md#AgentConnectionSideQuestionEvent), [`AgentConnectionExtensionUiRequest`](types.ts.md#AgentConnectionExtensionUiRequest)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`emit`](daemon-agent-connection.ts.md#DaemonAgentConnection.emit), [`AgentConnectionEventListener`](types.ts.md#AgentConnectionEventListener), [`emit`](in-process-agent-connection.ts.md#InProcessAgentConnection.emit)  (3 test-only)

### `AgentConnectionEventCursor`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:285`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L285)
- signature: `interface AgentConnectionEventCursor`
- members:
  - `generation` — [`L286`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L286)
  - `sequence` — [`L287`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L287)
- used by: [`lastEventCursor`](types.ts.md#AgentConnectionSnapshot.lastEventCursor), [`fromCursor`](types.ts.md#AgentConnectionReplayInfo.fromCursor), [`toCursor`](types.ts.md#AgentConnectionReplayInfo.toCursor)

### `AgentConnectionEventListener`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:632`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L632)
- signature: `type AgentConnectionEventListener`
- uses (calls/refs, reference-scoped): [`AgentConnectionEvent`](types.ts.md#AgentConnectionEvent)
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`subscribe`](daemon-agent-connection.ts.md#DaemonAgentConnection.subscribe), [`subscribe`](types.ts.md#AgentConnection.subscribe), [`subscribe`](in-process-agent-connection.ts.md#InProcessAgentConnection.subscribe), [`listeners`](daemon-agent-connection.ts.md#DaemonAgentConnection.listeners), [`listeners`](in-process-agent-connection.ts.md#InProcessAgentConnection.listeners), [`subscribe`](types.ts.md#AgentConnectionSessionWatcher.subscribe)  (1 test-only)

### `AgentConnectionExecuteBashOptions`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:474`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L474)
- signature: `interface AgentConnectionExecuteBashOptions`
- members:
  - `excludeFromContext` — [`L475`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L475)
  - `runId` — [`L483`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L483) — Caller-generated id echoed on the run's bash_start/bash_end events, so the
  - `transient` — [`L477`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L477) — Run without recording into the session (side-conversation bash).
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`executeBash`](daemon-agent-connection.ts.md#DaemonAgentConnection.executeBash), [`executeBash`](types.ts.md#AgentConnection.executeBash), [`executeBash`](in-process-agent-connection.ts.md#InProcessAgentConnection.executeBash)

### `AgentConnectionExtensionUiRequest`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:534`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L534)
- signature: `interface AgentConnectionExtensionUiRequest`
- members:
  - `id` — [`L535`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L535)
  - `method` — [`L536`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L536)
  - `payload` — [`L537`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L537)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`runRpcModeWithConnectionInternal`](../rpc/rpc-mode.ts.md#runRpcModeWithConnectionInternal), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`handleDaemonMessage`](daemon-agent-connection.ts.md#DaemonAgentConnection.handleDaemonMessage), [`resolveConnectionExtensionUiRequest`](../interactive/interactive-mode.ts.md#InteractiveMode.resolveConnectionExtensionUiRequest), [`AgentConnectionEvent`](types.ts.md#AgentConnectionEvent), [`handleConnectionExtensionUiRequest`](../interactive/interactive-mode.ts.md#InteractiveMode.handleConnectionExtensionUiRequest), [`expectsConnectionExtensionUiResponse`](../interactive/interactive-mode.ts.md#InteractiveMode.expectsConnectionExtensionUiResponse)  (2 test-only)

### `AgentConnectionExtensionUiResponse`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:532`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L532)
- signature: `type AgentConnectionExtensionUiResponse`
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`runRpcModeWithConnectionInternal`](../rpc/rpc-mode.ts.md#runRpcModeWithConnectionInternal), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`resolveConnectionExtensionUiRequest`](../interactive/interactive-mode.ts.md#InteractiveMode.resolveConnectionExtensionUiRequest), [`rpc-mode.ts`](../rpc/rpc-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-mode.ts), [`handleConnectionExtensionUiRequest`](../interactive/interactive-mode.ts.md#InteractiveMode.handleConnectionExtensionUiRequest), [`respondToExtensionUiRequest`](types.ts.md#AgentConnection.respondToExtensionUiRequest), [`respondToExtensionUiRequest`](daemon-agent-connection.ts.md#DaemonAgentConnection.respondToExtensionUiRequest), [`respondToExtensionUiRequest`](in-process-agent-connection.ts.md#InProcessAgentConnection.respondToExtensionUiRequest)  (1 test-only)

### `AgentConnectionForkOptions`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:490`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L490)
- signature: `interface AgentConnectionForkOptions`
- members:
  - `position` — [`L491`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L491)
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`fork`](types.ts.md#AgentConnection.fork), [`selectedText`](daemon-agent-connection.ts.md#DaemonAgentConnection.fork.Promise.typeLiteral698.selectedText), [`fork`](in-process-agent-connection.ts.md#InProcessAgentConnection.fork), [`fork`](daemon-agent-connection.ts.md#DaemonAgentConnection.fork)

### `AgentConnectionGitStateEntry`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:232`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L232)
- signature: `interface AgentConnectionGitStateEntry`
- members:
  - `branch` — [`L237`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L237)
  - `commit` — [`L236`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L236)
  - `git` — [`L234`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L234)
  - `repoUrl` — [`L235`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L235)
  - `type` — [`L233`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L233)
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionEntryBase`](types.ts.md#AgentConnectionSessionEntryBase)
- used by: [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`AgentConnectionSessionEntry`](types.ts.md#AgentConnectionSessionEntry)  (1 test-only)

### `AgentConnectionHeartbeat`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:526`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L526)
- signature: `interface AgentConnectionHeartbeat`
- members:
  - `firstMessage` — [`L529`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L529)
  - `job` — [`L527`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L527)
  - `sessionName` — [`L528`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L528)
- uses (calls/refs, reference-scoped): [`AgentCronJob`](../../core/cron-jobs.ts.md#AgentCronJob)
- used by: [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`daemon-mode.ts`](../daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`daemon-supervisor.ts`](../daemon/daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`handleCommand`](../daemon/daemon-supervisor.ts.md#DaemonSupervisor.handleCommand), [`agents-view-mode.ts`](../agents-view/agents-view-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agents-view-agents-view-mode.ts), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`daemon-protocol.ts`](../daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`rpc-client.ts`](../rpc/rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`rpc-types.ts`](../rpc/rpc-types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-types.ts), [`createActionPanel`](../interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.createActionPanel), [`populateHeartbeatList`](../interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.populateHeartbeatList), [`reconcileUnifiedSessions`](../agents-view/agents-view-state.ts.md#reconcileUnifiedSessions), [`heartbeat-manager.ts`](../interactive/components/heartbeat-manager.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-heartbeat-manager.ts), [`RpcResponse`](../rpc/rpc-types.ts.md#RpcResponse), [`createHeartbeatListPanel`](../interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.createHeartbeatListPanel), [`manageHeartbeat`](../interactive/interactive-mode.ts.md#InteractiveMode.manageHeartbeat), [`aggregateSessionHeartbeats`](../agents-view/agents-view-state.ts.md#aggregateSessionHeartbeats), [`updateSubagentSummaryLine`](../interactive/interactive-mode.ts.md#InteractiveMode.updateSubagentSummaryLine), [`setHeartbeats`](../interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.setHeartbeats), [`formatHeartbeatDetails`](../interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.formatHeartbeatDetails), [`confirmSelection`](../interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.confirmSelection), [`listDaemonHeartbeats`](../daemon/heartbeat-catalog.ts.md#listDaemonHeartbeats), [`listHeartbeats`](../daemon/daemon-mode.ts.md#AgentDaemon.listHeartbeats), [`scopeHeartbeatsToSession`](../interactive/heartbeat-scope.ts.md#scopeHeartbeatsToSession), [`agents-view-state.ts`](../agents-view/agents-view-state.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agents-view-agents-view-state.ts), [`heartbeat-catalog.ts`](../daemon/heartbeat-catalog.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-heartbeat-catalog.ts), [`scheduleHeartbeatManagerRefresh`](../interactive/interactive-mode.ts.md#InteractiveMode.scheduleHeartbeatManagerRefresh), [`heartbeats`](../interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.heartbeats), [`sessionLabel`](../interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.sessionLabel), [`runAction`](../interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.runAction), [`action`](../interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.availableActions.Array.typeLiteral116.action), [`findHeartbeat`](../interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.findHeartbeat), [`formatStatus`](../interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.formatStatus), [`<constructor>`](../interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.-constructor), [`heartbeatSnapshot`](../daemon/daemon-supervisor.ts.md#ResidentWorker.heartbeatSnapshot), [`heartbeats`](../interactive/interactive-mode.ts.md#InteractiveMode.heartbeats), [`listHeartbeats`](daemon-agent-connection.ts.md#DaemonAgentConnection.listHeartbeats), [`getTrayHeartbeatLabel`](../interactive/interactive-mode.ts.md#InteractiveMode.getTrayHeartbeatLabel)  (+14 more; 13 test-only)

### `AgentConnectionLabelEntry`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:211`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L211)
- signature: `interface AgentConnectionLabelEntry`
- members:
  - `label` — [`L214`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L214)
  - `targetId` — [`L213`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L213)
  - `type` — [`L212`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L212)
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionEntryBase`](types.ts.md#AgentConnectionSessionEntryBase)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`AgentConnectionSessionEntry`](types.ts.md#AgentConnectionSessionEntry)  (1 test-only)

### `AgentConnectionModel`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:51`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L51) — documented in [packages-coding-agent-src-modes-agent-connection-types.ts](../../../../../../concepts/packages-coding-agent-src-modes-agent-connection-types.ts.md)
- signature: `type AgentConnectionModel`
- uses (calls/refs, reference-scoped): [`Model`](../../../../ai/src/types.ts.md#Model), [`Api`](../../../../ai/src/types.ts.md#Api)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`showModelsSelector`](../interactive/interactive-mode.ts.md#InteractiveMode.showModelsSelector), [`applySelectedModel`](../interactive/interactive-mode.ts.md#InteractiveMode.applySelectedModel), [`snapshot.ts`](snapshot.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-snapshot.ts), [`ensureModelProviderConfigured`](../interactive/interactive-mode.ts.md#InteractiveMode.ensureModelProviderConfigured), [`getConnectionAvailableModels`](../interactive/interactive-mode.ts.md#InteractiveMode.getConnectionAvailableModels), [`getCurrentModel`](../interactive/interactive-mode.ts.md#InteractiveMode.getCurrentModel), [`getCachedModelCandidates`](../interactive/interactive-mode.ts.md#InteractiveMode.getCachedModelCandidates), [`getModelSelectorRefreshPromise`](../interactive/interactive-mode.ts.md#InteractiveMode.getModelSelectorRefreshPromise), [`setModel`](in-process-agent-connection.ts.md#InProcessAgentConnection.setModel), [`completeModelSelection`](../interactive/interactive-mode.ts.md#InteractiveMode.completeModelSelection), [`getScopedModelsFromModelIds`](../interactive/interactive-mode.ts.md#InteractiveMode.getScopedModelsFromModelIds), [`model`](types.ts.md#AgentConnectionState.model), [`isModelProviderConfigured`](../interactive/interactive-mode.ts.md#InteractiveMode.isModelProviderConfigured), [`model`](types.ts.md#AgentConnectionScopedModel.model), [`getModelCandidates`](../interactive/interactive-mode.ts.md#InteractiveMode.getModelCandidates), [`models`](types.ts.md#AgentConnectionModelCatalog.models), [`getAvailableModels`](in-process-agent-connection.ts.md#InProcessAgentConnection.getAvailableModels), [`setModel`](types.ts.md#AgentConnection.setModel), [`toConnectionModel`](snapshot.ts.md#toConnectionModel), [`connectionModelsRefreshInFlight`](../interactive/interactive-mode.ts.md#InteractiveMode.connectionModelsRefreshInFlight), [`getAvailableModels`](types.ts.md#AgentConnection.getAvailableModels), [`getConnectionModelCatalog`](../interactive/interactive-mode.ts.md#InteractiveMode.getConnectionModelCatalog), [`connectionModels`](../interactive/interactive-mode.ts.md#InteractiveMode.connectionModels), [`getAvailableModels`](daemon-agent-connection.ts.md#DaemonAgentConnection.getAvailableModels), [`connectionModelCatalog`](../interactive/interactive-mode.ts.md#InteractiveMode.connectionModelCatalog), [`setModel`](daemon-agent-connection.ts.md#DaemonAgentConnection.setModel), [`model`](types.ts.md#AgentConnectionModelCycleResult.model)  (18 test-only)

### `AgentConnectionModelCatalog`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:52`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L52)
- signature: `interface AgentConnectionModelCatalog`
- members:
  - `configuredProviders` — [`L54`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L54)
  - `models` — [`L53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L53)
- uses (calls/refs, reference-scoped): [`AgentConnectionModel`](types.ts.md#AgentConnectionModel)
- used by: [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`applyConnectionModelCatalog`](../interactive/interactive-mode.ts.md#InteractiveMode.applyConnectionModelCatalog), [`getModelCatalog`](daemon-agent-connection.ts.md#DaemonAgentConnection.getModelCatalog), [`getModelCatalog`](in-process-agent-connection.ts.md#InProcessAgentConnection.getModelCatalog), [`getModelCatalog`](types.ts.md#AgentConnection.getModelCatalog)  (6 test-only)

### `AgentConnectionModelChangeEntry`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:166`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L166)
- signature: `interface AgentConnectionModelChangeEntry`
- members:
  - `modelId` — [`L169`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L169)
  - `provider` — [`L168`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L168)
  - `type` — [`L167`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L167)
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionEntryBase`](types.ts.md#AgentConnectionSessionEntryBase)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`AgentConnectionSessionEntry`](types.ts.md#AgentConnectionSessionEntry)  (3 test-only)

### `AgentConnectionModelCycleResult`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:317`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L317)
- signature: `interface AgentConnectionModelCycleResult`
- members:
  - `isScoped` — [`L321`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L321)
  - `model` — [`L318`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L318)
  - `serviceTier` — [`L320`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L320)
  - `thinkingLevel` — [`L319`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L319)
- uses (calls/refs, reference-scoped): [`AgentConnectionModel`](types.ts.md#AgentConnectionModel), [`ThinkingLevel`](../../../../agent/src/types.ts.md#ThinkingLevel), [`ServiceTier`](../../../../ai/src/types.ts.md#ServiceTier)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`cycleModel`](types.ts.md#AgentConnection.cycleModel), [`cycleModel`](in-process-agent-connection.ts.md#InProcessAgentConnection.cycleModel), [`cycleModel`](daemon-agent-connection.ts.md#DaemonAgentConnection.cycleModel)

### `AgentConnectionNavigateTreeOptions`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:498`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L498)
- signature: `interface AgentConnectionNavigateTreeOptions`
- members:
  - `customInstructions` — [`L500`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L500)
  - `label` — [`L502`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L502)
  - `replaceInstructions` — [`L501`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L501)
  - `summarize` — [`L499`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L499)
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`navigateTree`](daemon-agent-connection.ts.md#DaemonAgentConnection.navigateTree), [`navigateTree`](types.ts.md#AgentConnection.navigateTree), [`navigateTree`](in-process-agent-connection.ts.md#InProcessAgentConnection.navigateTree)

### `AgentConnectionNavigateTreeResult`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:505`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L505)
- signature: `interface AgentConnectionNavigateTreeResult`
- members:
  - `aborted` — [`L508`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L508)
  - `cancelled` — [`L507`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L507)
  - `editorText` — [`L506`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L506)
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`bindCurrentSessionExtensions`](../interactive/interactive-mode.ts.md#InteractiveMode.bindCurrentSessionExtensions), [`showTreeSelector`](../interactive/interactive-mode.ts.md#InteractiveMode.showTreeSelector), [`navigateTree`](daemon-agent-connection.ts.md#DaemonAgentConnection.navigateTree), [`navigateTree`](types.ts.md#AgentConnection.navigateTree), [`navigateTree`](in-process-agent-connection.ts.md#InProcessAgentConnection.navigateTree)

### `AgentConnectionNewSessionOptions`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:486`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L486)
- signature: `interface AgentConnectionNewSessionOptions`
- members:
  - `parentSession` — [`L487`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L487)
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`newSession`](types.ts.md#AgentConnection.newSession), [`newSession`](daemon-agent-connection.ts.md#DaemonAgentConnection.newSession), [`newSession`](in-process-agent-connection.ts.md#InProcessAgentConnection.newSession)

### `AgentConnectionParentMetadata`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:290`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L290)
- signature: `interface AgentConnectionParentMetadata`
- members:
  - `activeSessionId` — [`L291`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L291)
  - `childId` — [`L294`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L294)
  - `nodeId` — [`L293`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L293)
  - `sessionId` — [`L292`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L292)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`renderResyncedSession`](../interactive/interactive-mode.ts.md#InteractiveMode.renderResyncedSession), [`renderInitialMessages`](../interactive/interactive-mode.ts.md#InteractiveMode.renderInitialMessages), [`parent`](types.ts.md#AgentConnectionSnapshot.parent)

### `AgentConnectionPromptAdmissionError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:438`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L438)
- doc: Prompt admission failure; only a confirmed cancellation is retry-safe.
- signature: `class AgentConnectionPromptAdmissionError`
- members:
  - `<constructor>(message: string, status: "unknown" | "cancelled" | "owned" | "unsupported", options?: ErrorOptions | undefined)` — [`L441`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L441) — Prompt admission failure; only a confirmed cancellation is retry-safe.
  - `cancelled` — [`L439`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L439)
- used by: [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`run`](../interactive/interactive-mode.ts.md#InteractiveMode.run), [`promptWithAdmissionCancellation`](daemon-agent-connection.ts.md#DaemonAgentConnection.promptWithAdmissionCancellation)  (1 test-only)

### `AgentConnectionPromptOptions`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:452`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L452)
- signature: `interface AgentConnectionPromptOptions`
- members:
  - `images` — [`L453`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L453)
  - `queueIfBusy` — [`L455`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L455)
  - `signal` — [`L458`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L458) — Cancel admission while it is still waiting; accepted prompts remain session-owned.
  - `source` — [`L456`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L456)
  - `streamingBehavior` — [`L454`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L454)
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../../ai/src/types.ts.md#ImageContent), [`InputSource`](../../core/extensions/types.ts.md#InputSource)
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`promptWithAdmissionCancellation`](daemon-agent-connection.ts.md#DaemonAgentConnection.promptWithAdmissionCancellation), [`prompt`](in-process-agent-connection.ts.md#InProcessAgentConnection.prompt), [`promptAndWait`](in-process-agent-connection.ts.md#InProcessAgentConnection.promptAndWait), [`prompt`](daemon-agent-connection.ts.md#DaemonAgentConnection.prompt), [`prompt`](types.ts.md#AgentConnection.prompt), [`promptAndWait`](types.ts.md#AgentConnection.promptAndWait), [`promptAndWait`](daemon-agent-connection.ts.md#DaemonAgentConnection.promptAndWait)

### `AgentConnectionQueueMode`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:50`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L50)
- doc: Client-side interaction boundary consumed by InteractiveMode.
- signature: `type AgentConnectionQueueMode`
- used by: [`DaemonCommand`](../daemon/daemon-protocol.ts.md#DaemonCommand), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`daemon-protocol.ts`](../daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`followUpMode`](types.ts.md#AgentConnectionState.followUpMode), [`setFollowUpMode`](types.ts.md#AgentConnection.setFollowUpMode), [`setSteeringMode`](types.ts.md#AgentConnection.setSteeringMode), [`steeringMode`](types.ts.md#AgentConnectionState.steeringMode), [`setFollowUpMode`](in-process-agent-connection.ts.md#InProcessAgentConnection.setFollowUpMode), [`setSteeringMode`](in-process-agent-connection.ts.md#InProcessAgentConnection.setSteeringMode), [`setFollowUpMode`](daemon-agent-connection.ts.md#DaemonAgentConnection.setFollowUpMode), [`setSteeringMode`](daemon-agent-connection.ts.md#DaemonAgentConnection.setSteeringMode)

### `AgentConnectionQueueState`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:516`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L516)
- signature: `interface AgentConnectionQueueState`
- members:
  - `followUp` — [`L518`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L518)
  - `steering` — [`L517`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L517)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`handleEvent`](../interactive/interactive-mode.ts.md#InteractiveMode.handleEvent), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`resetCurrentSessionRenderState`](../interactive/interactive-mode.ts.md#InteractiveMode.resetCurrentSessionRenderState), [`move`](../interactive/queue-selection.ts.md#QueueSelection.move), [`replaceConnectionQueue`](../interactive/interactive-mode.ts.md#InteractiveMode.replaceConnectionQueue), [`sync`](../interactive/queue-selection.ts.md#QueueSelection.sync), [`liveImageMarkerIds`](../interactive/interactive-mode.ts.md#InteractiveMode.liveImageMarkerIds), [`connectionQueue`](../interactive/interactive-mode.ts.md#InteractiveMode.connectionQueue), [`getAllQueuedMessages`](../interactive/interactive-mode.ts.md#InteractiveMode.getAllQueuedMessages), [`flatten`](../interactive/queue-selection.ts.md#flatten), [`abortAndClearQueue`](in-process-agent-connection.ts.md#InProcessAgentConnection.abortAndClearQueue), [`getQueue`](in-process-agent-connection.ts.md#InProcessAgentConnection.getQueue), [`queue-selection.ts`](../interactive/queue-selection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-queue-selection.ts), [`abortAndClearQueue`](daemon-agent-connection.ts.md#DaemonAgentConnection.abortAndClearQueue), [`getQueue`](types.ts.md#AgentConnection.getQueue), [`abortAndClearQueue`](types.ts.md#AgentConnection.abortAndClearQueue), [`clearQueue`](in-process-agent-connection.ts.md#InProcessAgentConnection.clearQueue), [`clearQueue`](types.ts.md#AgentConnection.clearQueue), [`clearQueue`](daemon-agent-connection.ts.md#DaemonAgentConnection.clearQueue), [`getQueue`](daemon-agent-connection.ts.md#DaemonAgentConnection.getQueue)  (2 test-only)

### `AgentConnectionQueuedMessageLane`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:521`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L521)
- signature: `type AgentConnectionQueuedMessageLane`
- uses (calls/refs, reference-scoped): [`QueuedMessageLane`](../../core/session-action-store.ts.md#QueuedMessageLane)
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`mutateQueuedMessage`](types.ts.md#AgentConnection.mutateQueuedMessage), [`mutateQueuedMessage`](daemon-agent-connection.ts.md#DaemonAgentConnection.mutateQueuedMessage), [`mutateQueuedMessage`](in-process-agent-connection.ts.md#InProcessAgentConnection.mutateQueuedMessage)

### `AgentConnectionQueuedMessageMutation`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:522`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L522)
- signature: `type AgentConnectionQueuedMessageMutation`
- uses (calls/refs, reference-scoped): [`QueuedMessageMutation`](../../core/session-action-store.ts.md#QueuedMessageMutation)
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`mutateQueuedMessage`](types.ts.md#AgentConnection.mutateQueuedMessage), [`mutateQueuedMessage`](daemon-agent-connection.ts.md#DaemonAgentConnection.mutateQueuedMessage), [`mutateQueuedMessage`](in-process-agent-connection.ts.md#InProcessAgentConnection.mutateQueuedMessage)

### `AgentConnectionQueuedMessageMutationStatus`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:524`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L524)
- doc: "unsupported" is returned only by remote connections whose daemon predates queued-message mutation.
- signature: `type AgentConnectionQueuedMessageMutationStatus`
- uses (calls/refs, reference-scoped): [`QueuedMessageMutationStatus`](../../core/session-action-store.ts.md#QueuedMessageMutationStatus)
- used by: [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`applyQueueSelection`](../interactive/interactive-mode.ts.md#InteractiveMode.applyQueueSelection), [`mutateQueuedMessage`](types.ts.md#AgentConnection.mutateQueuedMessage), [`mutateQueuedMessage`](daemon-agent-connection.ts.md#DaemonAgentConnection.mutateQueuedMessage), [`mutateQueuedMessage`](in-process-agent-connection.ts.md#InProcessAgentConnection.mutateQueuedMessage)

### `AgentConnectionReplayInfo`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:276`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L276)
- signature: `interface AgentConnectionReplayInfo`
- members:
  - `fromCursor` — [`L280`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L280)
  - `fromSequence` — [`L278`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L278)
  - `reason` — [`L282`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L282)
  - `status` — [`L277`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L277)
  - `toCursor` — [`L281`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L281)
  - `toSequence` — [`L279`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L279)
- uses (calls/refs, reference-scoped): [`AgentConnectionEventCursor`](types.ts.md#AgentConnectionEventCursor), [`AgentConnectionReplayStatus`](types.ts.md#AgentConnectionReplayStatus)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`replay`](types.ts.md#AgentConnectionSnapshot.replay)

### `AgentConnectionReplayStatus`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:274`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L274)
- signature: `type AgentConnectionReplayStatus`
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`status`](types.ts.md#AgentConnectionReplayInfo.status)

### `AgentConnectionResourceCollision`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:86`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L86)
- signature: `interface AgentConnectionResourceCollision`
- members:
  - `loserPath` — [`L90`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L90)
  - `loserSource` — [`L92`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L92)
  - `name` — [`L88`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L88)
  - `resourceType` — [`L87`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L87)
  - `winnerPath` — [`L89`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L89)
  - `winnerSource` — [`L91`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L91)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`formatDiagnostics`](../interactive/interactive-mode.ts.md#InteractiveMode.formatDiagnostics), [`collision`](types.ts.md#AgentConnectionResourceDiagnostic.collision)

### `AgentConnectionResourceContextFile`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:375`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L375)
- signature: `interface AgentConnectionResourceContextFile`
- members:
  - `artifact` — [`L377`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L377)
  - `path` — [`L376`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L376)
- uses (calls/refs, reference-scoped): [`AgentConnectionArtifactReference`](types.ts.md#AgentConnectionArtifactReference)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`showLoadedResources`](../interactive/interactive-mode.ts.md#InteractiveMode.showLoadedResources), [`contextFiles`](types.ts.md#AgentConnectionResourceSnapshot.contextFiles)

### `AgentConnectionResourceDiagnostic`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:95`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L95)
- signature: `interface AgentConnectionResourceDiagnostic`
- members:
  - `collision` — [`L99`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L99)
  - `message` — [`L97`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L97)
  - `path` — [`L98`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L98)
  - `type` — [`L96`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L96)
- uses (calls/refs, reference-scoped): [`AgentConnectionResourceCollision`](types.ts.md#AgentConnectionResourceCollision)
- used by: [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`showLoadedResources`](../interactive/interactive-mode.ts.md#InteractiveMode.showLoadedResources), [`formatDiagnostics`](../interactive/interactive-mode.ts.md#InteractiveMode.formatDiagnostics), [`getBuiltInCommandConflictDiagnostics`](../interactive/interactive-mode.ts.md#InteractiveMode.getBuiltInCommandConflictDiagnostics), [`extensions`](types.ts.md#AgentConnectionResourceDiagnostics.extensions), [`prompts`](types.ts.md#AgentConnectionResourceDiagnostics.prompts), [`skills`](types.ts.md#AgentConnectionResourceDiagnostics.skills), [`themes`](types.ts.md#AgentConnectionResourceDiagnostics.themes)  (1 test-only)

### `AgentConnectionResourceDiagnostics`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:410`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L410)
- signature: `interface AgentConnectionResourceDiagnostics`
- members:
  - `extensions` — [`L413`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L413)
  - `prompts` — [`L412`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L412)
  - `skills` — [`L411`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L411)
  - `themes` — [`L414`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L414)
- uses (calls/refs, reference-scoped): [`AgentConnectionResourceDiagnostic`](types.ts.md#AgentConnectionResourceDiagnostic)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`showLoadedResources`](../interactive/interactive-mode.ts.md#InteractiveMode.showLoadedResources), [`createAgentConnectionResourceSnapshot`](snapshot.ts.md#createAgentConnectionResourceSnapshot), [`diagnostics`](types.ts.md#AgentConnectionResourceSnapshot.diagnostics)  (1 test-only)

### `AgentConnectionResourceExtension`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:397`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L397)
- signature: `interface AgentConnectionResourceExtension`
- members:
  - `artifact` — [`L400`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L400)
  - `path` — [`L398`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L398)
  - `sourceInfo` — [`L399`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L399)
- uses (calls/refs, reference-scoped): [`AgentConnectionSourceInfo`](types.ts.md#AgentConnectionSourceInfo), [`AgentConnectionArtifactReference`](types.ts.md#AgentConnectionArtifactReference)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`extensions`](types.ts.md#AgentConnectionResourceSnapshot.extensions)  (1 test-only)

### `AgentConnectionResourcePrompt`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:388`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L388)
- signature: `interface AgentConnectionResourcePrompt`
- members:
  - `argumentHint` — [`L391`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L391)
  - `artifact` — [`L394`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L394)
  - `description` — [`L390`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L390)
  - `filePath` — [`L392`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L392)
  - `name` — [`L389`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L389)
  - `sourceInfo` — [`L393`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L393)
- uses (calls/refs, reference-scoped): [`AgentConnectionSourceInfo`](types.ts.md#AgentConnectionSourceInfo), [`AgentConnectionArtifactReference`](types.ts.md#AgentConnectionArtifactReference)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`showLoadedResources`](../interactive/interactive-mode.ts.md#InteractiveMode.showLoadedResources), [`prompts`](types.ts.md#AgentConnectionResourceSnapshot.prompts)

### `AgentConnectionResourceSkill`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:380`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L380)
- signature: `interface AgentConnectionResourceSkill`
- members:
  - `artifact` — [`L385`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L385)
  - `description` — [`L382`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L382)
  - `filePath` — [`L383`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L383)
  - `name` — [`L381`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L381)
  - `sourceInfo` — [`L384`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L384)
- uses (calls/refs, reference-scoped): [`AgentConnectionSourceInfo`](types.ts.md#AgentConnectionSourceInfo), [`AgentConnectionArtifactReference`](types.ts.md#AgentConnectionArtifactReference)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`showLoadedResources`](../interactive/interactive-mode.ts.md#InteractiveMode.showLoadedResources), [`skills`](types.ts.md#AgentConnectionResourceSnapshot.skills)  (1 test-only)

### `AgentConnectionResourceSnapshot`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:417`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L417)
- signature: `interface AgentConnectionResourceSnapshot`
- members:
  - `contextFiles` — [`L418`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L418)
  - `diagnostics` — [`L423`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L423)
  - `extensions` — [`L421`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L421)
  - `prompts` — [`L420`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L420)
  - `skills` — [`L419`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L419)
  - `themes` — [`L422`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L422)
- uses (calls/refs, reference-scoped): [`AgentConnectionResourceContextFile`](types.ts.md#AgentConnectionResourceContextFile), [`AgentConnectionResourceDiagnostics`](types.ts.md#AgentConnectionResourceDiagnostics), [`AgentConnectionResourceExtension`](types.ts.md#AgentConnectionResourceExtension), [`AgentConnectionResourcePrompt`](types.ts.md#AgentConnectionResourcePrompt), [`AgentConnectionResourceSkill`](types.ts.md#AgentConnectionResourceSkill), [`AgentConnectionResourceTheme`](types.ts.md#AgentConnectionResourceTheme)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`daemon-protocol.ts`](../daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`showLoadedResources`](../interactive/interactive-mode.ts.md#InteractiveMode.showLoadedResources), [`createAgentConnectionResourceSnapshot`](snapshot.ts.md#createAgentConnectionResourceSnapshot), [`snapshot.ts`](snapshot.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-snapshot.ts), [`getResourceSnapshot`](types.ts.md#AgentConnection.getResourceSnapshot), [`getResourceSnapshot`](in-process-agent-connection.ts.md#InProcessAgentConnection.getResourceSnapshot), [`getResourceSnapshot`](daemon-agent-connection.ts.md#DaemonAgentConnection.getResourceSnapshot), [`connectionResourceSnapshot`](../interactive/interactive-mode.ts.md#InteractiveMode.connectionResourceSnapshot), [`DaemonResourceSnapshot`](../daemon/daemon-protocol.ts.md#DaemonResourceSnapshot)  (2 test-only)

### `AgentConnectionResourceTheme`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:403`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L403)
- signature: `interface AgentConnectionResourceTheme`
- members:
  - `artifact` — [`L407`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L407)
  - `name` — [`L404`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L404)
  - `sourceInfo` — [`L406`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L406)
  - `sourcePath` — [`L405`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L405)
- uses (calls/refs, reference-scoped): [`AgentConnectionSourceInfo`](types.ts.md#AgentConnectionSourceInfo), [`AgentConnectionArtifactReference`](types.ts.md#AgentConnectionArtifactReference)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`showLoadedResources`](../interactive/interactive-mode.ts.md#InteractiveMode.showLoadedResources), [`themes`](types.ts.md#AgentConnectionResourceSnapshot.themes)

### `AgentConnectionRlmChildAgentActivity`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:542`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L542)
- signature: `interface AgentConnectionRlmChildAgentActivity`
- members:
  - `kind` — [`L543`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L543)
  - `toolName` — [`L544`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L544)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`activity`](types.ts.md#AgentConnectionRlmChildAgentSnapshot.activity)

### `AgentConnectionRlmChildAgentSnapshot`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:547`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L547)
- signature: `interface AgentConnectionRlmChildAgentSnapshot`
- members:
  - `activeSessionId` — [`L551`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L551) — The child's own daemon active-session id, for attaching to it directly.
  - `activity` — [`L568`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L568)
  - `answerPreview` — [`L559`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L559)
  - `durationMs` — [`L558`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L558)
  - `error` — [`L570`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L570) — Failure reason when status is "error".
  - `id` — [`L548`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L548)
  - `label` — [`L556`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L556)
  - `model` — [`L555`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L555) — Exact provider/model selector used by the child.
  - `parentId` — [`L549`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L549)
  - `recap` — [`L566`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L566) — Latest recap of what the subagent is doing.
  - `repliedSinceTask` — [`L560`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L560)
  - `sessionDir` — [`L567`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L567)
  - `sessionName` — [`L553`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L553) — Stable daemon-visible session name for addressing/displaying the child.
  - `status` — [`L557`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L557)
  - `tokenCount` — [`L564`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L564) — Context size (tokens) of the subagent's latest turn.
  - `toolUseCount` — [`L562`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L562) — Number of tool executions the subagent has started so far.
- uses (calls/refs, reference-scoped): [`AgentConnectionRlmChildAgentActivity`](types.ts.md#AgentConnectionRlmChildAgentActivity), [`AgentConnectionRlmChildAgentStatus`](types.ts.md#AgentConnectionRlmChildAgentStatus)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`daemon-mode.ts`](../daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`daemon-protocol.ts`](../daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`acpUpdatesForSessionEvent`](../acp/acp-events.ts.md#acpUpdatesForSessionEvent), [`rlmChildSnapshotForActiveSession`](../daemon/daemon-session-list.ts.md#rlmChildSnapshotForActiveSession), [`daemon-session-list.ts`](../daemon/daemon-session-list.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-session-list.ts), [`AgentConnectionSessionEvent`](types.ts.md#AgentConnectionSessionEvent), [`buildRlmChildSnapshotsWithPassiveRlmSubagents`](../daemon/daemon-mode.ts.md#AgentDaemon.buildRlmChildSnapshotsWithPassiveRlmSubagents), [`subagent-summary-line.ts`](../interactive/components/subagent-summary-line.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-subagent-summary-line.ts), [`buildRlmChildSnapshots`](../daemon/daemon-session-list.ts.md#buildRlmChildSnapshots), [`countDirectSubagentStatuses`](../interactive/components/subagent-summary-line.ts.md#countDirectSubagentStatuses), [`scopeHeartbeatsToSession`](../interactive/heartbeat-scope.ts.md#scopeHeartbeatsToSession), [`stampRlmChildActiveSessionId`](../daemon/daemon-mode.ts.md#AgentDaemon.stampRlmChildActiveSessionId), [`updateSubagentSummary`](../interactive/interactive-mode.ts.md#InteractiveMode.updateSubagentSummary), [`replaceSubagentSummary`](../interactive/interactive-mode.ts.md#InteractiveMode.replaceSubagentSummary), [`mergeSubagentSnapshot`](../interactive/interactive-mode.ts.md#mergeSubagentSnapshot), [`subagentSnapshots`](../interactive/interactive-mode.ts.md#InteractiveMode.subagentSnapshots), [`seedSubagentSummary`](../interactive/interactive-mode.ts.md#InteractiveMode.seedSubagentSummary), [`removeSubagentSnapshot`](../interactive/interactive-mode.ts.md#InteractiveMode.removeSubagentSnapshot), [`heartbeat-scope.ts`](../interactive/heartbeat-scope.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-heartbeat-scope.ts), [`children`](types.ts.md#AgentConnectionSnapshot.children), [`children`](../daemon/daemon-protocol.ts.md#DaemonSessionSnapshot.children)  (9 test-only)

### `AgentConnectionRlmChildAgentStatus`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:540`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L540)
- signature: `type AgentConnectionRlmChildAgentStatus`
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`status`](types.ts.md#AgentConnectionRlmChildAgentSnapshot.status)

### `AgentConnectionSavedSessionInfo`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:121`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L121)
- doc: Saved-session registry row for the current local TUI migration.
- signature: `interface AgentConnectionSavedSessionInfo`
- members:
  - `agentStatus` — [`L134`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L134)
  - `allMessagesText` — [`L133`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L133)
  - `created` — [`L129`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L129)
  - `cwd` — [`L124`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L124)
  - `firstMessage` — [`L132`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L132)
  - `id` — [`L123`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L123)
  - `messageCount` — [`L131`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L131)
  - `modified` — [`L130`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L130)
  - `name` — [`L125`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L125)
  - `parentSessionPath` — [`L127`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L127)
  - `path` — [`L122`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L122)
  - `rlmDepth` — [`L128`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L128)
  - `state` — [`L126`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L126)
- uses (calls/refs, reference-scoped): [`AgentConnectionSavedSessionState`](types.ts.md#AgentConnectionSavedSessionState), [`AgentConnectionAgentStatus`](types.ts.md#AgentConnectionAgentStatus)
- used by: [`agents-view-mode.ts`](../agents-view/agents-view-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agents-view-agents-view-mode.ts), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`summaryForUnifiedRecord`](../agents-view/agents-view-state.ts.md#summaryForUnifiedRecord), [`deserializeSavedSessionInfo`](../daemon/saved-session-info.ts.md#deserializeSavedSessionInfo), [`reconcileUnifiedSessions`](../agents-view/agents-view-state.ts.md#reconcileUnifiedSessions), [`refreshSavedSessions`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.refreshSavedSessions), [`createUnifiedSearchableText`](../agents-view/agents-view-state.ts.md#createUnifiedSearchableText), [`saved-session-catalog.ts`](../daemon/saved-session-catalog.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-saved-session-catalog.ts), [`listDaemonSavedSessions`](../daemon/saved-session-catalog.ts.md#listDaemonSavedSessions), [`listSavedSessions`](in-process-agent-connection.ts.md#InProcessAgentConnection.listSavedSessions), [`agents-view-state.ts`](../agents-view/agents-view-state.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agents-view-agents-view-state.ts), [`findParentRecord`](../agents-view/agents-view-state.ts.md#findParentRecord), [`saved-session-info.ts`](../daemon/saved-session-info.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-saved-session-info.ts), [`listSavedSessions`](types.ts.md#AgentConnection.listSavedSessions), [`listSavedSessions`](daemon-agent-connection.ts.md#DaemonAgentConnection.listSavedSessions), [`savedIdentityAliases`](../agents-view/agents-view-state.ts.md#savedIdentityAliases), [`AgentConnectionSessionListCallbacks`](types.ts.md#AgentConnectionSessionListCallbacks), [`lastSuccessfulSavedSessions`](../agents-view/agents-view-mode.ts.md#AgentsViewPersistentState.typeLiteral18.lastSuccessfulSavedSessions), [`saved`](../agents-view/agents-view-state.ts.md#UnifiedSessionRecord.saved), [`savedSessions`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.savedSessions), [`savedSessions`](../agents-view/agents-view-mode.ts.md#AgentsViewPersistentState.typeLiteral18.savedSessions), [`lastSuccessfulSavedSessions`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.lastSuccessfulSavedSessions)  (5 test-only)

### `AgentConnectionSavedSessionScope`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L56)
- signature: `type AgentConnectionSavedSessionScope`
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`daemon-protocol.ts`](../daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`saved-session-catalog.ts`](../daemon/saved-session-catalog.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-saved-session-catalog.ts), [`listDaemonSavedSessions`](../daemon/saved-session-catalog.ts.md#listDaemonSavedSessions), [`listSavedSessions`](in-process-agent-connection.ts.md#InProcessAgentConnection.listSavedSessions), [`listSavedSessions`](types.ts.md#AgentConnection.listSavedSessions), [`listSavedSessions`](daemon-agent-connection.ts.md#DaemonAgentConnection.listSavedSessions), [`DaemonSavedSessionListCommand`](../daemon/daemon-protocol.ts.md#DaemonSavedSessionListCommand)

### `AgentConnectionSavedSessionState`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:102`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L102)
- signature: `interface AgentConnectionSavedSessionState`
- members:
  - `status` — [`L103`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L103)
- uses (calls/refs, reference-scoped): [`AgentConnectionSavedSessionStateStatus`](types.ts.md#AgentConnectionSavedSessionStateStatus)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`daemon-protocol.ts`](../daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`AgentConnectionSessionStateEntry`](types.ts.md#AgentConnectionSessionStateEntry), [`state`](../daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.state), [`state`](types.ts.md#AgentConnectionSavedSessionInfo.state)

### `AgentConnectionSavedSessionStateStatus`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:73`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L73)
- signature: `type AgentConnectionSavedSessionStateStatus`
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`AgentConnectionSavedSessionState`](types.ts.md#AgentConnectionSavedSessionState)

### `AgentConnectionScopedModel`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:312`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L312)
- signature: `interface AgentConnectionScopedModel`
- members:
  - `model` — [`L313`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L313)
  - `thinkingLevel` — [`L314`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L314)
- uses (calls/refs, reference-scoped): [`AgentConnectionModel`](types.ts.md#AgentConnectionModel), [`ThinkingLevel`](../../../../agent/src/types.ts.md#ThinkingLevel)
- used by: [`DaemonCommand`](../daemon/daemon-protocol.ts.md#DaemonCommand), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`daemon-protocol.ts`](../daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`showModelsSelector`](../interactive/interactive-mode.ts.md#InteractiveMode.showModelsSelector), [`getCachedModelCandidates`](../interactive/interactive-mode.ts.md#InteractiveMode.getCachedModelCandidates), [`scopedModels`](types.ts.md#AgentConnectionState.scopedModels), [`getScopedModelsFromModelIds`](../interactive/interactive-mode.ts.md#InteractiveMode.getScopedModelsFromModelIds), [`getModelCandidates`](../interactive/interactive-mode.ts.md#InteractiveMode.getModelCandidates), [`setScopedModels`](types.ts.md#AgentConnection.setScopedModels), [`setScopedModels`](in-process-agent-connection.ts.md#InProcessAgentConnection.setScopedModels), [`setScopedModels`](daemon-agent-connection.ts.md#DaemonAgentConnection.setScopedModels)  (2 test-only)

### `AgentConnectionServiceTierChangeEntry`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:161`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L161)
- signature: `interface AgentConnectionServiceTierChangeEntry`
- members:
  - `serviceTier` — [`L163`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L163)
  - `type` — [`L162`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L162)
- uses (calls/refs, reference-scoped): [`ServiceTier`](../../../../ai/src/types.ts.md#ServiceTier), [`AgentConnectionSessionEntryBase`](types.ts.md#AgentConnectionSessionEntryBase)
- used by: [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`AgentConnectionSessionEntry`](types.ts.md#AgentConnectionSessionEntry)  (2 test-only)

### `AgentConnectionSessionContext`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:267`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L267)
- signature: `interface AgentConnectionSessionContext`
- members:
  - `messages` — [`L268`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L268)
  - `model` — [`L271`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L271)
  - `serviceTier` — [`L270`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L270)
  - `thinkingLevel` — [`L269`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L269)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage), [`ServiceTier`](../../../../ai/src/types.ts.md#ServiceTier)
- used by: [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`daemon-protocol.ts`](../daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`limitTranscript`](../interactive/interactive-mode.ts.md#InteractiveMode.renderSessionContext.options-typeLiteral2780.limitTranscript), [`getInitialSnapshot`](daemon-agent-connection.ts.md#DaemonAgentConnection.getInitialSnapshot), [`renderInitialMessages`](../interactive/interactive-mode.ts.md#InteractiveMode.renderInitialMessages), [`getSessionContextFromConnectionSnapshot`](../interactive/interactive-mode.ts.md#InteractiveMode.getSessionContextFromConnectionSnapshot), [`getSessionContext`](daemon-agent-connection.ts.md#DaemonAgentConnection.getSessionContext), [`sessionContext`](types.ts.md#AgentConnectionSnapshot.sessionContext), [`getSessionContext`](in-process-agent-connection.ts.md#InProcessAgentConnection.getSessionContext), [`getSessionContext`](types.ts.md#AgentConnection.getSessionContext), [`sessionContext`](../daemon/daemon-protocol.ts.md#DaemonSessionSnapshot.sessionContext), [`renderSessionContext`](../interactive/interactive-mode.ts.md#InteractiveMode.renderSessionContext)  (7 test-only)

### `AgentConnectionSessionEntry`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:241`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L241)
- signature: `type AgentConnectionSessionEntry`
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionMessageEntry`](types.ts.md#AgentConnectionSessionMessageEntry), [`AgentConnectionSessionStateEntry`](types.ts.md#AgentConnectionSessionStateEntry), [`AgentConnectionModelChangeEntry`](types.ts.md#AgentConnectionModelChangeEntry), [`AgentConnectionAgentStatusEntry`](types.ts.md#AgentConnectionAgentStatusEntry), [`AgentConnectionServiceTierChangeEntry`](types.ts.md#AgentConnectionServiceTierChangeEntry), [`AgentConnectionBranchSummaryEntry`](types.ts.md#AgentConnectionBranchSummaryEntry), [`AgentConnectionChildUsageAttributionEntry`](types.ts.md#AgentConnectionChildUsageAttributionEntry), [`AgentConnectionCompactionEntry`](types.ts.md#AgentConnectionCompactionEntry), [`AgentConnectionCustomEntry`](types.ts.md#AgentConnectionCustomEntry), [`AgentConnectionCustomMessageEntry`](types.ts.md#AgentConnectionCustomMessageEntry), [`AgentConnectionLabelEntry`](types.ts.md#AgentConnectionLabelEntry), [`AgentConnectionSessionInfoEntry`](types.ts.md#AgentConnectionSessionInfoEntry), [`AgentConnectionThinkingLevelChangeEntry`](types.ts.md#AgentConnectionThinkingLevelChangeEntry), [`AgentConnectionGitStateEntry`](types.ts.md#AgentConnectionGitStateEntry)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`entry`](types.ts.md#AgentConnectionSessionTreeFlatNode.entry)  (3 test-only)

### `AgentConnectionSessionEntryBase`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:144`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L144)
- signature: `interface AgentConnectionSessionEntryBase`
- members:
  - `id` — [`L146`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L146)
  - `parentId` — [`L147`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L147)
  - `timestamp` — [`L148`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L148)
  - `type` — [`L145`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L145)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`render`](../interactive/components/tree-selector.ts.md#TreeList.render), [`handleInput`](../interactive/components/tree-selector.ts.md#TreeList.handleInput), [`recalculateVisualStructure`](../interactive/components/tree-selector.ts.md#TreeList.recalculateVisualStructure), [`<constructor>`](../interactive/components/tree-selector.ts.md#TreeList.-constructor), [`buildActivePath`](../interactive/components/tree-selector.ts.md#TreeList.buildActivePath), [`findBranchSegmentStart`](../interactive/components/tree-selector.ts.md#TreeList.findBranchSegmentStart), [`findNearestVisibleIndex`](../interactive/components/tree-selector.ts.md#TreeList.findNearestVisibleIndex), [`buildSessionTreeFromFlatNodes`](daemon-agent-connection.ts.md#buildSessionTreeFromFlatNodes), [`updateNodeLabel`](../interactive/components/tree-selector.ts.md#TreeList.updateNodeLabel), [`AgentConnectionSessionMessageEntry`](types.ts.md#AgentConnectionSessionMessageEntry), [`AgentConnectionSessionStateEntry`](types.ts.md#AgentConnectionSessionStateEntry), [`AgentConnectionModelChangeEntry`](types.ts.md#AgentConnectionModelChangeEntry), [`AgentConnectionAgentStatusEntry`](types.ts.md#AgentConnectionAgentStatusEntry), [`AgentConnectionServiceTierChangeEntry`](types.ts.md#AgentConnectionServiceTierChangeEntry), [`AgentConnectionBranchSummaryEntry`](types.ts.md#AgentConnectionBranchSummaryEntry), [`AgentConnectionChildUsageAttributionEntry`](types.ts.md#AgentConnectionChildUsageAttributionEntry), [`AgentConnectionCompactionEntry`](types.ts.md#AgentConnectionCompactionEntry), [`AgentConnectionCustomEntry`](types.ts.md#AgentConnectionCustomEntry), [`AgentConnectionCustomMessageEntry`](types.ts.md#AgentConnectionCustomMessageEntry), [`AgentConnectionLabelEntry`](types.ts.md#AgentConnectionLabelEntry), [`AgentConnectionSessionInfoEntry`](types.ts.md#AgentConnectionSessionInfoEntry), [`AgentConnectionThinkingLevelChangeEntry`](types.ts.md#AgentConnectionThinkingLevelChangeEntry), [`AgentConnectionGitStateEntry`](types.ts.md#AgentConnectionGitStateEntry)  (8 test-only)

### `AgentConnectionSessionEvent`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:573`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L573)
- signature: `type AgentConnectionSessionEvent`
- uses (calls/refs, reference-scoped): [`ThinkingLevel`](../../../../agent/src/types.ts.md#ThinkingLevel), [`AgentEvent`](../../../../agent/src/types.ts.md#AgentEvent), [`GoalState`](../../core/goals.ts.md#GoalState), [`ServiceTier`](../../../../ai/src/types.ts.md#ServiceTier), [`RefinementResult`](../../core/refinement/refinement.ts.md#RefinementResult), [`AgentConnectionRlmChildAgentSnapshot`](types.ts.md#AgentConnectionRlmChildAgentSnapshot), [`KernelSentAgentMessage`](../../core/kernel/index.ts.md#KernelSentAgentMessage), [`AuthSourceToken`](../../core/auth-storage.ts.md#AuthSourceToken), [`CompactionResult`](../../core/compaction/compaction.ts.md#CompactionResult), [`SessionActionSnapshot`](../../core/session-action-store.ts.md#SessionActionSnapshot)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`handleEvent`](../interactive/interactive-mode.ts.md#InteractiveMode.handleEvent), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`daemon-protocol.ts`](../daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`acpUpdatesForSessionEvent`](../acp/acp-events.ts.md#acpUpdatesForSessionEvent), [`DaemonOutbound`](../daemon/daemon-protocol.ts.md#DaemonOutbound), [`handleEvent`](../interactive/agent-activity.ts.md#AgentActivityTracker.handleEvent), [`AgentConnectionEvent`](types.ts.md#AgentConnectionEvent), [`finishSideQuestionBash`](../interactive/interactive-mode.ts.md#InteractiveMode.finishSideQuestionBash), [`updateConnectionStateFromEvent`](../interactive/interactive-mode.ts.md#InteractiveMode.updateConnectionStateFromEvent), [`acp-events.ts`](../acp/acp-events.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-acp-acp-events.ts), [`applyAuthStaleEvent`](../interactive/interactive-mode.ts.md#InteractiveMode.applyAuthStaleEvent), [`agent-activity.ts`](../interactive/agent-activity.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-agent-activity.ts)  (11 test-only)

### `AgentConnectionSessionHeader`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:58`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L58)
- signature: `interface AgentConnectionSessionHeader`
- members:
  - `branch` — [`L69`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L69)
  - `commit` — [`L68`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L68)
  - `cwd` — [`L63`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L63)
  - `git` — [`L66`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L66)
  - `id` — [`L61`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L61)
  - `parentSession` — [`L64`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L64)
  - `repoUrl` — [`L67`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L67)
  - `rlmDepth` — [`L65`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L65)
  - `timestamp` — [`L62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L62)
  - `type` — [`L59`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L59)
  - `version` — [`L60`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L60)
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`daemon-protocol.ts`](../daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`getSessionHeader`](in-process-agent-connection.ts.md#InProcessAgentConnection.getSessionHeader), [`getSessionHeader`](types.ts.md#AgentConnection.getSessionHeader), [`getSessionHeader`](daemon-agent-connection.ts.md#DaemonAgentConnection.getSessionHeader), [`DaemonSessionHeader`](../daemon/daemon-protocol.ts.md#DaemonSessionHeader)

### `AgentConnectionSessionInfoEntry`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:217`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L217)
- signature: `interface AgentConnectionSessionInfoEntry`
- members:
  - `name` — [`L219`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L219)
  - `type` — [`L218`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L218)
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionEntryBase`](types.ts.md#AgentConnectionSessionEntryBase)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`AgentConnectionSessionEntry`](types.ts.md#AgentConnectionSessionEntry)  (1 test-only)

### `AgentConnectionSessionListCallbacks`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:139`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L139)
- signature: `interface AgentConnectionSessionListCallbacks`
- members:
  - `onProgress` — [`L140`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L140)
  - `onSession` — [`L141`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L141)
- uses (calls/refs, reference-scoped): [`AgentConnectionSavedSessionInfo`](types.ts.md#AgentConnectionSavedSessionInfo), [`AgentConnectionSessionListProgress`](types.ts.md#AgentConnectionSessionListProgress)
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`saved-session-catalog.ts`](../daemon/saved-session-catalog.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-saved-session-catalog.ts), [`listDaemonSavedSessions`](../daemon/saved-session-catalog.ts.md#listDaemonSavedSessions), [`listSavedSessions`](in-process-agent-connection.ts.md#InProcessAgentConnection.listSavedSessions), [`listSavedSessions`](types.ts.md#AgentConnection.listSavedSessions), [`listSavedSessions`](daemon-agent-connection.ts.md#DaemonAgentConnection.listSavedSessions)

### `AgentConnectionSessionListProgress`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:137`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L137)
- signature: `type AgentConnectionSessionListProgress`
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`onProgress`](types.ts.md#AgentConnectionSessionListCallbacks.onProgress)

### `AgentConnectionSessionMessageEntry`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:151`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L151)
- signature: `interface AgentConnectionSessionMessageEntry`
- members:
  - `message` — [`L153`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L153)
  - `type` — [`L152`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L152)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage), [`AgentConnectionSessionEntryBase`](types.ts.md#AgentConnectionSessionEntryBase)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`AgentConnectionSessionEntry`](types.ts.md#AgentConnectionSessionEntry)  (5 test-only)

### `AgentConnectionSessionStateEntry`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:222`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L222)
- signature: `interface AgentConnectionSessionStateEntry`
- members:
  - `state` — [`L224`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L224)
  - `type` — [`L223`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L223)
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionEntryBase`](types.ts.md#AgentConnectionSessionEntryBase), [`AgentConnectionSavedSessionState`](types.ts.md#AgentConnectionSavedSessionState)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`AgentConnectionSessionEntry`](types.ts.md#AgentConnectionSessionEntry)  (1 test-only)

### `AgentConnectionSessionTreeFlatNode`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:257`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L257)
- signature: `interface AgentConnectionSessionTreeFlatNode`
- members:
  - `entry` — [`L258`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L258)
  - `label` — [`L259`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L259)
  - `labelTimestamp` — [`L260`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L260)
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionEntry`](types.ts.md#AgentConnectionSessionEntry)
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`render`](../interactive/components/tree-selector.ts.md#TreeList.render), [`handleInput`](../interactive/components/tree-selector.ts.md#TreeList.handleInput), [`recalculateVisualStructure`](../interactive/components/tree-selector.ts.md#TreeList.recalculateVisualStructure), [`<constructor>`](../interactive/components/tree-selector.ts.md#TreeList.-constructor), [`AgentConnectionSessionTreeNode`](types.ts.md#AgentConnectionSessionTreeNode), [`buildActivePath`](../interactive/components/tree-selector.ts.md#TreeList.buildActivePath), [`findBranchSegmentStart`](../interactive/components/tree-selector.ts.md#TreeList.findBranchSegmentStart), [`findNearestVisibleIndex`](../interactive/components/tree-selector.ts.md#TreeList.findNearestVisibleIndex), [`buildSessionTreeFromFlatNodes`](daemon-agent-connection.ts.md#buildSessionTreeFromFlatNodes), [`getSessionTree`](daemon-agent-connection.ts.md#DaemonAgentConnection.getSessionTree), [`updateNodeLabel`](../interactive/components/tree-selector.ts.md#TreeList.updateNodeLabel)  (3 test-only)

### `AgentConnectionSessionTreeNode`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:263`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L263)
- signature: `interface AgentConnectionSessionTreeNode`
- members:
  - `children` — [`L264`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L264)
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionTreeFlatNode`](types.ts.md#AgentConnectionSessionTreeFlatNode)
- used by: [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`daemon-protocol.ts`](../daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`showTreeSelector`](../interactive/interactive-mode.ts.md#InteractiveMode.showTreeSelector), [`<constructor>`](../interactive/components/tree-selector.ts.md#TreeSelectorComponent.-constructor), [`getSelectedNode`](../interactive/components/tree-selector.ts.md#TreeList.getSelectedNode), [`tree-selector.ts`](../interactive/components/tree-selector.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-tree-selector.ts), [`<constructor>`](../interactive/components/tree-selector.ts.md#TreeList.-constructor), [`node`](../interactive/components/tree-selector.ts.md#FlatNode.node), [`buildSessionTreeFromFlatNodes`](daemon-agent-connection.ts.md#buildSessionTreeFromFlatNodes), [`tree`](types.ts.md#AgentConnection.getSessionTree.Promise.typeLiteral133.tree), [`tree`](daemon-agent-connection.ts.md#DaemonAgentConnection.getSessionTree.Promise.typeLiteral440.tree), [`tree`](in-process-agent-connection.ts.md#InProcessAgentConnection.getSessionTree.Promise.typeLiteral24.tree), [`tree`](types.ts.md#AgentConnectionSnapshot.sessionTree.typeLiteral11.tree), [`tree`](../daemon/daemon-protocol.ts.md#DaemonSessionSnapshot.sessionTree.typeLiteral26.tree)  (3 test-only)

### `AgentConnectionSessionWatcher`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:755`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L755)
- signature: `interface AgentConnectionSessionWatcher`
- members:
  - `close(method)` — [`L760`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L760)
  - `getCommands(method)` — [`L757`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L757)
  - `getMessages(method)` — [`L756`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L756)
  - `getToolDefinition(method)` — [`L759`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L759)
  - `subscribe(method)` — [`L758`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L758)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage), [`AgentConnectionEventListener`](types.ts.md#AgentConnectionEventListener), [`AgentConnectionSlashCommand`](types.ts.md#AgentConnectionSlashCommand), [`AgentConnectionToolDefinition`](types.ts.md#AgentConnectionToolDefinition)
- used by: [`runRpcModeWithConnectionInternal`](../rpc/rpc-mode.ts.md#runRpcModeWithConnectionInternal), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`rpc-mode.ts`](../rpc/rpc-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-mode.ts), [`watchSession`](daemon-agent-connection.ts.md#DaemonAgentConnection.watchSession), [`watchSession`](in-process-agent-connection.ts.md#InProcessAgentConnection.watchSession), [`watchSession`](types.ts.md#AgentConnection.watchSession)

### `AgentConnectionSideQuestionEvent`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:461`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L461)
- signature: `interface AgentConnectionSideQuestionEvent`
- members:
  - `answer` — [`L464`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L464)
  - `errorMessage` — [`L466`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L466)
  - `id` — [`L462`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L462)
  - `question` — [`L463`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L463)
  - `status` — [`L465`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L465)
- used by: [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`setupEditorSubmitHandler`](../interactive/interactive-mode.ts.md#InteractiveMode.setupEditorSubmitHandler), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`daemon-protocol.ts`](../daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`DaemonOutbound`](../daemon/daemon-protocol.ts.md#DaemonOutbound), [`handleSideQuestion`](../interactive/interactive-mode.ts.md#InteractiveMode.handleSideQuestion), [`render`](../interactive/components/side-question.ts.md#SideQuestionComponent.render), [`AgentConnectionEvent`](types.ts.md#AgentConnectionEvent), [`clearSideQuestion`](../interactive/interactive-mode.ts.md#InteractiveMode.clearSideQuestion), [`addTurn`](../interactive/components/side-question.ts.md#SideQuestionComponent.addTurn), [`finishSideQuestionBash`](../interactive/interactive-mode.ts.md#InteractiveMode.finishSideQuestionBash), [`interruptOrClearInput`](../interactive/interactive-mode.ts.md#InteractiveMode.interruptOrClearInput), [`side-question.ts`](../interactive/components/side-question.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-side-question.ts), [`renderAnswer`](../interactive/components/side-question.ts.md#SideQuestionComponent.renderAnswer), [`renderHint`](../interactive/components/side-question.ts.md#SideQuestionComponent.renderHint), [`handleSideQuestionEvent`](../interactive/interactive-mode.ts.md#InteractiveMode.handleSideQuestionEvent), [`update`](../interactive/components/side-question.ts.md#SideQuestionComponent.update), [`hasInterruptibleWork`](../interactive/interactive-mode.ts.md#InteractiveMode.hasInterruptibleWork), [`<constructor>`](../interactive/components/side-question.ts.md#SideQuestionComponent.-constructor), [`event`](../interactive/components/side-question.ts.md#SideQuestionTurnState.event), [`sideQuestionEvent`](../interactive/interactive-mode.ts.md#InteractiveMode.sideQuestionEvent), [`observeSideQuestionEvent`](daemon-agent-connection.ts.md#DaemonAgentConnection.observeSideQuestionEvent), [`sideQuestionTurns`](../interactive/interactive-mode.ts.md#InteractiveMode.sideQuestionTurns)  (1 test-only)

### `AgentConnectionSideQuestionTurn`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:469`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L469)
- signature: `interface AgentConnectionSideQuestionTurn`
- members:
  - `answer` — [`L471`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L471)
  - `question` — [`L470`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L470)
- used by: [`DaemonCommand`](../daemon/daemon-protocol.ts.md#DaemonCommand), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`daemon-protocol.ts`](../daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`startSideQuestion`](in-process-agent-connection.ts.md#InProcessAgentConnection.startSideQuestion), [`startSideQuestion`](daemon-agent-connection.ts.md#DaemonAgentConnection.startSideQuestion), [`startSideQuestion`](types.ts.md#AgentConnection.startSideQuestion)  (1 test-only)

### `AgentConnectionSlashCommand`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:355`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L355)
- signature: `interface AgentConnectionSlashCommand`
- members:
  - `argumentHint` — [`L359`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L359)
  - `description` — [`L358`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L358)
  - `name` — [`L356`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L356)
  - `registeredName` — [`L357`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L357)
  - `source` — [`L360`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L360)
  - `sourceInfo` — [`L361`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L361)
- uses (calls/refs, reference-scoped): [`AgentConnectionSourceInfo`](types.ts.md#AgentConnectionSourceInfo)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`setupEditorSubmitHandler`](../interactive/interactive-mode.ts.md#InteractiveMode.setupEditorSubmitHandler), [`runRpcModeWithConnectionInternal`](../rpc/rpc-mode.ts.md#runRpcModeWithConnectionInternal), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`createBaseAutocompleteProvider`](../interactive/interactive-mode.ts.md#InteractiveMode.createBaseAutocompleteProvider), [`createAgentConnectionCommands`](snapshot.ts.md#createAgentConnectionCommands), [`snapshot.ts`](snapshot.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-snapshot.ts), [`getBuiltInCommandConflictDiagnostics`](../interactive/interactive-mode.ts.md#InteractiveMode.getBuiltInCommandConflictDiagnostics), [`isRecognizedSlashCommand`](../interactive/interactive-mode.ts.md#InteractiveMode.isRecognizedSlashCommand), [`getCommands`](types.ts.md#AgentConnection.getCommands), [`connectionCommands`](../interactive/interactive-mode.ts.md#InteractiveMode.connectionCommands), [`getCommands`](in-process-agent-connection.ts.md#InProcessAgentConnection.getCommands), [`getCommands`](daemon-agent-connection.ts.md#DaemonAgentConnection.getCommands), [`getCommands`](types.ts.md#AgentConnectionSessionWatcher.getCommands)  (1 test-only)

### `AgentConnectionSnapshot`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:297`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L297)
- signature: `interface AgentConnectionSnapshot`
- members:
  - `children` — [`L306`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L306) — Live RLM child agents (including grandchildren) known to the host at snapshot time.
  - `lastEventCursor` — [`L308`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L308)
  - `lastEventSequence` — [`L307`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L307)
  - `leafId` — [`L303`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L303)
  - `messages` — [`L299`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L299)
  - `parent` — [`L304`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L304)
  - `replay` — [`L309`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L309)
  - `sessionContext` — [`L302`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L302)
  - `sessionTree` — [`L303`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L303)
  - `state` — [`L298`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L298)
  - `streamingMessage` — [`L301`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L301) — In-flight assistant message, kept separate from finalized transcript messages.
  - `tree` — [`L303`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L303)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage), [`AgentConnectionState`](types.ts.md#AgentConnectionState), [`AgentConnectionRlmChildAgentSnapshot`](types.ts.md#AgentConnectionRlmChildAgentSnapshot), [`AgentConnectionSessionTreeNode`](types.ts.md#AgentConnectionSessionTreeNode), [`AgentConnectionSessionContext`](types.ts.md#AgentConnectionSessionContext), [`AgentConnectionEventCursor`](types.ts.md#AgentConnectionEventCursor), [`AgentConnectionParentMetadata`](types.ts.md#AgentConnectionParentMetadata), [`AgentConnectionReplayInfo`](types.ts.md#AgentConnectionReplayInfo)
- used by: [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`attach`](daemon-agent-connection.ts.md#DaemonAgentConnection.attach), [`handleDaemonMessage`](daemon-agent-connection.ts.md#DaemonAgentConnection.handleDaemonMessage), [`renderResyncedSession`](../interactive/interactive-mode.ts.md#InteractiveMode.renderResyncedSession), [`mapDaemonSessionSnapshot`](daemon-agent-connection.ts.md#mapDaemonSessionSnapshot), [`getInitialSnapshot`](daemon-agent-connection.ts.md#DaemonAgentConnection.getInitialSnapshot), [`AgentConnectionEvent`](types.ts.md#AgentConnectionEvent), [`renderInitialMessages`](../interactive/interactive-mode.ts.md#InteractiveMode.renderInitialMessages), [`latestSnapshot`](daemon-agent-connection.ts.md#DaemonAgentConnection.latestSnapshot), [`snapshot.ts`](snapshot.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-snapshot.ts), [`createAgentConnectionSnapshot`](snapshot.ts.md#createAgentConnectionSnapshot), [`getSessionContextFromConnectionSnapshot`](../interactive/interactive-mode.ts.md#InteractiveMode.getSessionContextFromConnectionSnapshot), [`recoverFailedSnapshot`](daemon-agent-connection.ts.md#DaemonAgentConnection.recoverFailedSnapshot), [`observeStreamingMessage`](daemon-agent-connection.ts.md#DaemonAgentConnection.observeStreamingMessage), [`getState`](daemon-agent-connection.ts.md#DaemonAgentConnection.getState), [`getMessages`](daemon-agent-connection.ts.md#DaemonAgentConnection.getMessages), [`getSessionTree`](daemon-agent-connection.ts.md#DaemonAgentConnection.getSessionTree), [`getSessionContext`](daemon-agent-connection.ts.md#DaemonAgentConnection.getSessionContext), [`getInitialSnapshot`](types.ts.md#AgentConnection.getInitialSnapshot), [`getInitialSnapshot`](in-process-agent-connection.ts.md#InProcessAgentConnection.getInitialSnapshot)  (4 test-only)

### `AgentConnectionSourceInfo`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:78`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L78)
- signature: `interface AgentConnectionSourceInfo`
- members:
  - `baseDir` — [`L83`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L83)
  - `origin` — [`L82`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L82)
  - `path` — [`L79`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L79)
  - `scope` — [`L81`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L81)
  - `source` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L80)
- uses (calls/refs, reference-scoped): [`AgentConnectionSourceOrigin`](types.ts.md#AgentConnectionSourceOrigin), [`AgentConnectionSourceScope`](types.ts.md#AgentConnectionSourceScope)
- used by: [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`showLoadedResources`](../interactive/interactive-mode.ts.md#InteractiveMode.showLoadedResources), [`rpc-types.ts`](../rpc/rpc-types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-types.ts), [`formatDiagnostics`](../interactive/interactive-mode.ts.md#InteractiveMode.formatDiagnostics), [`formatPackagePath`](../interactive/interactive-mode.ts.md#InteractiveMode.formatScopeGroups.options-typeLiteral862.formatPackagePath), [`getBuiltInCommandConflictDiagnostics`](../interactive/interactive-mode.ts.md#InteractiveMode.getBuiltInCommandConflictDiagnostics), [`getCompactExtensionLabels`](../interactive/interactive-mode.ts.md#InteractiveMode.getCompactExtensionLabels), [`color`](../interactive/interactive-mode.ts.md#InteractiveMode.getDisplaySourceInfo.typeLiteral800.color), [`getAutocompleteSourceTag`](../interactive/interactive-mode.ts.md#InteractiveMode.getAutocompleteSourceTag), [`getShortPath`](../interactive/interactive-mode.ts.md#InteractiveMode.getShortPath), [`formatPathWithSource`](../interactive/interactive-mode.ts.md#InteractiveMode.formatPathWithSource), [`getCompactExtensionLabel`](../interactive/interactive-mode.ts.md#InteractiveMode.getCompactExtensionLabel), [`sourceInfo`](../interactive/interactive-mode.ts.md#InteractiveMode.buildScopeGroups.Array.typeLiteral820.packages.Map.Array.typeLiteral822.sourceInfo), [`getCompactPackageSourceLabel`](../interactive/interactive-mode.ts.md#InteractiveMode.getCompactPackageSourceLabel), [`getCompactPathLabel`](../interactive/interactive-mode.ts.md#InteractiveMode.getCompactPathLabel), [`isPackageSource`](../interactive/interactive-mode.ts.md#InteractiveMode.isPackageSource), [`getScopeGroup`](../interactive/interactive-mode.ts.md#InteractiveMode.getScopeGroup), [`getAutocompleteSourceLabel`](../interactive/interactive-mode.ts.md#InteractiveMode.getAutocompleteSourceLabel), [`formatPath`](../interactive/interactive-mode.ts.md#InteractiveMode.formatScopeGroups.options-typeLiteral862.formatPath), [`sourceInfo`](types.ts.md#AgentConnectionSlashCommand.sourceInfo), [`sourceInfo`](types.ts.md#AgentConnectionResourceTheme.sourceInfo), [`findSourceInfoForPath`](../interactive/interactive-mode.ts.md#InteractiveMode.findSourceInfoForPath), [`sourceInfo`](types.ts.md#AgentConnectionResourcePrompt.sourceInfo), [`sourceInfo`](types.ts.md#AgentConnectionResourceSkill.sourceInfo), [`sourceInfo`](../interactive/interactive-mode.ts.md#InteractiveMode.buildScopeGroups.items-Array.typeLiteral819.sourceInfo), [`sourceInfo`](../interactive/interactive-mode.ts.md#InteractiveMode.showLoadedResources.options-typeLiteral987.extensions.Array.typeLiteral988.sourceInfo), [`getDisplaySourceInfo`](../interactive/interactive-mode.ts.md#InteractiveMode.getDisplaySourceInfo), [`sourceInfo`](types.ts.md#AgentConnectionResourceExtension.sourceInfo), [`sourceInfo`](../interactive/interactive-mode.ts.md#InteractiveMode.buildScopeGroups.Array.typeLiteral820.paths.Array.typeLiteral821.sourceInfo), [`sourceInfo`](../interactive/interactive-mode.ts.md#InteractiveMode.formatScopeGroups.groups-Array.typeLiteral859.packages.Map.Array.typeLiteral861.sourceInfo), [`sourceInfo`](../interactive/interactive-mode.ts.md#InteractiveMode.formatScopeGroups.groups-Array.typeLiteral859.paths.Array.typeLiteral860.sourceInfo), [`sourceInfo`](../rpc/rpc-types.ts.md#RpcSlashCommand.sourceInfo)  (2 test-only)

### `AgentConnectionSourceOrigin`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:76`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L76)
- signature: `type AgentConnectionSourceOrigin`
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`origin`](types.ts.md#AgentConnectionSourceInfo.origin)

### `AgentConnectionSourceScope`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:75`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L75)
- signature: `type AgentConnectionSourceScope`
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`scope`](types.ts.md#AgentConnectionSourceInfo.scope)

### `AgentConnectionState`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:324`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L324)
- signature: `interface AgentConnectionState`
- members:
  - `activeSessionId` — [`L325`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L325)
  - `activeToolNames` — [`L349`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L349)
  - `autoCompactionEnabled` — [`L342`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L342)
  - `availableThinkingLevels` — [`L330`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L330)
  - `compactionCount` — [`L345`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L345)
  - `contextUsage` — [`L350`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L350)
  - `cwd` — [`L326`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L326)
  - `followUpMode` — [`L336`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L336)
  - `goal` — [`L346`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L346)
  - `heartbeat` — [`L347`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L347)
  - `isBashRunning` — [`L333`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L333)
  - `isCompacting` — [`L332`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L332)
  - `isStreaming` — [`L331`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L331)
  - `leafId` — [`L341`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L341)
  - `messageCount` — [`L343`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L343)
  - `model` — [`L327`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L327)
  - `recap` — [`L352`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L352) — One-line recap of the agent's recent work, shown above the prompt.
  - `retryAttempt` — [`L334`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L334)
  - `scopedModels` — [`L348`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L348)
  - `serviceTier` — [`L329`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L329)
  - `sessionActions` — [`L344`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L344)
  - `sessionDir` — [`L340`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L340)
  - `sessionFile` — [`L337`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L337)
  - `sessionId` — [`L338`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L338)
  - `sessionName` — [`L339`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L339)
  - `steeringMode` — [`L335`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L335)
  - `thinkingLevel` — [`L328`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L328)
- uses (calls/refs, reference-scoped): [`AgentCronJob`](../../core/cron-jobs.ts.md#AgentCronJob), [`AgentConnectionModel`](types.ts.md#AgentConnectionModel), [`ThinkingLevel`](../../../../agent/src/types.ts.md#ThinkingLevel), [`GoalState`](../../core/goals.ts.md#GoalState), [`ServiceTier`](../../../../ai/src/types.ts.md#ServiceTier), [`SessionStats`](../../core/session-stats.ts.md#SessionStats), [`AgentConnectionQueueMode`](types.ts.md#AgentConnectionQueueMode), [`contextUsage`](../../core/session-stats.ts.md#SessionStats.contextUsage), [`SessionActionSnapshot`](../../core/session-action-store.ts.md#SessionActionSnapshot), [`AgentConnectionScopedModel`](types.ts.md#AgentConnectionScopedModel)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`main`](../../main.ts.md#main), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`showSettingsSelector`](../interactive/interactive-mode.ts.md#InteractiveMode.showSettingsSelector), [`setupEditorSubmitHandler`](../interactive/interactive-mode.ts.md#InteractiveMode.setupEditorSubmitHandler), [`runRpcModeWithConnectionInternal`](../rpc/rpc-mode.ts.md#runRpcModeWithConnectionInternal), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`daemon-protocol.ts`](../daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`createAgentConnectionState`](snapshot.ts.md#createAgentConnectionState), [`attach`](daemon-agent-connection.ts.md#DaemonAgentConnection.attach), [`runAgentsViewMode`](../agents-view/agents-view-mode.ts.md#runAgentsViewMode), [`DaemonOutbound`](../daemon/daemon-protocol.ts.md#DaemonOutbound), [`run`](../interactive/interactive-mode.ts.md#InteractiveMode.run), [`runAcpModeWithConnection`](../acp/acp-mode.ts.md#runAcpModeWithConnection), [`handleDaemonMessage`](daemon-agent-connection.ts.md#DaemonAgentConnection.handleDaemonMessage), [`handleTracesCommand`](../interactive/interactive-mode.ts.md#InteractiveMode.handleTracesCommand), [`handleUpdateCommand`](../interactive/interactive-mode.ts.md#InteractiveMode.handleUpdateCommand), [`renderResyncedSession`](../interactive/interactive-mode.ts.md#InteractiveMode.renderResyncedSession), [`completeSnapshotAssembly`](daemon-agent-connection.ts.md#DaemonAgentConnection.completeSnapshotAssembly), [`showModelsSelector`](../interactive/interactive-mode.ts.md#InteractiveMode.showModelsSelector), [`daemon-extension-binding.ts`](../daemon/daemon-extension-binding.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-extension-binding.ts), [`subscribeToAgent`](../interactive/interactive-mode.ts.md#InteractiveMode.subscribeToAgent), [`applyRuntimeSettings`](../interactive/interactive-mode.ts.md#InteractiveMode.applyRuntimeSettings), [`applySelectedModel`](../interactive/interactive-mode.ts.md#InteractiveMode.applySelectedModel), [`getInitialSnapshot`](daemon-agent-connection.ts.md#DaemonAgentConnection.getInitialSnapshot), [`AgentConnectionEvent`](types.ts.md#AgentConnectionEvent), [`renderInitialMessages`](../interactive/interactive-mode.ts.md#InteractiveMode.renderInitialMessages), [`handleMessage`](../../cli/daemon-command.ts.md#DaemonAttachTerminal.handleMessage), [`snapshot.ts`](snapshot.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-snapshot.ts), [`connectionState`](../interactive/interactive-mode.ts.md#InteractiveMode.connectionState), [`patchConnectionState`](../interactive/interactive-mode.ts.md#InteractiveMode.patchConnectionState), [`handleFastCommand`](../interactive/interactive-mode.ts.md#InteractiveMode.handleFastCommand), [`manageHeartbeat`](../interactive/interactive-mode.ts.md#InteractiveMode.manageHeartbeat), [`applyReplacementSnapshot`](daemon-agent-connection.ts.md#DaemonAgentConnection.applyReplacementSnapshot), [`getSessionContextFromConnectionSnapshot`](../interactive/interactive-mode.ts.md#InteractiveMode.getSessionContextFromConnectionSnapshot), [`handleHeartbeatCommand`](../interactive/interactive-mode.ts.md#InteractiveMode.handleHeartbeatCommand), [`recoverFailedSnapshot`](daemon-agent-connection.ts.md#DaemonAgentConnection.recoverFailedSnapshot)  (+33 more; 18 test-only)

### `AgentConnectionSwitchSessionOptions`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:494`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L494)
- signature: `interface AgentConnectionSwitchSessionOptions`
- members:
  - `cwdOverride` — [`L495`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L495)
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`cancelled`](daemon-agent-connection.ts.md#DaemonAgentConnection.switchSession.Promise.typeLiteral664.cancelled), [`switchSession`](types.ts.md#AgentConnection.switchSession), [`switchSession`](daemon-agent-connection.ts.md#DaemonAgentConnection.switchSession), [`switchSession`](in-process-agent-connection.ts.md#InProcessAgentConnection.switchSession)

### `AgentConnectionThinkingLevelChangeEntry`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:156`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L156)
- signature: `interface AgentConnectionThinkingLevelChangeEntry`
- members:
  - `thinkingLevel` — [`L158`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L158)
  - `type` — [`L157`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L157)
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionEntryBase`](types.ts.md#AgentConnectionSessionEntryBase)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`getEntryDisplayText`](../interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`applyFilter`](../interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](../interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`AgentConnectionSessionEntry`](types.ts.md#AgentConnectionSessionEntry)  (1 test-only)

### `AgentConnectionToolDefinition`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:426`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L426)
- signature: `interface AgentConnectionToolDefinition`
- members:
  - `description` — [`L429`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L429)
  - `label` — [`L428`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L428)
  - `name` — [`L427`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L427)
  - `parameters` — [`L432`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L432)
  - `promptGuidelines` — [`L431`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L431)
  - `promptSnippet` — [`L430`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L430)
  - `renderShell` — [`L433`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L433)
  - `replayBuiltInToolName` — [`L434`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L434)
- uses (calls/refs, reference-scoped): [`ReplayBuiltInToolName`](../../core/extensions/types.ts.md#ReplayBuiltInToolName)
- used by: [`interactive-mode.ts`](../interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`updateDisplay`](../interactive/components/tool-execution.ts.md#ToolExecutionComponent.updateDisplay), [`tool-execution.ts`](../interactive/components/tool-execution.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-tool-execution.ts), [`createToolExecutionDefinition`](../interactive/interactive-mode.ts.md#InteractiveMode.createToolExecutionDefinition), [`createAgentConnectionToolDefinition`](tool-definition.ts.md#createAgentConnectionToolDefinition), [`panelHeader`](../interactive/components/tool-execution.ts.md#ToolExecutionComponent.panelHeader), [`ToolExecutionDefinition`](../interactive/components/tool-execution.ts.md#ToolExecutionDefinition), [`getRenderShell`](../interactive/components/tool-execution.ts.md#ToolExecutionComponent.getRenderShell), [`tool-definition.ts`](tool-definition.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-tool-definition.ts), [`getToolDefinition`](in-process-agent-connection.ts.md#InProcessAgentConnection.getToolDefinition), [`getToolDefinition`](types.ts.md#AgentConnection.getToolDefinition), [`matchesBuiltInReplayMetadata`](../interactive/components/tool-execution.ts.md#matchesBuiltInReplayMetadata), [`getToolDefinition`](daemon-agent-connection.ts.md#DaemonAgentConnection.getToolDefinition), [`getToolDefinition`](types.ts.md#AgentConnectionSessionWatcher.getToolDefinition)

### `AgentConnectionUserMessage`
- def: [`packages/coding-agent/src/modes/agent-connection/types.ts:511`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L511)
- signature: `interface AgentConnectionUserMessage`
- members:
  - `entryId` — [`L512`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L512)
  - `text` — [`L513`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/types.ts#L513)
- used by: [`daemon-agent-connection.ts`](daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-index.ts), [`getUserMessagesForForking`](types.ts.md#AgentConnection.getUserMessagesForForking), [`getUserMessagesForForking`](in-process-agent-connection.ts.md#InProcessAgentConnection.getUserMessagesForForking), [`getUserMessagesForForking`](daemon-agent-connection.ts.md#DaemonAgentConnection.getUserMessagesForForking)


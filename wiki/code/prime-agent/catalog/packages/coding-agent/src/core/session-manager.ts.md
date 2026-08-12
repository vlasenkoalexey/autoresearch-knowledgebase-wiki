---
title: 'Module: packages/coding-agent/src/core/session-manager.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/session-manager.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`session-manager.ts`/
symbols:
  SessionManager: SessionManager#
  SessionManager.appendMessage: SessionManager#appendMessage().
  CompactionEntry.type: CompactionEntry#type.
  CustomEntry.type: CustomEntry#type.
  LabelEntry.type: LabelEntry#type.
  ModelChangeEntry.type: ModelChangeEntry#type.
  ChildUsageAttributionEntry.type: ChildUsageAttributionEntry#type.
  SessionInfoEntry.type: SessionInfoEntry#type.
  AgentStatusEntry.type: AgentStatusEntry#type.
  GitStateEntry.type: GitStateEntry#type.
  BranchSummaryEntry.type: BranchSummaryEntry#type.
  SessionStateEntry.type: SessionStateEntry#type.
  ThinkingLevelChangeEntry.type: ThinkingLevelChangeEntry#type.
  ServiceTierChangeEntry.type: ServiceTierChangeEntry#type.
  CustomMessageEntry.type: CustomMessageEntry#type.
  SessionMessageEntry.type: SessionMessageEntry#type.
  SessionEntryBase.id: SessionEntryBase#id.
  buildSessionContext: buildSessionContext().
  SessionManager.createBranchedSession: SessionManager#createBranchedSession().
  SessionManager.getEntries: SessionManager#getEntries().
  SessionManager.newSession: SessionManager#newSession().
  SessionManager.getSessionFile: SessionManager#getSessionFile().
  SessionManager.create: SessionManager#create().
  SessionEntry: SessionEntry#
  scanSessionInfo: scanSessionInfo().
  SessionManager.inMemory: SessionManager#inMemory().
  SessionManager.open: SessionManager#open().
  SessionManager.appendChildUsageAttribution: SessionManager#appendChildUsageAttribution().
  SessionManager.forkFrom: SessionManager#forkFrom().
  SessionContext.messages: SessionContext#messages.
  SessionMessageEntry.message: SessionMessageEntry#message.
  SessionManager.getHeader: SessionManager#getHeader().
  SessionManager.setSessionFile: SessionManager#setSessionFile().
  applyChildUsageAttributions: applyChildUsageAttributions().
  SessionManager._persist: SessionManager#_persist().
  SessionEntryBase.parentId: SessionEntryBase#parentId.
  SessionManager.materializeSessionFile: SessionManager#materializeSessionFile().
  SessionManager.appendSessionState: SessionManager#appendSessionState().
  SessionInfo: SessionInfo#
  SessionManager.getSessionId: SessionManager#getSessionId().
  SessionInfo.id: SessionInfo#id.
  SessionManager._buildIndex: SessionManager#_buildIndex().
  updateLastActivityTime: updateLastActivityTime().
  SessionEntryBase.timestamp: SessionEntryBase#timestamp.
  SessionInfo.path: SessionInfo#path.
  SessionHeader.type: SessionHeader#type.
  migrateV1ToV2: migrateV1ToV2().
  SessionManager.getActiveGitContext: SessionManager#getActiveGitContext().
  migrateToCurrentVersion: migrateToCurrentVersion().
  SessionManager.getSessionState: SessionManager#getSessionState().
  SessionManager.appendLabelChange: SessionManager#appendLabelChange().
  SessionManager.getLatestAgentStatus: SessionManager#getLatestAgentStatus().
  SessionState.status: SessionState#status.
  readSessionInfo: readSessionInfo().
  SessionManager.appendSessionInfo: SessionManager#appendSessionInfo().
  SessionManager.getSessionName: SessionManager#getSessionName().
  SessionManager.hasUserContent: SessionManager#hasUserContent().
  SessionManager.getBranch: SessionManager#getBranch().
  migrateV2ToV3: migrateV2ToV3().
  SessionManager.appendCompaction: SessionManager#appendCompaction().
  SessionManager.appendCustomEntry: SessionManager#appendCustomEntry().
  finalizeLoadedEntries: finalizeLoadedEntries().
  SessionManager.appendCustomMessageEntry: SessionManager#appendCustomMessageEntry().
  getLatestCompactionEntry: getLatestCompactionEntry().
  SessionManager.flushNow: SessionManager#flushNow().
  SessionManager.getCwd: SessionManager#getCwd().
  SessionManager.getSessionArtifactDir: SessionManager#getSessionArtifactDir().
  SessionManager.appendAgentStatus: SessionManager#appendAgentStatus().
  SessionManager.appendThinkingLevelChange: SessionManager#appendThinkingLevelChange().
  SessionManager.appendModelChange: SessionManager#appendModelChange().
  SessionManager.list: SessionManager#list().
  SessionManager.getLeafId: SessionManager#getLeafId().
  FileEntry: FileEntry#
  SessionManager.buildSessionContext: SessionManager#buildSessionContext().
  SessionManager.byId: SessionManager#byId.
  SessionManager.branchWithSummary: SessionManager#branchWithSummary().
  SessionManager.leafId: SessionManager#leafId.
  SessionManager.appendServiceTierChange: SessionManager#appendServiceTierChange().
  SessionHeader: SessionHeader#
  SessionManager.getTree: SessionManager#getTree().
  loadEntriesFromFile: loadEntriesFromFile().
  SessionInfo.rlmDepth: SessionInfo#rlmDepth.
  SessionManager._appendEntry: SessionManager#_appendEntry().
  SessionManager.appendGitState: SessionManager#appendGitState().
  SessionHeader.id: SessionHeader#id.
  SessionTreeNode.children: SessionTreeNode#children.
  SessionTreeFlatNode.entry: SessionTreeFlatNode#entry.
  SessionManager.sessionFile: SessionManager#sessionFile.
  SessionManager.listAll: SessionManager#listAll().
  SessionInfo.parentSessionPath: SessionInfo#parentSessionPath.
  extractTextContent: extractTextContent().
  SessionMessageEntry: SessionMessageEntry#
  AgentStatus.summary: AgentStatus#summary.
  SessionInfo.state: SessionInfo#state.
  SessionManager.branch: SessionManager#branch().
  CompactionEntry: CompactionEntry#
  SessionManager.recordGitStateIfChanged: SessionManager#recordGitStateIfChanged().
  SessionInfo.name: SessionInfo#name.
  SessionHeader.rlmDepth: SessionHeader#rlmDepth.
  SessionContext.model: SessionContext#model.
  loadEntriesFromFileAsync.options-typeLiteral226.streamThresholdBytes: loadEntriesFromFileAsync().(options)typeLiteral226:streamThresholdBytes.
  SessionManager._rewriteFile: SessionManager#_rewriteFile().
  SessionManager.fileEntries: SessionManager#fileEntries.
  SessionManager.persistListeners: SessionManager#persistListeners.
  resolveSessionRlmDepth: resolveSessionRlmDepth().
  generateId: generateId().
  CustomEntry.customType: CustomEntry#customType.
  SessionInfo.modified: SessionInfo#modified.
  SessionManager.openAsync: SessionManager#openAsync().
  SessionHeader.timestamp: SessionHeader#timestamp.
  SessionInfo.messageCount: SessionInfo#messageCount.
  AgentStatus.taskState: AgentStatus#taskState.
  resolveLegacySessionRlmDepth: resolveLegacySessionRlmDepth().
  listSessionsFromDir: listSessionsFromDir().
  LabelEntry: LabelEntry#
  SessionEntryBase: SessionEntryBase#
  SessionManager.appendCustomMessageEntryWithRollback: SessionManager#appendCustomMessageEntryWithRollback().
  SessionHeader.git: SessionHeader#git.
  BranchSummaryEntry: BranchSummaryEntry#
  SessionHeader.cwd: SessionHeader#cwd.
  CustomEntry.data: CustomEntry#data.
  SessionInfo.firstMessage: SessionInfo#firstMessage.
  SessionManager.persist: SessionManager#persist.
  isMessageWithContent: isMessageWithContent().
  extractOversizedMessageSummary.typeLiteral384.textPreview: extractOversizedMessageSummary().typeLiteral384:textPreview.
  SessionManager.getSessionDir: SessionManager#getSessionDir().
  SessionManager._appendEntryWithRollback: SessionManager#_appendEntryWithRollback().
  SessionManager.getFlatTree: SessionManager#getFlatTree().
  CompactionEntry.summary: CompactionEntry#summary.
  AgentStatus.basedOnMessageCount: AgentStatus#basedOnMessageCount.
  createUniqueSessionFileTarget: createUniqueSessionFileTarget().
  getDefaultSessionDir: getDefaultSessionDir().
  SessionManager.getEntry: SessionManager#getEntry().
  CustomEntry: CustomEntry#
  SessionContext.serviceTier: SessionContext#serviceTier.
  SessionInfo.agentStatus: SessionInfo#agentStatus.
  sessionHeaderMatchesCwd: sessionHeaderMatchesCwd().
  SessionManager.getLabel: SessionManager#getLabel().
  CustomMessageEntry.content: CustomMessageEntry#content.
  SessionManager.flushed: SessionManager#flushed.
  SessionHeader.parentSession: SessionHeader#parentSession.
  BranchSummaryEntry.summary: BranchSummaryEntry#summary.
  AgentStatus: AgentStatus#
  SessionInfo.cwd: SessionInfo#cwd.
  SessionManager.continueRecent: SessionManager#continueRecent().
  CompactionEntry.tokensBefore: CompactionEntry#tokensBefore.
  SessionStateEntry: SessionStateEntry#
  migrateSessionEntries: migrateSessionEntries().
  ThinkingLevelChangeEntry: ThinkingLevelChangeEntry#
  ModelChangeEntry: ModelChangeEntry#
  findMostRecentSession: findMostRecentSession().
  SessionManager.getLeafEntry: SessionManager#getLeafEntry().
  SessionHeader.version: SessionHeader#version.
  SessionTreeNode: SessionTreeNode#
  SessionInfo.created: SessionInfo#created.
  SessionInfo.allMessagesText: SessionInfo#allMessagesText.
  readSessionHeader: readSessionHeader().
  SessionManager.cwd: SessionManager#cwd.
  ServiceTierChangeEntry: ServiceTierChangeEntry#
  CompactionEntry.firstKeptEntryId: CompactionEntry#firstKeptEntryId.
  SessionContext.thinkingLevel: SessionContext#thinkingLevel.
  SessionManager.sessionId: SessionManager#sessionId.
  SessionManager.labelsById: SessionManager#labelsById.
  SessionState: SessionState#
  parseEntriesFromBufferAsync: parseEntriesFromBufferAsync().
  deriveChildRlmDepth: deriveChildRlmDepth().
  isValidSessionFile: isValidSessionFile().
  sessionInfoMatchesCwd: sessionInfoMatchesCwd().
  SessionManager.getChildren: SessionManager#getChildren().
  CURRENT_SESSION_VERSION: CURRENT_SESSION_VERSION.
  LabelEntry.targetId: LabelEntry#targetId.
  AgentStatusEntry: AgentStatusEntry#
  CustomMessageEntry.customType: CustomMessageEntry#customType.
  parseSessionEntries: parseSessionEntries().
  SessionManager.labelTimestampsById: SessionManager#labelTimestampsById.
  AssistantSessionMessageEntry: AssistantSessionMessageEntry#
  ModelChangeEntry.provider: ModelChangeEntry#provider.
  ModelChangeEntry.modelId: ModelChangeEntry#modelId.
  GitStateEntry: GitStateEntry#
  SessionManager._notifyPersistListeners: SessionManager#_notifyPersistListeners().
  SessionManager.appendCustomEntryWithRollback: SessionManager#appendCustomEntryWithRollback().
  ChildUsageAttributionEntry.childUsage: ChildUsageAttributionEntry#childUsage.
  SessionInfoEntry: SessionInfoEntry#
  ReadonlySessionManager: ReadonlySessionManager#
  sessionInfoCache: sessionInfoCache.
  LabelEntry.label: LabelEntry#label.
  AgentTaskState: AgentTaskState#
  createUniqueSessionFileTarget.typeLiteral30.sessionFile: createUniqueSessionFileTarget().typeLiteral30:sessionFile.
  parseEntriesFromBuffer: parseEntriesFromBuffer().
  loadEntriesFromFileAsync: loadEntriesFromFileAsync().
  findMostRecentSessionForCwd: findMostRecentSessionForCwd().
  getSessionModifiedDateFromLastActivity: getSessionModifiedDateFromLastActivity().
  SessionManager.onPersist: SessionManager#onPersist().
  ChildUsageAttributionEntry: ChildUsageAttributionEntry#
  ChildUsageAttributionEntry.aggregateUsage: ChildUsageAttributionEntry#aggregateUsage.
  CustomMessageEntry: CustomMessageEntry#
  appendEntryFromBuffer: appendEntryFromBuffer().
  SessionListCallbacks: SessionListCallbacks#
  CompactionEntry.customInstructions: CompactionEntry#customInstructions.
  BranchSummaryEntry.fromId: BranchSummaryEntry#fromId.
  SessionStateEntry.state: SessionStateEntry#state.
  SessionTreeFlatNode.labelTimestamp: SessionTreeFlatNode#labelTimestamp.
  SessionContext: SessionContext#
  createUniqueSessionFileTarget.typeLiteral30.sessionId: createUniqueSessionFileTarget().typeLiteral30:sessionId.
  extractJsonStringPropertyPrefix: extractJsonStringPropertyPrefix().
  SessionManager.sessionDir: SessionManager#sessionDir.
  normalizeSessionStateStatus: normalizeSessionStateStatus().
  SessionListCallbacks.onProgress: SessionListCallbacks#onProgress.
  SessionManager.isPersisted: SessionManager#isPersisted().
  NewSessionOptions.parentSession: NewSessionOptions#parentSession.
  ThinkingLevelChangeEntry.thinkingLevel: ThinkingLevelChangeEntry#thinkingLevel.
  CustomMessageEntry.details: CustomMessageEntry#details.
  CustomMessageEntry.display: CustomMessageEntry#display.
  createSessionId: createSessionId().
  isValidRlmDepth: isValidRlmDepth().
  resolveSessionRlmDepth.header-typeLiteral247.parentSession: resolveSessionRlmDepth().(header)typeLiteral247:parentSession.
  normalizeCwd: normalizeCwd().
  extractOversizedMessageSummary.typeLiteral384.role: extractOversizedMessageSummary().typeLiteral384:role.
  rootRlmDepthFromEnv: rootRlmDepthFromEnv().
  appendCappedSearchText: appendCappedSearchText().
  SessionInfoCacheEntry: SessionInfoCacheEntry#
  SessionListItem: SessionListItem#
  SessionManager.resetLeaf: SessionManager#resetLeaf().
  ServiceTierChangeEntry.serviceTier: ServiceTierChangeEntry#serviceTier.
  CompactionEntry.details: CompactionEntry#details.
  BranchSummaryEntry.details: BranchSummaryEntry#details.
  ChildUsageAttributionEntry.targetId: ChildUsageAttributionEntry#targetId.
  ChildUsageAttributionEntry.origin: ChildUsageAttributionEntry#origin.
  SessionInfoEntry.name: SessionInfoEntry#name.
  SessionStateStatus: SessionStateStatus#
  AgentStatusEntry.status: AgentStatusEntry#status.
  extractOversizedMessageSummary.typeLiteral384.timestamp: extractOversizedMessageSummary().typeLiteral384:timestamp.
  SessionListCallbacks.onSession: SessionListCallbacks#onSession.
  SESSION_LIST_SEARCH_TEXT_MAX_CHARS: SESSION_LIST_SEARCH_TEXT_MAX_CHARS.
  SESSION_LIST_LARGE_MESSAGE_PREVIEW_MAX_CHARS: SESSION_LIST_LARGE_MESSAGE_PREVIEW_MAX_CHARS.
  SESSION_ASYNC_PARSE_YIELD_BYTES: SESSION_ASYNC_PARSE_YIELD_BYTES.
  NewSessionOptions: NewSessionOptions#
  NewSessionOptions.id: NewSessionOptions#id.
  SessionPersistListener: SessionPersistListener#
  CompactionEntry.fromHook: CompactionEntry#fromHook.
  BranchSummaryEntry.fromHook: BranchSummaryEntry#fromHook.
  GitStateEntry.git: GitStateEntry#git.
  SessionTreeFlatNode: SessionTreeFlatNode#
  SessionTreeFlatNode.label: SessionTreeFlatNode#label.
  getSessionFilePath: getSessionFilePath().
  resolveLegacySessionRlmDepth.header-typeLiteral248.rlmDepth: resolveLegacySessionRlmDepth().(header)typeLiteral248:rlmDepth.
  resolveLegacySessionRlmDepth.header-typeLiteral248.parentSession: resolveLegacySessionRlmDepth().(header)typeLiteral248:parentSession.
  legacyChildDepthFromPath: legacyChildDepthFromPath().
  SessionInfoCacheEntry.size: SessionInfoCacheEntry#size.
  SessionInfoCacheEntry.mtimeMs: SessionInfoCacheEntry#mtimeMs.
  SessionInfoCacheEntry.info: SessionInfoCacheEntry#info.
  SESSION_LIST_PARSE_MAX_LINE_CHARS: SESSION_LIST_PARSE_MAX_LINE_CHARS.
  SESSION_STREAMING_LOAD_THRESHOLD_BYTES: SESSION_STREAMING_LOAD_THRESHOLD_BYTES.
  CONTENT_ENTRY_TYPES: CONTENT_ENTRY_TYPES.
  realpathIfPresent: realpathIfPresent().
  statMetadataIfPresent: statMetadataIfPresent().
  NewSessionOptions.rlmDepth: NewSessionOptions#rlmDepth.
  getSessionArtifactPath: getSessionArtifactPath().
  generateId.byId-typeLiteral40.has: generateId().(byId)typeLiteral40:has().
  resolveSessionRlmDepth.header-typeLiteral247.rlmDepth: resolveSessionRlmDepth().(header)typeLiteral247:rlmDepth.
  looksLikeMessageEntry: looksLikeMessageEntry().
  extractOversizedMessageSummary: extractOversizedMessageSummary().
  SessionListProgress: SessionListProgress#
  SessionEntryBase.type: SessionEntryBase#type.
---
# Module: [`packages/coding-agent/src/core/session-manager.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts)

## Classes
### `AgentStatus`
- def: [`packages/coding-agent/src/core/session-manager.ts:209`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L209)
- doc: Latest short status for an agent, shown in the agents view.
- signature: `interface AgentStatus`
- members:
  - `basedOnMessageCount` — [`L213`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L213) — Message count this status was derived from, used to skip redundant work.
  - `summary` — [`L210`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L210)
  - `taskState` — [`L211`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L211)
- uses (calls/refs, reference-scoped): [`AgentTaskState`](session-manager.ts.md#AgentTaskState)
- used by: [`summaryForActiveSession`](../modes/daemon/daemon-session-list.ts.md#summaryForActiveSession), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`summaryForInactiveSession`](../modes/daemon/daemon-session-list.ts.md#summaryForInactiveSession), [`summarize`](../modes/daemon/daemon-session-summarizer.ts.md#DaemonSessionSummarizer.summarize), [`active-session-state.ts`](../modes/daemon/active-session-state.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-active-session-state.ts), [`getLatestAgentStatus`](session-manager.ts.md#SessionManager.getLatestAgentStatus), [`appendAgentStatus`](session-manager.ts.md#SessionManager.appendAgentStatus), [`refreshReplacedSessionState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.refreshReplacedSessionState), [`daemon-session-summarizer.ts`](../modes/daemon/daemon-session-summarizer.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-session-summarizer.ts), [`summaryState`](../modes/daemon/active-session-state.ts.md#ActiveSessionState.summaryState), [`summarizer`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.summarizer), [`createConnectionState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createConnectionState), [`agentStatusChanged`](../modes/daemon/daemon-session-summarizer.ts.md#agentStatusChanged), [`isSummaryCurrent`](../modes/daemon/daemon-session-list.ts.md#isSummaryCurrent), [`agentStatus`](session-manager.ts.md#SessionInfo.agentStatus), [`AgentStatusEntry`](session-manager.ts.md#AgentStatusEntry)  (4 test-only)

### `AgentStatusEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:217`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L217)
- doc: Append-only status entry; ignored by buildSessionContext and other readers.
- signature: `interface AgentStatusEntry`
- members:
  - `status` — [`L219`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L219)
  - `type` — [`L218`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L218)
- uses (calls/refs, reference-scoped): [`SessionEntryBase`](session-manager.ts.md#SessionEntryBase), [`AgentStatus`](session-manager.ts.md#AgentStatus)
- used by: [`createAgentSession`](sdk.ts.md#createAgentSession), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`SessionEntry`](session-manager.ts.md#SessionEntry), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`open`](session-manager.ts.md#SessionManager.open), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`handleCompactHostRequest`](agent-session.ts.md#AgentSession.handleCompactHostRequest), [`getHeader`](session-manager.ts.md#SessionManager.getHeader), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`prepareBranchEntries`](compaction/branch-summarization.ts.md#prepareBranchEntries), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`_restoreLateIpythonSentAgentMessages`](agent-session.ts.md#AgentSession._restoreLateIpythonSentAgentMessages), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`_loadPersistedGoalState`](agent-session.ts.md#AgentSession._loadPersistedGoalState), [`findTurnStartIndex`](compaction/compaction.ts.md#findTurnStartIndex), [`findValidCutPoints`](compaction/compaction.ts.md#findValidCutPoints), [`getActiveGitContext`](session-manager.ts.md#SessionManager.getActiveGitContext), [`migrateV1ToV2`](session-manager.ts.md#migrateV1ToV2), [`_loadRefinementHistory`](agent-session.ts.md#AgentSession._loadRefinementHistory)  (+15 more; 40 test-only)

### `AgentTaskState`
- def: [`packages/coding-agent/src/core/session-manager.ts:206`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L206)
- doc: Whether an idle agent's turn left the task complete or awaiting more input.
- signature: `type AgentTaskState`
- used by: [`daemon-session-list.ts`](../modes/daemon/daemon-session-list.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-session-list.ts), [`daemon-session-summarizer.ts`](../modes/daemon/daemon-session-summarizer.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-session-summarizer.ts), [`parseAgentStatusResponse`](../modes/daemon/daemon-session-summarizer.ts.md#parseAgentStatusResponse), [`taskState`](../modes/daemon/daemon-session-list.ts.md#SessionSummary.taskState), [`taskState`](session-manager.ts.md#AgentStatus.taskState), [`AgentStatusResult`](../modes/daemon/daemon-session-summarizer.ts.md#AgentStatusResult)

### `AssistantSessionMessageEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:108`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L108)
- signature: `type AssistantSessionMessageEntry`
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../../ai/src/types.ts.md#AssistantMessage), [`SessionMessageEntry`](session-manager.ts.md#SessionMessageEntry)
- used by: [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions)

### `BranchSummaryEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:139`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L139)
- signature: `interface BranchSummaryEntry`
- members:
  - `details` — [`L144`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L144) — Extension-specific data (not sent to LLM)
  - `fromHook` — [`L146`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L146) — True if generated by an extension, false if pi-generated
  - `fromId` — [`L141`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L141)
  - `summary` — [`L142`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L142)
  - `type` — [`L140`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L140)
- uses (calls/refs, reference-scoped): [`SessionEntryBase`](session-manager.ts.md#SessionEntryBase)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`createAgentSession`](sdk.ts.md#createAgentSession), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`SessionEntry`](session-manager.ts.md#SessionEntry), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`open`](session-manager.ts.md#SessionManager.open), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`handleCompactHostRequest`](agent-session.ts.md#AgentSession.handleCompactHostRequest), [`getHeader`](session-manager.ts.md#SessionManager.getHeader), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`prepareBranchEntries`](compaction/branch-summarization.ts.md#prepareBranchEntries), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`_restoreLateIpythonSentAgentMessages`](agent-session.ts.md#AgentSession._restoreLateIpythonSentAgentMessages), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`_loadPersistedGoalState`](agent-session.ts.md#AgentSession._loadPersistedGoalState), [`findTurnStartIndex`](compaction/compaction.ts.md#findTurnStartIndex), [`findValidCutPoints`](compaction/compaction.ts.md#findValidCutPoints)  (+21 more; 42 test-only)

### `ChildUsageAttributionEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:170`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L170)
- doc: Records usage folded into a parent assistant message after an RLM child run.
- signature: `interface ChildUsageAttributionEntry`
- members:
  - `aggregateUsage` — [`L174`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L174)
  - `childUsage` — [`L173`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L173)
  - `origin` — [`L175`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L175)
  - `targetId` — [`L172`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L172)
  - `type` — [`L171`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L171)
- uses (calls/refs, reference-scoped): [`Usage`](../../../ai/src/types.ts.md#Usage), [`SessionEntryBase`](session-manager.ts.md#SessionEntryBase)
- used by: [`createAgentSession`](sdk.ts.md#createAgentSession), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`SessionEntry`](session-manager.ts.md#SessionEntry), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`open`](session-manager.ts.md#SessionManager.open), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`handleCompactHostRequest`](agent-session.ts.md#AgentSession.handleCompactHostRequest), [`getHeader`](session-manager.ts.md#SessionManager.getHeader), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`prepareBranchEntries`](compaction/branch-summarization.ts.md#prepareBranchEntries), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`_restoreLateIpythonSentAgentMessages`](agent-session.ts.md#AgentSession._restoreLateIpythonSentAgentMessages), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`_loadPersistedGoalState`](agent-session.ts.md#AgentSession._loadPersistedGoalState), [`findTurnStartIndex`](compaction/compaction.ts.md#findTurnStartIndex), [`findValidCutPoints`](compaction/compaction.ts.md#findValidCutPoints), [`getActiveGitContext`](session-manager.ts.md#SessionManager.getActiveGitContext), [`migrateV1ToV2`](session-manager.ts.md#migrateV1ToV2), [`_loadRefinementHistory`](agent-session.ts.md#AgentSession._loadRefinementHistory)  (+14 more; 40 test-only)

### `CompactionEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:126`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L126)
- signature: `interface CompactionEntry`
- members:
  - `customInstructions` — [`L136`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L136) — User instructions that guided the summary (from `/compact <instructions>`)
  - `details` — [`L132`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L132) — Extension-specific data (e.g., ArtifactIndex, version markers for structured compaction)
  - `firstKeptEntryId` — [`L129`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L129)
  - `fromHook` — [`L134`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L134) — True if generated by an extension, undefined/false if pi-generated (backward compatible)
  - `summary` — [`L128`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L128)
  - `tokensBefore` — [`L130`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L130)
  - `type` — [`L127`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L127)
- uses (calls/refs, reference-scoped): [`SessionEntryBase`](session-manager.ts.md#SessionEntryBase)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`createAgentSession`](sdk.ts.md#createAgentSession), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`SessionEntry`](session-manager.ts.md#SessionEntry), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`open`](session-manager.ts.md#SessionManager.open), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`handleCompactHostRequest`](agent-session.ts.md#AgentSession.handleCompactHostRequest), [`getHeader`](session-manager.ts.md#SessionManager.getHeader), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`prepareBranchEntries`](compaction/branch-summarization.ts.md#prepareBranchEntries), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`compaction.ts`](compaction/compaction.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-compaction-compaction.ts), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`_restoreLateIpythonSentAgentMessages`](agent-session.ts.md#AgentSession._restoreLateIpythonSentAgentMessages), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`_loadPersistedGoalState`](agent-session.ts.md#AgentSession._loadPersistedGoalState), [`findTurnStartIndex`](compaction/compaction.ts.md#findTurnStartIndex)  (+21 more; 45 test-only)

### `CustomEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:159`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L159)
- doc: Custom entry for extensions to store extension-specific data in the session.
- signature: `interface CustomEntry`
- members:
  - `customType` — [`L161`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L161)
  - `data` — [`L162`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L162)
  - `type` — [`L160`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L160)
- uses (calls/refs, reference-scoped): [`SessionEntryBase`](session-manager.ts.md#SessionEntryBase)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`createAgentSession`](sdk.ts.md#createAgentSession), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`SessionEntry`](session-manager.ts.md#SessionEntry), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`open`](session-manager.ts.md#SessionManager.open), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`handleCompactHostRequest`](agent-session.ts.md#AgentSession.handleCompactHostRequest), [`getHeader`](session-manager.ts.md#SessionManager.getHeader), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`prepareBranchEntries`](compaction/branch-summarization.ts.md#prepareBranchEntries), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`_restoreLateIpythonSentAgentMessages`](agent-session.ts.md#AgentSession._restoreLateIpythonSentAgentMessages), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`_loadPersistedGoalState`](agent-session.ts.md#AgentSession._loadPersistedGoalState), [`findTurnStartIndex`](compaction/compaction.ts.md#findTurnStartIndex), [`findValidCutPoints`](compaction/compaction.ts.md#findValidCutPoints), [`getActiveGitContext`](session-manager.ts.md#SessionManager.getActiveGitContext), [`migrateV1ToV2`](session-manager.ts.md#migrateV1ToV2)  (+18 more; 41 test-only)

### `CustomMessageEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:240`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L240)
- doc: Custom message entry for extensions to inject messages into LLM context.
- signature: `interface CustomMessageEntry`
- members:
  - `content` — [`L243`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L243)
  - `customType` — [`L242`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L242)
  - `details` — [`L244`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L244)
  - `display` — [`L245`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L245)
  - `type` — [`L241`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L241)
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../ai/src/types.ts.md#ImageContent), [`TextContent`](../../../ai/src/types.ts.md#TextContent), [`SessionEntryBase`](session-manager.ts.md#SessionEntryBase)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`createAgentSession`](sdk.ts.md#createAgentSession), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`SessionEntry`](session-manager.ts.md#SessionEntry), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`open`](session-manager.ts.md#SessionManager.open), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`handleCompactHostRequest`](agent-session.ts.md#AgentSession.handleCompactHostRequest), [`getHeader`](session-manager.ts.md#SessionManager.getHeader), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`prepareBranchEntries`](compaction/branch-summarization.ts.md#prepareBranchEntries), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`_restoreLateIpythonSentAgentMessages`](agent-session.ts.md#AgentSession._restoreLateIpythonSentAgentMessages), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`_loadPersistedGoalState`](agent-session.ts.md#AgentSession._loadPersistedGoalState), [`findTurnStartIndex`](compaction/compaction.ts.md#findTurnStartIndex), [`findValidCutPoints`](compaction/compaction.ts.md#findValidCutPoints), [`getActiveGitContext`](session-manager.ts.md#SessionManager.getActiveGitContext), [`migrateV1ToV2`](session-manager.ts.md#migrateV1ToV2)  (+16 more; 40 test-only)

### `FileEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:266`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L266)
- doc: Raw file entry (includes header)
- signature: `type FileEntry`
- uses (calls/refs, reference-scoped): [`SessionEntry`](session-manager.ts.md#SessionEntry), [`SessionHeader`](session-manager.ts.md#SessionHeader)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`context-tree.ts`](context-tree.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-context-tree.ts), [`migrateV1ToV2`](session-manager.ts.md#migrateV1ToV2), [`migrateToCurrentVersion`](session-manager.ts.md#migrateToCurrentVersion), [`migrateV2ToV3`](session-manager.ts.md#migrateV2ToV3), [`sessionEntriesFromFile`](context-tree.ts.md#sessionEntriesFromFile), [`finalizeLoadedEntries`](session-manager.ts.md#finalizeLoadedEntries), [`loadEntriesFromFile`](session-manager.ts.md#loadEntriesFromFile), [`streamThresholdBytes`](session-manager.ts.md#loadEntriesFromFileAsync.options-typeLiteral226.streamThresholdBytes), [`fileEntries`](session-manager.ts.md#SessionManager.fileEntries), [`persistListeners`](session-manager.ts.md#SessionManager.persistListeners), [`migrateSessionEntries`](session-manager.ts.md#migrateSessionEntries), [`parseEntriesFromBufferAsync`](session-manager.ts.md#parseEntriesFromBufferAsync), [`parseSessionEntries`](session-manager.ts.md#parseSessionEntries), [`parseEntriesFromBuffer`](session-manager.ts.md#parseEntriesFromBuffer), [`appendEntryFromBuffer`](session-manager.ts.md#appendEntryFromBuffer)  (1 test-only)

### `GitStateEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:223`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L223)
- doc: Append-only repo-state entry; ignored by buildSessionContext and other readers.
- signature: `interface GitStateEntry`
- members:
  - `git` — [`L225`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L225)
  - `type` — [`L224`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L224)
- uses (calls/refs, reference-scoped): [`SessionEntryBase`](session-manager.ts.md#SessionEntryBase), [`GitContext`](../utils/git.ts.md#GitContext)
- used by: [`createAgentSession`](sdk.ts.md#createAgentSession), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`SessionEntry`](session-manager.ts.md#SessionEntry), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`open`](session-manager.ts.md#SessionManager.open), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`handleCompactHostRequest`](agent-session.ts.md#AgentSession.handleCompactHostRequest), [`getHeader`](session-manager.ts.md#SessionManager.getHeader), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`prepareBranchEntries`](compaction/branch-summarization.ts.md#prepareBranchEntries), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`_restoreLateIpythonSentAgentMessages`](agent-session.ts.md#AgentSession._restoreLateIpythonSentAgentMessages), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`_loadPersistedGoalState`](agent-session.ts.md#AgentSession._loadPersistedGoalState), [`findTurnStartIndex`](compaction/compaction.ts.md#findTurnStartIndex), [`findValidCutPoints`](compaction/compaction.ts.md#findValidCutPoints), [`getActiveGitContext`](session-manager.ts.md#SessionManager.getActiveGitContext), [`migrateV1ToV2`](session-manager.ts.md#migrateV1ToV2), [`_loadRefinementHistory`](agent-session.ts.md#AgentSession._loadRefinementHistory)  (+15 more; 40 test-only)

### `LabelEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:179`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L179)
- doc: Label entry for user-defined bookmarks/markers on entries.
- signature: `interface LabelEntry`
- members:
  - `label` — [`L182`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L182)
  - `targetId` — [`L181`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L181)
  - `type` — [`L180`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L180)
- uses (calls/refs, reference-scoped): [`SessionEntryBase`](session-manager.ts.md#SessionEntryBase)
- used by: [`createAgentSession`](sdk.ts.md#createAgentSession), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`SessionEntry`](session-manager.ts.md#SessionEntry), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`open`](session-manager.ts.md#SessionManager.open), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`handleCompactHostRequest`](agent-session.ts.md#AgentSession.handleCompactHostRequest), [`getHeader`](session-manager.ts.md#SessionManager.getHeader), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`prepareBranchEntries`](compaction/branch-summarization.ts.md#prepareBranchEntries), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`_restoreLateIpythonSentAgentMessages`](agent-session.ts.md#AgentSession._restoreLateIpythonSentAgentMessages), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`_loadPersistedGoalState`](agent-session.ts.md#AgentSession._loadPersistedGoalState), [`findTurnStartIndex`](compaction/compaction.ts.md#findTurnStartIndex), [`findValidCutPoints`](compaction/compaction.ts.md#findValidCutPoints), [`getActiveGitContext`](session-manager.ts.md#SessionManager.getActiveGitContext), [`migrateV1ToV2`](session-manager.ts.md#migrateV1ToV2), [`_loadRefinementHistory`](agent-session.ts.md#AgentSession._loadRefinementHistory)  (+15 more; 40 test-only)

### `ModelChangeEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:120`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L120)
- signature: `interface ModelChangeEntry`
- members:
  - `modelId` — [`L123`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L123)
  - `provider` — [`L122`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L122)
  - `type` — [`L121`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L121)
- uses (calls/refs, reference-scoped): [`SessionEntryBase`](session-manager.ts.md#SessionEntryBase)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`createAgentSession`](sdk.ts.md#createAgentSession), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`SessionEntry`](session-manager.ts.md#SessionEntry), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`open`](session-manager.ts.md#SessionManager.open), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`handleCompactHostRequest`](agent-session.ts.md#AgentSession.handleCompactHostRequest), [`getHeader`](session-manager.ts.md#SessionManager.getHeader), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`prepareBranchEntries`](compaction/branch-summarization.ts.md#prepareBranchEntries), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`_restoreLateIpythonSentAgentMessages`](agent-session.ts.md#AgentSession._restoreLateIpythonSentAgentMessages), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`_loadPersistedGoalState`](agent-session.ts.md#AgentSession._loadPersistedGoalState), [`findTurnStartIndex`](compaction/compaction.ts.md#findTurnStartIndex), [`findValidCutPoints`](compaction/compaction.ts.md#findValidCutPoints), [`getActiveGitContext`](session-manager.ts.md#SessionManager.getActiveGitContext), [`migrateV1ToV2`](session-manager.ts.md#migrateV1ToV2)  (+16 more; 43 test-only)

### `NewSessionOptions`
- def: [`packages/coding-agent/src/core/session-manager.ts:87`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L87)
- signature: `interface NewSessionOptions`
- members:
  - `id` — [`L88`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L88)
  - `parentSession` — [`L89`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L89)
  - `rlmDepth` — [`L91`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L91) — Explicit RLM spawn depth. An explicitly undefined value suppresses parent derivation.
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`newSession`](session-manager.ts.md#SessionManager.newSession)

### `ReadonlySessionManager`
- def: [`packages/coding-agent/src/core/session-manager.ts:310`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L310)
- signature: `type ReadonlySessionManager`
- uses (calls/refs, reference-scoped): [`SessionManager`](session-manager.ts.md#SessionManager)
- used by: [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`branch-summarization.ts`](compaction/branch-summarization.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-compaction-branch-summarization.ts), [`sessionManager`](extensions/types.ts.md#ExtensionContext.sessionManager), [`collectEntriesForBranchSummary`](compaction/branch-summarization.ts.md#collectEntriesForBranchSummary)

### `ServiceTierChangeEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:115`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L115)
- signature: `interface ServiceTierChangeEntry`
- members:
  - `serviceTier` — [`L117`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L117)
  - `type` — [`L116`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L116)
- uses (calls/refs, reference-scoped): [`ServiceTier`](../../../ai/src/types.ts.md#ServiceTier), [`SessionEntryBase`](session-manager.ts.md#SessionEntryBase)
- used by: [`createAgentSession`](sdk.ts.md#createAgentSession), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`SessionEntry`](session-manager.ts.md#SessionEntry), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`open`](session-manager.ts.md#SessionManager.open), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`handleCompactHostRequest`](agent-session.ts.md#AgentSession.handleCompactHostRequest), [`getHeader`](session-manager.ts.md#SessionManager.getHeader), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`prepareBranchEntries`](compaction/branch-summarization.ts.md#prepareBranchEntries), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`_restoreLateIpythonSentAgentMessages`](agent-session.ts.md#AgentSession._restoreLateIpythonSentAgentMessages), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`_loadPersistedGoalState`](agent-session.ts.md#AgentSession._loadPersistedGoalState), [`findTurnStartIndex`](compaction/compaction.ts.md#findTurnStartIndex), [`findValidCutPoints`](compaction/compaction.ts.md#findValidCutPoints), [`getActiveGitContext`](session-manager.ts.md#SessionManager.getActiveGitContext), [`migrateV1ToV2`](session-manager.ts.md#migrateV1ToV2), [`_loadRefinementHistory`](agent-session.ts.md#AgentSession._loadRefinementHistory)  (+15 more; 42 test-only)

### `SessionContext`
- def: [`packages/coding-agent/src/core/session-manager.ts:281`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L281)
- signature: `interface SessionContext`
- members:
  - `messages` — [`L282`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L282)
  - `model` — [`L285`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L285)
  - `serviceTier` — [`L284`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L284)
  - `thinkingLevel` — [`L283`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L283)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../agent/src/types.ts.md#AgentMessage), [`ServiceTier`](../../../ai/src/types.ts.md#ServiceTier)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`createAgentSession`](sdk.ts.md#createAgentSession), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`sessionOptionsOverride`](../main.ts.md#prepareRuntimeServices.options-typeLiteral166.sessionOptionsOverride), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`cancelled`](agent-session-runtime.ts.md#AgentSessionRuntime.newSession.Promise.typeLiteral136.cancelled), [`modelFallbackMessage`](../main.ts.md#resolvePreparedStartupModel.Promise.typeLiteral217.modelFallbackMessage), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`buildSessionContext`](session-manager.ts.md#SessionManager.buildSessionContext), [`buildSessionContext`](agent-session.ts.md#AgentSession.buildSessionContext)  (18 test-only)

### `SessionEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:249`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L249)
- doc: Session entry - has id/parentId for tree structure (returned by "read" methods in SessionManager)
- signature: `type SessionEntry`
- uses (calls/refs, reference-scoped): [`SessionMessageEntry`](session-manager.ts.md#SessionMessageEntry), [`CompactionEntry`](session-manager.ts.md#CompactionEntry), [`LabelEntry`](session-manager.ts.md#LabelEntry), [`BranchSummaryEntry`](session-manager.ts.md#BranchSummaryEntry), [`CustomEntry`](session-manager.ts.md#CustomEntry), [`SessionStateEntry`](session-manager.ts.md#SessionStateEntry), [`ModelChangeEntry`](session-manager.ts.md#ModelChangeEntry), [`ThinkingLevelChangeEntry`](session-manager.ts.md#ThinkingLevelChangeEntry), [`ServiceTierChangeEntry`](session-manager.ts.md#ServiceTierChangeEntry), [`AgentStatusEntry`](session-manager.ts.md#AgentStatusEntry), [`GitStateEntry`](session-manager.ts.md#GitStateEntry), [`SessionInfoEntry`](session-manager.ts.md#SessionInfoEntry), [`ChildUsageAttributionEntry`](session-manager.ts.md#ChildUsageAttributionEntry), [`CustomMessageEntry`](session-manager.ts.md#CustomMessageEntry)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`generateBranchSummary`](compaction/branch-summarization.ts.md#generateBranchSummary), [`prepareBranchEntries`](compaction/branch-summarization.ts.md#prepareBranchEntries), [`_persist`](session-manager.ts.md#SessionManager._persist), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`compaction.ts`](compaction/compaction.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-compaction-compaction.ts), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry), [`branch-summarization.ts`](compaction/branch-summarization.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-compaction-branch-summarization.ts), [`findTurnStartIndex`](compaction/compaction.ts.md#findTurnStartIndex), [`findValidCutPoints`](compaction/compaction.ts.md#findValidCutPoints), [`context-tree.ts`](context-tree.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-context-tree.ts), [`getLastAssistantUsage`](compaction/compaction.ts.md#getLastAssistantUsage), [`getBranch`](session-manager.ts.md#SessionManager.getBranch), [`sessionEntriesFromFile`](context-tree.ts.md#sessionEntriesFromFile), [`getLatestCompactionEntry`](session-manager.ts.md#getLatestCompactionEntry), [`getMessageFromEntryForCompaction`](compaction/compaction.ts.md#getMessageFromEntryForCompaction), [`FileEntry`](session-manager.ts.md#FileEntry), [`index.ts`](export-html/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-export-html-index.ts), [`buildSessionContext`](session-manager.ts.md#SessionManager.buildSessionContext), [`byId`](session-manager.ts.md#SessionManager.byId), [`extractFileOperations`](compaction/compaction.ts.md#extractFileOperations), [`_appendEntry`](session-manager.ts.md#SessionManager._appendEntry), [`entry`](session-manager.ts.md#SessionTreeFlatNode.entry), [`collectEntriesForBranchSummary`](compaction/branch-summarization.ts.md#collectEntriesForBranchSummary), [`getEntry`](session-manager.ts.md#SessionManager.getEntry), [`statusFromBranch`](context-tree.ts.md#statusFromBranch), [`getLeafEntry`](session-manager.ts.md#SessionManager.getLeafEntry), [`branchEntries`](context-tree.ts.md#branchEntries), [`getChildren`](session-manager.ts.md#SessionManager.getChildren), [`branchEntries`](extensions/types.ts.md#SessionBeforeCompactEvent.branchEntries), [`entries`](compaction/branch-summarization.ts.md#CollectEntriesResult.entries)  (+1 more; 6 test-only)

### `SessionEntryBase`
- def: [`packages/coding-agent/src/core/session-manager.ts:96`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L96)
- signature: `interface SessionEntryBase`
- members:
  - `id` — [`L98`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L98)
  - `parentId` — [`L99`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L99)
  - `timestamp` — [`L100`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L100)
  - `type` — [`L97`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L97)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`_startRlmChildRun`](agent-session.ts.md#AgentSession._startRlmChildRun), [`appendMessage`](session-manager.ts.md#SessionManager.appendMessage), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`_checkCompaction`](agent-session.ts.md#AgentSession._checkCompaction), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`appendSessionState`](session-manager.ts.md#SessionManager.appendSessionState), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`getActiveGitContext`](session-manager.ts.md#SessionManager.getActiveGitContext), [`migrateV1ToV2`](session-manager.ts.md#migrateV1ToV2), [`appendLabelChange`](session-manager.ts.md#SessionManager.appendLabelChange), [`getLatestAgentStatus`](session-manager.ts.md#SessionManager.getLatestAgentStatus), [`appendSessionInfo`](session-manager.ts.md#SessionManager.appendSessionInfo), [`getBranch`](session-manager.ts.md#SessionManager.getBranch), [`appendCompaction`](session-manager.ts.md#SessionManager.appendCompaction), [`appendCustomEntry`](session-manager.ts.md#SessionManager.appendCustomEntry), [`appendCustomMessageEntry`](session-manager.ts.md#SessionManager.appendCustomMessageEntry), [`appendAgentStatus`](session-manager.ts.md#SessionManager.appendAgentStatus), [`_thresholdCompactionNeeded`](agent-session.ts.md#AgentSession._thresholdCompactionNeeded), [`appendThinkingLevelChange`](session-manager.ts.md#SessionManager.appendThinkingLevelChange), [`appendModelChange`](session-manager.ts.md#SessionManager.appendModelChange), [`branchWithSummary`](session-manager.ts.md#SessionManager.branchWithSummary), [`appendServiceTierChange`](session-manager.ts.md#SessionManager.appendServiceTierChange), [`getTree`](session-manager.ts.md#SessionManager.getTree), [`exportToJsonl`](agent-session.ts.md#AgentSession.exportToJsonl), [`_appendEntry`](session-manager.ts.md#SessionManager._appendEntry), [`appendGitState`](session-manager.ts.md#SessionManager.appendGitState), [`collectEntriesForBranchSummary`](compaction/branch-summarization.ts.md#collectEntriesForBranchSummary), [`SessionMessageEntry`](session-manager.ts.md#SessionMessageEntry)  (+16 more; 26 test-only)

### `SessionHeader`
- def: [`packages/coding-agent/src/core/session-manager.ts:75`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L75)
- signature: `interface SessionHeader`
- members:
  - `cwd` — [`L80`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L80)
  - `git` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L84)
  - `id` — [`L78`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L78)
  - `parentSession` — [`L81`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L81)
  - `rlmDepth` — [`L83`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L83) — RLM spawn depth. Optional for backward compatibility. Forks preserve the source depth.
  - `timestamp` — [`L79`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L79)
  - `type` — [`L76`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L76)
  - `version` — [`L77`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L77)
- uses (calls/refs, reference-scoped): [`GitContext`](../utils/git.ts.md#GitContext)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`summaryForActiveSession`](../modes/daemon/daemon-session-list.ts.md#summaryForActiveSession), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`newSession`](session-manager.ts.md#SessionManager.newSession), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`open`](session-manager.ts.md#SessionManager.open), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`getHeader`](session-manager.ts.md#SessionManager.getHeader), [`performAgentTraceUpload`](agent-traces.ts.md#performAgentTraceUpload), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`cancelled`](agent-session-runtime.ts.md#AgentSessionRuntime.newSession.Promise.typeLiteral136.cancelled), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`materializeSessionFile`](session-manager.ts.md#SessionManager.materializeSessionFile), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`getActiveGitContext`](session-manager.ts.md#SessionManager.getActiveGitContext), [`migrateV1ToV2`](session-manager.ts.md#migrateV1ToV2), [`migrateToCurrentVersion`](session-manager.ts.md#migrateToCurrentVersion), [`agent-traces.ts`](agent-traces.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-traces.ts), [`previewAgentTraceFile`](agent-traces.ts.md#previewAgentTraceFile), [`migrateV2ToV3`](session-manager.ts.md#migrateV2ToV3), [`sessionEntriesFromFile`](context-tree.ts.md#sessionEntriesFromFile), [`finalizeLoadedEntries`](session-manager.ts.md#finalizeLoadedEntries), [`FileEntry`](session-manager.ts.md#FileEntry), [`exportToJsonl`](agent-session.ts.md#AgentSession.exportToJsonl), [`resolveHeaderParentSessionPath`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.resolveHeaderParentSessionPath), [`parentSessionId`](agent-traces.ts.md#resolveTraceContext.typeLiteral127.parentSessionId), [`openAsync`](session-manager.ts.md#SessionManager.openAsync), [`activeGitContext`](agent-traces.ts.md#activeGitContext), [`sessionHeaderMatchesCwd`](session-manager.ts.md#sessionHeaderMatchesCwd), [`readSessionHeader`](agent-traces.ts.md#readSessionHeader), [`readSessionHeader`](session-manager.ts.md#readSessionHeader), [`deriveChildRlmDepth`](session-manager.ts.md#deriveChildRlmDepth), [`isValidSessionFile`](session-manager.ts.md#isValidSessionFile), [`getSessionModifiedDateFromLastActivity`](session-manager.ts.md#getSessionModifiedDateFromLastActivity)  (+2 more; 13 test-only)

### `SessionInfo`
- def: [`packages/coding-agent/src/core/session-manager.ts:288`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L288)
- signature: `interface SessionInfo`
- members:
  - `agentStatus` — [`L307`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L307) — Latest persisted recap/verdict, so off-daemon sessions keep their status.
  - `allMessagesText` — [`L305`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L305)
  - `created` — [`L301`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L301)
  - `cwd` — [`L292`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L292) — Working directory where the session was started. Empty string for old sessions.
  - `firstMessage` — [`L304`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L304)
  - `id` — [`L290`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L290)
  - `messageCount` — [`L303`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L303)
  - `modified` — [`L302`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L302)
  - `name` — [`L294`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L294) — User-defined display name from session_info entries.
  - `parentSessionPath` — [`L298`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L298) — Path to the parent session (if this session was forked).
  - `path` — [`L289`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L289)
  - `rlmDepth` — [`L300`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L300) — Resolved RLM spawn depth.
  - `state` — [`L296`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L296) — Latest persisted lifecycle state from session_state entries.
- uses (calls/refs, reference-scoped): [`AgentStatus`](session-manager.ts.md#AgentStatus), [`SessionState`](session-manager.ts.md#SessionState)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`handleCommand`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.handleCommand), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`daemon-supervisor.ts`](../modes/daemon/daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`summaryForActiveSession`](../modes/daemon/daemon-session-list.ts.md#summaryForActiveSession), [`createRuntime`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRuntime), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`summaryForInactiveSession`](../modes/daemon/daemon-session-list.ts.md#summaryForInactiveSession), [`createAgentFamilyCatalog`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentFamilyCatalog), [`createAgentMessageListResult`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentMessageListResult), [`createAgentObserveListResult`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentObserveListResult), [`daemon-session-list.ts`](../modes/daemon/daemon-session-list.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-session-list.ts), [`serializeSavedSessionInfo`](../modes/daemon/saved-session-info.ts.md#serializeSavedSessionInfo), [`buildSessionListWithPassiveRlmSubagents`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.buildSessionListWithPassiveRlmSubagents), [`createOrReuseWorker`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.createOrReuseWorker), [`buildRlmChildSnapshotsWithPassiveRlmSubagents`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.buildRlmChildSnapshotsWithPassiveRlmSubagents), [`hydratePassiveRlmSubagent`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.hydratePassiveRlmSubagent), [`restoreRlmHeartbeatSession`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.restoreRlmHeartbeatSession), [`passiveAgentFamilyEntry`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.passiveAgentFamilyEntry), [`buildSessionList`](../modes/daemon/daemon-session-list.ts.md#buildSessionList), [`listPassiveRlmSubagents`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.listPassiveRlmSubagents), [`readSessionInfo`](session-manager.ts.md#readSessionInfo), [`handleCatalogRequest`](../modes/daemon/daemon-catalog-process.ts.md#handleCatalogRequest), [`assertSavedSiblingNameAvailable`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.assertSavedSiblingNameAvailable), [`list`](session-manager.ts.md#SessionManager.list), [`type`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.handleSavedSessionList.command-Extract.typeLiteral1475.type), [`mergeSessionLists`](../modes/daemon/daemon-supervisor.ts.md#mergeSessionLists), [`resolveSessionPath`](session-resolver.ts.md#resolveSessionPath), [`assertSupervisorSavedSessionNameAvailable`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.assertSupervisorSavedSessionNameAvailable), [`daemon-catalog-process.ts`](../modes/daemon/daemon-catalog-process.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-catalog-process.ts), [`familyCatalogEntries`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.familyCatalogEntries), [`listSavedSessionSiblings`](../modes/daemon/daemon-catalog-process.ts.md#listSavedSessionSiblings), [`listAll`](session-manager.ts.md#SessionManager.listAll), [`parentSessionPath`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.savedSessionNameReservationInput.Promise.typeLiteral1261.parentSessionPath), [`findPassiveRlmSubagent`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.findPassiveRlmSubagent), [`isPersistedCronJobRunnable`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.isPersistedCronJobRunnable), [`saved-session-info.ts`](../modes/daemon/saved-session-info.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-saved-session-info.ts), [`deserializeSessionInfo`](../modes/daemon/daemon-catalog-process.ts.md#deserializeSessionInfo), [`serializeSessionInfo`](../modes/daemon/daemon-catalog-process.ts.md#serializeSessionInfo), [`inactiveLifecycleForSession`](../modes/daemon/daemon-session-list.ts.md#inactiveLifecycleForSession)  (+20 more; 17 test-only)

### `SessionInfoCacheEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:995`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L995)
- signature: `interface SessionInfoCacheEntry`
- members:
  - `info` — [`L998`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L998)
  - `mtimeMs` — [`L997`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L997)
  - `size` — [`L996`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L996)
- uses (calls/refs, reference-scoped): [`SessionInfo`](session-manager.ts.md#SessionInfo)
- used by: [`readSessionInfo`](session-manager.ts.md#readSessionInfo), [`sessionInfoCache`](session-manager.ts.md#sessionInfoCache)

### `SessionInfoEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:186`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L186)
- doc: Session metadata entry (e.g., user-defined display name).
- signature: `interface SessionInfoEntry`
- members:
  - `name` — [`L188`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L188)
  - `type` — [`L187`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L187)
- uses (calls/refs, reference-scoped): [`SessionEntryBase`](session-manager.ts.md#SessionEntryBase)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`createAgentSession`](sdk.ts.md#createAgentSession), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`SessionEntry`](session-manager.ts.md#SessionEntry), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`open`](session-manager.ts.md#SessionManager.open), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`handleCompactHostRequest`](agent-session.ts.md#AgentSession.handleCompactHostRequest), [`getHeader`](session-manager.ts.md#SessionManager.getHeader), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`prepareBranchEntries`](compaction/branch-summarization.ts.md#prepareBranchEntries), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`_restoreLateIpythonSentAgentMessages`](agent-session.ts.md#AgentSession._restoreLateIpythonSentAgentMessages), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`_loadPersistedGoalState`](agent-session.ts.md#AgentSession._loadPersistedGoalState), [`findTurnStartIndex`](compaction/compaction.ts.md#findTurnStartIndex), [`findValidCutPoints`](compaction/compaction.ts.md#findValidCutPoints), [`getActiveGitContext`](session-manager.ts.md#SessionManager.getActiveGitContext), [`migrateV1ToV2`](session-manager.ts.md#migrateV1ToV2)  (+16 more; 40 test-only)

### `SessionListCallbacks`
- def: [`packages/coding-agent/src/core/session-manager.ts:1134`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1134)
- signature: `interface SessionListCallbacks`
- members:
  - `onProgress` — [`L1135`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1135)
  - `onSession` — [`L1136`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1136)
- uses (calls/refs, reference-scoped): [`SessionListItem`](session-manager.ts.md#SessionListItem), [`SessionListProgress`](session-manager.ts.md#SessionListProgress)
- used by: [`list`](session-manager.ts.md#SessionManager.list), [`listAll`](session-manager.ts.md#SessionManager.listAll), [`listSessionsFromDir`](session-manager.ts.md#listSessionsFromDir)

### `SessionListItem`
- def: [`packages/coding-agent/src/core/session-manager.ts:1132`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1132)
- signature: `type SessionListItem`
- uses (calls/refs, reference-scoped): [`SessionInfo`](session-manager.ts.md#SessionInfo)
- used by: [`SessionListCallbacks`](session-manager.ts.md#SessionListCallbacks)

### `SessionListProgress`
- def: [`packages/coding-agent/src/core/session-manager.ts:1131`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1131)
- signature: `type SessionListProgress`
- used by: [`onProgress`](session-manager.ts.md#SessionListCallbacks.onProgress)

### `SessionManager`
- def: [`packages/coding-agent/src/core/session-manager.ts:1191`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1191) — documented in [packages-coding-agent-src-core-session-manager.ts](../../../../../concepts/packages-coding-agent-src-core-session-manager.ts.md)
- doc: Manages conversation sessions as append-only trees stored in JSONL files.
- signature: `class SessionManager`
- members:
  - `appendAgentStatus(method)` — [`L1695`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1695) — Append the latest agent status (summary + completion judgment). Returns entry id.
  - `appendChildUsageAttribution(method)` — [`L1587`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1587) — Append an RLM child usage attribution and update the parent assistant aggregate in memory.
  - `appendCompaction(method)` — [`L1543`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1543) — Append a compaction summary as child of current leaf, then advance leaf. Returns entry id.
  - `appendCustomEntry(method)` — [`L1568`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1568) — Append a custom entry (for extensions) as child of current leaf, then advance leaf. Returns entry id.
  - `appendCustomEntryWithRollback(method)` — [`L1582`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1582) — Append a custom entry and undo its in-memory index if persistence fails.
  - `appendCustomMessageEntry(method)` — [`L1766`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1766) — Append a custom message entry (for extensions) that participates in LLM context.
  - `appendCustomMessageEntryWithRollback(method)` — [`L1790`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1790) — Append a custom message, undoing the append if persistence fails so a
  - `appendGitState(method)` — [`L1712`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1712) — Append a git state entry as child of current leaf, then advance leaf. Returns entry id.
  - `appendLabelChange(method)` — [`L1866`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1866) — Set or clear a label on an entry.
  - `appendMessage(method)` — [`L1490`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1490) — Append a message as child of current leaf, then advance leaf. Returns entry id. — documented in [packages-coding-agent-src-core-session-manager.ts](../../../../../concepts/packages-coding-agent-src-core-session-manager.ts.md)
  - `appendModelChange(method)` — [`L1529`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1529) — Append a model change as child of current leaf, then advance leaf. Returns entry id.
  - `appendServiceTierChange(method)` — [`L1516`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1516) — Append a service tier change as child of current leaf, then advance leaf. Returns entry id.
  - `appendSessionInfo(method)` — [`L1614`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1614) — Append a session info entry (e.g., display name). Returns entry id.
  - `appendSessionState(method)` — [`L1627`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1627) — Append a session lifecycle state entry. Returns entry id.
  - `appendThinkingLevelChange(method)` — [`L1503`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1503) — Append a thinking level change as child of current leaf, then advance leaf. Returns entry id.
  - `branch(method)` — [`L1999`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1999) — Start a new branch from an earlier entry.
  - `branchWithSummary(method)` — [`L2020`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L2020) — Start a new branch with a summary of the abandoned path.
  - `buildSessionContext(method)` — [`L1911`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1911) — Build the session context (what gets sent to the LLM).
  - `continueRecent(method)` — [`L2210`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L2210) — Continue the most recent session, or create new if none.
  - `create(method)` — [`L2147`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L2147) — Create a new session.
  - `createBranchedSession(method)` — [`L2044`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L2044) — Create a new session file containing only the path from root to the specified leaf.
  - `flushNow(method)` — [`L1449`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1449) — Force-write all in-memory entries to the session file immediately.
  - `forkFrom(method)` — [`L2231`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L2231) — Fork a session from another project directory into the current project.
  - `getActiveGitContext(method)` — [`L1734`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1734) — Active-branch git: nearest git_state from leaf to root, else the header snapshot.
  - `getBranch(method)` — [`L1894`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1894) — Walk from entry to root, returning all entries in path order.
  - `getChildren(method)` — [`L1844`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1844) — Get all direct children of an entry.
  - `getCwd(method)` — [`L1390`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1390)
  - `getEntries(method)` — [`L1933`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1933) — Get all session entries (excludes header). Returns a shallow copy.
  - `getEntry(method)` — [`L1837`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1837)
  - `getFlatTree(method)` — [`L1942`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1942) — Get the session as a tree structure. Returns a shallow defensive copy of all entries.
  - `getHeader(method)` — [`L1923`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1923) — Get session header.
  - `getLabel(method)` — [`L1857`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1857) — Get the label for an entry, if any.
  - `getLatestAgentStatus(method)` — [`L1745`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1745) — Get the latest agent status from the most recent agent_status entry, if any.
  - `getLeafEntry(method)` — [`L1833`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1833)
  - `getLeafId(method)` — [`L1829`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1829)
  - `getSessionArtifactDir(method)` — [`L1438`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1438)
  - `getSessionDir(method)` — [`L1394`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1394)
  - `getSessionFile(method)` — [`L1402`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1402)
  - `getSessionId(method)` — [`L1398`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1398)
  - `getSessionName(method)` — [`L1640`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1640) — Get the current session name from the latest session_info entry, if any.
  - `getSessionState(method)` — [`L1654`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1654) — Get the current session lifecycle state from the latest session_state entry, if any.
  - `getTree(method)` — [`L1950`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1950)
  - `hasUserContent(method)` — [`L1679`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1679) — True when the session holds user-meaningful persisted content, as opposed to
  - `inMemory(method)` — [`L2220`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L2220) — Create an in-memory session (no file persistence)
  - `isPersisted(method)` — [`L1386`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1386)
  - `list(method)` — [`L2294`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L2294) — List all sessions for a directory.
  - `listAll(method)` — [`L2318`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L2318) — List all sessions across all project directories.
  - `materializeSessionFile(method)` — [`L1406`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1406)
  - `newSession(method)` — [`L1268`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1268)
  - `onPersist(method)` — [`L1379`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1379)
  - `open(method)` — [`L2158`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L2158) — Open a specific session file.
  - `openAsync(method)` — [`L2191`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L2191) — Non-blocking open() for the daemon: parses off the event loop so a large load
  - `recordGitStateIfChanged(method)` — [`L1724`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1724)
  - `resetLeaf(method)` — [`L2011`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L2011) — Reset the leaf pointer to null (before any entries).
  - `setSessionFile(method)` — [`L1231`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1231) — Switch to a different session file (used for resume and branching).
  - `byId` — [`L1199`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1199)
  - `cwd` — [`L1195`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1195)
  - `fileEntries` — [`L1198`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1198)
  - `flushed` — [`L1197`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1197)
  - `labelTimestampsById` — [`L1201`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1201)
  - `labelsById` — [`L1200`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1200)
  - `leafId` — [`L1202`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1202)
  - `persist` — [`L1196`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1196)
  - `persistListeners` — [`L1203`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1203)
  - `sessionDir` — [`L1194`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1194)
  - `sessionFile` — [`L1193`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1193)
  - `sessionId` — [`L1192`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1192)
- protocol/private: `_appendEntry`[`L1477`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1477), `_appendEntryWithRollback`[`L1799`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1799), `_buildIndex`[`L1324`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1324), `_notifyPersistListeners`[`L1366`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1366), `_persist`[`L1456`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1456), `_rewriteFile`[`L1345`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1345)
- uses (calls/refs, reference-scoped): [`role`](../../../ai/src/types.ts.md#AssistantMessage.role), [`role`](../../../ai/src/types.ts.md#ToolResultMessage.role), [`role`](../../../ai/src/types.ts.md#UserMessage.role), [`role`](messages.ts.md#CustomMessage.role), [`role`](messages.ts.md#BashExecutionMessage.role), [`role`](messages.ts.md#BranchSummaryMessage.role), [`role`](messages.ts.md#CompactionSummaryMessage.role), [`usage`](../../../ai/src/types.ts.md#AssistantMessage.usage), [`type`](session-manager.ts.md#CompactionEntry.type), [`type`](session-manager.ts.md#CustomEntry.type), [`type`](session-manager.ts.md#LabelEntry.type), [`type`](session-manager.ts.md#ChildUsageAttributionEntry.type), [`type`](session-manager.ts.md#ModelChangeEntry.type), [`type`](session-manager.ts.md#AgentStatusEntry.type), [`type`](session-manager.ts.md#GitStateEntry.type), [`type`](session-manager.ts.md#SessionInfoEntry.type), [`type`](session-manager.ts.md#BranchSummaryEntry.type), [`type`](session-manager.ts.md#SessionStateEntry.type), [`type`](session-manager.ts.md#ServiceTierChangeEntry.type), [`type`](session-manager.ts.md#ThinkingLevelChangeEntry.type), [`type`](session-manager.ts.md#CustomMessageEntry.type), [`type`](session-manager.ts.md#SessionMessageEntry.type), [`id`](session-manager.ts.md#SessionEntryBase.id), [`ImageContent`](../../../ai/src/types.ts.md#ImageContent), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`SessionEntry`](session-manager.ts.md#SessionEntry), [`TextContent`](../../../ai/src/types.ts.md#TextContent), [`Message`](../../../ai/src/types.ts.md#Message), [`Usage`](../../../ai/src/types.ts.md#Usage), [`message`](session-manager.ts.md#SessionMessageEntry.message), [`CustomMessage`](messages.ts.md#CustomMessage), [`parentId`](session-manager.ts.md#SessionEntryBase.parentId), [`SessionInfo`](session-manager.ts.md#SessionInfo), [`timestamp`](session-manager.ts.md#SessionEntryBase.timestamp), [`type`](session-manager.ts.md#SessionHeader.type), [`migrateToCurrentVersion`](session-manager.ts.md#migrateToCurrentVersion), [`ServiceTier`](../../../ai/src/types.ts.md#ServiceTier), [`status`](session-manager.ts.md#SessionState.status), [`cloneUsage`](usage.ts.md#cloneUsage), [`FileEntry`](session-manager.ts.md#FileEntry)  (+99 more)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`main`](../main.ts.md#main), [`handleCommand`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.handleCommand), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`createAgentSession`](sdk.ts.md#createAgentSession), [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`_startRlmChildRun`](agent-session.ts.md#AgentSession._startRlmChildRun), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`agents-view-mode.ts`](../modes/agents-view/agents-view-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agents-view-agents-view-mode.ts), [`summaryForActiveSession`](../modes/daemon/daemon-session-list.ts.md#summaryForActiveSession), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`in-process-agent-connection.ts`](../modes/agent-connection/in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`_bindExtensionCore`](agent-session.ts.md#AgentSession._bindExtensionCore), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`createRlmSubagentRuntime`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRlmSubagentRuntime), [`_createInlineRlmSubagentRuntime`](agent-session.ts.md#AgentSession._createInlineRlmSubagentRuntime), [`createRuntime`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRuntime), [`runner.ts`](extensions/runner.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-runner.ts), [`sessionManager`](agent-session.ts.md#AgentSession.sessionManager), [`_processAgentEvent`](agent-session.ts.md#AgentSession._processAgentEvent), [`rehydrateCompletedRlmSubagentOnce`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.rehydrateCompletedRlmSubagentOnce), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`sdk.ts`](sdk.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-sdk.ts), [`sessionOptionsOverride`](../main.ts.md#prepareRuntimeServices.options-typeLiteral166.sessionOptionsOverride), [`<get>sessionFile`](agent-session.ts.md#AgentSession.-get-sessionFile), [`agent-session-runtime.ts`](agent-session-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-runtime.ts), [`agent-session-services.ts`](agent-session-services.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-services.ts), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`rlmChildSnapshotForActiveSession`](../modes/daemon/daemon-session-list.ts.md#rlmChildSnapshotForActiveSession), [`_buildRuntime`](agent-session.ts.md#AgentSession._buildRuntime), [`createRlmSubagentRuntime`](agent-session-runtime.ts.md#AgentSessionRuntime.createRlmSubagentRuntime), [`sendCustomMessage`](agent-session.ts.md#AgentSession.sendCustomMessage), [`<get>sessionId`](agent-session.ts.md#AgentSession.-get-sessionId), [`createAgentFamilyCatalog`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentFamilyCatalog), [`_emitExtensionEvent`](agent-session.ts.md#AgentSession._emitExtensionEvent), [`_applyRefine`](agent-session.ts.md#AgentSession._applyRefine), [`addRuntime`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.addRuntime), [`_checkCompaction`](agent-session.ts.md#AgentSession._checkCompaction)  (+102 more; 129 test-only)

### `SessionMessageEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:103`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L103)
- signature: `interface SessionMessageEntry`
- members:
  - `message` — [`L105`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L105)
  - `type` — [`L104`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L104)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../agent/src/types.ts.md#AgentMessage), [`SessionEntryBase`](session-manager.ts.md#SessionEntryBase)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`createAgentSession`](sdk.ts.md#createAgentSession), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`appendMessage`](session-manager.ts.md#SessionManager.appendMessage), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`SessionEntry`](session-manager.ts.md#SessionEntry), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`open`](session-manager.ts.md#SessionManager.open), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`handleCompactHostRequest`](agent-session.ts.md#AgentSession.handleCompactHostRequest), [`getHeader`](session-manager.ts.md#SessionManager.getHeader), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`prepareBranchEntries`](compaction/branch-summarization.ts.md#prepareBranchEntries), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`_restoreLateIpythonSentAgentMessages`](agent-session.ts.md#AgentSession._restoreLateIpythonSentAgentMessages), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`_loadPersistedGoalState`](agent-session.ts.md#AgentSession._loadPersistedGoalState), [`findTurnStartIndex`](compaction/compaction.ts.md#findTurnStartIndex), [`findValidCutPoints`](compaction/compaction.ts.md#findValidCutPoints)  (+19 more; 43 test-only)

### `SessionPersistListener`
- def: [`packages/coding-agent/src/core/session-manager.ts:94`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L94)
- signature: `type SessionPersistListener`
- used by: [`persistListeners`](session-manager.ts.md#SessionManager.persistListeners), [`onPersist`](session-manager.ts.md#SessionManager.onPersist)

### `SessionState`
- def: [`packages/coding-agent/src/core/session-manager.ts:195`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L195)
- signature: `interface SessionState`
- members:
  - `status` — [`L196`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L196)
- uses (calls/refs, reference-scoped): [`SessionStateStatus`](session-manager.ts.md#SessionStateStatus)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`addRuntime`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.addRuntime), [`appendSessionState`](session-manager.ts.md#SessionManager.appendSessionState), [`restoreRlmHeartbeatSession`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.restoreRlmHeartbeatSession), [`getSessionState`](session-manager.ts.md#SessionManager.getSessionState), [`deactivatePendingAgent`](../modes/agents-view/agents-view-mode.ts.md#AgentsViewMode.deactivatePendingAgent), [`handleCatalogRequest`](../modes/daemon/daemon-catalog-process.ts.md#handleCatalogRequest), [`state`](session-manager.ts.md#SessionInfo.state), [`isPersistedCronJobRunnable`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.isPersistedCronJobRunnable), [`inactiveLifecycleForSession`](../modes/daemon/daemon-session-list.ts.md#inactiveLifecycleForSession), [`archiveSession`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.archiveSession), [`SessionStateEntry`](session-manager.ts.md#SessionStateEntry)  (9 test-only)

### `SessionStateEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:200`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L200)
- doc: Session lifecycle state entry (e.g., inactive status for daemon-managed sessions).
- signature: `interface SessionStateEntry`
- members:
  - `state` — [`L202`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L202)
  - `type` — [`L201`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L201)
- uses (calls/refs, reference-scoped): [`SessionEntryBase`](session-manager.ts.md#SessionEntryBase), [`SessionState`](session-manager.ts.md#SessionState)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`createAgentSession`](sdk.ts.md#createAgentSession), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`SessionEntry`](session-manager.ts.md#SessionEntry), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`open`](session-manager.ts.md#SessionManager.open), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`handleCompactHostRequest`](agent-session.ts.md#AgentSession.handleCompactHostRequest), [`getHeader`](session-manager.ts.md#SessionManager.getHeader), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`prepareBranchEntries`](compaction/branch-summarization.ts.md#prepareBranchEntries), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`appendSessionState`](session-manager.ts.md#SessionManager.appendSessionState), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`_restoreLateIpythonSentAgentMessages`](agent-session.ts.md#AgentSession._restoreLateIpythonSentAgentMessages), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`_loadPersistedGoalState`](agent-session.ts.md#AgentSession._loadPersistedGoalState), [`findTurnStartIndex`](compaction/compaction.ts.md#findTurnStartIndex), [`findValidCutPoints`](compaction/compaction.ts.md#findValidCutPoints), [`getActiveGitContext`](session-manager.ts.md#SessionManager.getActiveGitContext)  (+16 more; 40 test-only)

### `SessionStateStatus`
- def: [`packages/coding-agent/src/core/session-manager.ts:193`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L193)
- signature: `type SessionStateStatus`
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`SessionState`](session-manager.ts.md#SessionState), [`normalizeSessionStateStatus`](session-manager.ts.md#normalizeSessionStateStatus)

### `SessionTreeFlatNode`
- def: [`packages/coding-agent/src/core/session-manager.ts:269`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L269)
- doc: Tree node for getTree() - defensive copy of session structure
- signature: `interface SessionTreeFlatNode`
- members:
  - `entry` — [`L270`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L270)
  - `label` — [`L272`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L272) — Resolved label for this entry, if any
  - `labelTimestamp` — [`L274`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L274) — Timestamp of the latest label change for this entry, if any
- uses (calls/refs, reference-scoped): [`SessionEntry`](session-manager.ts.md#SessionEntry)
- used by: [`getTree`](session-manager.ts.md#SessionManager.getTree), [`getFlatTree`](session-manager.ts.md#SessionManager.getFlatTree), [`SessionTreeNode`](session-manager.ts.md#SessionTreeNode)  (3 test-only)

### `SessionTreeNode`
- def: [`packages/coding-agent/src/core/session-manager.ts:277`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L277)
- signature: `interface SessionTreeNode`
- members:
  - `children` — [`L278`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L278)
- uses (calls/refs, reference-scoped): [`SessionTreeFlatNode`](session-manager.ts.md#SessionTreeFlatNode)
- used by: [`getTree`](session-manager.ts.md#SessionManager.getTree)  (2 test-only)

### `ThinkingLevelChangeEntry`
- def: [`packages/coding-agent/src/core/session-manager.ts:110`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L110)
- signature: `interface ThinkingLevelChangeEntry`
- members:
  - `thinkingLevel` — [`L112`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L112)
  - `type` — [`L111`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L111)
- uses (calls/refs, reference-scoped): [`SessionEntryBase`](session-manager.ts.md#SessionEntryBase)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`createAgentSession`](sdk.ts.md#createAgentSession), [`<constructor>`](agent-session.ts.md#AgentSession.-constructor), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`createAgentConnectionState`](../modes/agent-connection/snapshot.ts.md#createAgentConnectionState), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntries`](session-manager.ts.md#SessionManager.getEntries), [`signal`](agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`SessionEntry`](session-manager.ts.md#SessionEntry), [`scanSessionInfo`](session-manager.ts.md#scanSessionInfo), [`open`](session-manager.ts.md#SessionManager.open), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`forkFrom`](session-manager.ts.md#SessionManager.forkFrom), [`prepareCompaction`](compaction/compaction.ts.md#prepareCompaction), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`handleCompactHostRequest`](agent-session.ts.md#AgentSession.handleCompactHostRequest), [`getHeader`](session-manager.ts.md#SessionManager.getHeader), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`setSessionFile`](session-manager.ts.md#SessionManager.setSessionFile), [`prepareBranchEntries`](compaction/branch-summarization.ts.md#prepareBranchEntries), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`getMessageFromEntry`](compaction/compaction.ts.md#getMessageFromEntry), [`computeOwnAndTotalUsage`](context-tree.ts.md#computeOwnAndTotalUsage), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`computeContextUsageFromEntries`](context-tree.ts.md#computeContextUsageFromEntries), [`_buildIndex`](session-manager.ts.md#SessionManager._buildIndex), [`_restoreLateIpythonSentAgentMessages`](agent-session.ts.md#AgentSession._restoreLateIpythonSentAgentMessages), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry), [`updateLastActivityTime`](session-manager.ts.md#updateLastActivityTime), [`_loadPersistedGoalState`](agent-session.ts.md#AgentSession._loadPersistedGoalState), [`findTurnStartIndex`](compaction/compaction.ts.md#findTurnStartIndex), [`findValidCutPoints`](compaction/compaction.ts.md#findValidCutPoints), [`getActiveGitContext`](session-manager.ts.md#SessionManager.getActiveGitContext), [`migrateV1ToV2`](session-manager.ts.md#migrateV1ToV2)  (+16 more; 43 test-only)

## Functions
- `appendCappedSearchText(current: string, text: string)` — [`L915`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L915)
- `appendEntryFromBuffer(entries: FileEntry[], buffer: Buffer<ArrayBufferLike>, start?: number, end?: number)` — [`L613`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L613)
- `applyChildUsageAttributions(entries: FileEntry[])` — [`L447`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L447)
- `buildSessionContext(entries: SessionEntry[], leafId?: string | null | undefined, byId?: Map<string, SessionEntry> | undefined)` — [`L477`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L477) — Build the session context from entries using tree traversal.
- `createSessionId()` — [`L327`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L327)
- `createUniqueSessionFileTarget(sessionDir: string)` — [`L335`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L335)
- `deriveChildRlmDepth(parentHeader: Partial<SessionHeader> | undefined)` — [`L762`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L762)
- `extractJsonStringPropertyPrefix(text: string, propertyName: string, maxChars: number, startIndex?: number)` — [`L927`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L927)
- `extractOversizedMessageSummary(line: string)` — [`L970`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L970)
- `extractTextContent(message: Message)` — [`L850`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L850)
- `finalizeLoadedEntries(entries: FileEntry[])` — [`L652`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L652)
- `findMostRecentSession(sessionDir: string)` — [`L789`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L789) — Exported for testing
- `findMostRecentSessionForCwd(sessionDir: string, cwd: string)` — [`L821`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L821)
- `generateId(byId: { has(id: string): boolean; })` — [`L351`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L351) — Generate a unique short ID (8 hex chars, collision-checked)
- `getDefaultSessionDir(_cwd: string, agentDir?: string)` — [`L603`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L603) — Compute the default session directory for a cwd.
- `getLatestCompactionEntry(entries: SessionEntry[])` — [`L463`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L463)
- `getSessionArtifactPath(sessionDir: string, sessionId: string)` — [`L346`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L346)
- `getSessionFilePath(sessionDir: string, sessionId: string)` — [`L331`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L331)
- `getSessionModifiedDateFromLastActivity(lastActivityTime: number | undefined, header: SessionHeader, statsMtime: Date)` — [`L902`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L902)
- `has(method)` — [`L351`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L351)
- `isMessageWithContent(message: AgentMessage)` — [`L846`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L846)
- `isValidRlmDepth(value: unknown)` — [`L702`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L702)
- `isValidSessionFile(filePath: string)` — [`L779`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L779)
- `legacyChildDepthFromPath(sessionPath: string)` — [`L749`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L749)
- `listSessionsFromDir(dir: string, callbacks?: SessionListCallbacks | undefined, progressOffset?: number, progressTotal?: number | undefined)` — [`L1139`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1139)
- `loadEntriesFromFile(filePath: string)` — [`L663`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L663) — Exported for testing
- `loadEntriesFromFileAsync(filePath: string, options?: { streamThresholdBytes?: number | undefined; })` — [`L671`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L671)
- `looksLikeMessageEntry(line: string)` — [`L923`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L923)
- `migrateSessionEntries(entries: FileEntry[])` — [`L424`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L424) — Exported for testing
- `migrateToCurrentVersion(entries: FileEntry[])` — [`L411`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L411) — Run all necessary migrations to bring entries to current version.
- `migrateV1ToV2(entries: FileEntry[])` — [`L361`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L361) — Migrate v1 → v2: add id/parentId tree structure. Mutates in place.
- `migrateV2ToV3(entries: FileEntry[])` — [`L390`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L390) — Migrate v2 → v3: rename hookMessage role to custom. Mutates in place.
- `normalizeCwd(cwd: string)` — [`L804`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L804)
- `normalizeSessionStateStatus(value: unknown)` — [`L863`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L863)
- `parseEntriesFromBuffer(buffer: Buffer<ArrayBufferLike>)` — [`L622`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L622)
- `parseEntriesFromBufferAsync(buffer: Buffer<ArrayBufferLike>)` — [`L634`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L634)
- `parseSessionEntries(content: string)` — [`L429`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L429) — Exported for compaction.test.ts
- `readSessionHeader(filePath: string)` — [`L694`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L694)
- `readSessionInfo(filePath: string)` — [`L1005`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1005)
- `realpathIfPresent(path: string)` — [`L56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L56)
- `resolveLegacySessionRlmDepth(header: { rlmDepth?: number | undefined; parentSession?: string | undefined; }, sessionPath: string, visitedPaths: Set<string>)` — [`L713`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L713)
- `resolveSessionRlmDepth(header: { rlmDepth?: number | undefined; parentSession?: string | undefined; }, sessionPath: string)` — [`L706`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L706)
- `rootRlmDepthFromEnv()` — [`L767`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L767)
- `scanSessionInfo(filePath: string, stats: Stats | BigIntStats)` — [`L1021`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1021)
- `sessionHeaderMatchesCwd(header: Partial<SessionHeader> | undefined, cwd: string)` — [`L812`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L812)
- `sessionInfoMatchesCwd(session: SessionInfo, cwd: string)` — [`L808`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L808)
- `statMetadataIfPresent(path: string)` — [`L65`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L65)
- `updateLastActivityTime(lastActivityTime: number | undefined, entry: FileEntry)` — [`L873`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L873)

## Module values
- `CONTENT_ENTRY_TYPES` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L43)
- `CURRENT_SESSION_VERSION` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L33)
- `SESSION_ASYNC_PARSE_YIELD_BYTES` — [`L38`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L38)
- `SESSION_LIST_LARGE_MESSAGE_PREVIEW_MAX_CHARS` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L36)
- `SESSION_LIST_PARSE_MAX_LINE_CHARS` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L35)
- `SESSION_LIST_SEARCH_TEXT_MAX_CHARS` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L34)
- `SESSION_STREAMING_LOAD_THRESHOLD_BYTES` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L37)
- `parentSession` — [`L707`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L707)
- `parentSession` — [`L714`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L714)
- `rlmDepth` — [`L707`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L707)
- `rlmDepth` — [`L714`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L714)
- `role` — [`L971`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L971)
- `sessionFile` — [`L335`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L335)
- `sessionId` — [`L335`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L335)
- `sessionInfoCache` — [`L1003`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L1003)
- `streamThresholdBytes` — [`L673`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L673)
- `textPreview` — [`L973`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L973)
- `timestamp` — [`L972`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-manager.ts#L972)


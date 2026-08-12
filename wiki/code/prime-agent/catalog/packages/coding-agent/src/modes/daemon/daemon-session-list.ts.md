---
title: 'Module: packages/coding-agent/src/modes/daemon/daemon-session-list.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/daemon-session-list.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`daemon-session-list.ts`/
symbols:
  summaryForActiveSession: summaryForActiveSession().
  SessionSummary.activeSessionId: SessionSummary#activeSessionId.
  SessionSummary: SessionSummary#
  SessionSummary.sessionId: SessionSummary#sessionId.
  SessionSummary.id: SessionSummary#id.
  rlmChildSnapshotForActiveSession: rlmChildSnapshotForActiveSession().
  summaryForInactiveSession: summaryForInactiveSession().
  SessionSummary.sessionFile: SessionSummary#sessionFile.
  SessionSummary.activity: SessionSummary#activity.
  SessionSummary.sessionName: SessionSummary#sessionName.
  SessionSummary.workerPid: SessionSummary#workerPid.
  buildSessionList: buildSessionList().
  SessionSummary.isStreaming: SessionSummary#isStreaming.
  SessionSummary.lifecycle: SessionSummary#lifecycle.
  SessionSummary.runtimeKind: SessionSummary#runtimeKind.
  SessionSummary.cwd: SessionSummary#cwd.
  SessionSummary.sessionActions: SessionSummary#sessionActions.
  SessionSummary.parentActiveSessionId: SessionSummary#parentActiveSessionId.
  SessionSummary.messageCount: SessionSummary#messageCount.
  firstUserMessageText: firstUserMessageText().
  SessionSummary.isSessionActive: SessionSummary#isSessionActive.
  SessionSummary.rlmDepth: SessionSummary#rlmDepth.
  buildRlmChildSnapshots: buildRlmChildSnapshots().
  SessionSummary.taskState: SessionSummary#taskState.
  SessionSummary.parentSessionPath: SessionSummary#parentSessionPath.
  SessionSummary.attachedClients: SessionSummary#attachedClients.
  latestMessageActivityAt: latestMessageActivityAt().
  SessionSummary.isCompacting: SessionSummary#isCompacting.
  SessionSummary.parentSessionId: SessionSummary#parentSessionId.
  classifySessionRosterStatus: classifySessionRosterStatus().
  SessionSummary.hasActiveHeartbeat: SessionSummary#hasActiveHeartbeat.
  SessionSummary.created: SessionSummary#created.
  SessionSummary.modified: SessionSummary#modified.
  SessionSummary.model: SessionSummary#model.
  activeActivityForSession: activeActivityForSession().
  inactiveLifecycleForSession: inactiveLifecycleForSession().
  isSummaryCurrent: isSummaryCurrent().
  resolveAttachModelFallbackMessage: resolveAttachModelFallbackMessage().
  isActiveSessionBusy: isActiveSessionBusy().
  SessionSummary.firstMessage: SessionSummary#firstMessage.
  isSessionSummaryBusy: isSessionSummaryBusy().
  activeLifecycleForSession: activeLifecycleForSession().
  SessionSummary.spawnCode: SessionSummary#spawnCode.
  SessionSummary.summary: SessionSummary#summary.
  SessionSummary.streamingMessage: SessionSummary#streamingMessage.
  SessionSummary.rlmChildId: SessionSummary#rlmChildId.
  SessionSummary.lastActivityAt: SessionSummary#lastActivityAt.
  SessionLifecycle: SessionLifecycle#
  SessionActivity: SessionActivity#
  SessionSummary.hasRunningRlmChildren: SessionSummary#hasRunningRlmChildren.
  SessionSummary.unfinishedActionCount: SessionSummary#unfinishedActionCount.
  SessionSummary.workerState: SessionSummary#workerState.
  SessionSummary.isRunningTools: SessionSummary#isRunningTools.
  SessionSummary.rlmParentNodeId: SessionSummary#rlmParentNodeId.
  SessionSummary.modelFallbackMessage: SessionSummary#modelFallbackMessage.
  SessionSummary.diagnostics: SessionSummary#diagnostics.
  SessionSummary.hasRegisteredHeartbeat: SessionSummary#hasRegisteredHeartbeat.
  SessionSummary.hasRegisteredCronJob: SessionSummary#hasRegisteredCronJob.
  SessionSummary.thinkingLevel: SessionSummary#thinkingLevel.
  SessionSummary.repliedSinceTask: SessionSummary#repliedSinceTask.
  SessionSummary.isBashRunning: SessionSummary#isBashRunning.
  readMessageText: readMessageText().
  SessionRosterStatus: SessionRosterStatus#
  SPAWN_CODE_MAX_CHARS: SPAWN_CODE_MAX_CHARS.
  MAX_DATE_TIMESTAMP_MS: MAX_DATE_TIMESTAMP_MS.
---
# Module: [`packages/coding-agent/src/modes/daemon/daemon-session-list.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts)

## Classes
### `SessionActivity`
- def: [`packages/coding-agent/src/modes/daemon/daemon-session-list.ts:21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L21)
- signature: `type SessionActivity`
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`activity`](daemon-session-list.ts.md#SessionSummary.activity), [`restoreActiveSessionId`](daemon-mode.ts.md#DaemonModeOptions.worker.typeLiteral0.restoreActiveSessionId), [`activeActivityForSession`](daemon-session-list.ts.md#activeActivityForSession)  (2 test-only)

### `SessionLifecycle`
- def: [`packages/coding-agent/src/modes/daemon/daemon-session-list.ts:17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L17)
- signature: `type SessionLifecycle`
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`lifecycle`](daemon-session-list.ts.md#SessionSummary.lifecycle), [`restoreActiveSessionId`](daemon-mode.ts.md#DaemonModeOptions.worker.typeLiteral0.restoreActiveSessionId), [`inactiveLifecycleForSession`](daemon-session-list.ts.md#inactiveLifecycleForSession), [`activeLifecycleForSession`](daemon-session-list.ts.md#activeLifecycleForSession)  (2 test-only)

### `SessionRosterStatus`
- def: [`packages/coding-agent/src/modes/daemon/daemon-session-list.ts:22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L22)
- signature: `type SessionRosterStatus`
- used by: [`classifySessionRosterStatus`](daemon-session-list.ts.md#classifySessionRosterStatus)

### `SessionSummary`
- def: [`packages/coding-agent/src/modes/daemon/daemon-session-list.ts:30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L30) — documented in [packages-coding-agent-src-modes-daemon-daemon-session-list.ts](../../../../../../concepts/packages-coding-agent-src-modes-daemon-daemon-session-list.ts.md)
- signature: `interface SessionSummary`
- members:
  - `activeSessionId` — [`L45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L45)
  - `activity` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L33)
  - `attachedClients` — [`L58`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L58)
  - `created` — [`L63`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L63)
  - `cwd` — [`L49`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L49)
  - `diagnostics` — [`L75`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L75)
  - `firstMessage` — [`L65`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L65)
  - `hasActiveHeartbeat` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L35)
  - `hasRegisteredCronJob` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L39) — Any active or paused non-heartbeat scheduled job registered for this session.
  - `hasRegisteredHeartbeat` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L37) — Any active heartbeat registered for this session. Paused heartbeats do not pin residency.
  - `hasRunningRlmChildren` — [`L55`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L55)
  - `id` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L31)
  - `isBashRunning` — [`L54`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L54)
  - `isCompacting` — [`L53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L53)
  - `isRunningTools` — [`L57`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L57) — True while the agent is streaming with tool calls pending; drives the "running tools" label.
  - `isSessionActive` — [`L34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L34)
  - `isStreaming` — [`L52`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L52)
  - `lastActivityAt` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L41) — Latest message activity, used by the supervisor residency policy.
  - `lifecycle` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L32)
  - `messageCount` — [`L59`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L59)
  - `model` — [`L50`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L50)
  - `modelFallbackMessage` — [`L74`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L74)
  - `modified` — [`L64`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L64)
  - `parentActiveSessionId` — [`L66`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L66)
  - `parentSessionId` — [`L67`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L67)
  - `parentSessionPath` — [`L68`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L68)
  - `repliedSinceTask` — [`L70`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L70)
  - `rlmChildId` — [`L69`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L69)
  - `rlmDepth` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L44) — RLM spawn depth (0 for roots); fork edges preserve the source depth.
  - `rlmParentNodeId` — [`L71`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L71)
  - `runtimeKind` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L42)
  - `sessionActions` — [`L61`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L61)
  - `sessionFile` — [`L47`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L47)
  - `sessionId` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L46)
  - `sessionName` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L48)
  - `spawnCode` — [`L73`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L73) — Source of the IPython cell that spawned this subagent, for display.
  - `streamingMessage` — [`L62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L62)
  - `summary` — [`L77`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L77) — One-line background summary of what the agent is doing or just did.
  - `taskState` — [`L79`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L79) — Completion verdict for an idle session; absent while working or unjudged.
  - `thinkingLevel` — [`L51`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L51)
  - `unfinishedActionCount` — [`L60`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L60)
  - `workerPid` — [`L83`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L83) — Diagnostic process identity; clients must not use this as a stable session identifier.
  - `workerState` — [`L81`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L81) — Resident session-host process state, populated by the global supervisor.
- uses (calls/refs, reference-scoped): [`Model`](../../../../ai/src/types.ts.md#Model), [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage), [`Api`](../../../../ai/src/types.ts.md#Api), [`ThinkingLevel`](../../../../agent/src/types.ts.md#ThinkingLevel), [`AgentSessionRuntimeDiagnostic`](../../core/agent-session-services.ts.md#AgentSessionRuntimeDiagnostic), [`SessionActionSnapshot`](../../core/session-action-store.ts.md#SessionActionSnapshot), [`SessionLifecycle`](daemon-session-list.ts.md#SessionLifecycle), [`SessionActivity`](daemon-session-list.ts.md#SessionActivity), [`AgentTaskState`](../../core/session-manager.ts.md#AgentTaskState)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`main`](../../main.ts.md#main), [`daemon-mode.ts`](daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`main.ts`](../../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`daemon-supervisor.ts`](daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`handleCommand`](daemon-supervisor.ts.md#DaemonSupervisor.handleCommand), [`agents-view-mode.ts`](../agents-view/agents-view-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agents-view-agents-view-mode.ts), [`<constructor>`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.-constructor), [`daemon-agent-connection.ts`](../agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`summaryForActiveSession`](daemon-session-list.ts.md#summaryForActiveSession), [`launchWorker`](daemon-supervisor.ts.md#DaemonSupervisor.launchWorker), [`type`](daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type), [`daemon-protocol.ts`](daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`attach`](../agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.attach), [`buildAgentsViewRows`](../agents-view/agents-view-state.ts.md#buildAgentsViewRows), [`runAgentsViewMode`](../agents-view/agents-view-mode.ts.md#runAgentsViewMode), [`DaemonOutbound`](daemon-protocol.ts.md#DaemonOutbound), [`createAgentObserveSummary`](daemon-mode.ts.md#AgentDaemon.createAgentObserveSummary), [`summaryForInactiveSession`](daemon-session-list.ts.md#summaryForInactiveSession), [`createAgentMessageAgentSummary`](daemon-mode.ts.md#AgentDaemon.createAgentMessageAgentSummary), [`summaryForUnifiedRecord`](../agents-view/agents-view-state.ts.md#summaryForUnifiedRecord), [`daemon-launch.ts`](../../cli/daemon-launch.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-daemon-launch.ts), [`summary`](../agents-view/agents-view-state.ts.md#AgentsViewRow.summary), [`refreshWorkerSummaries`](daemon-supervisor.ts.md#DaemonSupervisor.refreshWorkerSummaries), [`agentPeerSummary`](daemon-supervisor.ts.md#DaemonSupervisor.agentPeerSummary), [`daemon-command.ts`](../../cli/daemon-command.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-daemon-command.ts), [`renderRow`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.renderRow), [`sessionPassivationSnapshot`](daemon-mode.ts.md#AgentDaemon.sessionPassivationSnapshot), [`getOrCreateTranscriptCache`](daemon-supervisor.ts.md#DaemonSupervisor.getOrCreateTranscriptCache), [`handleDeleteSelected`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.handleDeleteSelected), [`buildSessionListWithPassiveRlmSubagents`](daemon-mode.ts.md#AgentDaemon.buildSessionListWithPassiveRlmSubagents), [`setReplyTarget`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.setReplyTarget), [`summary`](../../main.ts.md#createDaemonClientConnection.Promise.typeLiteral503.summary), [`runIdleEvictionSweep`](daemon-supervisor.ts.md#DaemonSupervisor.runIdleEvictionSweep), [`reconcileUnifiedSessions`](../agents-view/agents-view-state.ts.md#reconcileUnifiedSessions), [`runOpen`](../../cli/daemon-command.ts.md#runOpen), [`workerEvictionSnapshot`](daemon-supervisor.ts.md#DaemonSupervisor.workerEvictionSnapshot), [`mapDaemonSessionSnapshot`](../agent-connection/daemon-agent-connection.ts.md#mapDaemonSessionSnapshot), [`buildSessionList`](daemon-session-list.ts.md#buildSessionList)  (+148 more; 51 test-only)

## Functions
- `activeActivityForSession(activeSession: ActiveSessionState)` — [`L454`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L454)
- `activeLifecycleForSession(activeSession: ActiveSessionState)` — [`L483`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L483)
- `buildRlmChildSnapshots(rootActiveSessionId: string, activeSessions: readonly ActiveSessionState[])` — [`L338`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L338) — Build snapshots for all RLM child sessions hosted by the daemon under the
- `buildSessionList(activeSessions: readonly ActiveSessionState[], savedSessions: readonly SessionInfo[], scheduledJobs?: readonly AgentCronJob[])` — [`L114`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L114)
- `classifySessionRosterStatus(summary: SessionSummary)` — [`L104`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L104)
- `firstUserMessageText(session: AgentSession)` — [`L415`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L415)
- `inactiveLifecycleForSession(session: SessionInfo)` — [`L475`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L475) — Lifecycle for an on-disk session not resident in the daemon. Explicitly
- `isActiveSessionBusy(activeSession: ActiveSessionState)` — [`L448`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L448)
- `isSessionSummaryBusy(summary: SessionSummary)` — [`L110`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L110)
- `isSummaryCurrent(activeSession: ActiveSessionState)` — [`L289`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L289)
- `latestMessageActivityAt(messages: readonly AgentMessage[])` — [`L273`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L273)
- `readMessageText(content: unknown)` — [`L428`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L428)
- `resolveAttachModelFallbackMessage(summary: SessionSummary, startupModelFallbackMessage: string | undefined)` — [`L94`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L94) — Pick the model fallback message to show when attaching to a daemon session.
- `rlmChildSnapshotForActiveSession(activeSession: ActiveSessionState, metadata: AgentSessionRuntimeMetadata, parentNodeId: string | undefined, parent: ActiveSessionState | undefined)` — [`L367`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L367)
- `summaryForActiveSession(activeSession: ActiveSessionState, savedSession?: SessionInfo | undefined, hasActiveHeartbeat?: boolean, hasRegisteredHeartbeat?: boolean, hasRegisteredCronJob?: boolean)` — [`L194`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L194) — documented in [packages-coding-agent-src-modes-daemon-daemon-session-list.ts](../../../../../../concepts/packages-coding-agent-src-modes-daemon-daemon-session-list.ts.md)
- `summaryForInactiveSession(session: SessionInfo, hasRegisteredHeartbeat?: boolean, hasRegisteredCronJob?: boolean)` — [`L294`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L294)

## Module values
- `MAX_DATE_TIMESTAMP_MS` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L27)
- `SPAWN_CODE_MAX_CHARS` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-list.ts#L26)


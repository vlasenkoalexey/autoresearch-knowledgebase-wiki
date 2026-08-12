---
title: 'Module: packages/coding-agent/src/modes/daemon/active-session-state.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/active-session-state.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`active-session-state.ts`/
symbols:
  ActiveSessionState.activeSessionId: ActiveSessionState#activeSessionId.
  ActiveSessionState.runtime: ActiveSessionState#runtime.
  ActiveSessionState: ActiveSessionState#
  DaemonSocketClient: DaemonSocketClient#
  DaemonSocketClient.socket: DaemonSocketClient#socket.
  DaemonSocketClient.attachedActiveSessionIds: DaemonSocketClient#attachedActiveSessionIds.
  DaemonSocketClient.catchupActiveSessionIds: DaemonSocketClient#catchupActiveSessionIds.
  ActiveSessionState.clients: ActiveSessionState#clients.
  DaemonSocketClient.id: DaemonSocketClient#id.
  ActiveSessionState.summaryState: ActiveSessionState#summaryState.
  resolveActiveSessionState: resolveActiveSessionState().
  DaemonSocketClient.snapshotStreaming: DaemonSocketClient#snapshotStreaming.
  DaemonSocketClient.capabilities: DaemonSocketClient#capabilities.
  ActiveSessionState.lastEventSequence: ActiveSessionState#lastEventSequence.
  ActiveSessionState.clientEnv: ActiveSessionState#clientEnv.
  ActiveSessionState.eventGeneration: ActiveSessionState#eventGeneration.
  DaemonSocketClient.backpressured: DaemonSocketClient#backpressured.
  ActiveSessionState.extensionUiRequests: ActiveSessionState#extensionUiRequests.
  createActiveSessionId: createActiveSessionId().
  DaemonSocketClient.detachInput: DaemonSocketClient#detachInput.
  DaemonSocketClient.supportsExtensionUi: DaemonSocketClient#supportsExtensionUi.
  DaemonSocketClient.snapshotActiveSessionIds: DaemonSocketClient#snapshotActiveSessionIds.
  DaemonSocketClient.catchupPurposes: DaemonSocketClient#catchupPurposes.
  formatSessionMatch: formatSessionMatch().
  DaemonSocketClient.transport: DaemonSocketClient#transport.
  DaemonSocketClient.snapshotActiveSessionCounts: DaemonSocketClient#snapshotActiveSessionCounts.
  ActiveSessionState.pendingAttaches: ActiveSessionState#pendingAttaches.
  DaemonSocketClient.catchupPromise: DaemonSocketClient#catchupPromise.
  DaemonSocketClient.capabilitiesByActiveSessionId: DaemonSocketClient#capabilitiesByActiveSessionId.
  DaemonSocketClient.authenticated: DaemonSocketClient#authenticated.
  DaemonSocketClient.snapshotTransferAbortControllers: DaemonSocketClient#snapshotTransferAbortControllers.
  DaemonSocketClient.catchupRetryTimer: DaemonSocketClient#catchupRetryTimer.
  ActiveSessionState.unsubscribe: ActiveSessionState#unsubscribe.
  uniqueStates: uniqueStates().
  formatAmbiguousSessionError: formatAmbiguousSessionError().
  AmbiguousActiveSessionError: AmbiguousActiveSessionError#
  DaemonSocketClient.snapshotTransferTails: DaemonSocketClient#snapshotTransferTails.
  ActiveSessionExtensionUiRequest: ActiveSessionExtensionUiRequest#
  ActiveSessionExtensionUiRequest.resolve: ActiveSessionExtensionUiRequest#resolve.
  AmbiguousActiveSessionError.-constructor: AmbiguousActiveSessionError#`<constructor>`().
  ActiveSessionIdIndex: ActiveSessionIdIndex#
  ActiveSessionIdIndex.has: ActiveSessionIdIndex#has().
---
# Module: [`packages/coding-agent/src/modes/daemon/active-session-state.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts)

## Classes
### `ActiveSessionExtensionUiRequest`
- def: [`packages/coding-agent/src/modes/daemon/active-session-state.ts:56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L56)
- signature: `interface ActiveSessionExtensionUiRequest`
- members:
  - `resolve` — [`L57`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L57)
- uses (calls/refs, reference-scoped): [`DaemonExtensionUIResponse`](daemon-protocol.ts.md#DaemonExtensionUIResponse)
- used by: [`handleCommand`](daemon-mode.ts.md#AgentDaemon.handleCommand), [`createExtensionUIContext`](daemon-extension-binding.ts.md#createExtensionUIContext), [`extensionUiRequests`](active-session-state.ts.md#ActiveSessionState.extensionUiRequests), [`cancelPendingExtensionUiRequests`](daemon-mode.ts.md#cancelPendingExtensionUiRequests)

### `ActiveSessionIdIndex`
- def: [`packages/coding-agent/src/modes/daemon/active-session-state.ts:60`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L60)
- signature: `interface ActiveSessionIdIndex`
- members:
  - `has(method)` — [`L61`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L61)
- used by: [`createActiveSessionId`](active-session-state.ts.md#createActiveSessionId)

### `ActiveSessionState`
- def: [`packages/coding-agent/src/modes/daemon/active-session-state.ts:34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L34) — documented in [packages-coding-agent-src-modes-daemon-active-session-state.ts](../../../../../../concepts/packages-coding-agent-src-modes-daemon-active-session-state.ts.md)
- signature: `interface ActiveSessionState`
- members:
  - `activeSessionId` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L35)
  - `clientEnv` — [`L53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L53) — Client env (e.g. herdr pane identity), merged over process.env for this
  - `clients` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L37)
  - `eventGeneration` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L41)
  - `extensionUiRequests` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L40)
  - `lastEventSequence` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L42)
  - `pendingAttaches` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L39) — Attach snapshots in flight: reserved for passivation busyness, but not yet event recipients.
  - `runtime` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L36) — documented in [packages-coding-agent-src-modes-daemon-active-session-state.ts](../../../../../../concepts/packages-coding-agent-src-modes-daemon-active-session-state.ts.md)
  - `summaryState` — [`L45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L45) — Latest background status summary, surfaced in the agents view.
  - `unsubscribe` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L43)
- uses (calls/refs, reference-scoped): [`DaemonSocketClient`](active-session-state.ts.md#DaemonSocketClient), [`AgentSessionRuntime`](../../core/agent-session-runtime.ts.md#AgentSessionRuntime), [`DaemonEventSequence`](daemon-protocol.ts.md#DaemonEventSequence), [`AgentStatus`](../../core/session-manager.ts.md#AgentStatus), [`ActiveSessionExtensionUiRequest`](active-session-state.ts.md#ActiveSessionExtensionUiRequest)
- used by: [`handleCommand`](daemon-mode.ts.md#AgentDaemon.handleCommand), [`daemon-mode.ts`](daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`summaryForActiveSession`](daemon-session-list.ts.md#summaryForActiveSession), [`createRlmSubagentRuntime`](daemon-mode.ts.md#AgentDaemon.createRlmSubagentRuntime), [`createRuntime`](daemon-mode.ts.md#AgentDaemon.createRuntime), [`rehydrateCompletedRlmSubagentOnce`](daemon-mode.ts.md#AgentDaemon.rehydrateCompletedRlmSubagentOnce), [`origin`](daemon-mode.ts.md#AgentDaemon.sendAgentSessionMessage.options-typeLiteral1160.origin), [`createSubagentRuntimeHost`](daemon-mode.ts.md#AgentDaemon.createSubagentRuntimeHost), [`createAgentObserveSummary`](daemon-mode.ts.md#AgentDaemon.createAgentObserveSummary), [`rlmChildSnapshotForActiveSession`](daemon-session-list.ts.md#rlmChildSnapshotForActiveSession), [`createExtensionUIContext`](daemon-extension-binding.ts.md#createExtensionUIContext), [`createAgentFamilyCatalog`](daemon-mode.ts.md#AgentDaemon.createAgentFamilyCatalog), [`createAgentMessageAgentSummary`](daemon-mode.ts.md#AgentDaemon.createAgentMessageAgentSummary), [`addRuntime`](daemon-mode.ts.md#AgentDaemon.addRuntime), [`createAgentMessageListResult`](daemon-mode.ts.md#AgentDaemon.createAgentMessageListResult), [`handleWorkerCommand`](daemon-mode.ts.md#AgentDaemon.handleWorkerCommand), [`createAgentObserveListResult`](daemon-mode.ts.md#AgentDaemon.createAgentObserveListResult), [`daemon-session-list.ts`](daemon-session-list.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-session-list.ts), [`bindActiveSessionState`](daemon-extension-binding.ts.md#bindActiveSessionState), [`getSessionState`](daemon-mode.ts.md#AgentDaemon.getSessionState), [`drainBackpressuredClientCatchups`](daemon-mode.ts.md#AgentDaemon.drainBackpressuredClientCatchups), [`createdAt`](daemon-mode.ts.md#AgentDaemon.recordRlmSubagentRegistryEntry.input-typeLiteral250.createdAt), [`sessionPassivationSnapshot`](daemon-mode.ts.md#AgentDaemon.sessionPassivationSnapshot), [`buildSessionListWithPassiveRlmSubagents`](daemon-mode.ts.md#AgentDaemon.buildSessionListWithPassiveRlmSubagents), [`deliveryMode`](daemon-mode.ts.md#AgentDaemon.createRlmHeartbeatForState.input-typeLiteral666.deliveryMode), [`sessions`](daemon-mode.ts.md#AgentDaemon.sessions), [`closeSessionOnce`](daemon-mode.ts.md#AgentDaemon.closeSessionOnce), [`buildRlmChildSnapshotsWithPassiveRlmSubagents`](daemon-mode.ts.md#AgentDaemon.buildRlmChildSnapshotsWithPassiveRlmSubagents), [`createHeartbeatForState`](daemon-mode.ts.md#AgentDaemon.createHeartbeatForState), [`daemon-extension-binding.ts`](daemon-extension-binding.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-extension-binding.ts), [`hydratePassiveRlmSubagent`](daemon-mode.ts.md#AgentDaemon.hydratePassiveRlmSubagent), [`createUpdateRestartSession`](daemon-mode.ts.md#AgentDaemon.createUpdateRestartSession), [`broadcastToSession`](daemon-mode.ts.md#AgentDaemon.broadcastToSession), [`summarize`](daemon-session-summarizer.ts.md#DaemonSessionSummarizer.summarize), [`runCronJob`](daemon-mode.ts.md#AgentDaemon.runCronJob), [`getOrCreateCronJobSession`](daemon-mode.ts.md#AgentDaemon.getOrCreateCronJobSession), [`passivateSession`](daemon-mode.ts.md#AgentDaemon.passivateSession), [`restoreRlmHeartbeatSession`](daemon-mode.ts.md#AgentDaemon.restoreRlmHeartbeatSession), [`status`](daemon-mode.ts.md#AgentDaemon.acceptAgentSessionMessage.Promise.typeLiteral2954.status), [`agentFamilyEntry`](daemon-mode.ts.md#AgentDaemon.agentFamilyEntry)  (+106 more; 33 test-only)

### `AmbiguousActiveSessionError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/modes/daemon/active-session-state.ts:73`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L73)
- signature: `class AmbiguousActiveSessionError`
- members:
  - `<constructor>(message: string)` — [`L74`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L74)
- used by: [`daemon-mode.ts`](daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`origin`](daemon-mode.ts.md#AgentDaemon.sendAgentSessionMessage.options-typeLiteral1160.origin), [`getOrHydrateBoundSessionState`](daemon-mode.ts.md#AgentDaemon.getOrHydrateBoundSessionState), [`getOrHydrateAuthorizedAgentFamilyTarget`](daemon-mode.ts.md#AgentDaemon.getOrHydrateAuthorizedAgentFamilyTarget), [`resolveActiveSessionState`](active-session-state.ts.md#resolveActiveSessionState), [`resolveAgentFamilySessionName`](daemon-mode.ts.md#AgentDaemon.resolveAgentFamilySessionName)

### `DaemonSocketClient`
- def: [`packages/coding-agent/src/modes/daemon/active-session-state.ts:8`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L8) — documented in [packages-coding-agent-src-modes-daemon-active-session-state.ts](../../../../../../concepts/packages-coding-agent-src-modes-daemon-active-session-state.ts.md)
- signature: `interface DaemonSocketClient`
- members:
  - `attachedActiveSessionIds` — [`L11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L11)
  - `authenticated` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L21)
  - `backpressured` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L20)
  - `capabilities` — [`L30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L30)
  - `capabilitiesByActiveSessionId` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L31)
  - `catchupActiveSessionIds` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L13) — Session events are dropped while the socket is blocked and replaced with one catch-up snapshot on drain.
  - `catchupPromise` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L17) — The single catch-up drain currently serving this client.
  - `catchupPurposes` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L15) — A real runtime replacement takes precedence over an ordinary resync for the same queued catch-up.
  - `catchupRetryTimer` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L19) — Delayed retry after transient catch-up snapshot preparation failure.
  - `detachInput` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L28)
  - `id` — [`L9`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L9)
  - `snapshotActiveSessionCounts` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L25)
  - `snapshotActiveSessionIds` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L24)
  - `snapshotStreaming` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L23)
  - `snapshotTransferAbortControllers` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L26)
  - `snapshotTransferTails` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L27)
  - `socket` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L10)
  - `supportsExtensionUi` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L29)
  - `transport` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L22)
- uses (calls/refs, reference-scoped): [`DaemonClientCapability`](daemon-protocol.ts.md#DaemonClientCapability)
- used by: [`handleCommand`](daemon-mode.ts.md#AgentDaemon.handleCommand), [`daemon-mode.ts`](daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`daemon-supervisor.ts`](daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`handleCommand`](daemon-supervisor.ts.md#DaemonSupervisor.handleCommand), [`handleWorkerFrame`](daemon-supervisor.ts.md#DaemonSupervisor.handleWorkerFrame), [`type`](daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type), [`shutdown`](daemon-supervisor.ts.md#DaemonSupervisor.shutdown), [`handleWorkerCommand`](daemon-mode.ts.md#AgentDaemon.handleWorkerCommand), [`handleConnection`](daemon-mode.ts.md#AgentDaemon.handleConnection), [`handleLine`](daemon-supervisor.ts.md#DaemonSupervisor.handleLine), [`cleanupSupervisorResourcesOnce`](daemon-supervisor.ts.md#DaemonSupervisor.cleanupSupervisorResourcesOnce), [`handleConnection`](daemon-supervisor.ts.md#DaemonSupervisor.handleConnection), [`handleLine`](daemon-mode.ts.md#AgentDaemon.handleLine), [`drainBackpressuredClientCatchups`](daemon-mode.ts.md#AgentDaemon.drainBackpressuredClientCatchups), [`closeSessionOnce`](daemon-mode.ts.md#AgentDaemon.closeSessionOnce), [`drainClientCatchups`](daemon-supervisor.ts.md#DaemonSupervisor.drainClientCatchups), [`streamWorkerSnapshot`](daemon-mode.ts.md#AgentDaemon.streamWorkerSnapshot), [`broadcastToSession`](daemon-mode.ts.md#AgentDaemon.broadcastToSession), [`workerEvictionSnapshot`](daemon-supervisor.ts.md#DaemonSupervisor.workerEvictionSnapshot), [`type`](daemon-mode.ts.md#AgentDaemon.prepareReplacementSnapshot.message-Extract.typeLiteral3411.type), [`shutdown`](daemon-mode.ts.md#AgentDaemon.shutdown), [`streamSnapshot`](daemon-supervisor.ts.md#DaemonSupervisor.streamSnapshot), [`cancelPreparedUpdateRestart`](daemon-mode.ts.md#AgentDaemon.cancelPreparedUpdateRestart), [`write`](daemon-mode.ts.md#AgentDaemon.write), [`clients`](active-session-state.ts.md#ActiveSessionState.clients), [`admission`](daemon-supervisor.ts.md#DaemonSupervisor.parseCommandAndRegisterPromptAdmission.typeLiteral846.admission), [`publicSummary`](daemon-supervisor.ts.md#DaemonSupervisor.publicSummary), [`type`](daemon-mode.ts.md#AgentDaemon.createAttachResult.command-Extract.typeLiteral2508.type), [`write`](daemon-supervisor.ts.md#DaemonSupervisor.write), [`beginUpdateRestartTransaction`](daemon-mode.ts.md#AgentDaemon.beginUpdateRestartTransaction), [`type`](daemon-mode.ts.md#AgentDaemon.beginReplacementSnapshot.message-Extract.typeLiteral3394.type), [`promoteOwnedWorker`](daemon-supervisor.ts.md#DaemonSupervisor.promoteOwnedWorker), [`findWorkerForClient`](daemon-supervisor.ts.md#DaemonSupervisor.findWorkerForClient), [`scheduleClientCatchupRetry`](daemon-mode.ts.md#AgentDaemon.scheduleClientCatchupRetry), [`detachClient`](daemon-supervisor.ts.md#DaemonSupervisor.detachClient), [`detachClientFromSession`](daemon-mode.ts.md#AgentDaemon.detachClientFromSession), [`finishClientSnapshotStreaming`](daemon-mode.ts.md#finishClientSnapshotStreaming), [`markClientSnapshotStreaming`](daemon-mode.ts.md#markClientSnapshotStreaming), [`revokeSupervisorClaim`](daemon-mode.ts.md#AgentDaemon.revokeSupervisorClaim), [`reserveSnapshotStream`](daemon-supervisor.ts.md#DaemonSupervisor.reserveSnapshotStream)  (+51 more; 39 test-only)

## Functions
- `createActiveSessionId(existingIds?: ActiveSessionIdIndex | undefined)` — [`L64`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L64)
- `formatAmbiguousSessionError(selector: string, states: readonly ActiveSessionState[])` — [`L129`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L129)
- `formatSessionMatch(state: ActiveSessionState)` — [`L133`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L133)
- `resolveActiveSessionState(sessions: ReadonlyMap<string, ActiveSessionState>, selector: string)` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L80)
- `uniqueStates(states: ActiveSessionState[])` — [`L121`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/active-session-state.ts#L121)


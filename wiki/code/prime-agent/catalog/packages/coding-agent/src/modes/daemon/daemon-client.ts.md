---
title: 'Module: packages/coding-agent/src/modes/daemon/daemon-client.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/daemon-client.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`daemon-client.ts`/
symbols:
  DaemonClient.request: DaemonClient#request().
  DaemonClient.close: DaemonClient#close().
  DaemonClient.connect: DaemonClient#connect().
  DaemonClient: DaemonClient#
  DaemonClient.requestWire: DaemonClient#requestWire().
  DaemonClient.handleLine: DaemonClient#handleLine().
  DaemonClient.-constructor: DaemonClient#`<constructor>`().
  DaemonClient.autoReconnect: DaemonClient#autoReconnect().
  DaemonClient.waitForHello: DaemonClient#waitForHello().
  DaemonClient.socket: DaemonClient#socket.
  DaemonClient.acknowledgeCommandResult: DaemonClient#acknowledgeCommandResult().
  DaemonHello: DaemonHello#
  DaemonClient.notifyClosed: DaemonClient#notifyClosed().
  DaemonClient.armPendingRequestTimeout: DaemonClient#armPendingRequestTimeout().
  DaemonClient.meetsCommandCompatibility: DaemonClient#meetsCommandCompatibility().
  DaemonClient.rejectAll: DaemonClient#rejectAll().
  DaemonSocketClosedError.-constructor: DaemonSocketClosedError#`<constructor>`().
  getDaemonSocketCloseReason: getDaemonSocketCloseReason().
  DaemonClientMessageListener: DaemonClientMessageListener#
  DaemonClient.disconnectForReconnect: DaemonClient#disconnectForReconnect().
  DaemonClient.resetTransportForReconnect: DaemonClient#resetTransportForReconnect().
  DaemonClient.supportsServerCapability: DaemonClient#supportsServerCapability().
  DaemonClient.onMessage: DaemonClient#onMessage().
  DaemonClient.onClose: DaemonClient#onClose().
  daemonEndpointDetails: daemonEndpointDetails().
  DaemonClient.reconnect: DaemonClient#reconnect().
  DaemonClient.-get-hello: DaemonClient#`<get>hello`().
  DaemonClient.pendingRequests: DaemonClient#pendingRequests.
  DaemonClient.reconnectOptions: DaemonClient#reconnectOptions.
  DaemonClient.helloMessage: DaemonClient#helloMessage.
  DaemonClient.emitReconnectStatus: DaemonClient#emitReconnectStatus().
  DaemonClient.-get-isConnected: DaemonClient#`<get>isConnected`().
  DaemonCapabilityUnavailableError.-constructor: DaemonCapabilityUnavailableError#`<constructor>`().
  DaemonClient.clearSocketReference: DaemonClient#clearSocketReference().
  DaemonClientRequestOptions: DaemonClientRequestOptions#
  DaemonClient.daemonClosingReason: DaemonClient#daemonClosingReason.
  DaemonClient.helloWaiters: DaemonClient#helloWaiters.
  DaemonClient.enableAutoReconnect: DaemonClient#enableAutoReconnect().
  DaemonClientCloseListener: DaemonClientCloseListener#
  PendingDaemonRequest.timeout: PendingDaemonRequest#timeout.
  DaemonClient.requestWorker: DaemonClient#requestWorker().
  DaemonCommandBody: DaemonCommandBody#
  DaemonClient.enableRequestRecovery: DaemonClient#enableRequestRecovery().
  DaemonWireCommandBody: DaemonWireCommandBody#
  DaemonClientRequestOptions.onProgress: DaemonClientRequestOptions#onProgress.
  DaemonClient.closed: DaemonClient#closed.
  isDaemonRequestProgress: isDaemonRequestProgress().
  isDaemonSavedSessionInfo: isDaemonSavedSessionInfo().
  DaemonClient.listeners: DaemonClient#listeners.
  DaemonClient.closeListeners: DaemonClient#closeListeners.
  DaemonCapabilityUnavailableError: DaemonCapabilityUnavailableError#
  DaemonClient.detachReader: DaemonClient#detachReader.
  DaemonClient.autoReconnectPromise: DaemonClient#autoReconnectPromise.
  DaemonClient.reconnectPromise: DaemonClient#reconnectPromise.
  DaemonClient.authenticateWorker: DaemonClient#authenticateWorker().
  DaemonClientProgressListener: DaemonClientProgressListener#
  PendingDaemonRequest.resolve: PendingDaemonRequest#resolve.
  PendingDaemonRequest.onProgress: PendingDaemonRequest#onProgress.
  PendingDaemonRequest.compatibilities: PendingDaemonRequest#compatibilities.
  DaemonClientReconnectOptions.onStatus: DaemonClientReconnectOptions#onStatus.
  PendingDaemonRequest.reject: PendingDaemonRequest#reject.
  PendingDaemonRequest.awaitingReconnect: PendingDaemonRequest#awaitingReconnect.
  DaemonClient.requestRecoveryEnabled: DaemonClient#requestRecoveryEnabled.
  isDaemonClosing: isDaemonClosing().
  isDaemonHello: isDaemonHello().
  isDaemonResponse: isDaemonResponse().
  PendingDaemonRequest: PendingDaemonRequest#
  PendingDaemonRequest.timeoutMs: PendingDaemonRequest#timeoutMs.
  PendingDaemonRequest.commandType: PendingDaemonRequest#commandType.
  PendingDaemonRequest.wireData: PendingDaemonRequest#wireData.
  PendingDaemonRequest.acknowledgeResult: PendingDaemonRequest#acknowledgeResult.
  DaemonSocketClosedError: DaemonSocketClosedError#
  DaemonClientReconnectStatus: DaemonClientReconnectStatus#
  DaemonClientReconnectOptions: DaemonClientReconnectOptions#
  DaemonClientReconnectOptions.recoverDaemon: DaemonClientReconnectOptions#recoverDaemon.
  DaemonClient.requestId: DaemonClient#requestId.
  DaemonClient.protocolClientId: DaemonClient#protocolClientId.
  DistributiveOmit: DistributiveOmit#
  DaemonClientReconnectOptions.timeoutMs: DaemonClientReconnectOptions#timeoutMs.
  DEFAULT_RECONNECT_TIMEOUT_MS: DEFAULT_RECONNECT_TIMEOUT_MS.
  RECONNECT_CONNECT_TIMEOUT_MS: RECONNECT_CONNECT_TIMEOUT_MS.
  RECONNECT_HELLO_TIMEOUT_MS: RECONNECT_HELLO_TIMEOUT_MS.
  MAX_RECONNECT_DELAY_MS: MAX_RECONNECT_DELAY_MS.
  delay: delay().
  isDaemonSavedSessionAgentStatus: isDaemonSavedSessionAgentStatus().
  DaemonHello.Extract.typeLiteral0.type: DaemonHello#Extract:typeLiteral0:type.
---
# Module: [`packages/coding-agent/src/modes/daemon/daemon-client.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts)

## Classes
### `DaemonCapabilityUnavailableError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/modes/daemon/daemon-client.ts:72`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L72)
- signature: `class DaemonCapabilityUnavailableError`
- members:
  - `<constructor>(command: "abort" | "prompt" | "kill" | "shutdown" | "restart" | "steer" | "follow_up" | "compact" | "refine" | "list" | "rename" | "fork" | "create" | "reload" | "extension_ui_response" | ... 82 more ... | "retry_worker", capability: DaemonServerCapability | undefined, afterReconnect?: boolean)` — [`L73`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L73)
- uses (calls/refs, reference-scoped): [`DaemonCommand`](daemon-protocol.ts.md#DaemonCommand), [`DaemonServerCapability`](daemon-protocol.ts.md#DaemonServerCapability)
- used by: [`main.ts`](../../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`daemon-agent-connection.ts`](../agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`request`](daemon-client.ts.md#DaemonClient.request), [`summary`](../../main.ts.md#createDaemonClientConnection.Promise.typeLiteral503.summary), [`handleLine`](daemon-client.ts.md#DaemonClient.handleLine), [`promptWithAdmissionCancellation`](../agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.promptWithAdmissionCancellation)  (1 test-only)

### `DaemonClient`
- def: [`packages/coding-agent/src/modes/daemon/daemon-client.ts:107`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L107)
- signature: `class DaemonClient`
- members:
  - `<constructor>(socketPath: string)` — [`L128`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L128)
  - `<get>hello` — [`L130`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L130)
  - `<get>isConnected` — [`L134`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L134)
  - `acknowledgeCommandResult(method)` — [`L498`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L498)
  - `armPendingRequestTimeout(method)` — [`L388`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L388)
  - `authenticateWorker(method)` — [`L331`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L331)
  - `autoReconnect(method)` — [`L553`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L553)
  - `clearSocketReference(method)` — [`L414`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L414)
  - `close(method)` — [`L399`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L399)
  - `connect(method)` — [`L169`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L169)
  - `disconnectForReconnect(method)` — [`L243`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L243)
  - `emitReconnectStatus(method)` — [`L601`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L601)
  - `enableAutoReconnect(method)` — [`L288`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L288) — Reconnect a global/raw daemon client after supervisor replacement.
  - `enableRequestRecovery(method)` — [`L283`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L283) — Keep in-flight command promises alive and resend their stable envelopes after reconnect.
  - `handleLine(method)` — [`L423`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L423)
  - `meetsCommandCompatibility(method)` — [`L321`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L321)
  - `notifyClosed(method)` — [`L539`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L539)
  - `onClose(method)` — [`L275`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L275)
  - `onMessage(method)` — [`L268`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L268)
  - `reconnect(method)` — [`L225`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L225)
  - `rejectAll(method)` — [`L516`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L516)
  - `request(method)` — [`L293`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L293)
  - `requestWire(method)` — [`L343`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L343)
  - `requestWorker(method)` — [`L339`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L339)
  - `resetTransportForReconnect(method)` — [`L255`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L255) — Discard a partially recovered transport so the next retry can reconnect cleanly.
  - `supportsServerCapability(method)` — [`L138`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L138)
  - `waitForHello(method)` — [`L143`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L143) — Wait for the daemon_hello greeting sent on connect.
  - `autoReconnectPromise` — [`L117`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L117)
  - `closeListeners` — [`L111`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L111)
  - `closed` — [`L118`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L118)
  - `daemonClosingReason` — [`L120`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L120)
  - `detachReader` — [`L109`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L109)
  - `helloMessage` — [`L119`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L119)
  - `helloWaiters` — [`L122`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L122)
  - `listeners` — [`L110`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L110)
  - `pendingRequests` — [`L112`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L112)
  - `protocolClientId` — [`L114`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L114)
  - `reconnectOptions` — [`L116`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L116)
  - `reconnectPromise` — [`L121`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L121)
  - `requestId` — [`L113`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L113)
  - `requestRecoveryEnabled` — [`L115`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L115)
  - `socket` — [`L108`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L108)
- uses (calls/refs, reference-scoped): [`DaemonCommand`](daemon-protocol.ts.md#DaemonCommand), [`DaemonOutbound`](daemon-protocol.ts.md#DaemonOutbound), [`DaemonResponse`](daemon-protocol.ts.md#DaemonResponse), [`createDaemonCommandEnvelope`](daemon-protocol.ts.md#createDaemonCommandEnvelope), [`DAEMON_PROTOCOL_VERSION`](daemon-protocol.ts.md#DAEMON_PROTOCOL_VERSION), [`serializeJsonLine`](../rpc/jsonl.ts.md#serializeJsonLine), [`attachJsonlLineReader`](../rpc/jsonl.ts.md#attachJsonlLineReader), [`getDaemonCommandCompatibilities`](daemon-protocol.ts.md#getDaemonCommandCompatibilities), [`DaemonHello`](daemon-client.ts.md#DaemonHello), [`DaemonWorkerCommand`](daemon-worker-protocol.ts.md#DaemonWorkerCommand), [`isDaemonMutatingCommand`](daemon-protocol.ts.md#isDaemonMutatingCommand), [`<constructor>`](daemon-client.ts.md#DaemonSocketClosedError.-constructor), [`version`](daemon-protocol.ts.md#DaemonProtocolInfo.version), [`DaemonClientMessageListener`](daemon-client.ts.md#DaemonClientMessageListener), [`daemonEndpointDetails`](daemon-client.ts.md#daemonEndpointDetails), [`DaemonClosingReason`](daemon-protocol.ts.md#DaemonClosingReason), [`capability`](daemon-protocol.ts.md#DaemonCommandCompatibility.capability), [`DaemonCommandEnvelope`](daemon-protocol.ts.md#DaemonCommandEnvelope), [`DaemonWorkerCommandBody`](daemon-worker-protocol.ts.md#DaemonWorkerCommandBody), [`<constructor>`](daemon-client.ts.md#DaemonCapabilityUnavailableError.-constructor), [`DaemonClientRequestOptions`](daemon-client.ts.md#DaemonClientRequestOptions), [`DaemonServerCapability`](daemon-protocol.ts.md#DaemonServerCapability), [`DaemonClientCloseListener`](daemon-client.ts.md#DaemonClientCloseListener), [`timeout`](daemon-client.ts.md#PendingDaemonRequest.timeout), [`DaemonCommandBody`](daemon-client.ts.md#DaemonCommandBody), [`DaemonCommandCompatibility`](daemon-protocol.ts.md#DaemonCommandCompatibility), [`DaemonProtocolVersion`](daemon-protocol.ts.md#DaemonProtocolVersion), [`DaemonWireCommandBody`](daemon-client.ts.md#DaemonWireCommandBody), [`DAEMON_COMMAND_ENVELOPE_MIN_PROTOCOL_VERSION`](daemon-protocol.ts.md#DAEMON_COMMAND_ENVELOPE_MIN_PROTOCOL_VERSION), [`isDaemonRequestProgress`](daemon-client.ts.md#isDaemonRequestProgress), [`minProtocol`](daemon-protocol.ts.md#DaemonCommandCompatibility.minProtocol), [`onProgress`](daemon-client.ts.md#DaemonClientRequestOptions.onProgress), [`compatibilities`](daemon-client.ts.md#PendingDaemonRequest.compatibilities), [`onProgress`](daemon-client.ts.md#PendingDaemonRequest.onProgress), [`onStatus`](daemon-client.ts.md#DaemonClientReconnectOptions.onStatus), [`resolve`](daemon-client.ts.md#PendingDaemonRequest.resolve), [`awaitingReconnect`](daemon-client.ts.md#PendingDaemonRequest.awaitingReconnect), [`reject`](daemon-client.ts.md#PendingDaemonRequest.reject), [`isDaemonClosing`](daemon-client.ts.md#isDaemonClosing), [`isDaemonHello`](daemon-client.ts.md#isDaemonHello)  (+16 more)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`daemon-mode.ts`](daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`main.ts`](../../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`agents-view-mode.ts`](../agents-view/agents-view-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agents-view-agents-view-mode.ts), [`daemon-agent-connection.ts`](../agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`package-manager-cli.ts`](../../package-manager-cli.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-package-manager-cli.ts), [`attach`](../agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.attach), [`originActiveSessionId`](../../package-manager-cli.ts.md#runDaemonUpdateRestartCoordinator.options-typeLiteral607.originActiveSessionId), [`<constructor>`](../agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.-constructor), [`daemon-launch.ts`](../../cli/daemon-launch.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-daemon-launch.ts), [`run`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.run), [`daemon-command.ts`](../../cli/daemon-command.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-daemon-command.ts), [`requestData`](../agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.requestData), [`handleDeleteSelected`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.handleDeleteSelected), [`restoreDaemonUpdateRestartSession`](../../package-manager-cli.ts.md#restoreDaemonUpdateRestartSession), [`daemon-ps.ts`](../../cli/daemon-ps.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-daemon-ps.ts), [`summary`](../../main.ts.md#createDaemonClientConnection.Promise.typeLiteral503.summary), [`dispose`](../agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.dispose), [`runOpen`](../../cli/daemon-command.ts.md#runOpen), [`runDaemonClientCommand`](../../cli/daemon-command.ts.md#runDaemonClientCommand), [`finish`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.finish), [`refreshSessions`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.refreshSessions), [`deactivatePendingAgent`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.deactivatePendingAgent), [`restoreDaemonUpdateRestart`](../../package-manager-cli.ts.md#restoreDaemonUpdateRestart), [`restoreConnectionAfterUpdate`](../agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.restoreConnectionAfterUpdate), [`openAgentsViewSession`](../agents-view/agents-view-mode.ts.md#openAgentsViewSession), [`reconnectClient`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.reconnectClient), [`saved-session-catalog.ts`](saved-session-catalog.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-saved-session-catalog.ts), [`stopAgentForDeletion`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.stopAgentForDeletion), [`runAgentsViewCommand`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.runAgentsViewCommand), [`prepareConnectedDaemonUpdateRestart`](../../package-manager-cli.ts.md#prepareConnectedDaemonUpdateRestart), [`probeDaemonVersion`](../../cli/daemon-launch.ts.md#probeDaemonVersion), [`createNewSession`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.createNewSession), [`killSubagent`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.killSubagent), [`listDaemonSavedSessions`](saved-session-catalog.ts.md#listDaemonSavedSessions), [`sendPrompt`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.sendPrompt), [`prepareDaemonUpdateRestart`](../../package-manager-cli.ts.md#prepareDaemonUpdateRestart), [`renameSession`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.renameSession), [`probeRunningDaemonSessions`](../../cli/daemon-launch.ts.md#probeRunningDaemonSessions)  (+59 more; 29 test-only)

### `DaemonClientCloseListener`
- def: [`packages/coding-agent/src/modes/daemon/daemon-client.ts:32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L32)
- signature: `type DaemonClientCloseListener`
- used by: [`onClose`](daemon-client.ts.md#DaemonClient.onClose), [`closeListeners`](daemon-client.ts.md#DaemonClient.closeListeners)  (6 test-only)

### `DaemonClientMessageListener`
- def: [`packages/coding-agent/src/modes/daemon/daemon-client.ts:31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L31)
- signature: `type DaemonClientMessageListener`
- uses (calls/refs, reference-scoped): [`DaemonOutbound`](daemon-protocol.ts.md#DaemonOutbound)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`daemon-command.ts`](../../cli/daemon-command.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-daemon-command.ts), [`onMessage`](daemon-client.ts.md#DaemonClient.onMessage), [`listeners`](daemon-client.ts.md#DaemonClient.listeners)  (6 test-only)

### `DaemonClientProgressListener`
- def: [`packages/coding-agent/src/modes/daemon/daemon-client.ts:33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L33)
- signature: `type DaemonClientProgressListener`
- uses (calls/refs, reference-scoped): [`DaemonRequestProgress`](daemon-protocol.ts.md#DaemonRequestProgress)
- used by: [`DaemonClientRequestOptions`](daemon-client.ts.md#DaemonClientRequestOptions), [`onProgress`](daemon-client.ts.md#PendingDaemonRequest.onProgress)

### `DaemonClientReconnectOptions`
- def: [`packages/coding-agent/src/modes/daemon/daemon-client.ts:96`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L96)
- signature: `interface DaemonClientReconnectOptions`
- members:
  - `onStatus` — [`L99`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L99)
  - `recoverDaemon` — [`L97`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L97)
  - `timeoutMs` — [`L98`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L98)
- uses (calls/refs, reference-scoped): [`DaemonClientReconnectStatus`](daemon-client.ts.md#DaemonClientReconnectStatus)
- used by: [`autoReconnect`](daemon-client.ts.md#DaemonClient.autoReconnect), [`reconnectOptions`](daemon-client.ts.md#DaemonClient.reconnectOptions), [`emitReconnectStatus`](daemon-client.ts.md#DaemonClient.emitReconnectStatus), [`enableAutoReconnect`](daemon-client.ts.md#DaemonClient.enableAutoReconnect)  (1 test-only)

### `DaemonClientReconnectStatus`
- def: [`packages/coding-agent/src/modes/daemon/daemon-client.ts:91`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L91)
- signature: `type DaemonClientReconnectStatus`
- used by: [`emitReconnectStatus`](daemon-client.ts.md#DaemonClient.emitReconnectStatus), [`onStatus`](daemon-client.ts.md#DaemonClientReconnectOptions.onStatus)

### `DaemonClientRequestOptions`
- def: [`packages/coding-agent/src/modes/daemon/daemon-client.ts:35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L35)
- signature: `interface DaemonClientRequestOptions`
- members:
  - `onProgress` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L36)
- uses (calls/refs, reference-scoped): [`DaemonClientProgressListener`](daemon-client.ts.md#DaemonClientProgressListener)
- used by: [`request`](daemon-client.ts.md#DaemonClient.request), [`requestWire`](daemon-client.ts.md#DaemonClient.requestWire)  (4 test-only)

### `DaemonCommandBody`
- def: [`packages/coding-agent/src/modes/daemon/daemon-client.ts:25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L25)
- signature: `type DaemonCommandBody`
- uses (calls/refs, reference-scoped): [`DaemonCommand`](daemon-protocol.ts.md#DaemonCommand), [`DistributiveOmit`](daemon-client.ts.md#DistributiveOmit)
- used by: [`request`](daemon-client.ts.md#DaemonClient.request), [`DaemonWireCommandBody`](daemon-client.ts.md#DaemonWireCommandBody)

### `DaemonHello`
- def: [`packages/coding-agent/src/modes/daemon/daemon-client.ts:29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L29)
- signature: `type DaemonHello`
- members:
  - `type` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L29)
- uses (calls/refs, reference-scoped): [`DaemonOutbound`](daemon-protocol.ts.md#DaemonOutbound)
- used by: [`package-manager-cli.ts`](../../package-manager-cli.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-package-manager-cli.ts), [`daemon-launch.ts`](../../cli/daemon-launch.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-daemon-launch.ts), [`waitForHello`](daemon-client.ts.md#DaemonClient.waitForHello), [`prepareConnectedDaemonUpdateRestart`](../../package-manager-cli.ts.md#prepareConnectedDaemonUpdateRestart), [`validateReplacementDaemon`](../../package-manager-cli.ts.md#validateReplacementDaemon), [`<constructor>`](../../cli/daemon-launch.ts.md#StaleDaemonError.-constructor), [`shutdownConnectedDaemonAndWait`](../../cli/daemon-launch.ts.md#shutdownConnectedDaemonAndWait), [`meetsCommandCompatibility`](daemon-client.ts.md#DaemonClient.meetsCommandCompatibility), [`<get>hello`](daemon-client.ts.md#DaemonClient.-get-hello), [`helloMessage`](daemon-client.ts.md#DaemonClient.helloMessage), [`helloWaiters`](daemon-client.ts.md#DaemonClient.helloWaiters), [`processIdentityFromDaemonHello`](../../cli/daemon-launch.ts.md#processIdentityFromDaemonHello), [`processIdentityFromDaemonHello`](../../package-manager-cli.ts.md#processIdentityFromDaemonHello), [`DaemonVersionProbe`](../../cli/daemon-launch.ts.md#DaemonVersionProbe), [`isDaemonHello`](daemon-client.ts.md#isDaemonHello)  (5 test-only)

### `DaemonSocketClosedError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/modes/daemon/daemon-client.ts:57`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L57)
- signature: `class DaemonSocketClosedError`
- members:
  - `<constructor>(socketPath: string, daemonClosingReason?: DaemonClosingReason | undefined, cause?: string | undefined)` — [`L58`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L58)
- uses (calls/refs, reference-scoped): [`daemonEndpointDetails`](daemon-client.ts.md#daemonEndpointDetails), [`DaemonClosingReason`](daemon-protocol.ts.md#DaemonClosingReason)
- used by: [`connect`](daemon-client.ts.md#DaemonClient.connect), [`getDaemonSocketCloseReason`](daemon-client.ts.md#getDaemonSocketCloseReason), [`disconnectForReconnect`](daemon-client.ts.md#DaemonClient.disconnectForReconnect), [`resetTransportForReconnect`](daemon-client.ts.md#DaemonClient.resetTransportForReconnect)  (2 test-only)

### `DaemonWireCommandBody`
- def: [`packages/coding-agent/src/modes/daemon/daemon-client.ts:27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L27)
- signature: `type DaemonWireCommandBody`
- uses (calls/refs, reference-scoped): [`DaemonWorkerCommandBody`](daemon-worker-protocol.ts.md#DaemonWorkerCommandBody), [`DaemonCommandBody`](daemon-client.ts.md#DaemonCommandBody)
- used by: [`requestWire`](daemon-client.ts.md#DaemonClient.requestWire)

### `DistributiveOmit`
- def: [`packages/coding-agent/src/modes/daemon/daemon-client.ts:24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L24)
- signature: `type DistributiveOmit`
- used by: [`DaemonCommandBody`](daemon-client.ts.md#DaemonCommandBody)

### `PendingDaemonRequest`
- def: [`packages/coding-agent/src/modes/daemon/daemon-client.ts:39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L39)
- signature: `interface PendingDaemonRequest`
- members:
  - `acknowledgeResult` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L48)
  - `awaitingReconnect` — [`L47`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L47)
  - `commandType` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L44)
  - `compatibilities` — [`L50`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L50) — Re-checked against the new hello before a reconnect replay.
  - `onProgress` — [`L45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L45)
  - `reject` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L41)
  - `resolve` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L40)
  - `timeout` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L42)
  - `timeoutMs` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L43)
  - `wireData` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L46)
- uses (calls/refs, reference-scoped): [`DaemonResponse`](daemon-protocol.ts.md#DaemonResponse), [`DaemonCommandCompatibility`](daemon-protocol.ts.md#DaemonCommandCompatibility), [`DaemonClientProgressListener`](daemon-client.ts.md#DaemonClientProgressListener)
- used by: [`requestWire`](daemon-client.ts.md#DaemonClient.requestWire), [`handleLine`](daemon-client.ts.md#DaemonClient.handleLine), [`armPendingRequestTimeout`](daemon-client.ts.md#DaemonClient.armPendingRequestTimeout), [`rejectAll`](daemon-client.ts.md#DaemonClient.rejectAll), [`pendingRequests`](daemon-client.ts.md#DaemonClient.pendingRequests)

## Functions
- `daemonEndpointDetails(socketPath: string)` — [`L53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L53)
- `delay(ms: number)` — [`L610`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L610)
- `getDaemonSocketCloseReason(error: Error)` — [`L87`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L87)
- `isDaemonClosing(value: unknown)` — [`L614`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L614)
- `isDaemonHello(value: unknown)` — [`L622`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L622)
- `isDaemonRequestProgress(value: unknown)` — [`L640`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L640)
- `isDaemonResponse(value: unknown)` — [`L630`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L630)
- `isDaemonSavedSessionAgentStatus(value: unknown)` — [`L680`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L680)
- `isDaemonSavedSessionInfo(value: unknown)` — [`L662`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L662)

## Module values
- `DEFAULT_RECONNECT_TIMEOUT_MS` — [`L102`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L102)
- `MAX_RECONNECT_DELAY_MS` — [`L105`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L105)
- `RECONNECT_CONNECT_TIMEOUT_MS` — [`L103`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L103)
- `RECONNECT_HELLO_TIMEOUT_MS` — [`L104`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client.ts#L104)


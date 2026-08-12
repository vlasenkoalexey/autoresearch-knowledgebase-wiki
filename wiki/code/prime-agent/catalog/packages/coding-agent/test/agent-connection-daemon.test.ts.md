---
title: 'Module: packages/coding-agent/test/agent-connection-daemon.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/agent-connection-daemon.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`agent-connection-daemon.test.ts`/
symbols:
  createAttachResult: createAttachResult().
  createConnectionState: createConnectionState().
  FakeDaemonClient.request: FakeDaemonClient#request().
  FakeDaemonClient.requests: FakeDaemonClient#requests.
  asDaemonClient: asDaemonClient().
  FakeDaemonClient: FakeDaemonClient#
  FakeDaemonClient.emitMessage: FakeDaemonClient#emitMessage().
  emitSequencedQueueUpdate: emitSequencedQueueUpdate().
  FakeDaemonClient.attachResultFactory: FakeDaemonClient#attachResultFactory.
  FakeDaemonClient.emitClose: FakeDaemonClient#emitClose().
  FakeDaemonClient.reconnectCount: FakeDaemonClient#reconnectCount.
  FakeDaemonClient.connected: FakeDaemonClient#connected.
  FakeDaemonClient.close: FakeDaemonClient#close().
  FakeDaemonClient.disconnectForReconnect: FakeDaemonClient#disconnectForReconnect().
  CreateAttachResultOptions.parent: CreateAttachResultOptions#parent.
  FakeDaemonClient.hello: FakeDaemonClient#hello.
  CreateAttachResultOptions.sessionContext: CreateAttachResultOptions#sessionContext.
  CreateAttachResultOptions.sessionTree: CreateAttachResultOptions#sessionTree.
  FakeDaemonClient.closeCount: FakeDaemonClient#closeCount.
  FakeDaemonClient.promptError: FakeDaemonClient#promptError.
  FakeDaemonClient.serverCapabilities: FakeDaemonClient#serverCapabilities.
  FakeDaemonClient.connect: FakeDaemonClient#connect().
  FakeDaemonClient.reconnect: FakeDaemonClient#reconnect().
  FakeDaemonClient.updateRestartSessions: FakeDaemonClient#updateRestartSessions.
  FakeDaemonClient.messageListeners: FakeDaemonClient#messageListeners.
  FakeDaemonClient.closeListeners: FakeDaemonClient#closeListeners.
  FakeDaemonClient.promptGate: FakeDaemonClient#promptGate.
  FakeDaemonClient.cancelPromptAdmissionStatus: FakeDaemonClient#cancelPromptAdmissionStatus.
  CreateAttachResultOptions.replay: CreateAttachResultOptions#replay.
  FakeDaemonClient.reconnectError: FakeDaemonClient#reconnectError.
  FakeDaemonClient.onMessage: FakeDaemonClient#onMessage().
  FakeDaemonClient.onClose: FakeDaemonClient#onClose().
  FakeDaemonClient.waitForHello: FakeDaemonClient#waitForHello().
  FakeDaemonClient.resetTransportForReconnect: FakeDaemonClient#resetTransportForReconnect().
  FakeDaemonClient.connectionStateFactory: FakeDaemonClient#connectionStateFactory.
  CreateAttachResultOptions.streamingMessage: CreateAttachResultOptions#streamingMessage.
  FakeDaemonClient.promptResponseError: FakeDaemonClient#promptResponseError.
  FakeDaemonClient.getMessageListenerCount: FakeDaemonClient#getMessageListenerCount().
  FakeDaemonClient.getCloseListenerCount: FakeDaemonClient#getCloseListenerCount().
  CreateAttachResultOptions.state: CreateAttachResultOptions#state.
  CreateAttachResultOptions.messages: CreateAttachResultOptions#messages.
  FakeDaemonClient.requestTimeouts: FakeDaemonClient#requestTimeouts.
  FakeDaemonClient.restoredAttachGate: FakeDaemonClient#restoredAttachGate.
  FakeDaemonClient.emitCloseOnClose: FakeDaemonClient#emitCloseOnClose.
  FakeDaemonClient.attachFailures: FakeDaemonClient#attachFailures.
  FakeDaemonClient.supportsServerCapability: FakeDaemonClient#supportsServerCapability().
  FakeDaemonClient.restoredAttachCompleted: FakeDaemonClient#restoredAttachCompleted.
  FakeDaemonClient.resetTransportCount: FakeDaemonClient#resetTransportCount.
  FakeDaemonClient.connectionStateGate: FakeDaemonClient#connectionStateGate.
  FakeDaemonClient.abortBashUnknownCommand: FakeDaemonClient#abortBashUnknownCommand.
  FakeDaemonClient.abortAndClearQueueUnknownCommand: FakeDaemonClient#abortAndClearQueueUnknownCommand.
  FakeDaemonClient.cronAddGate: FakeDaemonClient#cronAddGate.
  CreateAttachResultOptions: CreateAttachResultOptions#
  CreateAttachResultOptions.omitSessionContext: CreateAttachResultOptions#omitSessionContext.
  FakeDaemonClient.enableRequestRecovery: FakeDaemonClient#enableRequestRecovery().
---
# Module: [`packages/coding-agent/test/agent-connection-daemon.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts)

## Classes
### `CreateAttachResultOptions`
- def: [`packages/coding-agent/test/agent-connection-daemon.test.ts:595`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L595)
- signature: `interface CreateAttachResultOptions`
- members:
  - `messages` — [`L597`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L597)
  - `omitSessionContext` — [`L600`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L600)
  - `parent` — [`L602`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L602)
  - `replay` — [`L603`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L603)
  - `sessionContext` — [`L599`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L599)
  - `sessionTree` — [`L601`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L601)
  - `state` — [`L596`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L596)
  - `streamingMessage` — [`L598`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L598)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../agent/src/types.ts.md#AgentMessage), [`DaemonAttachResult`](../src/modes/daemon/daemon-protocol.ts.md#DaemonAttachResult), [`snapshot`](../src/modes/daemon/daemon-protocol.ts.md#DaemonAttachResult.snapshot), [`AgentConnectionState`](../src/modes/agent-connection/types.ts.md#AgentConnectionState), [`replay`](../src/modes/daemon/daemon-protocol.ts.md#DaemonAttachResult.replay), [`sessionContext`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSessionSnapshot.sessionContext), [`parent`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSessionSnapshot.parent), [`sessionTree`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSessionSnapshot.sessionTree)
- used by: (1 test-only callers)

### `FakeDaemonClient`
- def: [`packages/coding-agent/test/agent-connection-daemon.test.ts:34`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L34)
- signature: `class FakeDaemonClient`
- members:
  - `close(method)` — [`L540`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L540)
  - `connect(method)` — [`L501`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L501)
  - `disconnectForReconnect(method)` — [`L548`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L548)
  - `emitClose(method)` — [`L493`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L493)
  - `emitMessage(method)` — [`L487`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L487)
  - `enableRequestRecovery(method)` — [`L499`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L499)
  - `getCloseListenerCount(method)` — [`L536`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L536)
  - `getMessageListenerCount(method)` — [`L532`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L532)
  - `onClose(method)` — [`L480`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L480)
  - `onMessage(method)` — [`L473`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L473)
  - `reconnect(method)` — [`L521`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L521)
  - `request(method)` — [`L69`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L69)
  - `resetTransportForReconnect(method)` — [`L516`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L516)
  - `supportsServerCapability(method)` — [`L469`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L469)
  - `waitForHello(method)` — [`L512`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L512)
  - `abortAndClearQueueUnknownCommand` — [`L50`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L50)
  - `abortBashUnknownCommand` — [`L49`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L49)
  - `attachFailures` — [`L46`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L46)
  - `attachResultFactory` — [`L37`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L37)
  - `cancelPromptAdmissionStatus` — [`L55`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L55)
  - `closeCount` — [`L40`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L40)
  - `closeListeners` — [`L67`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L67)
  - `connected` — [`L42`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L42)
  - `connectionStateFactory` — [`L48`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L48)
  - `connectionStateGate` — [`L47`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L47)
  - `cronAddGate` — [`L51`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L51)
  - `emitCloseOnClose` — [`L41`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L41)
  - `hello` — [`L58`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L58)
  - `messageListeners` — [`L66`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L66)
  - `promptError` — [`L53`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L53)
  - `promptGate` — [`L52`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L52)
  - `promptResponseError` — [`L54`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L54)
  - `reconnectCount` — [`L43`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L43)
  - `reconnectError` — [`L45`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L45)
  - `requestTimeouts` — [`L36`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L36)
  - `requests` — [`L35`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L35)
  - `resetTransportCount` — [`L44`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L44)
  - `restoredAttachCompleted` — [`L39`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L39)
  - `restoredAttachGate` — [`L38`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L38)
  - `serverCapabilities` — [`L56`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L56)
  - `updateRestartSessions` — [`L57`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L57)
- uses (calls/refs, reference-scoped): [`getModel`](../../ai/src/models.ts.md#getModel), [`DaemonCommand`](../src/modes/daemon/daemon-protocol.ts.md#DaemonCommand), [`DaemonOutbound`](../src/modes/daemon/daemon-protocol.ts.md#DaemonOutbound), [`DaemonAttachResult`](../src/modes/daemon/daemon-protocol.ts.md#DaemonAttachResult), [`DaemonResponse`](../src/modes/daemon/daemon-protocol.ts.md#DaemonResponse), [`AgentConnectionState`](../src/modes/agent-connection/types.ts.md#AgentConnectionState), [`DAEMON_PROTOCOL_INFO`](../src/modes/daemon/daemon-protocol.ts.md#DAEMON_PROTOCOL_INFO), [`DaemonHello`](../src/modes/daemon/daemon-client.ts.md#DaemonHello), [`clientId`](../src/modes/daemon/daemon-protocol.ts.md#DaemonAttachClientMetadata.clientId), [`capabilities`](../src/modes/daemon/daemon-protocol.ts.md#DaemonAttachClientMetadata.capabilities), [`DAEMON_SCHEMA_REVISION`](../src/modes/daemon/daemon-protocol.ts.md#DAEMON_SCHEMA_REVISION), [`<constructor>`](../src/modes/daemon/daemon-client.ts.md#DaemonSocketClosedError.-constructor), [`DaemonClientMessageListener`](../src/modes/daemon/daemon-client.ts.md#DaemonClientMessageListener), [`DaemonClientRequestOptions`](../src/modes/daemon/daemon-client.ts.md#DaemonClientRequestOptions), [`DaemonClientCloseListener`](../src/modes/daemon/daemon-client.ts.md#DaemonClientCloseListener), [`onProgress`](../src/modes/daemon/daemon-client.ts.md#DaemonClientRequestOptions.onProgress), [`fallbackCwd`](../src/core/session-cwd.ts.md#SessionCwdIssue.fallbackCwd), [`id`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.id), [`allMessagesText`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.allMessagesText), [`created`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.created), [`cwd`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.cwd), [`firstMessage`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.firstMessage), [`messageCount`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.messageCount), [`modified`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.modified), [`path`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.path), [`sessionFile`](../src/core/session-cwd.ts.md#SessionCwdIssue.sessionFile), [`name`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.name), [`sessionCwd`](../src/core/session-cwd.ts.md#SessionCwdIssue.sessionCwd)  (2 test-only)
- used by: (3 test-only callers)

## Functions
- `asDaemonClient(client: FakeDaemonClient)` — [`L555`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L555)
- `createAttachResult(activeSessionId: string, clientId: string | undefined, capabilities: readonly string[] | undefined, lastEventSequence: number, options?: CreateAttachResultOptions)` — [`L606`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L606)
- `createConnectionState(activeSessionId: string, sessionId: string)` — [`L559`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L559)
- `emitSequencedQueueUpdate(client: FakeDaemonClient, activeSessionId: string, sequence: number)` — [`L679`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-daemon.test.ts#L679)


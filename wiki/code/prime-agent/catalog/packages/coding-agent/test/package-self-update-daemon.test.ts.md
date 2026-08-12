---
title: 'Module: packages/coding-agent/test/package-self-update-daemon.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/package-self-update-daemon.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`package-self-update-daemon.test.ts`/
symbols:
  mockState: mockState.
  MockDaemonRequest.type: MockDaemonRequest#type.
  MockUpdateRestartSession.queue.typeLiteral10.actions.typeLiteral11.actions: MockUpdateRestartSession#queue.typeLiteral10:actions.typeLiteral11:actions.
  MockUpdateRestartManifest.sessions: MockUpdateRestartManifest#sessions.
  MockUpdateRestartSession.queue.typeLiteral10.nextTurn: MockUpdateRestartSession#queue.typeLiteral10:nextTurn.
  MockUpdateRestartSession.queue: MockUpdateRestartSession#queue.
  MockUpdateRestartSession.queue.typeLiteral10.actions: MockUpdateRestartSession#queue.typeLiteral10:actions.
  useFixedOwnerHello: useFixedOwnerHello().
  MockUpdateRestartSession.activeSessionId: MockUpdateRestartSession#activeSessionId.
  MockUpdateRestartSession.sessionId: MockUpdateRestartSession#sessionId.
  MockUpdateRestartSession.sessionFile: MockUpdateRestartSession#sessionFile.
  MockUpdateRestartSession.cwd: MockUpdateRestartSession#cwd.
  MockUpdateRestartSession.config: MockUpdateRestartSession#config.
  MockUpdateRestartSession.queue.typeLiteral10.actions.typeLiteral11.formatVersion: MockUpdateRestartSession#queue.typeLiteral10:actions.typeLiteral11:formatVersion.
  MockUpdateRestartSession.shouldResume: MockUpdateRestartSession#shouldResume.
  MockUpdateRestartSession.wasStreaming: MockUpdateRestartSession#wasStreaming.
  MockUpdateRestartSession.wasCompacting: MockUpdateRestartSession#wasCompacting.
  MockUpdateRestartSession.wasBashRunning: MockUpdateRestartSession#wasBashRunning.
  MockUpdateRestartSession.hadRunningRlmChildren: MockUpdateRestartSession#hadRunningRlmChildren.
  MockUpdateRestartSession.wasRetrying: MockUpdateRestartSession#wasRetrying.
  MockUpdateRestartSession.hadAcceptedPromptInFlight: MockUpdateRestartSession#hadAcceptedPromptInFlight.
  MockUpdateRestartManifest.formatVersion: MockUpdateRestartManifest#formatVersion.
  MockUpdateRestartManifest.createdAt: MockUpdateRestartManifest#createdAt.
  MockRecoveryAction.payload: MockRecoveryAction#payload.
  MockCustomMessage: MockCustomMessage#
  MockRunningDaemonProbe: MockRunningDaemonProbe#
  MockUpdateRestartSession.runtimeMetadata: MockUpdateRestartSession#runtimeMetadata.
  MockRecoveryAction: MockRecoveryAction#
  MockRecoveryAction.payload.typeLiteral7.kind: MockRecoveryAction#payload.typeLiteral7:kind.
  MockRecoveryAction.payload.typeLiteral7.text: MockRecoveryAction#payload.typeLiteral7:text.
  createMockTurnExecutionPolicy: createMockTurnExecutionPolicy().
  MockRecoveryAction.id: MockRecoveryAction#id.
  MockRecoveryAction.source: MockRecoveryAction#source.
  MockRecoveryAction.delivery: MockRecoveryAction#delivery.
  MockRecoveryAction.wake: MockRecoveryAction#wake.
  MockRecoveryAction.agentMessageId: MockRecoveryAction#agentMessageId.
  MockUpdateRestartManifest: MockUpdateRestartManifest#
  MockDaemonRequest.sessionPath: MockDaemonRequest#sessionPath.
  MockDaemonResponse: MockDaemonResponse#
  MockDaemonRequest.customMessage: MockDaemonRequest#customMessage.
  MockDaemonRequest.prefixMessages: MockDaemonRequest#prefixMessages.
  MockDaemonRequest.messages: MockDaemonRequest#messages.
  MockDaemonRequest.runtimeMetadata: MockDaemonRequest#runtimeMetadata.
  MockSessionSummary: MockSessionSummary#
  MockSessionSummary.isStreaming: MockSessionSummary#isStreaming.
  MockSessionSummary.isCompacting: MockSessionSummary#isCompacting.
  MockSessionSummary.sessionActions: MockSessionSummary#sessionActions.
  MockSessionSummary.sessionActions.typeLiteral0.queuedCount: MockSessionSummary#sessionActions.typeLiteral0:queuedCount.
  MockCustomMessage.role: MockCustomMessage#role.
  MockCustomMessage.customType: MockCustomMessage#customType.
  MockCustomMessage.content: MockCustomMessage#content.
  MockCustomMessage.display: MockCustomMessage#display.
  MockCustomMessage.timestamp: MockCustomMessage#timestamp.
  MockDaemonRequest: MockDaemonRequest#
  MockSessionSummary.id: MockSessionSummary#id.
  MockSessionSummary.activeSessionId: MockSessionSummary#activeSessionId.
  MockSessionSummary.isBashRunning: MockSessionSummary#isBashRunning.
  MockSessionSummary.hasRunningRlmChildren: MockSessionSummary#hasRunningRlmChildren.
  MockSessionSummary.sessionActions.typeLiteral0.steering: MockSessionSummary#sessionActions.typeLiteral0:steering.
  MockSessionSummary.sessionActions.typeLiteral0.followUps: MockSessionSummary#sessionActions.typeLiteral0:followUps.
  MockRecoveryAction.queueKey: MockRecoveryAction#queueKey.
  MockUpdateRestartSession: MockUpdateRestartSession#
  MockDaemonRequest.activeSessionId: MockDaemonRequest#activeSessionId.
  MockCustomMessage.details: MockCustomMessage#details.
  MockRecoveryAction.snapshot: MockRecoveryAction#snapshot.
  MockDaemonRequest.message: MockDaemonRequest#message.
  MockDaemonRequest.agentMessageId: MockDaemonRequest#agentMessageId.
  MockDaemonRequest.content: MockDaemonRequest#content.
  MockDaemonRequest.queueKey: MockDaemonRequest#queueKey.
  MockDaemonRequest.snapshot: MockDaemonRequest#snapshot.
---
# Module: [`packages/coding-agent/test/package-self-update-daemon.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts)

## Classes
### `MockCustomMessage`
- def: [`packages/coding-agent/test/package-self-update-daemon.test.ts:42`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L42)
- signature: `interface MockCustomMessage`
- members:
  - `content` — [`L45`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L45)
  - `customType` — [`L44`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L44)
  - `details` — [`L48`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L48)
  - `display` — [`L46`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L46)
  - `role` — [`L43`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L43)
  - `timestamp` — [`L47`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L47)
- used by: (5 test-only callers)

### `MockDaemonRequest`
- def: [`packages/coding-agent/test/package-self-update-daemon.test.ts:105`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L105)
- signature: `interface MockDaemonRequest`
- members:
  - `activeSessionId` — [`L107`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L107)
  - `agentMessageId` — [`L109`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L109)
  - `content` — [`L112`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L112)
  - `customMessage` — [`L110`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L110)
  - `message` — [`L108`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L108)
  - `messages` — [`L113`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L113)
  - `prefixMessages` — [`L111`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L111)
  - `queueKey` — [`L114`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L114)
  - `runtimeMetadata` — [`L117`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L117)
  - `sessionPath` — [`L116`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L116)
  - `snapshot` — [`L115`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L115)
  - `type` — [`L106`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L106)
- uses (calls/refs, reference-scoped): [`AgentSessionRuntimeMetadata`](../src/core/agent-session-runtime.ts.md#AgentSessionRuntimeMetadata)  (1 test-only)
- used by: (2 test-only callers)

### `MockDaemonResponse`
- def: [`packages/coding-agent/test/package-self-update-daemon.test.ts:120`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L120)
- signature: `type MockDaemonResponse`
- used by: (2 test-only callers)

### `MockRecoveryAction`
- def: [`packages/coding-agent/test/package-self-update-daemon.test.ts:51`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L51)
- signature: `interface MockRecoveryAction`
- members:
  - `agentMessageId` — [`L58`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L58)
  - `delivery` — [`L54`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L54)
  - `id` — [`L52`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L52)
  - `kind` — [`L59`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L59)
  - `payload` — [`L59`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L59)
  - `queueKey` — [`L56`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L56)
  - `snapshot` — [`L57`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L57)
  - `source` — [`L53`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L53)
  - `text` — [`L59`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L59)
  - `wake` — [`L55`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L55)
- used by: (2 test-only callers)

### `MockRunningDaemonProbe`
- def: [`packages/coding-agent/test/package-self-update-daemon.test.ts:40`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L40)
- signature: `type MockRunningDaemonProbe`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `MockSessionSummary`
- def: [`packages/coding-agent/test/package-self-update-daemon.test.ts:30`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L30)
- signature: `interface MockSessionSummary`
- members:
  - `activeSessionId` — [`L32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L32)
  - `followUps` — [`L37`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L37)
  - `hasRunningRlmChildren` — [`L36`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L36)
  - `id` — [`L31`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L31)
  - `isBashRunning` — [`L35`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L35)
  - `isCompacting` — [`L34`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L34)
  - `isStreaming` — [`L33`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L33)
  - `queuedCount` — [`L37`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L37)
  - `sessionActions` — [`L37`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L37)
  - `steering` — [`L37`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L37)
- used by: (2 test-only callers)

### `MockUpdateRestartManifest`
- def: [`packages/coding-agent/test/package-self-update-daemon.test.ts:82`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L82)
- signature: `interface MockUpdateRestartManifest`
- members:
  - `createdAt` — [`L84`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L84)
  - `formatVersion` — [`L83`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L83)
  - `sessions` — [`L85`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L85)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `MockUpdateRestartSession`
- def: [`packages/coding-agent/test/package-self-update-daemon.test.ts:62`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L62)
- signature: `interface MockUpdateRestartSession`
- members:
  - `actions` — [`L70`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L70)
  - `actions` — [`L70`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L70)
  - `activeSessionId` — [`L63`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L63)
  - `config` — [`L67`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L67)
  - `cwd` — [`L66`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L66)
  - `formatVersion` — [`L70`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L70)
  - `hadAcceptedPromptInFlight` — [`L79`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L79)
  - `hadRunningRlmChildren` — [`L77`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L77)
  - `nextTurn` — [`L71`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L71)
  - `queue` — [`L69`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L69)
  - `runtimeMetadata` — [`L68`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L68)
  - `sessionFile` — [`L65`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L65)
  - `sessionId` — [`L64`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L64)
  - `shouldResume` — [`L73`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L73)
  - `wasBashRunning` — [`L76`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L76)
  - `wasCompacting` — [`L75`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L75)
  - `wasRetrying` — [`L78`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L78)
  - `wasStreaming` — [`L74`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L74)
- uses (calls/refs, reference-scoped): [`AgentSessionRuntimeMetadata`](../src/core/agent-session-runtime.ts.md#AgentSessionRuntimeMetadata)  (2 test-only)
- used by: (2 test-only callers)

## Functions
- `createMockTurnExecutionPolicy()` — [`L88`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L88)
- `useFixedOwnerHello()` — [`L166`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L166)

## Module values
- `mockState` — [`L122`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/package-self-update-daemon.test.ts#L122)


---
title: 'Module: packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/regressions/`4656-resume-active-session.test.ts`/
symbols:
  createAttachResult: createAttachResult().
  createConnectionState: createConnectionState().
  ResumeDaemonClient.request: ResumeDaemonClient#request().
  createSocketClient: createSocketClient().
  targetActiveSessionId: targetActiveSessionId.
  ResumeDaemonClient.requests: ResumeDaemonClient#requests.
  SupervisorHarness: SupervisorHarness#
  ResumeDaemonClient.emitMessage: ResumeDaemonClient#emitMessage().
  asDaemonClient: asDaemonClient().
  sourceActiveSessionId: sourceActiveSessionId.
  ResumeDaemonClient.messageListeners: ResumeDaemonClient#messageListeners.
  ResumeDaemonClient.-constructor: ResumeDaemonClient#`<constructor>`().
  ResumeDaemonClient.onMessage: ResumeDaemonClient#onMessage().
  ResumeDaemonClient.onClose: ResumeDaemonClient#onClose().
  ResumeDaemonClient.closeListeners: ResumeDaemonClient#closeListeners.
  ResumeDaemonClient: ResumeDaemonClient#
  SupervisorHarness.handleCommand: SupervisorHarness#handleCommand().
  ResumeDaemonClient.close: ResumeDaemonClient#close().
---
# Module: [`packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts)

## Classes
### `ResumeDaemonClient`
- def: [`packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts:24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L24)
- signature: `class ResumeDaemonClient`
- members:
  - `<constructor>(switchTarget?: string)` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L29)
  - `close(method)` — [`L121`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L121)
  - `emitMessage(method)` — [`L115`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L115)
  - `onClose(method)` — [`L110`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L110)
  - `onMessage(method)` — [`L105`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L105)
  - `request(method)` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L31)
  - `closeListeners` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L27)
  - `messageListeners` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L26)
  - `requests` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L25)
- uses (calls/refs, reference-scoped): [`role`](../../../../ai/src/types.ts.md#AssistantMessage.role), [`role`](../../../../ai/src/types.ts.md#ToolResultMessage.role), [`role`](../../../../ai/src/types.ts.md#UserMessage.role), [`role`](../../../src/core/messages.ts.md#CustomMessage.role), [`role`](../../../src/core/messages.ts.md#BashExecutionMessage.role), [`role`](../../../src/core/messages.ts.md#BranchSummaryMessage.role), [`role`](../../../src/core/messages.ts.md#CompactionSummaryMessage.role), [`timestamp`](../../../../ai/src/types.ts.md#AssistantMessage.timestamp), [`timestamp`](../../../../ai/src/types.ts.md#ToolResultMessage.timestamp), [`timestamp`](../../../../ai/src/types.ts.md#UserMessage.timestamp), [`DaemonCommand`](../../../src/modes/daemon/daemon-protocol.ts.md#DaemonCommand), [`timestamp`](../../../src/core/messages.ts.md#CustomMessage.timestamp), [`timestamp`](../../../src/core/messages.ts.md#BashExecutionMessage.timestamp), [`DaemonOutbound`](../../../src/modes/daemon/daemon-protocol.ts.md#DaemonOutbound), [`timestamp`](../../../src/core/messages.ts.md#CompactionSummaryMessage.timestamp), [`timestamp`](../../../src/core/messages.ts.md#BranchSummaryMessage.timestamp), [`snapshot`](../../../src/modes/daemon/daemon-protocol.ts.md#DaemonAttachResult.snapshot), [`DaemonResponse`](../../../src/modes/daemon/daemon-protocol.ts.md#DaemonResponse), [`messages`](../../../src/modes/daemon/daemon-protocol.ts.md#DaemonSessionSnapshot.messages), [`lastEventSequence`](../../../src/modes/daemon/daemon-protocol.ts.md#DaemonAttachResult.lastEventSequence), [`DaemonClientMessageListener`](../../../src/modes/daemon/daemon-client.ts.md#DaemonClientMessageListener), [`lastEventCursor`](../../../src/modes/daemon/daemon-protocol.ts.md#DaemonAttachResult.lastEventCursor), [`DaemonClientCloseListener`](../../../src/modes/daemon/daemon-client.ts.md#DaemonClientCloseListener)  (2 test-only)
- used by: (2 test-only callers)

### `SupervisorHarness`
- def: [`packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts:207`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L207)
- signature: `interface SupervisorHarness`
- members:
  - `handleCommand(method)` — [`L208`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L208)
- uses (calls/refs, reference-scoped): [`DaemonCommand`](../../../src/modes/daemon/daemon-protocol.ts.md#DaemonCommand), [`DaemonSocketClient`](../../../src/modes/daemon/active-session-state.ts.md#DaemonSocketClient), [`DaemonResponse`](../../../src/modes/daemon/daemon-protocol.ts.md#DaemonResponse)
- used by: (1 test-only callers)

## Functions
- `asDaemonClient(client: ResumeDaemonClient)` — [`L192`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L192)
- `createAttachResult(activeSessionId: string, messages?: AgentMessage[])` — [`L153`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L153)
- `createConnectionState(activeSessionId: string)` — [`L124`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L124)
- `createSocketClient(id: string, attachedActiveSessionIds: string[])` — [`L196`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L196)

## Module values
- `sourceActiveSessionId` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L21)
- `targetActiveSessionId` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4656-resume-active-session.test.ts#L22)


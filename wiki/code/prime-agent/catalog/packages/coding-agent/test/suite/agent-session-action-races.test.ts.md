---
title: 'Module: packages/coding-agent/test/suite/agent-session-action-races.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/agent-session-action-races.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/`agent-session-action-races.test.ts`/
symbols:
  deliveredCount: deliveredCount().
  createContextMessage: createContextMessage().
  CommitFenceInternals._actionStore: CommitFenceInternals#_actionStore.
  CommitFenceInternals._acquireSessionActionCommitFence: CommitFenceInternals#_acquireSessionActionCommitFence().
  CommitFenceInternals: CommitFenceInternals#
  CommitFenceInternals._acquireSessionActionCommitFence.Promise.typeLiteral1.release: CommitFenceInternals#_acquireSessionActionCommitFence().Promise:typeLiteral1:release().
  yieldToEventLoop: yieldToEventLoop().
  CommitFenceInternals._refineInFlight: CommitFenceInternals#_refineInFlight.
  ActionKind: ActionKind#
  CommitFenceInternals._scheduleSessionInputPump: CommitFenceInternals#_scheduleSessionInputPump().
  CommitFenceInternals._pendingSessionActionFenceWaiters: CommitFenceInternals#_pendingSessionActionFenceWaiters.
  CommitFenceInternals._acquireDirectTurnAdmissionFence: CommitFenceInternals#_acquireDirectTurnAdmissionFence().
  CommitFenceInternals._promptInjectedMessage: CommitFenceInternals#_promptInjectedMessage().
  CommitFenceInternals._acquireDirectTurnAdmissionFence.Promise.typeLiteral0.release: CommitFenceInternals#_acquireDirectTurnAdmissionFence().Promise:typeLiteral0:release().
  CommitFenceInternals._promptInjectedMessage.message-typeLiteral2.role: CommitFenceInternals#_promptInjectedMessage().(message)typeLiteral2:role.
  CommitFenceInternals._promptInjectedMessage.message-typeLiteral2.customType: CommitFenceInternals#_promptInjectedMessage().(message)typeLiteral2:customType.
  CommitFenceInternals._promptInjectedMessage.message-typeLiteral2.content: CommitFenceInternals#_promptInjectedMessage().(message)typeLiteral2:content.
  CommitFenceInternals._promptInjectedMessage.message-typeLiteral2.display: CommitFenceInternals#_promptInjectedMessage().(message)typeLiteral2:display.
  CommitFenceInternals._promptInjectedMessage.message-typeLiteral2.details: CommitFenceInternals#_promptInjectedMessage().(message)typeLiteral2:details.
  CommitFenceInternals._promptInjectedMessage.message-typeLiteral2.timestamp: CommitFenceInternals#_promptInjectedMessage().(message)typeLiteral2:timestamp.
  CommitFenceInternals._promptInjectedMessage.options-typeLiteral3.returnAfterAccepted: CommitFenceInternals#_promptInjectedMessage().(options)typeLiteral3:returnAfterAccepted.
---
# Module: [`packages/coding-agent/test/suite/agent-session-action-races.test.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts)

## Classes
### `ActionKind`
- def: [`packages/coding-agent/test/suite/agent-session-action-races.test.ts:8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L8)
- signature: `type ActionKind`
- used by: (2 test-only callers)

### `CommitFenceInternals`
- def: [`packages/coding-agent/test/suite/agent-session-action-races.test.ts:10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L10)
- signature: `interface CommitFenceInternals`
- members:
  - `release(method)` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L15)
  - `release(method)` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L16)
  - `content` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L22)
  - `customType` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L21)
  - `details` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L24)
  - `display` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L23)
  - `returnAfterAccepted` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L27)
  - `role` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L20)
  - `timestamp` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L25)
- protocol/private: `_acquireDirectTurnAdmissionFence`[`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L15), `_acquireSessionActionCommitFence`[`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L16), `_actionStore`[`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L11), `_pendingSessionActionFenceWaiters`[`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L12), `_promptInjectedMessage`[`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L17), `_refineInFlight`[`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L13), `_scheduleSessionInputPump`[`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L14)
- uses (calls/refs, reference-scoped): [`SessionAction`](../../src/core/session-action-store.ts.md#SessionAction), [`ActionStore`](../../src/core/session-action-store.ts.md#ActionStore)
- used by: (1 test-only callers)

## Functions
- `createContextMessage(content: string)` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L40)
- `deliveredCount(harness: Harness, kind: ActionKind, text: string)` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L31)
- `yieldToEventLoop()` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-action-races.test.ts#L36)


---
title: 'Module: packages/coding-agent/test/agent-connection-in-process.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/agent-connection-in-process.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`agent-connection-in-process.test.ts`/
symbols:
  userMessage: userMessage().
  createFakeSession: createFakeSession().
  FakeSessionControl.session: FakeSessionControl#session.
  FakeRuntime.-constructor: FakeRuntime#`<constructor>`().
  asRuntime: asRuntime().
  RuntimeSession: RuntimeSession#
  FakeRuntime.replaceSession: FakeRuntime#replaceSession().
  RuntimeRebindCallback: RuntimeRebindCallback#
  RuntimeBeforeInvalidateCallback: RuntimeBeforeInvalidateCallback#
  FakeSessionControl.emit: FakeSessionControl#emit().
  FakeRuntime._session: FakeRuntime#_session.
  FakeRuntime.rebindSession: FakeRuntime#rebindSession.
  FakeRuntime.beforeSessionInvalidate: FakeRuntime#beforeSessionInvalidate.
  FakeSessionControl.listenerCount: FakeSessionControl#listenerCount().
  FakeRuntime.-get-session: FakeRuntime#`<get>session`().
  FakeRuntime.setRebindSession: FakeRuntime#setRebindSession().
  FakeRuntime.setBeforeSessionInvalidate: FakeRuntime#setBeforeSessionInvalidate().
  FakeRuntime.invalidateCurrentSession: FakeRuntime#invalidateCurrentSession().
  FakeRuntime.dispose: FakeRuntime#dispose().
  FakeSessionControl.unsubscribeCount: FakeSessionControl#unsubscribeCount().
  FakeRuntime.disposed: FakeRuntime#disposed.
  FakeSessionControl: FakeSessionControl#
  FakeRuntime: FakeRuntime#
---
# Module: [`packages/coding-agent/test/agent-connection-in-process.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts)

## Classes
### `FakeRuntime`
- def: [`packages/coding-agent/test/agent-connection-in-process.test.ts:21`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L21)
- signature: `class FakeRuntime`
- members:
  - `<constructor>(session: AgentSession)` — [`L27`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L27)
  - `<get>session` — [`L31`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L31)
  - `dispose(method)` — [`L52`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L52)
  - `invalidateCurrentSession(method)` — [`L43`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L43)
  - `replaceSession(method)` — [`L47`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L47)
  - `setBeforeSessionInvalidate(method)` — [`L39`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L39)
  - `setRebindSession(method)` — [`L35`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L35)
  - `beforeSessionInvalidate` — [`L24`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L24)
  - `disposed` — [`L25`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L25)
  - `rebindSession` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L23)
- protocol/private: `_session`[`L22`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L22)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (2 test-only callers)

### `FakeSessionControl`
- def: [`packages/coding-agent/test/agent-connection-in-process.test.ts:14`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L14)
- signature: `interface FakeSessionControl`
- members:
  - `emit(method)` — [`L18`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L18)
  - `listenerCount(method)` — [`L16`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L16)
  - `unsubscribeCount(method)` — [`L17`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L17)
  - `session` — [`L15`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L15)
- uses (calls/refs, reference-scoped): [`AgentSessionEvent`](../src/core/agent-session.ts.md#AgentSessionEvent)  (1 test-only)
- used by: (2 test-only callers)

### `RuntimeBeforeInvalidateCallback`
- def: [`packages/coding-agent/test/agent-connection-in-process.test.ts:12`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L12)
- signature: `type RuntimeBeforeInvalidateCallback`
- uses (calls/refs, reference-scoped): [`AgentSessionRuntime`](../src/core/agent-session-runtime.ts.md#AgentSessionRuntime), [`setBeforeSessionInvalidate`](../src/core/agent-session-runtime.ts.md#AgentSessionRuntime.setBeforeSessionInvalidate)
- used by: (2 test-only callers)

### `RuntimeRebindCallback`
- def: [`packages/coding-agent/test/agent-connection-in-process.test.ts:11`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L11)
- signature: `type RuntimeRebindCallback`
- uses (calls/refs, reference-scoped): [`AgentSessionRuntime`](../src/core/agent-session-runtime.ts.md#AgentSessionRuntime), [`setRebindSession`](../src/core/agent-session-runtime.ts.md#AgentSessionRuntime.setRebindSession)
- used by: (2 test-only callers)

### `RuntimeSession`
- def: [`packages/coding-agent/test/agent-connection-in-process.test.ts:10`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L10)
- signature: `type RuntimeSession`
- uses (calls/refs, reference-scoped): [`<get>session`](../src/core/agent-session-runtime.ts.md#AgentSessionRuntime.-get-session), [`AgentSessionRuntime`](../src/core/agent-session-runtime.ts.md#AgentSessionRuntime)
- used by: (6 test-only callers)

## Functions
- `asRuntime(runtime: FakeRuntime)` — [`L57`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L57)
- `createFakeSession(id: string, messages: AgentMessage[])` — [`L69`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L69)
- `userMessage(text: string, timestamp: number)` — [`L61`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-connection-in-process.test.ts#L61)


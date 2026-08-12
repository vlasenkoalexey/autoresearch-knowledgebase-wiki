---
title: 'Module: packages/coding-agent/test/agent-session-recursion.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/agent-session-recursion.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`agent-session-recursion.test.ts`/
symbols:
  waitFor: waitFor().
  assistantMessage: assistantMessage().
  userText: userText().
  InspectableRlmSession: InspectableRlmSession#
  usage: usage().
  InspectableRlmSession._activeRlmChildRuns: InspectableRlmSession#_activeRlmChildRuns.
  rlmCommOpenData: rlmCommOpenData().
  InspectableRlmSession._rlmChildCleanupFailures: InspectableRlmSession#_rlmChildCleanupFailures.
  InspectableRlmRun.status: InspectableRlmRun#status.
  encodeTestMessage: encodeTestMessage().
  InspectableRlmDirSession._rlmKernelEnv: InspectableRlmDirSession#_rlmKernelEnv().
  streamAnswer: streamAnswer().
  InspectableRlmRun.session: InspectableRlmRun#session.
  InspectableRlmSession._createKernelHostHandlers: InspectableRlmSession#_createKernelHostHandlers().
  InspectableRlmDirSession: InspectableRlmDirSession#
  rlmCommOpen: rlmCommOpen().
  InspectableRlmSession._deletingRlmChildren.Map.typeLiteral47.subagent: InspectableRlmSession#_deletingRlmChildren.Map:typeLiteral47:subagent.
  model: model.
  InspectableRlmRun.detachedDeletion: InspectableRlmRun#detachedDeletion.
  KernelCommTestApi.handleCommMessage: KernelCommTestApi#handleCommMessage().
  InspectableRlmRun.id: InspectableRlmRun#id.
  InspectableRlmSession._rlmChildSessions: InspectableRlmSession#_rlmChildSessions.
  InspectableRlmRun.error: InspectableRlmRun#error.
  findLastMessage: findLastMessage().
  TestCommMessage: TestCommMessage#
  KernelCommTestApi: KernelCommTestApi#
  CapturedCommReply.commId: CapturedCommReply#commId.
  CapturedCommReply.data: CapturedCommReply#data.
  KernelCommTestApi.sendCommMessage: KernelCommTestApi#sendCommMessage().
  CapturedCommReply: CapturedCommReply#
  TestCommMessage.header: TestCommMessage#header.
  TestCommMessage.parent_header: TestCommMessage#parent_header.
  TestCommMessage.metadata: TestCommMessage#metadata.
  TestCommMessage.content: TestCommMessage#content.
  InspectableRlmRun.sessionDir: InspectableRlmRun#sessionDir.
  InspectableRlmSession._deletingRlmChildren: InspectableRlmSession#_deletingRlmChildren.
  InspectableRlmSession._rlmChildUnsubscribes: InspectableRlmSession#_rlmChildUnsubscribes.
  InspectableRlmDirSession._ensureRlmSessionDir: InspectableRlmDirSession#_ensureRlmSessionDir().
  TestCommMessage.header.typeLiteral46.msg_type: TestCommMessage#header.typeLiteral46:msg_type.
  InspectableRlmRun: InspectableRlmRun#
  InspectableRlmRun.settled: InspectableRlmRun#settled.
  InspectableRlmSession._deletingRlmChildren.Map.typeLiteral47.promise: InspectableRlmSession#_deletingRlmChildren.Map:typeLiteral47:promise.
  KernelPumpTestApi: KernelPumpTestApi#
  KernelPumpTestApi.iopub: KernelPumpTestApi#iopub.
  KernelPumpTestApi.startIopubPump: KernelPumpTestApi#startIopubPump().
  KernelExecuteTestApi: KernelExecuteTestApi#
  KernelExecuteTestApi.start: KernelExecuteTestApi#start.
  KernelExecuteTestApi.state: KernelExecuteTestApi#state.
  KernelExecuteTestApi.activeExecution: KernelExecuteTestApi#activeExecution.
  KernelExecuteTestApi.shell: KernelExecuteTestApi#shell.
  KernelExecuteTestApi.connection: KernelExecuteTestApi#connection.
  asyncFrames: asyncFrames().
  expectSettlesWithin: expectSettlesWithin().
  InspectableRlmRun.abort: InspectableRlmRun#abort.
  InspectableRlmSession._reapDeletedRlmSubagentRuntimesAfterCompaction: InspectableRlmSession#_reapDeletedRlmSubagentRuntimesAfterCompaction().
  KernelExecuteTestApi.shell.typeLiteral51.send: KernelExecuteTestApi#shell.typeLiteral51:send().
  KernelExecuteTestApi.shell.typeLiteral51.close: KernelExecuteTestApi#shell.typeLiteral51:close().
  KernelExecuteTestApi.connection.typeLiteral52.ip: KernelExecuteTestApi#connection.typeLiteral52:ip.
  KernelExecuteTestApi.connection.typeLiteral52.transport: KernelExecuteTestApi#connection.typeLiteral52:transport.
  KernelExecuteTestApi.connection.typeLiteral52.shell_port: KernelExecuteTestApi#connection.typeLiteral52:shell_port.
  KernelExecuteTestApi.connection.typeLiteral52.iopub_port: KernelExecuteTestApi#connection.typeLiteral52:iopub_port.
  KernelExecuteTestApi.connection.typeLiteral52.stdin_port: KernelExecuteTestApi#connection.typeLiteral52:stdin_port.
  KernelExecuteTestApi.connection.typeLiteral52.control_port: KernelExecuteTestApi#connection.typeLiteral52:control_port.
  KernelExecuteTestApi.connection.typeLiteral52.hb_port: KernelExecuteTestApi#connection.typeLiteral52:hb_port.
  KernelExecuteTestApi.connection.typeLiteral52.signature_scheme: KernelExecuteTestApi#connection.typeLiteral52:signature_scheme.
  KernelExecuteTestApi.connection.typeLiteral52.key: KernelExecuteTestApi#connection.typeLiteral52:key.
  KernelExecuteTestApi.connection.typeLiteral52.kernel_name: KernelExecuteTestApi#connection.typeLiteral52:kernel_name.
---
# Module: [`packages/coding-agent/test/agent-session-recursion.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts)

## Classes
### `CapturedCommReply`
- def: [`packages/coding-agent/test/agent-session-recursion.test.ts:106`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L106)
- signature: `interface CapturedCommReply`
- members:
  - `commId` — [`L107`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L107)
  - `data` — [`L108`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L108)
- used by: (1 test-only callers)

### `InspectableRlmDirSession`
- def: [`packages/coding-agent/test/agent-session-recursion.test.ts:3184`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L3184)
- signature: `interface InspectableRlmDirSession`
- protocol/private: `_ensureRlmSessionDir`[`L3185`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L3185), `_rlmKernelEnv`[`L3186`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L3186)
- used by: (1 test-only callers)

### `InspectableRlmRun`
- def: [`packages/coding-agent/test/agent-session-recursion.test.ts:111`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L111)
- signature: `interface InspectableRlmRun`
- members:
  - `abort` — [`L114`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L114)
  - `detachedDeletion` — [`L118`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L118)
  - `error` — [`L117`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L117)
  - `id` — [`L112`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L112)
  - `session` — [`L119`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L119)
  - `sessionDir` — [`L113`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L113)
  - `settled` — [`L116`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L116)
  - `status` — [`L115`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L115)
- uses (calls/refs, reference-scoped): [`AgentSession`](../src/core/agent-session.ts.md#AgentSession), [`listRlmSubagents`](../src/core/agent-session.ts.md#AgentSession.listRlmSubagents), [`subagents`](../src/core/rlm-runtime.ts.md#RlmListSubagentsResult.subagents)
- used by: (2 test-only callers)

### `InspectableRlmSession`
- def: [`packages/coding-agent/test/agent-session-recursion.test.ts:122`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L122)
- signature: `interface InspectableRlmSession`
- members:
  - `promise` — [`L128`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L128)
  - `subagent` — [`L127`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L127)
- protocol/private: `_activeRlmChildRuns`[`L123`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L123), `_createKernelHostHandlers`[`L134`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L134), `_deletingRlmChildren`[`L124`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L124), `_reapDeletedRlmSubagentRuntimesAfterCompaction`[`L135`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L135), `_rlmChildCleanupFailures`[`L131`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L131), `_rlmChildSessions`[`L132`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L132), `_rlmChildUnsubscribes`[`L133`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L133)
- uses (calls/refs, reference-scoped): [`AgentSession`](../src/core/agent-session.ts.md#AgentSession), [`listRlmSubagents`](../src/core/agent-session.ts.md#AgentSession.listRlmSubagents), [`subagents`](../src/core/rlm-runtime.ts.md#RlmListSubagentsResult.subagents), [`HostRequestHandlers`](../src/core/kernel/index.ts.md#HostRequestHandlers)  (1 test-only)
- used by: (1 test-only callers)

### `KernelCommTestApi`
- def: [`packages/coding-agent/test/agent-session-recursion.test.ts:101`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L101)
- signature: `interface KernelCommTestApi`
- members:
  - `handleCommMessage(method)` — [`L102`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L102)
  - `sendCommMessage(method)` — [`L103`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L103)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `KernelExecuteTestApi`
- def: [`packages/coding-agent/test/agent-session-recursion.test.ts:143`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L143)
- signature: `interface KernelExecuteTestApi`
- members:
  - `close(method)` — [`L149`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L149)
  - `send(method)` — [`L148`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L148)
  - `activeExecution` — [`L146`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L146)
  - `connection` — [`L151`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L151)
  - `control_port` — [`L157`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L157)
  - `hb_port` — [`L158`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L158)
  - `iopub_port` — [`L155`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L155)
  - `ip` — [`L152`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L152)
  - `kernel_name` — [`L161`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L161)
  - `key` — [`L160`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L160)
  - `shell` — [`L147`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L147)
  - `shell_port` — [`L154`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L154)
  - `signature_scheme` — [`L159`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L159)
  - `start` — [`L144`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L144)
  - `state` — [`L145`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L145)
  - `stdin_port` — [`L156`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L156)
  - `transport` — [`L153`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L153)
- used by: (1 test-only callers)

### `KernelPumpTestApi`
- def: [`packages/coding-agent/test/agent-session-recursion.test.ts:138`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L138)
- signature: `interface KernelPumpTestApi`
- members:
  - `startIopubPump(method)` — [`L140`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L140)
  - `iopub` — [`L139`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L139)
- used by: (1 test-only callers)

### `TestCommMessage`
- def: [`packages/coding-agent/test/agent-session-recursion.test.ts:94`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L94)
- signature: `interface TestCommMessage`
- members:
  - `content` — [`L98`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L98)
  - `header` — [`L95`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L95)
  - `metadata` — [`L97`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L97)
  - `msg_type` — [`L95`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L95)
  - `parent_header` — [`L96`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L96)
- used by: (4 test-only callers)

## Functions
- `assistantMessage(text: string, messageUsage?: Usage)` — [`L72`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L72)
- `asyncFrames(frames: Buffer<ArrayBufferLike>[][])` — [`L193`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L193)
- `encodeTestMessage(message: TestCommMessage)` — [`L182`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L182)
- `expectSettlesWithin(promise: Promise<void>, timeoutMs: number)` — [`L215`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L215)
- `findLastMessage(messages: readonly AgentMessage[], predicate: (message: AgentMessage) => boolean)` — [`L223`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L223)
- `rlmCommOpen(commId: string, prompt: string, kwargs?: Record<string, unknown>)` — [`L178`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L178)
- `rlmCommOpenData(commId: string, data: Record<string, unknown>)` — [`L165`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L165)
- `streamAnswer(text: string)` — [`L85`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L85)
- `usage(input?: number, output?: number)` — [`L61`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L61)
- `userText(context: Context)` — [`L44`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L44)
- `waitFor(condition: () => boolean)` — [`L205`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L205)

## Module values
- `model` — [`L42`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-session-recursion.test.ts#L42)


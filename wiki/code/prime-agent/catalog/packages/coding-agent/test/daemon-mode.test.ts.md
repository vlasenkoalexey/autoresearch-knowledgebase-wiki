---
title: 'Module: packages/coding-agent/test/daemon-mode.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/daemon-mode.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`daemon-mode.test.ts`/
symbols:
  makeState: makeState().
  makePersistedRlmDaemonFixture.options-typeLiteral7972.childAdmissionGate: makePersistedRlmDaemonFixture().(options)typeLiteral7972:childAdmissionGate.
  makeClient: makeClient().
  makeCronJob.input-typeLiteral2800.deliveryMode: makeCronJob().(input)typeLiteral2800:deliveryMode.
  makePersistedRlmDaemonFixture: makePersistedRlmDaemonFixture().
  makeRuntimeSession: makeRuntimeSession().
  makeAgentFamilyState.typeLiteral2185.state: makeAgentFamilyState().typeLiteral2185:state.
  makeAgentFamilyState.typeLiteral2185.acceptAgentMessagePrompt: makeAgentFamilyState().typeLiteral2185:acceptAgentMessagePrompt.
  makeCronAdmissionFixture.options-typeLiteral7918.acceptingAgentMessage: makeCronAdmissionFixture().(options)typeLiteral7918:acceptingAgentMessage.
  makeAgentFamilyState: makeAgentFamilyState().
  makeCronJob.input-typeLiteral2800.source: makeCronJob().(input)typeLiteral2800:source.
  makeCronJob.input-typeLiteral2800.activeSessionId: makeCronJob().(input)typeLiteral2800:activeSessionId.
  makeCronAdmissionFixture: makeCronAdmissionFixture().
  makeCronJob: makeCronJob().
  makeCronJob.input-typeLiteral2800.id: makeCronJob().(input)typeLiteral2800:id.
  makePersistedRlmDaemonFixture.options-typeLiteral7972.childRuntimeGate: makePersistedRlmDaemonFixture().(options)typeLiteral7972:childRuntimeGate.
  makePersistedRlmDaemonFixture.options-typeLiteral7972.childBindingGate: makePersistedRlmDaemonFixture().(options)typeLiteral7972:childBindingGate.
  makePersistedRlmDaemonFixture.options-typeLiteral7972.grandchildRuntimeGate: makePersistedRlmDaemonFixture().(options)typeLiteral7972:grandchildRuntimeGate.
  makePersistedRlmDaemonFixture.options-typeLiteral7972.childDisposeGate: makePersistedRlmDaemonFixture().(options)typeLiteral7972:childDisposeGate.
  CronAdmissionActivity: CronAdmissionActivity#
  makePersistedRlmDaemonFixture.options-typeLiteral7972.childRuntimeStarted: makePersistedRlmDaemonFixture().(options)typeLiteral7972:childRuntimeStarted.
  makePersistedRlmDaemonFixture.options-typeLiteral7972.childBindingStarted: makePersistedRlmDaemonFixture().(options)typeLiteral7972:childBindingStarted.
  makePersistedRlmDaemonFixture.options-typeLiteral7972.grandchildRuntimeStarted: makePersistedRlmDaemonFixture().(options)typeLiteral7972:grandchildRuntimeStarted.
  makePersistedRlmDaemonFixture.options-typeLiteral7972.childDisposeStarted: makePersistedRlmDaemonFixture().(options)typeLiteral7972:childDisposeStarted.
  makePersistedRlmDaemonFixture.options-typeLiteral7972.childAdmissionStarted: makePersistedRlmDaemonFixture().(options)typeLiteral7972:childAdmissionStarted.
  CronAdmissionActivity.Partial.typeLiteral7917.isStreaming: CronAdmissionActivity#Partial:typeLiteral7917:isStreaming.
  CronAdmissionActivity.Partial.typeLiteral7917.isCompacting: CronAdmissionActivity#Partial:typeLiteral7917:isCompacting.
  CronAdmissionActivity.Partial.typeLiteral7917.isRetrying: CronAdmissionActivity#Partial:typeLiteral7917:isRetrying.
  CronAdmissionActivity.Partial.typeLiteral7917.isBashRunning: CronAdmissionActivity#Partial:typeLiteral7917:isBashRunning.
  CronAdmissionActivity.Partial.typeLiteral7917.hasPendingSessionWork: CronAdmissionActivity#Partial:typeLiteral7917:hasPendingSessionWork.
  CronAdmissionActivity.Partial.typeLiteral7917.unfinishedActionCount: CronAdmissionActivity#Partial:typeLiteral7917:unfinishedActionCount.
---
# Module: [`packages/coding-agent/test/daemon-mode.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts)

## Classes
### `CronAdmissionActivity`
- def: [`packages/coding-agent/test/daemon-mode.test.ts:9571`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9571)
- signature: `type CronAdmissionActivity`
- members:
  - `hasPendingSessionWork` — [`L9576`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9576)
  - `isBashRunning` — [`L9575`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9575)
  - `isCompacting` — [`L9573`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9573)
  - `isRetrying` — [`L9574`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9574)
  - `isStreaming` — [`L9572`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9572)
  - `unfinishedActionCount` — [`L9577`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9577)
- used by: (1 test-only callers)

## Functions
- `makeAgentFamilyState(activeSessionId: string, sessionName: string, parent?: ActiveSessionState | undefined)` — [`L9867`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9867)
- `makeClient(id: string, activeSessionId: string, supportsExtensionUi?: boolean)` — [`L9931`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9931)
- `makeCronAdmissionFixture(activity?: Partial<{ isStreaming: boolean; isCompacting: boolean; isRetrying: boolean; isBashRunning: boolean; hasPendingSessionWork: boolean; unfinishedActionCount: number; }>, options?: { ...; })` — [`L9580`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9580)
- `makeCronJob(input: { id: string; source: AgentCronJobSource | undefined; activeSessionId: string; deliveryMode?: AgentHeartbeatDeliveryMode | undefined; })` — [`L9644`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9644)
- `makePersistedRlmDaemonFixture(tempDir: string, options?: { childRuntimeStarted?: (() => void) | undefined; childRuntimeGate?: Promise<void> | undefined; childBindingStarted?: (() => void) | undefined; childBindingGate?: Promise<...> | undefined; ... 5 more ...; childAdmissionGate?: Promise<...> | undefined; })` — [`L9668`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9668)
- `makeRuntimeSession(sessionManager: SessionManager)` — [`L9834`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9834)
- `makeState(activeSessionId: string, parentActiveSessionId?: string | undefined)` — [`L9915`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9915)

## Module values
- `acceptAgentMessagePrompt` — [`L9871`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9871)
- `acceptingAgentMessage` — [`L9582`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9582)
- `activeSessionId` — [`L9647`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9647)
- `childAdmissionGate` — [`L9680`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9680)
- `childAdmissionStarted` — [`L9679`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9679)
- `childBindingGate` — [`L9674`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9674)
- `childBindingStarted` — [`L9673`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9673)
- `childDisposeGate` — [`L9678`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9678)
- `childDisposeStarted` — [`L9677`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9677)
- `childRuntimeGate` — [`L9672`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9672)
- `childRuntimeStarted` — [`L9671`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9671)
- `deliveryMode` — [`L9648`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9648)
- `grandchildRuntimeGate` — [`L9676`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9676)
- `grandchildRuntimeStarted` — [`L9675`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9675)
- `id` — [`L9645`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9645)
- `source` — [`L9646`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9646)
- `state` — [`L9871`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-mode.test.ts#L9871)


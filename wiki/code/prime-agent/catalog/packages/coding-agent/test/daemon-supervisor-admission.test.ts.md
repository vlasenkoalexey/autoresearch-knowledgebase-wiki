---
title: 'Module: packages/coding-agent/test/daemon-supervisor-admission.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/daemon-supervisor-admission.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`daemon-supervisor-admission.test.ts`/
symbols:
  createHarness: createHarness().
  admissionFor: admissionFor().
  SupervisorHarness.handleLine: SupervisorHarness#handleLine().
  client: client().
  commandLine: commandLine().
  AdmissionRecord.workerAdmissionId: AdmissionRecord#workerAdmissionId.
  waitFor: waitFor().
  SupervisorHarness.promptAdmissions: SupervisorHarness#promptAdmissions.
  AdmissionRecord.status: AdmissionRecord#status.
  createHarness.options-typeLiteral212.forwardToWorker: createHarness().(options)typeLiteral212:forwardToWorker.
  SupervisorHarness.clients: SupervisorHarness#clients.
  AdmissionRecord.client: AdmissionRecord#client.
  createHarness.options-typeLiteral212.findWorker: createHarness().(options)typeLiteral212:findWorker.
  AdmissionRecord: AdmissionRecord#
  SupervisorHarness: SupervisorHarness#
  AdmissionRecord.controller: AdmissionRecord#controller.
  AdmissionRecord.worker: AdmissionRecord#worker.
  SupervisorHarness.handleConnection: SupervisorHarness#handleConnection().
  AdmissionRecord.activeSessionId: AdmissionRecord#activeSessionId.
  AdmissionRecord.publicAdmissionId: AdmissionRecord#publicAdmissionId.
  createHarness.options-typeLiteral212.ready: createHarness().(options)typeLiteral212:ready.
  createHarness.options-typeLiteral212.assertCurrent: createHarness().(options)typeLiteral212:assertCurrent.
  createHarness.options-typeLiteral212.commandJournal: createHarness().(options)typeLiteral212:commandJournal.
  createHarness.options-typeLiteral212.commandJournal.typeLiteral219.lookup: createHarness().(options)typeLiteral212:commandJournal.typeLiteral219:lookup.
  createHarness.options-typeLiteral212.commandJournal.typeLiteral219.begin: createHarness().(options)typeLiteral212:commandJournal.typeLiteral219:begin.
  createHarness.options-typeLiteral212.commandJournal.typeLiteral219.recordResult: createHarness().(options)typeLiteral212:commandJournal.typeLiteral219:recordResult.
  createHarness.options-typeLiteral212.commandJournal.typeLiteral219.acknowledge: createHarness().(options)typeLiteral212:commandJournal.typeLiteral219:acknowledge.
  createHarness.options-typeLiteral212.updateRestartPhase: createHarness().(options)typeLiteral212:updateRestartPhase.
  AdmissionRecord.workerActiveSessionId: AdmissionRecord#workerActiveSessionId.
---
# Module: [`packages/coding-agent/test/daemon-supervisor-admission.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts)

## Classes
### `AdmissionRecord`
- def: [`packages/coding-agent/test/daemon-supervisor-admission.test.ts:15`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L15)
- signature: `interface AdmissionRecord`
- members:
  - `activeSessionId` — [`L17`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L17)
  - `client` — [`L16`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L16)
  - `controller` — [`L21`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L21)
  - `publicAdmissionId` — [`L18`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L18)
  - `status` — [`L20`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L20)
  - `worker` — [`L22`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L22)
  - `workerActiveSessionId` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L23)
  - `workerAdmissionId` — [`L19`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L19)
- uses (calls/refs, reference-scoped): [`DaemonSocketClient`](../src/modes/daemon/active-session-state.ts.md#DaemonSocketClient)
- used by: (3 test-only callers)

### `SupervisorHarness`
- def: [`packages/coding-agent/test/daemon-supervisor-admission.test.ts:26`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L26)
- signature: `interface SupervisorHarness`
- members:
  - `handleConnection(method)` — [`L27`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L27)
  - `handleLine(method)` — [`L28`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L28)
  - `clients` — [`L29`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L29)
  - `promptAdmissions` — [`L30`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L30)
- uses (calls/refs, reference-scoped): [`DaemonSocketClient`](../src/modes/daemon/active-session-state.ts.md#DaemonSocketClient)  (1 test-only)
- used by: (3 test-only callers)

## Functions
- `admissionFor(supervisor: SupervisorHarness, owner: DaemonSocketClient)` — [`L41`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L41)
- `client(id: string)` — [`L33`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L33)
- `commandLine(command: DaemonCommand & { id: string; }, clientId?: string | undefined)` — [`L37`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L37)
- `createHarness(options?: { ready?: Promise<void> | undefined; assertCurrent?: (() => Promise<void>) | undefined; findWorker?: ((client: DaemonSocketClient, selector: string) => Promise<...>) | undefined; forwardToWorker?: ((worker: unknown, command: DaemonCommand) => Promise<...>) | undefined; commandJournal?: { ...; } | undefined; updateRestartPhase?: "prepared" | ... 2 more ... | undefined; })` — [`L55`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L55)
- `waitFor(predicate: () => boolean)` — [`L45`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L45)

## Module values
- `acknowledge` — [`L65`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L65)
- `assertCurrent` — [`L58`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L58)
- `begin` — [`L63`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L63)
- `commandJournal` — [`L61`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L61)
- `findWorker` — [`L59`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L59)
- `forwardToWorker` — [`L60`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L60)
- `lookup` — [`L62`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L62)
- `ready` — [`L57`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L57)
- `recordResult` — [`L64`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L64)
- `updateRestartPhase` — [`L67`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-admission.test.ts#L67)


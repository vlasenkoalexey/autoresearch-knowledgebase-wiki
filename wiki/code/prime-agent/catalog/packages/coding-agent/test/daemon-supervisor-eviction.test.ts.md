---
title: 'Module: packages/coding-agent/test/daemon-supervisor-eviction.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/daemon-supervisor-eviction.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`daemon-supervisor-eviction.test.ts`/
symbols:
  makeSummary: makeSummary().
  makeWorker: makeWorker().
  makeSupervisor: makeSupervisor().
  SupervisorInternals.workers: SupervisorInternals#workers.
  WorkerFixture.client: WorkerFixture#client.
  WorkerFixture.client.typeLiteral3.requestWorker: WorkerFixture#client.typeLiteral3:requestWorker.
  SupervisorInternals.stopWorker: SupervisorInternals#stopWorker.
  WorkerFixture.descriptor: WorkerFixture#descriptor.
  WorkerFixture.client.typeLiteral3.request: WorkerFixture#client.typeLiteral3:request.
  SupervisorInternals.createOrReuseWorker: SupervisorInternals#createOrReuseWorker.
  SupervisorInternals.runIdleEvictionSweep: SupervisorInternals#runIdleEvictionSweep().
  SupervisorInternals.catalog: SupervisorInternals#catalog.
  SupervisorInternals.handleCommand: SupervisorInternals#handleCommand().
  WorkerFixture.summaries: WorkerFixture#summaries.
  tempDirs: tempDirs.
  SupervisorInternals.catalog.typeLiteral5.resolve: SupervisorInternals#catalog.typeLiteral5:resolve.
  WorkerFixture: WorkerFixture#
  WorkerFixture.descriptor.typeLiteral0.workerId: WorkerFixture#descriptor.typeLiteral0:workerId.
  WorkerFixture.descriptor.typeLiteral0.rootActiveSessionId: WorkerFixture#descriptor.typeLiteral0:rootActiveSessionId.
  WorkerFixture.descriptor.typeLiteral0.createCommand: WorkerFixture#descriptor.typeLiteral0:createCommand.
  SupervisorInternals: SupervisorInternals#
  SupervisorInternals.log: SupervisorInternals#log.
  WorkerFixture.descriptor.typeLiteral0.lifecycle: WorkerFixture#descriptor.typeLiteral0:lifecycle.
  WorkerFixture.descriptor.typeLiteral0.rootSessionId: WorkerFixture#descriptor.typeLiteral0:rootSessionId.
  WorkerFixture.descriptor.typeLiteral0.pid: WorkerFixture#descriptor.typeLiteral0:pid.
  WorkerFixture.descriptor.typeLiteral0.createCommand.typeLiteral1.type: WorkerFixture#descriptor.typeLiteral0:createCommand.typeLiteral1:type.
  WorkerFixture.descriptor.typeLiteral0.createCommand.typeLiteral1.config: WorkerFixture#descriptor.typeLiteral0:createCommand.typeLiteral1:config.
  WorkerFixture.intentionalStop: WorkerFixture#intentionalStop.
  SupervisorInternals.clients: SupervisorInternals#clients.
  SupervisorInternals.clients.Set.typeLiteral4.id: SupervisorInternals#clients.Set:typeLiteral4:id.
  SupervisorInternals.clients.Set.typeLiteral4.attachedActiveSessionIds: SupervisorInternals#clients.Set:typeLiteral4:attachedActiveSessionIds.
  SupervisorInternals.idleEvictionFence: SupervisorInternals#idleEvictionFence.
  SupervisorInternals.catalog.typeLiteral5.stop: SupervisorInternals#catalog.typeLiteral5:stop.
  SupervisorInternals.scheduleIdleEvictionSweep: SupervisorInternals#scheduleIdleEvictionSweep().
  SupervisorInternals.shutdown: SupervisorInternals#shutdown().
  WorkerFixture.descriptor.typeLiteral0.ownerClientId: WorkerFixture#descriptor.typeLiteral0:ownerClientId.
  WorkerFixture.descriptor.typeLiteral0.stopRequestedAt: WorkerFixture#descriptor.typeLiteral0:stopRequestedAt.
  WorkerFixture.descriptor.typeLiteral0.createCommand.typeLiteral1.config.typeLiteral2.sessionDir: WorkerFixture#descriptor.typeLiteral0:createCommand.typeLiteral1:config.typeLiteral2:sessionDir.
  WorkerFixture.client.typeLiteral3.close: WorkerFixture#client.typeLiteral3:close.
  WorkerFixture.updateRestartPrepareClient: WorkerFixture#updateRestartPrepareClient.
---
# Module: [`packages/coding-agent/test/daemon-supervisor-eviction.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts)

## Classes
### `SupervisorInternals`
- def: [`packages/coding-agent/test/daemon-supervisor-eviction.test.ts:30`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L30)
- signature: `interface SupervisorInternals`
- members:
  - `handleCommand(method)` — [`L41`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L41)
  - `runIdleEvictionSweep(method)` — [`L39`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L39)
  - `scheduleIdleEvictionSweep(method)` — [`L38`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L38)
  - `shutdown(method)` — [`L40`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L40)
  - `attachedActiveSessionIds` — [`L32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L32)
  - `catalog` — [`L34`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L34)
  - `clients` — [`L32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L32)
  - `createOrReuseWorker` — [`L35`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L35)
  - `id` — [`L32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L32)
  - `idleEvictionFence` — [`L33`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L33)
  - `log` — [`L37`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L37)
  - `resolve` — [`L34`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L34)
  - `stop` — [`L34`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L34)
  - `stopWorker` — [`L36`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L36)
  - `workers` — [`L31`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L31)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `WorkerFixture`
- def: [`packages/coding-agent/test/daemon-supervisor-eviction.test.ts:9`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L9)
- signature: `interface WorkerFixture`
- members:
  - `client` — [`L20`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L20)
  - `close` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L23)
  - `config` — [`L18`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L18)
  - `createCommand` — [`L18`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L18)
  - `descriptor` — [`L10`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L10)
  - `intentionalStop` — [`L26`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L26)
  - `lifecycle` — [`L12`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L12)
  - `ownerClientId` — [`L16`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L16)
  - `pid` — [`L15`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L15)
  - `request` — [`L21`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L21)
  - `requestWorker` — [`L22`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L22)
  - `rootActiveSessionId` — [`L13`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L13)
  - `rootSessionId` — [`L14`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L14)
  - `sessionDir` — [`L18`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L18)
  - `stopRequestedAt` — [`L17`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L17)
  - `summaries` — [`L25`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L25)
  - `type` — [`L18`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L18)
  - `updateRestartPrepareClient` — [`L27`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L27)
  - `workerId` — [`L11`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L11)
- uses (calls/refs, reference-scoped): [`SessionSummary`](../src/modes/daemon/daemon-session-list.ts.md#SessionSummary)
- used by: (4 test-only callers)

## Functions
- `makeSummary(id: string, now: number, overrides?: Partial<SessionSummary>)` — [`L50`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L50)
- `makeSupervisor(idleEvictionMinutes?: number | "off")` — [`L90`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L90)
- `makeWorker(id: string, summaries: SessionSummary[])` — [`L69`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L69)

## Module values
- `tempDirs` — [`L44`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-eviction.test.ts#L44)


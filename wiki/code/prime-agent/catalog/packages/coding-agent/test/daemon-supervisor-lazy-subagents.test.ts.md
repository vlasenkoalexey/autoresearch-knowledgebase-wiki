---
title: 'Module: packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`daemon-supervisor-lazy-subagents.test.ts`/
symbols:
  worker: worker().
  summary: summary().
  tempDirs: tempDirs.
  WorkerFixture.client: WorkerFixture#client.
  WorkerFixture.client.typeLiteral4.request: WorkerFixture#client.typeLiteral4:request.
  SupervisorInternals: SupervisorInternals#
  SupervisorInternals.workers: SupervisorInternals#workers.
  SupervisorInternals.familyCatalogEntry: SupervisorInternals#familyCatalogEntry().
  SupervisorInternals.handleCommand: SupervisorInternals#handleCommand().
  SupervisorInternals.createOrReuseWorker: SupervisorInternals#createOrReuseWorker().
  SupervisorInternals.createOrReuseWorker.command-typeLiteral0.type: SupervisorInternals#createOrReuseWorker().(command)typeLiteral0:type.
  SupervisorInternals.createOrReuseWorker.command-typeLiteral0.sessionPath: SupervisorInternals#createOrReuseWorker().(command)typeLiteral0:sessionPath.
  SupervisorInternals.findSummaryInWorker: SupervisorInternals#findSummaryInWorker().
  SupervisorInternals.createOrReuseWorker.command-typeLiteral0.name: SupervisorInternals#createOrReuseWorker().(command)typeLiteral0:name.
  WorkerFixture.summaries: WorkerFixture#summaries.
  WorkerFixture: WorkerFixture#
  SupervisorInternals.refreshWorkerSummaries: SupervisorInternals#refreshWorkerSummaries().
  WorkerFixture.descriptor: WorkerFixture#descriptor.
  SupervisorInternals.assertSupervisorSavedSessionNameAvailable: SupervisorInternals#assertSupervisorSavedSessionNameAvailable().
  WorkerFixture.descriptor.typeLiteral1.rootActiveSessionId: WorkerFixture#descriptor.typeLiteral1:rootActiveSessionId.
  WorkerFixture.client.typeLiteral4.requestWorker: WorkerFixture#client.typeLiteral4:requestWorker.
  SupervisorInternals.syncAgentPeers: SupervisorInternals#syncAgentPeers().
  SupervisorInternals.assertSavedSiblingNameAvailable: SupervisorInternals#assertSavedSiblingNameAvailable().
  WorkerFixture.descriptor.typeLiteral1.workerId: WorkerFixture#descriptor.typeLiteral1:workerId.
  WorkerFixture.descriptor.typeLiteral1.lifecycle: WorkerFixture#descriptor.typeLiteral1:lifecycle.
  WorkerFixture.descriptor.typeLiteral1.rootSessionId: WorkerFixture#descriptor.typeLiteral1:rootSessionId.
  WorkerFixture.descriptor.typeLiteral1.pid: WorkerFixture#descriptor.typeLiteral1:pid.
  WorkerFixture.descriptor.typeLiteral1.authenticationToken: WorkerFixture#descriptor.typeLiteral1:authenticationToken.
  WorkerFixture.descriptor.typeLiteral1.ownerClientId: WorkerFixture#descriptor.typeLiteral1:ownerClientId.
  WorkerFixture.descriptor.typeLiteral1.createCommand: WorkerFixture#descriptor.typeLiteral1:createCommand.
  WorkerFixture.descriptor.typeLiteral1.createCommand.typeLiteral2.config: WorkerFixture#descriptor.typeLiteral1:createCommand.typeLiteral2:config.
  WorkerFixture.descriptor.typeLiteral1.createCommand.typeLiteral2.config.typeLiteral3.cwd: WorkerFixture#descriptor.typeLiteral1:createCommand.typeLiteral2:config.typeLiteral3:cwd.
---
# Module: [`packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts)

## Classes
### `SupervisorInternals`
- def: [`packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts:16`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L16)
- signature: `interface SupervisorInternals`
- members:
  - `assertSavedSiblingNameAvailable(method)` — [`L26`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L26)
  - `assertSupervisorSavedSessionNameAvailable(method)` — [`L25`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L25)
  - `createOrReuseWorker(method)` — [`L21`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L21)
  - `familyCatalogEntry(method)` — [`L31`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L31)
  - `findSummaryInWorker(method)` — [`L20`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L20)
  - `handleCommand(method)` — [`L32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L32)
  - `refreshWorkerSummaries(method)` — [`L18`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L18)
  - `syncAgentPeers(method)` — [`L19`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L19)
  - `name` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L23)
  - `sessionPath` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L23)
  - `type` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L23)
  - `workers` — [`L17`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L17)
- uses (calls/refs, reference-scoped): [`SessionSummary`](../src/modes/daemon/daemon-session-list.ts.md#SessionSummary), [`AgentFamilyCatalogEntry`](../src/core/agent-messages.ts.md#AgentFamilyCatalogEntry)  (1 test-only)
- used by: (1 test-only callers)

### `WorkerFixture`
- def: [`packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts:35`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L35)
- signature: `interface WorkerFixture`
- members:
  - `authenticationToken` — [`L42`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L42)
  - `client` — [`L46`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L46)
  - `config` — [`L44`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L44)
  - `createCommand` — [`L44`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L44)
  - `cwd` — [`L44`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L44)
  - `descriptor` — [`L36`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L36)
  - `lifecycle` — [`L38`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L38)
  - `ownerClientId` — [`L43`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L43)
  - `pid` — [`L41`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L41)
  - `request` — [`L47`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L47)
  - `requestWorker` — [`L48`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L48)
  - `rootActiveSessionId` — [`L39`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L39)
  - `rootSessionId` — [`L40`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L40)
  - `summaries` — [`L50`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L50)
  - `workerId` — [`L37`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L37)
- uses (calls/refs, reference-scoped): [`SessionSummary`](../src/modes/daemon/daemon-session-list.ts.md#SessionSummary)
- used by: (6 test-only callers)

## Functions
- `summary(overrides: Partial<SessionSummary> & Pick<SessionSummary, "id" | "sessionId">)` — [`L59`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L59)
- `worker(workerId: string, summaries?: SessionSummary[])` — [`L74`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L74)

## Module values
- `tempDirs` — [`L53`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-lazy-subagents.test.ts#L53)


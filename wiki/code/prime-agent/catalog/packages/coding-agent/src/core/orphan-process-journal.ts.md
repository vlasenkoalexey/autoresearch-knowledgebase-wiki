---
title: 'Module: packages/coding-agent/src/core/orphan-process-journal.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/orphan-process-journal.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`orphan-process-journal.ts`/
symbols:
  readActiveOrphanProcesses: readActiveOrphanProcesses().
  recordOrphanProcessState: recordOrphanProcessState().
  ORPHAN_PROCESS_JOURNAL_ENV: ORPHAN_PROCESS_JOURNAL_ENV.
  isOrphanProcessIdentityCurrent: isOrphanProcessIdentityCurrent().
  ActiveOrphanProcess.pid: ActiveOrphanProcess#pid.
  clearOrphanProcessJournal: clearOrphanProcessJournal().
  OrphanProcessRecord: OrphanProcessRecord#
  OrphanProcessRecord.pid: OrphanProcessRecord#pid.
  OrphanProcessRecord.processStartId: OrphanProcessRecord#processStartId.
  OrphanProcessRecord.active: OrphanProcessRecord#active.
  OrphanProcessRecord.version: OrphanProcessRecord#version.
  OrphanProcessRecord.ownerPid: OrphanProcessRecord#ownerPid.
  OrphanProcessRecord.recordedAt: OrphanProcessRecord#recordedAt.
  ActiveOrphanProcess: ActiveOrphanProcess#
  ActiveOrphanProcess.processStartId: ActiveOrphanProcess#processStartId.
---
# Module: [`packages/coding-agent/src/core/orphan-process-journal.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts)

## Classes
### `ActiveOrphanProcess`
- def: [`packages/coding-agent/src/core/orphan-process-journal.ts:15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts#L15)
- signature: `interface ActiveOrphanProcess`
- members:
  - `pid` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts#L16)
  - `processStartId` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts#L17)
- used by: [`recoverUncertainWorkerOperations`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.recoverUncertainWorkerOperations), [`runOwnedSessionWorkerFrontend`](../cli/owned-session-worker.ts.md#runOwnedSessionWorkerFrontend), [`forceStopTrackedWorkers`](../cli/daemon-ps.ts.md#forceStopTrackedWorkers), [`readActiveOrphanProcesses`](orphan-process-journal.ts.md#readActiveOrphanProcesses), [`isOrphanProcessIdentityCurrent`](orphan-process-journal.ts.md#isOrphanProcessIdentityCurrent)  (2 test-only)

### `OrphanProcessRecord`
- def: [`packages/coding-agent/src/core/orphan-process-journal.ts:6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts#L6)
- signature: `interface OrphanProcessRecord`
- members:
  - `active` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts#L11)
  - `ownerPid` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts#L9)
  - `pid` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts#L8)
  - `processStartId` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts#L10)
  - `recordedAt` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts#L12)
  - `version` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts#L7)
- used by: [`readActiveOrphanProcesses`](orphan-process-journal.ts.md#readActiveOrphanProcesses), [`recordOrphanProcessState`](orphan-process-journal.ts.md#recordOrphanProcessState)

## Functions
- `clearOrphanProcessJournal(path: string)` — [`L90`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts#L90)
- `isOrphanProcessIdentityCurrent(orphan: ActiveOrphanProcess)` — [`L86`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts#L86)
- `readActiveOrphanProcesses(path: string, ownerPid: number)` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts#L47)
- `recordOrphanProcessState(pid: number, active: boolean)` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts#L20)

## Module values
- `ORPHAN_PROCESS_JOURNAL_ENV` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/orphan-process-journal.ts#L4)


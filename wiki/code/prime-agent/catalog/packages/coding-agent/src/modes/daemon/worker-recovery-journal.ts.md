---
title: 'Module: packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`worker-recovery-journal.ts`/
symbols:
  WorkerRecoveryJournal.record: WorkerRecoveryJournal#record().
  parseRecords: parseRecords().
  WorkerRecoveryRecord.activeSessionId: WorkerRecoveryRecord#activeSessionId.
  WorkerRecoveryRecord.busy: WorkerRecoveryRecord#busy.
  WorkerRecoveryRecord.operation: WorkerRecoveryRecord#operation.
  WorkerRecoveryRecord: WorkerRecoveryRecord#
  WorkerRecoveryRecord.sessionId: WorkerRecoveryRecord#sessionId.
  WorkerRecoveryRecord.sessionFile: WorkerRecoveryRecord#sessionFile.
  WorkerRecoveryJournal.-constructor: WorkerRecoveryJournal#`<constructor>`().
  WorkerRecoveryJournal.latest: WorkerRecoveryJournal#latest.
  WorkerRecoveryJournal: WorkerRecoveryJournal#
  WorkerRecoveryJournal.readLatest: WorkerRecoveryJournal#readLatest().
  WorkerRecoveryJournal.getLatest: WorkerRecoveryJournal#getLatest().
  WorkerRecoveryJournal.append: WorkerRecoveryJournal#append().
  WorkerRecoveryJournal.compact: WorkerRecoveryJournal#compact().
  WorkerRecoveryRecord.version: WorkerRecoveryRecord#version.
  WorkerRecoveryRecord.recordedAt: WorkerRecoveryRecord#recordedAt.
---
# Module: [`packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts)

## Classes
### `WorkerRecoveryJournal`
- def: [`packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts:58`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L58)
- signature: `class WorkerRecoveryJournal`
- members:
  - `<constructor>(path: string)` — [`L61`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L61)
  - `append(method)` — [`L95`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L95)
  - `compact(method)` — [`L106`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L106)
  - `getLatest(method)` — [`L87`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L87)
  - `readLatest(method)` — [`L91`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L91)
  - `record(method)` — [`L66`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L66)
  - `latest` — [`L59`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L59)
- uses (calls/refs, reference-scoped): [`parseRecords`](worker-recovery-journal.ts.md#parseRecords), [`activeSessionId`](worker-recovery-journal.ts.md#WorkerRecoveryRecord.activeSessionId), [`busy`](worker-recovery-journal.ts.md#WorkerRecoveryRecord.busy), [`operation`](worker-recovery-journal.ts.md#WorkerRecoveryRecord.operation), [`WorkerRecoveryRecord`](worker-recovery-journal.ts.md#WorkerRecoveryRecord), [`sessionFile`](worker-recovery-journal.ts.md#WorkerRecoveryRecord.sessionFile), [`version`](worker-recovery-journal.ts.md#WorkerRecoveryRecord.version), [`recordedAt`](worker-recovery-journal.ts.md#WorkerRecoveryRecord.recordedAt)
- used by: [`daemon-mode.ts`](daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`daemon-supervisor.ts`](daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`<constructor>`](daemon-mode.ts.md#AgentDaemon.-constructor), [`recoverUncertainWorkerOperations`](daemon-supervisor.ts.md#DaemonSupervisor.recoverUncertainWorkerOperations), [`recordWorkerRecoveryState`](daemon-mode.ts.md#AgentDaemon.recordWorkerRecoveryState), [`recoveryJournal`](daemon-mode.ts.md#AgentDaemon.recoveryJournal)  (2 test-only)

### `WorkerRecoveryRecord`
- def: [`packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts:14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L14)
- signature: `interface WorkerRecoveryRecord`
- members:
  - `activeSessionId` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L16)
  - `busy` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L19)
  - `operation` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L20)
  - `recordedAt` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L21)
  - `sessionFile` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L18)
  - `sessionId` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L17)
  - `version` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L15)
- used by: [`recoverUncertainWorkerOperations`](daemon-supervisor.ts.md#DaemonSupervisor.recoverUncertainWorkerOperations), [`recordWorkerRecoveryState`](daemon-mode.ts.md#AgentDaemon.recordWorkerRecoveryState), [`record`](worker-recovery-journal.ts.md#WorkerRecoveryJournal.record), [`parseRecords`](worker-recovery-journal.ts.md#parseRecords), [`latest`](worker-recovery-journal.ts.md#WorkerRecoveryJournal.latest), [`readLatest`](worker-recovery-journal.ts.md#WorkerRecoveryJournal.readLatest), [`getLatest`](worker-recovery-journal.ts.md#WorkerRecoveryJournal.getLatest), [`append`](worker-recovery-journal.ts.md#WorkerRecoveryJournal.append)  (2 test-only)

## Functions
- `parseRecords(path: string)` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/worker-recovery-journal.ts#L24)


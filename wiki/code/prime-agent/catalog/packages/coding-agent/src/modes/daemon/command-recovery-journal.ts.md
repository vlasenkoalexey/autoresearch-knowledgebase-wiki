---
title: 'Module: packages/coding-agent/src/modes/daemon/command-recovery-journal.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/command-recovery-journal.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`command-recovery-journal.ts`/
symbols:
  CommandRecoveryJournal.begin: CommandRecoveryJournal#begin().
  CommandRecoveryJournal.acknowledge: CommandRecoveryJournal#acknowledge().
  CommandRecoveryJournal.load: CommandRecoveryJournal#load().
  CommandRecoveryJournal.recordResult: CommandRecoveryJournal#recordResult().
  CommandRecoveryJournal.compact: CommandRecoveryJournal#compact().
  CommandRecoveryJournal.lookup: CommandRecoveryJournal#lookup().
  CommandRecoveryJournal.-constructor: CommandRecoveryJournal#`<constructor>`().
  CommandRecoveryJournal.entries: CommandRecoveryJournal#entries.
  JournalRecord: JournalRecord#
  createCommandIdempotencyKey: createCommandIdempotencyKey().
  CommandRecoveryJournal.append: CommandRecoveryJournal#append().
  JournalEntry.response: JournalEntry#response.
  ResultRecord.response: ResultRecord#response.
  JournalEntry.received: JournalEntry#received.
  ReceivedRecord.key: ReceivedRecord#key.
  ResultRecord.type: ResultRecord#type.
  ResultRecord.key: ResultRecord#key.
  CommandRecoveryJournal.recordCount: CommandRecoveryJournal#recordCount.
  ReceivedRecord.clientId: ReceivedRecord#clientId.
  ReceivedRecord.commandId: ReceivedRecord#commandId.
  CommandJournalBeginResult: CommandJournalBeginResult#
  ReceivedRecord.version: ReceivedRecord#version.
  ReceivedRecord.type: ReceivedRecord#type.
  ResultRecord.version: ResultRecord#version.
  AcknowledgedRecord.type: AcknowledgedRecord#type.
  AcknowledgedRecord.key: AcknowledgedRecord#key.
  CommandRecoveryJournal: CommandRecoveryJournal#
  JournalEntry: JournalEntry#
  ReceivedRecord: ReceivedRecord#
  ReceivedRecord.recordedAt: ReceivedRecord#recordedAt.
  ResultRecord.recordedAt: ResultRecord#recordedAt.
  AcknowledgedRecord.version: AcknowledgedRecord#version.
  ReceivedRecord.commandType: ReceivedRecord#commandType.
  ResultRecord: ResultRecord#
  AcknowledgedRecord.recordedAt: AcknowledgedRecord#recordedAt.
  COMPACT_AFTER_RECORDS: COMPACT_AFTER_RECORDS.
  AcknowledgedRecord: AcknowledgedRecord#
---
# Module: [`packages/coding-agent/src/modes/daemon/command-recovery-journal.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts)

## Classes
### `AcknowledgedRecord`
- def: [`packages/coding-agent/src/modes/daemon/command-recovery-journal.ts:23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L23)
- signature: `interface AcknowledgedRecord`
- members:
  - `key` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L26)
  - `recordedAt` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L27)
  - `type` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L25)
  - `version` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L24)
- used by: [`acknowledge`](command-recovery-journal.ts.md#CommandRecoveryJournal.acknowledge), [`load`](command-recovery-journal.ts.md#CommandRecoveryJournal.load), [`compact`](command-recovery-journal.ts.md#CommandRecoveryJournal.compact), [`JournalRecord`](command-recovery-journal.ts.md#JournalRecord)

### `CommandJournalBeginResult`
- def: [`packages/coding-agent/src/modes/daemon/command-recovery-journal.ts:37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L37)
- signature: `type CommandJournalBeginResult`
- uses (calls/refs, reference-scoped): [`DaemonResponse`](daemon-protocol.ts.md#DaemonResponse)
- used by: [`begin`](command-recovery-journal.ts.md#CommandRecoveryJournal.begin), [`lookup`](command-recovery-journal.ts.md#CommandRecoveryJournal.lookup)

### `CommandRecoveryJournal`
- def: [`packages/coding-agent/src/modes/daemon/command-recovery-journal.ts:53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L53)
- doc: Append-only command journal used at the supervisor boundary. A received
- signature: `class CommandRecoveryJournal`
- members:
  - `<constructor>(path: string)` — [`L57`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L57) — Append-only command journal used at the supervisor boundary. A received
  - `acknowledge(method)` — [`L111`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L111)
  - `append(method)` — [`L174`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L174)
  - `begin(method)` — [`L73`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L73)
  - `compact(method)` — [`L186`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L186)
  - `load(method)` — [`L128`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L128)
  - `lookup(method)` — [`L62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L62)
  - `recordResult(method)` — [`L91`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L91)
  - `entries` — [`L54`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L54)
  - `recordCount` — [`L55`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L55)
- uses (calls/refs, reference-scoped): [`DaemonResponse`](daemon-protocol.ts.md#DaemonResponse), [`DaemonClientId`](daemon-protocol.ts.md#DaemonClientId), [`DaemonCommandId`](daemon-protocol.ts.md#DaemonCommandId), [`JournalRecord`](command-recovery-journal.ts.md#JournalRecord), [`createCommandIdempotencyKey`](command-recovery-journal.ts.md#createCommandIdempotencyKey), [`response`](command-recovery-journal.ts.md#JournalEntry.response), [`received`](command-recovery-journal.ts.md#JournalEntry.received), [`response`](command-recovery-journal.ts.md#ResultRecord.response), [`key`](command-recovery-journal.ts.md#ReceivedRecord.key), [`key`](command-recovery-journal.ts.md#ResultRecord.key), [`type`](command-recovery-journal.ts.md#ResultRecord.type), [`CommandJournalBeginResult`](command-recovery-journal.ts.md#CommandJournalBeginResult), [`clientId`](command-recovery-journal.ts.md#ReceivedRecord.clientId), [`commandId`](command-recovery-journal.ts.md#ReceivedRecord.commandId), [`key`](command-recovery-journal.ts.md#AcknowledgedRecord.key), [`type`](command-recovery-journal.ts.md#AcknowledgedRecord.type), [`type`](command-recovery-journal.ts.md#ReceivedRecord.type), [`version`](command-recovery-journal.ts.md#ReceivedRecord.version), [`version`](command-recovery-journal.ts.md#ResultRecord.version), [`JournalEntry`](command-recovery-journal.ts.md#JournalEntry), [`ReceivedRecord`](command-recovery-journal.ts.md#ReceivedRecord), [`recordedAt`](command-recovery-journal.ts.md#ReceivedRecord.recordedAt), [`recordedAt`](command-recovery-journal.ts.md#ResultRecord.recordedAt), [`version`](command-recovery-journal.ts.md#AcknowledgedRecord.version), [`ResultRecord`](command-recovery-journal.ts.md#ResultRecord), [`COMPACT_AFTER_RECORDS`](command-recovery-journal.ts.md#COMPACT_AFTER_RECORDS), [`commandType`](command-recovery-journal.ts.md#ReceivedRecord.commandType), [`recordedAt`](command-recovery-journal.ts.md#AcknowledgedRecord.recordedAt)
- used by: [`daemon-supervisor.ts`](daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`handleCommand`](daemon-supervisor.ts.md#DaemonSupervisor.handleCommand), [`start`](daemon-supervisor.ts.md#DaemonSupervisor.start), [`handleLine`](daemon-supervisor.ts.md#DaemonSupervisor.handleLine), [`commandJournal`](daemon-supervisor.ts.md#DaemonSupervisor.commandJournal)  (2 test-only)

### `JournalEntry`
- def: [`packages/coding-agent/src/modes/daemon/command-recovery-journal.ts:32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L32)
- signature: `interface JournalEntry`
- members:
  - `received` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L33)
  - `response` — [`L34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L34)
- uses (calls/refs, reference-scoped): [`DaemonResponse`](daemon-protocol.ts.md#DaemonResponse), [`ReceivedRecord`](command-recovery-journal.ts.md#ReceivedRecord)
- used by: [`begin`](command-recovery-journal.ts.md#CommandRecoveryJournal.begin), [`load`](command-recovery-journal.ts.md#CommandRecoveryJournal.load), [`recordResult`](command-recovery-journal.ts.md#CommandRecoveryJournal.recordResult), [`compact`](command-recovery-journal.ts.md#CommandRecoveryJournal.compact), [`lookup`](command-recovery-journal.ts.md#CommandRecoveryJournal.lookup), [`entries`](command-recovery-journal.ts.md#CommandRecoveryJournal.entries)

### `JournalRecord`
- def: [`packages/coding-agent/src/modes/daemon/command-recovery-journal.ts:30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L30)
- signature: `type JournalRecord`
- uses (calls/refs, reference-scoped): [`ReceivedRecord`](command-recovery-journal.ts.md#ReceivedRecord), [`ResultRecord`](command-recovery-journal.ts.md#ResultRecord), [`AcknowledgedRecord`](command-recovery-journal.ts.md#AcknowledgedRecord)
- used by: [`load`](command-recovery-journal.ts.md#CommandRecoveryJournal.load), [`compact`](command-recovery-journal.ts.md#CommandRecoveryJournal.compact), [`append`](command-recovery-journal.ts.md#CommandRecoveryJournal.append)

### `ReceivedRecord`
- def: [`packages/coding-agent/src/modes/daemon/command-recovery-journal.ts:5`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L5)
- signature: `interface ReceivedRecord`
- members:
  - `clientId` — [`L9`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L9)
  - `commandId` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L10)
  - `commandType` — [`L11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L11)
  - `key` — [`L8`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L8)
  - `recordedAt` — [`L12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L12)
  - `type` — [`L7`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L7)
  - `version` — [`L6`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L6)
- uses (calls/refs, reference-scoped): [`DaemonClientId`](daemon-protocol.ts.md#DaemonClientId), [`DaemonCommandId`](daemon-protocol.ts.md#DaemonCommandId)
- used by: [`begin`](command-recovery-journal.ts.md#CommandRecoveryJournal.begin), [`acknowledge`](command-recovery-journal.ts.md#CommandRecoveryJournal.acknowledge), [`load`](command-recovery-journal.ts.md#CommandRecoveryJournal.load), [`compact`](command-recovery-journal.ts.md#CommandRecoveryJournal.compact), [`JournalRecord`](command-recovery-journal.ts.md#JournalRecord), [`received`](command-recovery-journal.ts.md#JournalEntry.received)

### `ResultRecord`
- def: [`packages/coding-agent/src/modes/daemon/command-recovery-journal.ts:15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L15)
- signature: `interface ResultRecord`
- members:
  - `key` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L18)
  - `recordedAt` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L20)
  - `response` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L19)
  - `type` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L17)
  - `version` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L16)
- uses (calls/refs, reference-scoped): [`DaemonResponse`](daemon-protocol.ts.md#DaemonResponse)
- used by: [`acknowledge`](command-recovery-journal.ts.md#CommandRecoveryJournal.acknowledge), [`load`](command-recovery-journal.ts.md#CommandRecoveryJournal.load), [`recordResult`](command-recovery-journal.ts.md#CommandRecoveryJournal.recordResult), [`compact`](command-recovery-journal.ts.md#CommandRecoveryJournal.compact), [`JournalRecord`](command-recovery-journal.ts.md#JournalRecord)

## Functions
- `createCommandIdempotencyKey(clientId: string, commandId: string)` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L44)

## Module values
- `COMPACT_AFTER_RECORDS` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/command-recovery-journal.ts#L42)


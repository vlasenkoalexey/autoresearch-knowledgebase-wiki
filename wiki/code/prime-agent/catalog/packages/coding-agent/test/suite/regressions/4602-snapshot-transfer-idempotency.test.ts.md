---
title: 'Module: packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/regressions/`4602-snapshot-transfer-idempotency.test.ts`/
symbols:
  streamedResult: streamedResult().
  workerHarness: workerHarness().
  summary: summary().
  activeSessionId: activeSessionId.
  frame: frame().
  socketClient: socketClient().
  snapshotFrames: snapshotFrames().
  WorkerHarness.transcriptCaches: WorkerHarness#transcriptCaches.
  WorkerHarness.snapshotCache: WorkerHarness#snapshotCache.
  WorkerHarness: WorkerHarness#
  WorkerHarness.descriptor: WorkerHarness#descriptor.
  snapshotId: snapshotId.
  WorkerHarness.summaries: WorkerHarness#summaries.
  WorkerHarness.descriptor.typeLiteral0.workerId: WorkerHarness#descriptor.typeLiteral0:workerId.
  WorkerHarness.snapshotGenerations: WorkerHarness#snapshotGenerations.
  WorkerHarness.snapshotLoads: WorkerHarness#snapshotLoads.
  WorkerHarness.descriptor.typeLiteral0.lifecycle: WorkerHarness#descriptor.typeLiteral0:lifecycle.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.transcript: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:transcript.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.result: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:result.
  WorkerHarness.client: WorkerHarness#client.
  WorkerHarness.descriptor.typeLiteral0.pid: WorkerHarness#descriptor.typeLiteral0:pid.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.validation: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:validation.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.validation.typeLiteral3.promise: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:validation.typeLiteral3:promise.
  WorkerHarness.intentionalStop: WorkerHarness#intentionalStop.
  WorkerHarness.stopRevision: WorkerHarness#stopRevision.
  WorkerHarness.client.typeLiteral1.close: WorkerHarness#client.typeLiteral1:close.
  WorkerHarness.client.typeLiteral1.request: WorkerHarness#client.typeLiteral1:request.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.incoming: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:incoming.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.retired: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:retired.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.validation.typeLiteral3.resolve: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:validation.typeLiteral3:resolve.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.validation.typeLiteral3.reject: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:validation.typeLiteral3:reject.
---
# Module: [`packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts)

## Classes
### `WorkerHarness`
- def: [`packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts:25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L25)
- signature: `interface WorkerHarness`
- members:
  - `client` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L27)
  - `close` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L27)
  - `descriptor` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L26)
  - `incoming` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L38)
  - `intentionalStop` — [`L45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L45)
  - `lifecycle` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L26)
  - `pid` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L26)
  - `promise` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L40)
  - `reject` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L40)
  - `request` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L27)
  - `resolve` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L40)
  - `result` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L37)
  - `retired` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L39)
  - `snapshotCache` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L29)
  - `snapshotGenerations` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L31)
  - `snapshotLoads` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L44)
  - `stopRevision` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L46)
  - `summaries` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L28)
  - `transcript` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L36)
  - `transcriptCaches` — [`L30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L30)
  - `validation` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L40)
  - `workerId` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L26)
- uses (calls/refs, reference-scoped): [`SessionSummary`](../../../src/modes/daemon/daemon-session-list.ts.md#SessionSummary), [`DaemonAttachResult`](../../../src/modes/daemon/daemon-protocol.ts.md#DaemonAttachResult), [`SnapshotTranscriptCache`](../../../src/modes/daemon/snapshot-transcript-cache.ts.md#SnapshotTranscriptCache)
- used by: (2 test-only callers)

## Functions
- `frame(message: DaemonOutbound, snapshotPurpose?: "attach" | "replacement" | "catchup" | undefined)` — [`L90`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L90)
- `snapshotFrames(messages: AgentMessage[])` — [`L143`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L143)
- `socketClient(id: string, socket: PassThrough)` — [`L131`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L131)
- `streamedResult(messages: AgentMessage[])` — [`L66`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L66)
- `summary()` — [`L49`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L49)
- `workerHarness()` — [`L109`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L109)

## Module values
- `activeSessionId` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L22)
- `snapshotId` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4602-snapshot-transfer-idempotency.test.ts#L23)


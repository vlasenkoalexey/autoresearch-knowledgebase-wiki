---
title: 'Module: packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/regressions/`4677-snapshot-catchup-replacement.test.ts`/
symbols:
  streamedResult: streamedResult().
  workerHarness: workerHarness().
  summary: summary().
  activeSessionId: activeSessionId.
  socketClient: socketClient().
  snapshotFrame: snapshotFrame().
  WorkerHarness.transcriptCaches: WorkerHarness#transcriptCaches.
  snapshotFrame.message-Extract.typeLiteral12.type: snapshotFrame().(message)Extract:typeLiteral12:type.
  tempDirectory: tempDirectory().
  WorkerHarness: WorkerHarness#
  WorkerHarness.snapshotCache: WorkerHarness#snapshotCache.
  WorkerHarness.descriptor: WorkerHarness#descriptor.
  WorkerHarness.descriptor.typeLiteral0.workerId: WorkerHarness#descriptor.typeLiteral0:workerId.
  WorkerHarness.summaries: WorkerHarness#summaries.
  WorkerHarness.snapshotLoads: WorkerHarness#snapshotLoads.
  WorkerHarness.stopRevision: WorkerHarness#stopRevision.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.transcript: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:transcript.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.result: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:result.
  directories: directories.
  WorkerHarness.client: WorkerHarness#client.
  WorkerHarness.snapshotGenerations: WorkerHarness#snapshotGenerations.
  WorkerHarness.descriptor.typeLiteral0.rootActiveSessionId: WorkerHarness#descriptor.typeLiteral0:rootActiveSessionId.
  WorkerHarness.descriptor.typeLiteral0.lifecycle: WorkerHarness#descriptor.typeLiteral0:lifecycle.
  WorkerHarness.descriptor.typeLiteral0.pid: WorkerHarness#descriptor.typeLiteral0:pid.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.validation: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:validation.
  WorkerHarness.intentionalStop: WorkerHarness#intentionalStop.
  WorkerHarness.client.typeLiteral1.request: WorkerHarness#client.typeLiteral1:request.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.incoming: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:incoming.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.retired: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:retired.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.validation.typeLiteral3.promise: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:validation.typeLiteral3:promise.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.validation.typeLiteral3.resolve: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:validation.typeLiteral3:resolve.
  WorkerHarness.snapshotGenerations.Map.Map.typeLiteral2.validation.typeLiteral3.reject: WorkerHarness#snapshotGenerations.Map:Map:typeLiteral2:validation.typeLiteral3:reject.
---
# Module: [`packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts)

## Classes
### `WorkerHarness`
- def: [`packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts:24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L24)
- signature: `interface WorkerHarness`
- members:
  - `client` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L26)
  - `descriptor` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L25)
  - `incoming` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L37)
  - `intentionalStop` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L44)
  - `lifecycle` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L25)
  - `pid` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L25)
  - `promise` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L39)
  - `reject` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L39)
  - `request` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L26)
  - `resolve` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L39)
  - `result` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L36)
  - `retired` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L38)
  - `rootActiveSessionId` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L25)
  - `snapshotCache` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L28)
  - `snapshotGenerations` — [`L30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L30)
  - `snapshotLoads` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L43)
  - `stopRevision` — [`L45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L45)
  - `summaries` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L27)
  - `transcript` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L35)
  - `transcriptCaches` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L29)
  - `validation` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L39)
  - `workerId` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L25)
- uses (calls/refs, reference-scoped): [`SessionSummary`](../../../src/modes/daemon/daemon-session-list.ts.md#SessionSummary), [`DaemonAttachResult`](../../../src/modes/daemon/daemon-protocol.ts.md#DaemonAttachResult), [`SnapshotTranscriptCache`](../../../src/modes/daemon/snapshot-transcript-cache.ts.md#SnapshotTranscriptCache)  (1 test-only)
- used by: (2 test-only callers)

## Functions
- `snapshotFrame(message: { type: "session_snapshot_begin"; activeSessionId: string; snapshotId: string; snapshot: Omit<DaemonSessionSnapshot, "messages">; messageCount: number; targetChunkBytes: number; purpose?: "attach" | ... 2 more ... | undefined; } | { ...; } | { ...; }, purpose?: "attach" | ... 1 more ... | "catchup")` — [`L95`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L95)
- `socketClient(id: string)` — [`L115`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L115)
- `streamedResult(snapshotId: string, messageCount: number, lastEventSequence: number)` — [`L77`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L77)
- `summary(messageCount: number)` — [`L60`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L60)
- `tempDirectory()` — [`L54`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L54)
- `workerHarness(result: DaemonAttachResult, transcript: SnapshotTranscriptCache)` — [`L128`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L128)

## Module values
- `activeSessionId` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L21)
- `directories` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L22)
- `type` — [`L98`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4677-snapshot-catchup-replacement.test.ts#L98)


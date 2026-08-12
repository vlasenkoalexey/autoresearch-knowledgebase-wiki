---
title: 'Module: packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`snapshot-transcript-cache.ts`/
symbols:
  SnapshotTranscriptCache.snapshotId: SnapshotTranscriptCache#snapshotId.
  SnapshotTranscriptCache.-constructor: SnapshotTranscriptCache#`<constructor>`().
  SnapshotTranscriptCache: SnapshotTranscriptCache#
  SnapshotTranscriptCache.storeChunk: SnapshotTranscriptCache#storeChunk().
  SnapshotTranscriptCache.dispose: SnapshotTranscriptCache#dispose().
  createSnapshotTranscriptChunks.options-typeLiteral5.signal: createSnapshotTranscriptChunks().(options)typeLiteral5:signal.
  SnapshotTranscriptCache.-get-complete: SnapshotTranscriptCache#`<get>complete`().
  SnapshotTranscriptCache.readChunk: SnapshotTranscriptCache#readChunk().
  SnapshotTranscriptCacheOptions.snapshotId: SnapshotTranscriptCacheOptions#snapshotId.
  SnapshotTranscriptCacheOptions.activeSessionId: SnapshotTranscriptCacheOptions#activeSessionId.
  SnapshotTranscriptCache.waitForChunk: SnapshotTranscriptCache#waitForChunk().
  SnapshotTranscriptCacheOptions.cacheRoot: SnapshotTranscriptCacheOptions#cacheRoot.
  SnapshotTranscriptCache.markComplete: SnapshotTranscriptCache#markComplete().
  SnapshotTranscriptCache.retain: SnapshotTranscriptCache#retain().
  SnapshotTranscriptCache.appendEncodedChunk: SnapshotTranscriptCache#appendEncodedChunk().
  SnapshotTranscriptCache.encodeMessages: SnapshotTranscriptCache#encodeMessages().
  SnapshotTranscriptCache.chunks: SnapshotTranscriptCache#chunks.
  createSnapshotTranscriptChunks.options-typeLiteral5.messages: createSnapshotTranscriptChunks().(options)typeLiteral5:messages.
  SnapshotTranscriptCache.disposeNow: SnapshotTranscriptCache#disposeNow().
  SnapshotTranscriptCacheOptions.messages: SnapshotTranscriptCacheOptions#messages.
  SnapshotTranscriptCacheOptions.targetChunkBytes: SnapshotTranscriptCacheOptions#targetChunkBytes.
  createSnapshotTranscriptChunks: createSnapshotTranscriptChunks().
  createSnapshotTranscriptChunks.options-typeLiteral5.activeSessionId: createSnapshotTranscriptChunks().(options)typeLiteral5:activeSessionId.
  createSnapshotTranscriptChunks.options-typeLiteral5.snapshotId: createSnapshotTranscriptChunks().(options)typeLiteral5:snapshotId.
  SnapshotTranscriptCache.markFailed: SnapshotTranscriptCache#markFailed().
  SNAPSHOT_TARGET_CHUNK_BYTES: SNAPSHOT_TARGET_CHUNK_BYTES.
  SnapshotTranscriptChunkSource: SnapshotTranscriptChunkSource#
  SnapshotTranscriptCache.-get-chunkCount: SnapshotTranscriptCache#`<get>chunkCount`().
  SnapshotTranscriptCache.cacheDirectory: SnapshotTranscriptCache#cacheDirectory.
  SnapshotTranscriptCache.chunkWaiters: SnapshotTranscriptCache#chunkWaiters.
  createSnapshotTranscriptChunks.options-typeLiteral5.targetChunkBytes: createSnapshotTranscriptChunks().(options)typeLiteral5:targetChunkBytes.
  SnapshotTranscriptCache.disposed: SnapshotTranscriptCache#disposed.
  SnapshotTranscriptCache.failure: SnapshotTranscriptCache#failure.
  SnapshotTranscriptCache.-get-fileBacked: SnapshotTranscriptCache#`<get>fileBacked`().
  SnapshotTranscriptCache.completed: SnapshotTranscriptCache#completed.
  SnapshotTranscriptChunk.buffer: SnapshotTranscriptChunk#buffer.
  SnapshotTranscriptCache.targetChunkBytes: SnapshotTranscriptCache#targetChunkBytes.
  SnapshotTranscriptChunk.path: SnapshotTranscriptChunk#path.
  SnapshotTranscriptCacheOptions.memoryCacheBytes: SnapshotTranscriptCacheOptions#memoryCacheBytes.
  SnapshotTranscriptCache.readers: SnapshotTranscriptCache#readers.
  SnapshotTranscriptCache.totalBytes: SnapshotTranscriptCache#totalBytes.
  SnapshotTranscriptCache.disposeRequested: SnapshotTranscriptCache#disposeRequested.
  SnapshotTranscriptCache.-get-bytes: SnapshotTranscriptCache#`<get>bytes`().
  SNAPSHOT_MEMORY_CACHE_BYTES: SNAPSHOT_MEMORY_CACHE_BYTES.
  SnapshotTranscriptChunk: SnapshotTranscriptChunk#
  SnapshotTranscriptCacheOptions: SnapshotTranscriptCacheOptions#
  SnapshotTranscriptCache.activeSessionId: SnapshotTranscriptCache#activeSessionId.
---
# Module: [`packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts)

## Classes
### `SnapshotTranscriptCache`
- def: [`packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts:74`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L74)
- signature: `class SnapshotTranscriptCache`
- members:
  - `<constructor>(options: SnapshotTranscriptCacheOptions)` — [`L91`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L91)
  - `<get>bytes` — [`L109`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L109)
  - `<get>chunkCount` — [`L101`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L101)
  - `<get>complete` — [`L105`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L105)
  - `<get>fileBacked` — [`L113`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L113)
  - `appendEncodedChunk(method)` — [`L137`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L137)
  - `dispose(method)` — [`L209`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L209)
  - `disposeNow(method)` — [`L216`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L216)
  - `encodeMessages(method)` — [`L227`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L227)
  - `markComplete(method)` — [`L144`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L144)
  - `markFailed(method)` — [`L163`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L163)
  - `readChunk(method)` — [`L117`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L117)
  - `retain(method)` — [`L193`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L193)
  - `storeChunk(method)` — [`L256`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L256)
  - `waitForChunk(method)` — [`L176`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L176)
  - `activeSessionId` — [`L89`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L89)
  - `cacheDirectory` — [`L76`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L76)
  - `chunkWaiters` — [`L83`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L83)
  - `chunks` — [`L75`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L75)
  - `completed` — [`L78`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L78)
  - `disposeRequested` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L80)
  - `disposed` — [`L81`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L81)
  - `failure` — [`L82`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L82)
  - `readers` — [`L79`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L79)
  - `snapshotId` — [`L88`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L88)
  - `targetChunkBytes` — [`L87`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L87)
  - `totalBytes` — [`L77`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L77)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage), [`snapshotId`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCacheOptions.snapshotId), [`activeSessionId`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCacheOptions.activeSessionId), [`cacheRoot`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCacheOptions.cacheRoot), [`messages`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCacheOptions.messages), [`targetChunkBytes`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCacheOptions.targetChunkBytes), [`SNAPSHOT_TARGET_CHUNK_BYTES`](snapshot-transcript-cache.ts.md#SNAPSHOT_TARGET_CHUNK_BYTES), [`buffer`](snapshot-transcript-cache.ts.md#SnapshotTranscriptChunk.buffer), [`memoryCacheBytes`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCacheOptions.memoryCacheBytes), [`path`](snapshot-transcript-cache.ts.md#SnapshotTranscriptChunk.path), [`SnapshotTranscriptCacheOptions`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCacheOptions), [`SnapshotTranscriptChunk`](snapshot-transcript-cache.ts.md#SnapshotTranscriptChunk), [`SNAPSHOT_MEMORY_CACHE_BYTES`](snapshot-transcript-cache.ts.md#SNAPSHOT_MEMORY_CACHE_BYTES)
- used by: [`daemon-supervisor.ts`](daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`handleWorkerFrame`](daemon-supervisor.ts.md#DaemonSupervisor.handleWorkerFrame), [`type`](daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type), [`stopWorkerUntracked`](daemon-supervisor.ts.md#DaemonSupervisor.stopWorkerUntracked), [`cleanupSupervisorResourcesOnce`](daemon-supervisor.ts.md#DaemonSupervisor.cleanupSupervisorResourcesOnce), [`getOrCreateTranscriptCache`](daemon-supervisor.ts.md#DaemonSupervisor.getOrCreateTranscriptCache), [`handleWorkerClose`](daemon-supervisor.ts.md#DaemonSupervisor.handleWorkerClose), [`cacheLoadedSnapshot`](daemon-supervisor.ts.md#DaemonSupervisor.cacheLoadedSnapshot), [`streamSnapshot`](daemon-supervisor.ts.md#DaemonSupervisor.streamSnapshot), [`failWorkerSnapshotCache`](daemon-supervisor.ts.md#DaemonSupervisor.failWorkerSnapshotCache), [`transcript`](daemon-supervisor.ts.md#SnapshotTranscriptGeneration.transcript), [`retireWorkerSnapshotCache`](daemon-supervisor.ts.md#DaemonSupervisor.retireWorkerSnapshotCache), [`failSnapshotGeneration`](daemon-supervisor.ts.md#DaemonSupervisor.failSnapshotGeneration), [`transcriptCaches`](daemon-supervisor.ts.md#ResidentWorker.transcriptCaches), [`createStreamedAttachResult`](daemon-supervisor.ts.md#DaemonSupervisor.createStreamedAttachResult), [`currentSnapshotGeneration`](daemon-supervisor.ts.md#DaemonSupervisor.currentSnapshotGeneration), [`deleteSnapshotGeneration`](daemon-supervisor.ts.md#DaemonSupervisor.deleteSnapshotGeneration), [`transcript`](daemon-supervisor.ts.md#WorkerAttachData.transcript)  (12 test-only)

### `SnapshotTranscriptCacheOptions`
- def: [`packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts:13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L13)
- signature: `interface SnapshotTranscriptCacheOptions`
- members:
  - `activeSessionId` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L14)
  - `cacheRoot` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L17)
  - `memoryCacheBytes` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L19)
  - `messages` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L16)
  - `snapshotId` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L15)
  - `targetChunkBytes` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L18)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage)
- used by: [`handleWorkerFrame`](daemon-supervisor.ts.md#DaemonSupervisor.handleWorkerFrame), [`getOrCreateTranscriptCache`](daemon-supervisor.ts.md#DaemonSupervisor.getOrCreateTranscriptCache), [`cacheLoadedSnapshot`](daemon-supervisor.ts.md#DaemonSupervisor.cacheLoadedSnapshot), [`<constructor>`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCache.-constructor), [`storeChunk`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCache.storeChunk), [`encodeMessages`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCache.encodeMessages)  (5 test-only)

### `SnapshotTranscriptChunk`
- def: [`packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts:8`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L8)
- signature: `interface SnapshotTranscriptChunk`
- members:
  - `buffer` — [`L9`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L9)
  - `path` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L10)
- used by: [`storeChunk`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCache.storeChunk), [`readChunk`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCache.readChunk), [`chunks`](snapshot-transcript-cache.ts.md#SnapshotTranscriptCache.chunks)

### `SnapshotTranscriptChunkSource`
- def: [`packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts:22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L22)
- signature: `type SnapshotTranscriptChunkSource`
- used by: [`handleCommand`](daemon-mode.ts.md#AgentDaemon.handleCommand), [`daemon-mode.ts`](daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`drainBackpressuredClientCatchups`](daemon-mode.ts.md#AgentDaemon.drainBackpressuredClientCatchups), [`streamWorkerSnapshot`](daemon-mode.ts.md#AgentDaemon.streamWorkerSnapshot)  (1 test-only)

## Functions
- `createSnapshotTranscriptChunks(options: { activeSessionId: string; snapshotId: string; messages: readonly AgentMessage[]; targetChunkBytes?: number | undefined; signal?: AbortSignal | undefined; })` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L27)

## Module values
- `SNAPSHOT_MEMORY_CACHE_BYTES` — [`L6`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L6)
- `SNAPSHOT_TARGET_CHUNK_BYTES` — [`L5`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L5)
- `activeSessionId` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L28)
- `messages` — [`L30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L30)
- `signal` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L32)
- `snapshotId` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L29)
- `targetChunkBytes` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/snapshot-transcript-cache.ts#L31)


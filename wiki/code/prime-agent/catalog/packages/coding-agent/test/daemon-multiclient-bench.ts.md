---
title: 'Module: packages/coding-agent/test/daemon-multiclient-bench.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/daemon-multiclient-bench.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`daemon-multiclient-bench.ts`/
symbols:
  createAssistantMessage: createAssistantMessage().
  printResults: printResults().
  runAttachV2: runAttachV2().
  main: main().
  runScenario: runScenario().
  runFanoutV2: runFanoutV2().
  loadSessionFixture.Promise.typeLiteral408.cleanup: loadSessionFixture().Promise:typeLiteral408:cleanup().
  runRealSessionBenchmark: runRealSessionBenchmark().
  printSessionLoad: printSessionLoad().
  writeToRecipient: writeToRecipient().
  attachMessages: attachMessages.
  runFanout: runFanout().
  runSessionAttach: runSessionAttach().
  generateSessionFixture: generateSessionFixture().
  runAttach: runAttach().
  streamCorpus: streamCorpus.
  BenchmarkResult: BenchmarkResult#
  writeBufferToRecipient: writeBufferToRecipient().
  createSocketHarness: createSocketHarness().
  SocketHarness.senders: SocketHarness#senders.
  createReceiver: createReceiver().
  memoryDeltaMiB: memoryDeltaMiB().
  MEBIBYTE: MEBIBYTE.
  Counters.maxSerializationMs: Counters#maxSerializationMs.
  createAttachResponse: createAttachResponse().
  SocketHarness.receivers: SocketHarness#receivers.
  Counters: Counters#
  Counters.serializations: Counters#serializations.
  Counters.writtenBytes: Counters#writtenBytes.
  createAttachResponseForMessages: createAttachResponseForMessages().
  loadSessionFixture.Promise.typeLiteral408.messages: loadSessionFixture().Promise:typeLiteral408:messages.
  loadSessionFixture.Promise.typeLiteral408.load: loadSessionFixture().Promise:typeLiteral408:load.
  Counters.serializationMs: Counters#serializationMs.
  Counters.writes: Counters#writes.
  socketPathForRun: socketPathForRun().
  createStreamingEvent: createStreamingEvent().
  STREAM_CHUNK_CHARS: STREAM_CHUNK_CHARS.
  SessionLoadResult.messageCount: SessionLoadResult#messageCount.
  socketCounter: socketCounter.
  repeatedText: repeatedText().
  CLIENT_COUNTS: CLIENT_COUNTS.
  STREAM_CHARS: STREAM_CHARS.
  ATTACH_HISTORY_MESSAGES: ATTACH_HISTORY_MESSAGES.
  ATTACH_MESSAGE_CHARS: ATTACH_MESSAGE_CHARS.
  BenchmarkResult.scenario: BenchmarkResult#scenario.
  SessionLoadResult: SessionLoadResult#
  SessionLoadResult.fileBytes: SessionLoadResult#fileBytes.
  SessionLoadResult.loadMs: SessionLoadResult#loadMs.
  SessionLoadResult.contextMs: SessionLoadResult#contextMs.
  SessionLoadResult.heapDeltaMiB: SessionLoadResult#heapDeltaMiB.
  SessionLoadResult.rssDeltaMiB: SessionLoadResult#rssDeltaMiB.
  SessionLoadResult.externalDeltaMiB: SessionLoadResult#externalDeltaMiB.
  SessionLoadResult.peakRssDeltaMiB: SessionLoadResult#peakRssDeltaMiB.
  Receiver: Receiver#
  Receiver.done: Receiver#done.
  Receiver.setExpectedBytes: Receiver#setExpectedBytes().
  SocketHarness: SocketHarness#
  removeSocketPath: removeSocketPath().
  writeStreamChunk: writeStreamChunk().
  SESSION_CLIENT_COUNTS: SESSION_CLIENT_COUNTS.
  BenchmarkResult.clients: BenchmarkResult#clients.
  BenchmarkResult.elapsedMs: BenchmarkResult#elapsedMs.
  BenchmarkResult.throughputMiBPerSecond: BenchmarkResult#throughputMiBPerSecond.
  BenchmarkResult.heapDeltaMiB: BenchmarkResult#heapDeltaMiB.
  BenchmarkResult.rssDeltaMiB: BenchmarkResult#rssDeltaMiB.
  BenchmarkResult.externalDeltaMiB: BenchmarkResult#externalDeltaMiB.
  BenchmarkResult.peakRssDeltaMiB: BenchmarkResult#peakRssDeltaMiB.
  GeneratedSessionFixture: GeneratedSessionFixture#
  GeneratedSessionFixture.file: GeneratedSessionFixture#file.
  GeneratedSessionFixture.directory: GeneratedSessionFixture#directory.
  GeneratedSessionFixture.bytes: GeneratedSessionFixture#bytes.
  GeneratedSessionFixture.messageCount: GeneratedSessionFixture#messageCount.
  SocketHarness.close: SocketHarness#close().
  loadSessionFixture: loadSessionFixture().
  sessionFileArg: sessionFileArg().
  generatedSessionMiBArg: generatedSessionMiBArg().
  closeWriteStream: closeWriteStream().
  SocketHarness.server: SocketHarness#server.
  SocketHarness.receiverSockets: SocketHarness#receiverSockets.
  SocketHarness.socketPath: SocketHarness#socketPath.
---
# Module: [`packages/coding-agent/test/daemon-multiclient-bench.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts)

## Classes
### `BenchmarkResult`
- def: [`packages/coding-agent/test/daemon-multiclient-bench.ts:46`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L46)
- signature: `interface BenchmarkResult`
- members:
  - `clients` — [`L48`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L48)
  - `elapsedMs` — [`L49`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L49)
  - `externalDeltaMiB` — [`L53`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L53)
  - `heapDeltaMiB` — [`L51`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L51)
  - `peakRssDeltaMiB` — [`L54`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L54)
  - `rssDeltaMiB` — [`L52`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L52)
  - `scenario` — [`L47`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L47)
  - `throughputMiBPerSecond` — [`L50`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L50)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (9 test-only callers)

### `Counters`
- def: [`packages/coding-agent/test/daemon-multiclient-bench.ts:38`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L38)
- signature: `interface Counters`
- members:
  - `maxSerializationMs` — [`L41`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L41)
  - `serializationMs` — [`L40`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L40)
  - `serializations` — [`L39`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L39)
  - `writes` — [`L42`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L42)
  - `writtenBytes` — [`L43`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L43)
- used by: (7 test-only callers)

### `GeneratedSessionFixture`
- def: [`packages/coding-agent/test/daemon-multiclient-bench.ts:57`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L57)
- signature: `interface GeneratedSessionFixture`
- members:
  - `bytes` — [`L60`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L60)
  - `directory` — [`L59`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L59)
  - `file` — [`L58`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L58)
  - `messageCount` — [`L61`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L61)
- used by: (2 test-only callers)

### `Receiver`
- def: [`packages/coding-agent/test/daemon-multiclient-bench.ts:75`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L75)
- signature: `interface Receiver`
- members:
  - `setExpectedBytes(method)` — [`L77`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L77)
  - `done` — [`L76`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L76)
- used by: (3 test-only callers)

### `SessionLoadResult`
- def: [`packages/coding-agent/test/daemon-multiclient-bench.ts:64`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L64)
- signature: `interface SessionLoadResult`
- members:
  - `contextMs` — [`L67`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L67)
  - `externalDeltaMiB` — [`L71`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L71)
  - `fileBytes` — [`L65`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L65)
  - `heapDeltaMiB` — [`L69`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L69)
  - `loadMs` — [`L66`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L66)
  - `messageCount` — [`L68`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L68)
  - `peakRssDeltaMiB` — [`L72`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L72)
  - `rssDeltaMiB` — [`L70`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L70)
- used by: (4 test-only callers)

### `SocketHarness`
- def: [`packages/coding-agent/test/daemon-multiclient-bench.ts:80`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L80)
- signature: `interface SocketHarness`
- members:
  - `close(method)` — [`L86`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L86)
  - `receiverSockets` — [`L84`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L84)
  - `receivers` — [`L83`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L83)
  - `senders` — [`L82`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L82)
  - `server` — [`L81`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L81)
  - `socketPath` — [`L85`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L85)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (7 test-only callers)

## Functions
- `cleanup(method)` — [`L563`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L563)
- `closeWriteStream(stream: WritableStream)` — [`L701`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L701)
- `createAssistantMessage(text: string)` — [`L215`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L215)
- `createAttachResponse(clientIndex: number)` — [`L267`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L267)
- `createAttachResponseForMessages(messages: readonly AgentMessage[] | readonly object[], clientIndex: number)` — [`L271`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L271)
- `createReceiver(socket: Socket)` — [`L112`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L112)
- `createSocketHarness(clientCount: number)` — [`L158`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L158)
- `createStreamingEvent(text: string, delta: string, sequence: number)` — [`L235`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L235)
- `generateSessionFixture(sizeMiB: number)` — [`L708`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L708)
- `generatedSessionMiBArg(args: readonly string[])` — [`L671`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L671)
- `loadSessionFixture(sessionFile: string)` — [`L560`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L560)
- `main()` — [`L775`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L775)
- `memoryDeltaMiB(after: MemoryUsage, before: MemoryUsage, field: keyof MemoryUsage)` — [`L552`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L552)
- `printResults(results: BenchmarkResult[], details?: string)` — [`L618`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L618)
- `printSessionLoad(sessionFile: string, result: SessionLoadResult)` — [`L643`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L643)
- `removeSocketPath(socketPath: string)` — [`L99`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L99)
- `repeatedText(length: number, seed: string)` — [`L255`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L255)
- `runAttach(clientCount: number)` — [`L460`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L460)
- `runAttachV2(messages: readonly AgentMessage[], clientCount: number, scenario: "attach-v2" | "session-attach-v2")` — [`L469`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L469)
- `runFanout(clientCount: number)` — [`L406`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L406)
- `runFanoutV2(clientCount: number)` — [`L420`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L420)
- `runRealSessionBenchmark(sessionFile: string)` — [`L759`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L759)
- `runScenario(scenario: "attach" | "fanout" | "fanout-v2" | "attach-v2" | "session-attach" | "session-attach-v2", clientCount: number, work: (harness: SocketHarness, counters: Counters, expectedBytes: number[]) => void)` — [`L357`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L357)
- `runSessionAttach(messages: readonly AgentMessage[], clientCount: number)` — [`L540`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L540)
- `sessionFileArg(args: readonly string[])` — [`L659`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L659)
- `socketPathForRun()` — [`L91`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L91)
- `writeBufferToRecipient(socket: Socket, buffer: string | Buffer<ArrayBufferLike>, counters: Counters)` — [`L349`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L349)
- `writeStreamChunk(stream: WritableStream, chunk: string)` — [`L687`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L687)
- `writeToRecipient(socket: Socket, message: object, counters: Counters)` — [`L334`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L334)

## Module values
- `ATTACH_HISTORY_MESSAGES` — [`L34`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L34)
- `ATTACH_MESSAGE_CHARS` — [`L35`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L35)
- `CLIENT_COUNTS` — [`L30`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L30)
- `MEBIBYTE` — [`L36`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L36)
- `SESSION_CLIENT_COUNTS` — [`L31`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L31)
- `STREAM_CHARS` — [`L32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L32)
- `STREAM_CHUNK_CHARS` — [`L33`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L33)
- `attachMessages` — [`L260`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L260)
- `load` — [`L562`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L562)
- `messages` — [`L561`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L561)
- `socketCounter` — [`L89`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L89)
- `streamCorpus` — [`L259`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-multiclient-bench.ts#L259)


---
title: 'Module: packages/coding-agent/src/modes/session-worker/private-framing.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/session-worker/private-framing.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/session-worker/`private-framing.ts`/
symbols:
  PrivateFrame: PrivateFrame#
  PrivateFrameDecoder.push: PrivateFrameDecoder#push().
  encodePrivateFrame: encodePrivateFrame().
  PrivateFrame.header: PrivateFrame#header.
  PrivateFrame.payload: PrivateFrame#payload.
  PrivateFramedChannel.-constructor: PrivateFramedChannel#`<constructor>`().
  PrivateFrameDecoder.-constructor: PrivateFrameDecoder#`<constructor>`().
  PrivateFrameDecoder.buffered: PrivateFrameDecoder#buffered.
  PrivateFramedChannel.detach: PrivateFramedChannel#detach().
  DEFAULT_PRIVATE_FRAME_LIMITS: DEFAULT_PRIVATE_FRAME_LIMITS.
  PrivateFramedChannel.handleData: PrivateFramedChannel#handleData.
  PrivateFramedChannel.onFrame: PrivateFramedChannel#onFrame().
  PrivateFramedChannel.send: PrivateFramedChannel#send().
  PrivateFramedChannel.close: PrivateFramedChannel#close().
  PrivateFramedChannel.handleEnd: PrivateFramedChannel#handleEnd.
  PrivateFramedChannel.handleClose: PrivateFramedChannel#handleClose.
  PrivateFrameDecoder.finish: PrivateFrameDecoder#finish().
  PrivateFramedChannel.listeners: PrivateFramedChannel#listeners.
  FRAME_PREFIX_BYTES: FRAME_PREFIX_BYTES.
  PrivateFramedChannel.decoder: PrivateFramedChannel#decoder.
  PrivateFrameDecoder: PrivateFrameDecoder#
  PrivateFrameListener: PrivateFrameListener#
  PrivateFrameLimits: PrivateFrameLimits#
  PrivateFrameHeaderValidator: PrivateFrameHeaderValidator#
  assertFrameLength: assertFrameLength().
  PrivateFramedChannel.closed: PrivateFramedChannel#closed.
  PrivateFrameLimits.maxHeaderBytes: PrivateFrameLimits#maxHeaderBytes.
  PrivateFrameLimits.maxPayloadBytes: PrivateFrameLimits#maxPayloadBytes.
  PrivateFramedChannel: PrivateFramedChannel#
  PrivateFrameDecoder.-get-bufferedBytes: PrivateFrameDecoder#`<get>bufferedBytes`().
  isObjectHeader: isObjectHeader().
---
# Module: [`packages/coding-agent/src/modes/session-worker/private-framing.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts)

## Classes
### `PrivateFrame`
- def: [`packages/coding-agent/src/modes/session-worker/private-framing.ts:15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L15)
- signature: `interface PrivateFrame`
- members:
  - `header` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L16)
  - `payload` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L17)
- used by: [`daemon-supervisor.ts`](../daemon/daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`handleWorkerFrame`](../daemon/daemon-supervisor.ts.md#DaemonSupervisor.handleWorkerFrame), [`handleConnection`](../daemon/daemon-mode.ts.md#AgentDaemon.handleConnection), [`daemon-worker-client.ts`](../daemon/daemon-worker-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-worker-client.ts), [`push`](private-framing.ts.md#PrivateFrameDecoder.push), [`handleFrame`](../daemon/daemon-worker-client.ts.md#DaemonWorkerClient.handleFrame), [`DaemonWorkerFrameListener`](../daemon/daemon-worker-client.ts.md#DaemonWorkerFrameListener), [`PrivateFrameListener`](private-framing.ts.md#PrivateFrameListener)  (8 test-only)

### `PrivateFrameDecoder`
- def: [`packages/coding-agent/src/modes/session-worker/private-framing.ts:53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L53)
- signature: `class PrivateFrameDecoder`
- members:
  - `<constructor>(validateHeader: PrivateFrameHeaderValidator<THeader>, limits?: PrivateFrameLimits)` — [`L56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L56)
  - `<get>bufferedBytes` — [`L61`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L61)
  - `finish(method)` — [`L114`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L114)
  - `push(method)` — [`L65`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L65)
  - `buffered` — [`L54`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L54)
- uses (calls/refs, reference-scoped): [`PrivateFrame`](private-framing.ts.md#PrivateFrame), [`header`](private-framing.ts.md#PrivateFrame.header), [`payload`](private-framing.ts.md#PrivateFrame.payload), [`DEFAULT_PRIVATE_FRAME_LIMITS`](private-framing.ts.md#DEFAULT_PRIVATE_FRAME_LIMITS), [`FRAME_PREFIX_BYTES`](private-framing.ts.md#FRAME_PREFIX_BYTES), [`PrivateFrameHeaderValidator`](private-framing.ts.md#PrivateFrameHeaderValidator), [`PrivateFrameLimits`](private-framing.ts.md#PrivateFrameLimits), [`assertFrameLength`](private-framing.ts.md#assertFrameLength), [`maxHeaderBytes`](private-framing.ts.md#PrivateFrameLimits.maxHeaderBytes), [`maxPayloadBytes`](private-framing.ts.md#PrivateFrameLimits.maxPayloadBytes), [`isObjectHeader`](private-framing.ts.md#isObjectHeader)
- used by: [`daemon-mode.ts`](../daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`handleConnection`](../daemon/daemon-mode.ts.md#AgentDaemon.handleConnection), [`<constructor>`](private-framing.ts.md#PrivateFramedChannel.-constructor), [`handleData`](private-framing.ts.md#PrivateFramedChannel.handleData), [`handleEnd`](private-framing.ts.md#PrivateFramedChannel.handleEnd), [`decoder`](private-framing.ts.md#PrivateFramedChannel.decoder)  (4 test-only)

### `PrivateFrameHeaderValidator`
- def: [`packages/coding-agent/src/modes/session-worker/private-framing.ts:20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L20)
- signature: `type PrivateFrameHeaderValidator`
- used by: [`<constructor>`](private-framing.ts.md#PrivateFramedChannel.-constructor), [`<constructor>`](private-framing.ts.md#PrivateFrameDecoder.-constructor)  (1 test-only)

### `PrivateFrameLimits`
- def: [`packages/coding-agent/src/modes/session-worker/private-framing.ts:5`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L5)
- signature: `interface PrivateFrameLimits`
- members:
  - `maxHeaderBytes` — [`L6`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L6)
  - `maxPayloadBytes` — [`L7`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L7)
- used by: [`push`](private-framing.ts.md#PrivateFrameDecoder.push), [`encodePrivateFrame`](private-framing.ts.md#encodePrivateFrame), [`<constructor>`](private-framing.ts.md#PrivateFramedChannel.-constructor), [`<constructor>`](private-framing.ts.md#PrivateFrameDecoder.-constructor), [`DEFAULT_PRIVATE_FRAME_LIMITS`](private-framing.ts.md#DEFAULT_PRIVATE_FRAME_LIMITS)

### `PrivateFrameListener`
- def: [`packages/coding-agent/src/modes/session-worker/private-framing.ts:121`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L121)
- signature: `type PrivateFrameListener`
- uses (calls/refs, reference-scoped): [`PrivateFrame`](private-framing.ts.md#PrivateFrame)
- used by: [`onFrame`](private-framing.ts.md#PrivateFramedChannel.onFrame), [`listeners`](private-framing.ts.md#PrivateFramedChannel.listeners)

### `PrivateFramedChannel`
- def: [`packages/coding-agent/src/modes/session-worker/private-framing.ts:123`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L123)
- signature: `class PrivateFramedChannel`
- members:
  - `<constructor>(stream: Duplex, validateHeader: PrivateFrameHeaderValidator<THeader>, limits?: PrivateFrameLimits)` — [`L128`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L128)
  - `close(method)` — [`L160`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L160)
  - `detach(method)` — [`L194`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L194)
  - `onFrame(method)` — [`L139`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L139)
  - `send(method)` — [`L144`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L144)
  - `closed` — [`L126`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L126)
  - `decoder` — [`L124`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L124)
  - `handleClose` — [`L189`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L189)
  - `handleData` — [`L169`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L169)
  - `handleEnd` — [`L181`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L181)
  - `listeners` — [`L125`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L125)
- uses (calls/refs, reference-scoped): [`push`](private-framing.ts.md#PrivateFrameDecoder.push), [`encodePrivateFrame`](private-framing.ts.md#encodePrivateFrame), [`<constructor>`](private-framing.ts.md#PrivateFrameDecoder.-constructor), [`DEFAULT_PRIVATE_FRAME_LIMITS`](private-framing.ts.md#DEFAULT_PRIVATE_FRAME_LIMITS), [`finish`](private-framing.ts.md#PrivateFrameDecoder.finish), [`PrivateFrameDecoder`](private-framing.ts.md#PrivateFrameDecoder), [`PrivateFrameListener`](private-framing.ts.md#PrivateFrameListener), [`PrivateFrameHeaderValidator`](private-framing.ts.md#PrivateFrameHeaderValidator), [`PrivateFrameLimits`](private-framing.ts.md#PrivateFrameLimits)
- used by: [`daemon-worker-client.ts`](../daemon/daemon-worker-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-worker-client.ts), [`requestWire`](../daemon/daemon-worker-client.ts.md#DaemonWorkerClient.requestWire), [`close`](../daemon/daemon-worker-client.ts.md#DaemonWorkerClient.close), [`connect`](../daemon/daemon-worker-client.ts.md#DaemonWorkerClient.connect), [`channel`](../daemon/daemon-worker-client.ts.md#DaemonWorkerClient.channel)  (1 test-only)

## Functions
- `assertFrameLength(name: string, value: number, maximum: number)` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L22)
- `encodePrivateFrame(header: THeader, payload?: Uint8Array<ArrayBufferLike>, limits?: PrivateFrameLimits)` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L32)
- `isObjectHeader(value: unknown)` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L28)

## Module values
- `DEFAULT_PRIVATE_FRAME_LIMITS` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L10)
- `FRAME_PREFIX_BYTES` — [`L3`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/session-worker/private-framing.ts#L3)


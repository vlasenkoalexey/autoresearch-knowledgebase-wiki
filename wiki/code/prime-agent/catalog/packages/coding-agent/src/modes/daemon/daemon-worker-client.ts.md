---
title: 'Module: packages/coding-agent/src/modes/daemon/daemon-worker-client.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/daemon-worker-client.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`daemon-worker-client.ts`/
symbols:
  DaemonWorkerClient.handleFrame: DaemonWorkerClient#handleFrame().
  DaemonWorkerClient.requestWire: DaemonWorkerClient#requestWire().
  DaemonWorkerClient.close: DaemonWorkerClient#close().
  DaemonWorkerClient.connect: DaemonWorkerClient#connect().
  DaemonWorkerClient.requestWorker: DaemonWorkerClient#requestWorker().
  DaemonWorkerClient.request: DaemonWorkerClient#request().
  DaemonWorkerClient.channel: DaemonWorkerClient#channel.
  DaemonWorkerClient.notifyClosed: DaemonWorkerClient#notifyClosed().
  DaemonWorkerClient.pending: DaemonWorkerClient#pending.
  DaemonWorkerClient.waitForHello: DaemonWorkerClient#waitForHello().
  DaemonWorkerClient.socket: DaemonWorkerClient#socket.
  DaemonWorkerClient.helloWaiters: DaemonWorkerClient#helloWaiters.
  DaemonWorkerClient: DaemonWorkerClient#
  DaemonCommandBody: DaemonCommandBody#
  DaemonWorkerFrameListener: DaemonWorkerFrameListener#
  DaemonWorkerClient.rejectAll: DaemonWorkerClient#rejectAll().
  DaemonWorkerWireCommandBody: DaemonWorkerWireCommandBody#
  DaemonWorkerWireCommand: DaemonWorkerWireCommand#
  DaemonWorkerClient.onFrame: DaemonWorkerClient#onFrame().
  DaemonWorkerClient.onClose: DaemonWorkerClient#onClose().
  DaemonWorkerClient.authenticateWorker: DaemonWorkerClient#authenticateWorker().
  DaemonHello: DaemonHello#
  DaemonWorkerClient.frameListeners: DaemonWorkerClient#frameListeners.
  DaemonWorkerClient.closeListeners: DaemonWorkerClient#closeListeners.
  DaemonWorkerClient.hello: DaemonWorkerClient#hello.
  DaemonWorkerAuthentication: DaemonWorkerAuthentication#
  isDaemonResponse: isDaemonResponse().
  DaemonWorkerCloseListener: DaemonWorkerCloseListener#
  DistributiveOmit: DistributiveOmit#
  DaemonWorkerClient.requestId: DaemonWorkerClient#requestId.
  DaemonWorkerClient.-constructor: DaemonWorkerClient#`<constructor>`().
  DaemonWorkerAuthentication.Omit.Extract.typeLiteral0.type: DaemonWorkerAuthentication#Omit:Extract:typeLiteral0:type.
  DaemonHello.Extract.typeLiteral5.type: DaemonHello#Extract:typeLiteral5:type.
---
# Module: [`packages/coding-agent/src/modes/daemon/daemon-worker-client.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts)

## Classes
### `DaemonCommandBody`
- def: [`packages/coding-agent/src/modes/daemon/daemon-worker-client.ts:13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L13)
- signature: `type DaemonCommandBody`
- uses (calls/refs, reference-scoped): [`DaemonCommand`](daemon-protocol.ts.md#DaemonCommand), [`DistributiveOmit`](daemon-worker-client.ts.md#DistributiveOmit)
- used by: [`request`](daemon-worker-client.ts.md#DaemonWorkerClient.request), [`DaemonWorkerWireCommandBody`](daemon-worker-client.ts.md#DaemonWorkerWireCommandBody)

### `DaemonHello`
- def: [`packages/coding-agent/src/modes/daemon/daemon-worker-client.ts:20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L20)
- signature: `type DaemonHello`
- members:
  - `type` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L20)
- uses (calls/refs, reference-scoped): [`DaemonOutbound`](daemon-protocol.ts.md#DaemonOutbound)
- used by: [`waitForHello`](daemon-worker-client.ts.md#DaemonWorkerClient.waitForHello), [`helloWaiters`](daemon-worker-client.ts.md#DaemonWorkerClient.helloWaiters), [`hello`](daemon-worker-client.ts.md#DaemonWorkerClient.hello)

### `DaemonWorkerAuthentication`
- def: [`packages/coding-agent/src/modes/daemon/daemon-worker-client.ts:16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L16)
- signature: `type DaemonWorkerAuthentication`
- members:
  - `type` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L16)
- uses (calls/refs, reference-scoped): [`DaemonWorkerCommand`](daemon-worker-protocol.ts.md#DaemonWorkerCommand)
- used by: [`authenticateWorker`](daemon-worker-client.ts.md#DaemonWorkerClient.authenticateWorker)

### `DaemonWorkerClient`
- def: [`packages/coding-agent/src/modes/daemon/daemon-worker-client.ts:22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L22)
- signature: `class DaemonWorkerClient`
- members:
  - `<constructor>(socketPath: string)` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L43)
  - `authenticateWorker(method)` — [`L119`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L119)
  - `close(method)` — [`L126`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L126)
  - `connect(method)` — [`L45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L45)
  - `handleFrame(method)` — [`L163`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L163)
  - `notifyClosed(method)` — [`L220`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L220)
  - `onClose(method)` — [`L106`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L106)
  - `onFrame(method)` — [`L101`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L101)
  - `rejectAll(method)` — [`L207`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L207)
  - `request(method)` — [`L111`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L111)
  - `requestWire(method)` — [`L134`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L134)
  - `requestWorker(method)` — [`L115`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L115)
  - `waitForHello(method)` — [`L81`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L81)
  - `channel` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L24)
  - `closeListeners` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L26)
  - `frameListeners` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L25)
  - `hello` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L36)
  - `helloWaiters` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L37)
  - `pending` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L27)
  - `requestId` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L35)
  - `socket` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L23)
- uses (calls/refs, reference-scoped): [`DaemonOutbound`](daemon-protocol.ts.md#DaemonOutbound), [`DaemonResponse`](daemon-protocol.ts.md#DaemonResponse), [`DaemonWorkerFrameHeader`](daemon-worker-protocol.ts.md#DaemonWorkerFrameHeader), [`serializeJsonLine`](../rpc/jsonl.ts.md#serializeJsonLine), [`PrivateFrame`](../session-worker/private-framing.ts.md#PrivateFrame), [`<constructor>`](../session-worker/private-framing.ts.md#PrivateFramedChannel.-constructor), [`header`](../session-worker/private-framing.ts.md#PrivateFrame.header), [`payload`](../session-worker/private-framing.ts.md#PrivateFrame.payload), [`isDaemonWorkerFrameHeader`](daemon-worker-protocol.ts.md#isDaemonWorkerFrameHeader), [`DaemonWorkerCommandBody`](daemon-worker-protocol.ts.md#DaemonWorkerCommandBody), [`DaemonCommandBody`](daemon-worker-client.ts.md#DaemonCommandBody), [`DaemonWorkerFrameListener`](daemon-worker-client.ts.md#DaemonWorkerFrameListener), [`close`](../session-worker/private-framing.ts.md#PrivateFramedChannel.close), [`onFrame`](../session-worker/private-framing.ts.md#PrivateFramedChannel.onFrame), [`send`](../session-worker/private-framing.ts.md#PrivateFramedChannel.send), [`DaemonWorkerWireCommand`](daemon-worker-client.ts.md#DaemonWorkerWireCommand), [`DaemonWorkerWireCommandBody`](daemon-worker-client.ts.md#DaemonWorkerWireCommandBody), [`DaemonHello`](daemon-worker-client.ts.md#DaemonHello), [`DaemonWorkerAuthentication`](daemon-worker-client.ts.md#DaemonWorkerAuthentication), [`isDaemonResponse`](daemon-worker-client.ts.md#isDaemonResponse), [`PrivateFramedChannel`](../session-worker/private-framing.ts.md#PrivateFramedChannel), [`DaemonWorkerCloseListener`](daemon-worker-client.ts.md#DaemonWorkerCloseListener)
- used by: [`daemon-supervisor.ts`](daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`handleCommand`](daemon-supervisor.ts.md#DaemonSupervisor.handleCommand), [`launchWorker`](daemon-supervisor.ts.md#DaemonSupervisor.launchWorker), [`type`](daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type), [`stopWorkerUntracked`](daemon-supervisor.ts.md#DaemonSupervisor.stopWorkerUntracked), [`shutdown`](daemon-supervisor.ts.md#DaemonSupervisor.shutdown), [`cleanupSupervisorResourcesOnce`](daemon-supervisor.ts.md#DaemonSupervisor.cleanupSupervisorResourcesOnce), [`refreshWorkerSummaries`](daemon-supervisor.ts.md#DaemonSupervisor.refreshWorkerSummaries), [`recoverWorker`](daemon-supervisor.ts.md#DaemonSupervisor.recoverWorker), [`runIdleEvictionSweep`](daemon-supervisor.ts.md#DaemonSupervisor.runIdleEvictionSweep), [`prepareUpdateRestartFenced`](daemon-supervisor.ts.md#DaemonSupervisor.prepareUpdateRestartFenced), [`handleWorkerClose`](daemon-supervisor.ts.md#DaemonSupervisor.handleWorkerClose), [`connectWorker`](daemon-supervisor.ts.md#DaemonSupervisor.connectWorker), [`forwardToWorker`](daemon-supervisor.ts.md#DaemonSupervisor.forwardToWorker), [`client`](daemon-supervisor.ts.md#ResidentWorker.client), [`failWorkerSnapshotCache`](daemon-supervisor.ts.md#DaemonSupervisor.failWorkerSnapshotCache), [`syncAgentPeers`](daemon-supervisor.ts.md#DaemonSupervisor.syncAgentPeers), [`requireAvailableWorkerClient`](daemon-supervisor.ts.md#DaemonSupervisor.requireAvailableWorkerClient), [`subscribeWorker`](daemon-supervisor.ts.md#DaemonSupervisor.subscribeWorker), [`updateRestartPrepareClient`](daemon-supervisor.ts.md#ResidentWorker.updateRestartPrepareClient)

### `DaemonWorkerCloseListener`
- def: [`packages/coding-agent/src/modes/daemon/daemon-worker-client.ts:19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L19)
- signature: `type DaemonWorkerCloseListener`
- used by: [`onClose`](daemon-worker-client.ts.md#DaemonWorkerClient.onClose), [`closeListeners`](daemon-worker-client.ts.md#DaemonWorkerClient.closeListeners)

### `DaemonWorkerFrameListener`
- def: [`packages/coding-agent/src/modes/daemon/daemon-worker-client.ts:18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L18)
- signature: `type DaemonWorkerFrameListener`
- uses (calls/refs, reference-scoped): [`DaemonWorkerFrameHeader`](daemon-worker-protocol.ts.md#DaemonWorkerFrameHeader), [`PrivateFrame`](../session-worker/private-framing.ts.md#PrivateFrame)
- used by: [`onFrame`](daemon-worker-client.ts.md#DaemonWorkerClient.onFrame), [`frameListeners`](daemon-worker-client.ts.md#DaemonWorkerClient.frameListeners)

### `DaemonWorkerWireCommand`
- def: [`packages/coding-agent/src/modes/daemon/daemon-worker-client.ts:15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L15)
- signature: `type DaemonWorkerWireCommand`
- uses (calls/refs, reference-scoped): [`DaemonCommand`](daemon-protocol.ts.md#DaemonCommand), [`DaemonWorkerCommand`](daemon-worker-protocol.ts.md#DaemonWorkerCommand)
- used by: [`requestWire`](daemon-worker-client.ts.md#DaemonWorkerClient.requestWire)

### `DaemonWorkerWireCommandBody`
- def: [`packages/coding-agent/src/modes/daemon/daemon-worker-client.ts:14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L14)
- signature: `type DaemonWorkerWireCommandBody`
- uses (calls/refs, reference-scoped): [`DaemonWorkerCommandBody`](daemon-worker-protocol.ts.md#DaemonWorkerCommandBody), [`DaemonCommandBody`](daemon-worker-client.ts.md#DaemonCommandBody)
- used by: [`requestWire`](daemon-worker-client.ts.md#DaemonWorkerClient.requestWire)

### `DistributiveOmit`
- def: [`packages/coding-agent/src/modes/daemon/daemon-worker-client.ts:12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L12)
- signature: `type DistributiveOmit`
- used by: [`DaemonCommandBody`](daemon-worker-client.ts.md#DaemonCommandBody)

## Functions
- `isDaemonResponse(value: unknown)` — [`L233`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-worker-client.ts#L233)


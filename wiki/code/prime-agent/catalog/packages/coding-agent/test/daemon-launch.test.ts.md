---
title: 'Module: packages/coding-agent/test/daemon-launch.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/daemon-launch.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`daemon-launch.test.ts`/
symbols:
  startFakeDaemon: startFakeDaemon().
  FakeDaemon.socketPath: FakeDaemon#socketPath.
  startCrashingDaemon: startCrashingDaemon().
  FakeDaemon.close: FakeDaemon#close.
  send: send().
  FakeDaemon: FakeDaemon#
  FakeDaemonOptions: FakeDaemonOptions#
  FakeDaemonOptions.sessions: FakeDaemonOptions#sessions.
  FakeDaemonOptions.busyClientOwnedSessionCount: FakeDaemonOptions#busyClientOwnedSessionCount.
  FakeDaemonOptions.failList: FakeDaemonOptions#failList.
  FakeDaemonOptions.respondToShutdown: FakeDaemonOptions#respondToShutdown.
  FakeDaemonOptions.protocolVersion: FakeDaemonOptions#protocolVersion.
  FakeDaemonOptions.appVersion: FakeDaemonOptions#appVersion.
  FakeDaemonOptions.schemaId: FakeDaemonOptions#schemaId.
  FakeDaemonOptions.serverCapabilities: FakeDaemonOptions#serverCapabilities.
  FakeDaemonOptions.onCommand: FakeDaemonOptions#onCommand.
---
# Module: [`packages/coding-agent/test/daemon-launch.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts)

## Classes
### `FakeDaemon`
- def: [`packages/coding-agent/test/daemon-launch.test.ts:32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L32)
- signature: `interface FakeDaemon`
- members:
  - `close` — [`L34`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L34)
  - `socketPath` — [`L33`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L33)
- used by: (3 test-only callers)

### `FakeDaemonOptions`
- def: [`packages/coding-agent/test/daemon-launch.test.ts:17`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L17)
- signature: `interface FakeDaemonOptions`
- members:
  - `appVersion` — [`L26`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L26)
  - `busyClientOwnedSessionCount` — [`L20`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L20)
  - `failList` — [`L22`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L22) — When true, the `list` command responds with a failure.
  - `onCommand` — [`L29`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L29)
  - `protocolVersion` — [`L25`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L25)
  - `respondToShutdown` — [`L24`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L24) — When false, the server ignores `shutdown` and stays up.
  - `schemaId` — [`L27`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L27)
  - `serverCapabilities` — [`L28`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L28)
  - `sessions` — [`L19`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L19) — Sessions returned for a `list` command.
- used by: (1 test-only callers)

## Functions
- `send(socket: Socket, message: unknown)` — [`L37`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L37)
- `startCrashingDaemon()` — [`L110`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L110)
- `startFakeDaemon(options?: FakeDaemonOptions)` — [`L41`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-launch.test.ts#L41)


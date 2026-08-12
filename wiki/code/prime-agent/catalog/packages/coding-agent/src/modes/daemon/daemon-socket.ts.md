---
title: 'Module: packages/coding-agent/src/modes/daemon/daemon-socket.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/daemon-socket.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`daemon-socket.ts`/
symbols:
  prepareDaemonSocketPath: prepareDaemonSocketPath().
  defaultDaemonSocketPath: defaultDaemonSocketPath().
  prepareUnixDaemonSocketPath: prepareUnixDaemonSocketPath().
  cleanupDaemonSocketPath: cleanupDaemonSocketPath().
  defaultDaemonSocketDir: defaultDaemonSocketDir().
  acquireDaemonSocketPathLease: acquireDaemonSocketPathLease().
  cleanupUnixDaemonSocketPath: cleanupUnixDaemonSocketPath().
  getDaemonSocketIdentity: getDaemonSocketIdentity().
  DaemonSocketIdentity: DaemonSocketIdentity#
  ensureDefaultDaemonSocketDir: ensureDefaultDaemonSocketDir().
  restrictDaemonSocketPath: restrictDaemonSocketPath().
  DaemonSocketPathLease: DaemonSocketPathLease#
  DaemonSocketPathLease.release: DaemonSocketPathLease#release().
  DaemonSocketIdentity.dev: DaemonSocketIdentity#dev.
  DaemonSocketIdentity.ino: DaemonSocketIdentity#ino.
  assertSocketLease: assertSocketLease().
  DAEMON_SOCKET_RELEASE_POLL_MS: DAEMON_SOCKET_RELEASE_POLL_MS.
  canConnectToUnixSocket: canConnectToUnixSocket().
  DAEMON_SOCKET_DIR_MODE: DAEMON_SOCKET_DIR_MODE.
  DAEMON_SOCKET_LOCK_STALE_MS: DAEMON_SOCKET_LOCK_STALE_MS.
  DAEMON_SOCKET_LOCK_UPDATE_MS: DAEMON_SOCKET_LOCK_UPDATE_MS.
  DaemonSocketPathLease.released: DaemonSocketPathLease#released.
  DAEMON_SOCKET_MODE: DAEMON_SOCKET_MODE.
  DAEMON_SOCKET_RELEASE_GRACE_MS: DAEMON_SOCKET_RELEASE_GRACE_MS.
  DaemonSocketPathLease.-constructor: DaemonSocketPathLease#`<constructor>`().
  delay: delay().
---
# Module: [`packages/coding-agent/src/modes/daemon/daemon-socket.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts)

## Classes
### `DaemonSocketIdentity`
- def: [`packages/coding-agent/src/modes/daemon/daemon-socket.ts:31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L31)
- signature: `interface DaemonSocketIdentity`
- members:
  - `dev` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L32)
  - `ino` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L33)
- used by: [`daemon-mode.ts`](daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`daemon-supervisor.ts`](daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`cleanupDaemonSocketPath`](daemon-socket.ts.md#cleanupDaemonSocketPath), [`prepareUnixDaemonSocketPath`](daemon-socket.ts.md#prepareUnixDaemonSocketPath), [`cleanupUnixDaemonSocketPath`](daemon-socket.ts.md#cleanupUnixDaemonSocketPath), [`getDaemonSocketIdentity`](daemon-socket.ts.md#getDaemonSocketIdentity), [`socketIdentity`](daemon-supervisor.ts.md#DaemonSupervisor.socketIdentity), [`socketIdentity`](daemon-mode.ts.md#AgentDaemon.socketIdentity)

### `DaemonSocketPathLease`
- def: [`packages/coding-agent/src/modes/daemon/daemon-socket.ts:14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L14)
- signature: `class DaemonSocketPathLease`
- members:
  - `<constructor>(socketPath: string, releaseLock: () => Promise<void>)` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L17)
  - `release(method)` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L22)
  - `released` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L15)
- used by: [`daemon-supervisor.ts`](daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`shutdown`](daemon-supervisor.ts.md#DaemonSupervisor.shutdown), [`cleanupSupervisorResourcesOnce`](daemon-supervisor.ts.md#DaemonSupervisor.cleanupSupervisorResourcesOnce), [`prepareDaemonSocketPath`](daemon-socket.ts.md#prepareDaemonSocketPath), [`cleanupDaemonSocketPath`](daemon-socket.ts.md#cleanupDaemonSocketPath), [`acquireDaemonSocketPathLease`](daemon-socket.ts.md#acquireDaemonSocketPathLease), [`socketLease`](daemon-supervisor.ts.md#DaemonSupervisor.socketLease), [`assertSocketLease`](daemon-socket.ts.md#assertSocketLease)

## Functions
- `acquireDaemonSocketPathLease(socketPath: string)` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L43)
- `assertSocketLease(socketPath: string, lease: DaemonSocketPathLease)` — [`L208`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L208)
- `canConnectToUnixSocket(socketPath: string)` — [`L240`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L240)
- `cleanupDaemonSocketPath(socketPath: string, expectedIdentity?: DaemonSocketIdentity | undefined, lease?: DaemonSocketPathLease | undefined)` — [`L150`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L150)
- `cleanupUnixDaemonSocketPath(socketPath: string, expectedIdentity?: DaemonSocketIdentity | undefined)` — [`L191`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L191)
- `defaultDaemonSocketDir()` — [`L214`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L214)
- `defaultDaemonSocketPath()` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L36)
- `delay(ms: number)` — [`L265`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L265)
- `ensureDefaultDaemonSocketDir(socketPath: string)` — [`L219`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L219)
- `getDaemonSocketIdentity(socketPath: string)` — [`L142`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L142)
- `prepareDaemonSocketPath(socketPath: string, lease?: DaemonSocketPathLease | undefined)` — [`L62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L62)
- `prepareUnixDaemonSocketPath(socketPath: string)` — [`L87`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L87)
- `restrictDaemonSocketPath(socketPath: string)` — [`L135`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L135)

## Module values
- `DAEMON_SOCKET_DIR_MODE` — [`L8`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L8)
- `DAEMON_SOCKET_LOCK_STALE_MS` — [`L11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L11)
- `DAEMON_SOCKET_LOCK_UPDATE_MS` — [`L12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L12)
- `DAEMON_SOCKET_MODE` — [`L7`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L7)
- `DAEMON_SOCKET_RELEASE_GRACE_MS` — [`L9`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L9)
- `DAEMON_SOCKET_RELEASE_POLL_MS` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-socket.ts#L10)


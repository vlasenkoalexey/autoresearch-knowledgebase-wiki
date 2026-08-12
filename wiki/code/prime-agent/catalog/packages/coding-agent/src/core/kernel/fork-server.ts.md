---
title: 'Module: packages/coding-agent/src/core/kernel/fork-server.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/kernel/fork-server.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/kernel/`fork-server.ts`/
symbols:
  ForkServer.start: ForkServer#start().
  ForkServer.spawnKernel: ForkServer#spawnKernel().
  forkKernel: forkKernel().
  ForkServer.onData: ForkServer#onData().
  ForkServer.dispose: ForkServer#dispose().
  ForkServer.ensureReady: ForkServer#ensureReady().
  ForkServer.rejectPending: ForkServer#rejectPending().
  ForkServerUnavailable.-constructor: ForkServerUnavailable#`<constructor>`().
  ForkServer.needsStartupEnvNotInTemplate: ForkServer#needsStartupEnvNotInTemplate().
  isForkServerEnabled: isForkServerEnabled().
  ForkServer.markDead: ForkServer#markDead().
  ForkServerUnavailable: ForkServerUnavailable#
  ForkServer.pending: ForkServer#pending.
  ForkServer.-constructor: ForkServer#`<constructor>`().
  servers: servers.
  registerForkServerCleanupOnce: registerForkServerCleanupOnce().
  disposeAllForkServers: disposeAllForkServers().
  ForkServer.buffer: ForkServer#buffer.
  keyFor: keyFor().
  SpawnParams.connectionPath: SpawnParams#connectionPath.
  SpawnParams.env: SpawnParams#env.
  ForkServer.socketDir: ForkServer#socketDir.
  ForkServer.dead: ForkServer#dead.
  ForkServer.params: ForkServer#params.
  ForkServer.-get-isDead: ForkServer#`<get>isDead`().
  ForkServer.withStderr: ForkServer#withStderr().
  ForkServerParams.python: ForkServerParams#python.
  ForkServer.conn: ForkServer#conn.
  affectsInterpreterStartup: affectsInterpreterStartup().
  ForkServerParams: ForkServerParams#
  SpawnParams: SpawnParams#
  PendingSpawn.typeLiteral0.reject: PendingSpawn#typeLiteral0:reject.
  PendingSpawn.typeLiteral0.timer: PendingSpawn#typeLiteral0:timer.
  ForkServer.launchEnv: ForkServer#launchEnv.
  ForkServer.readyPromise: ForkServer#readyPromise.
  ForkServer.stderrTail: ForkServer#stderrTail.
  READY_TIMEOUT_MS: READY_TIMEOUT_MS.
  SPAWN_TIMEOUT_MS: SPAWN_TIMEOUT_MS.
  SpawnParams.cwd: SpawnParams#cwd.
  PendingSpawn.typeLiteral0.resolve: PendingSpawn#typeLiteral0:resolve.
  ForkServer.proc: ForkServer#proc.
  ForkServer.server: ForkServer#server.
  ForkServer.failReady: ForkServer#failReady.
  ForkServer.abandoned: ForkServer#abandoned.
  ForkServer.onReady: ForkServer#onReady.
  cleanupRegistered: cleanupRegistered.
  STDERR_TAIL_MAX: STDERR_TAIL_MAX.
  INTERPRETER_STARTUP_ENV_EXACT: INTERPRETER_STARTUP_ENV_EXACT.
  PendingSpawn: PendingSpawn#
  ForkServer: ForkServer#
  ForkServer.nextId: ForkServer#nextId.
---
# Module: [`packages/coding-agent/src/core/kernel/fork-server.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts)

## Classes
### `ForkServer`
- def: [`packages/coding-agent/src/core/kernel/fork-server.ts:70`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L70)
- signature: `class ForkServer`
- members:
  - `<constructor>(params: ForkServerParams)` — [`L93`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L93)
  - `<get>isDead` — [`L100`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L100)
  - `dispose(method)` — [`L269`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L269)
  - `ensureReady(method)` — [`L114`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L114)
  - `markDead(method)` — [`L265`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L265)
  - `needsStartupEnvNotInTemplate(method)` — [`L109`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L109) — True if `env` overrides an interpreter-startup var to a value the template
  - `onData(method)` — [`L191`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L191)
  - `rejectPending(method)` — [`L256`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L256) — Reject any in-flight ensureReady/spawnKernel callers so none wait out a timeout.
  - `spawnKernel(method)` — [`L231`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L231)
  - `start(method)` — [`L125`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L125)
  - `withStderr(method)` — [`L250`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L250)
  - `abandoned` — [`L90`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L90)
  - `buffer` — [`L83`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L83)
  - `conn` — [`L79`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L79)
  - `dead` — [`L91`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L91)
  - `failReady` — [`L82`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L82)
  - `launchEnv` — [`L76`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L76)
  - `nextId` — [`L87`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L87)
  - `onReady` — [`L189`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L189)
  - `params` — [`L71`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L71)
  - `pending` — [`L88`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L88)
  - `proc` — [`L77`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L77)
  - `readyPromise` — [`L81`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L81)
  - `server` — [`L78`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L78)
  - `socketDir` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L80)
  - `stderrTail` — [`L86`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L86)
- uses (calls/refs, reference-scoped): [`<constructor>`](fork-server.ts.md#ForkServerUnavailable.-constructor), [`ForkServerUnavailable`](fork-server.ts.md#ForkServerUnavailable), [`connectionPath`](fork-server.ts.md#SpawnParams.connectionPath), [`env`](fork-server.ts.md#SpawnParams.env), [`python`](fork-server.ts.md#ForkServerParams.python), [`affectsInterpreterStartup`](fork-server.ts.md#affectsInterpreterStartup), [`ForkServerParams`](fork-server.ts.md#ForkServerParams), [`SpawnParams`](fork-server.ts.md#SpawnParams), [`reject`](fork-server.ts.md#PendingSpawn.typeLiteral0.reject), [`timer`](fork-server.ts.md#PendingSpawn.typeLiteral0.timer), [`FORK_SERVER_SCRIPT`](fork-server-script.ts.md#FORK_SERVER_SCRIPT), [`READY_TIMEOUT_MS`](fork-server.ts.md#READY_TIMEOUT_MS), [`SPAWN_TIMEOUT_MS`](fork-server.ts.md#SPAWN_TIMEOUT_MS), [`cwd`](fork-server.ts.md#SpawnParams.cwd), [`resolve`](fork-server.ts.md#PendingSpawn.typeLiteral0.resolve), [`PendingSpawn`](fork-server.ts.md#PendingSpawn), [`STDERR_TAIL_MAX`](fork-server.ts.md#STDERR_TAIL_MAX)
- used by: [`forkKernel`](fork-server.ts.md#forkKernel), [`servers`](fork-server.ts.md#servers), [`disposeAllForkServers`](fork-server.ts.md#disposeAllForkServers)

### `ForkServerParams`
- def: [`packages/coding-agent/src/core/kernel/fork-server.ts:52`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L52)
- signature: `interface ForkServerParams`
- members:
  - `python` — [`L53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L53)
- used by: [`start`](fork-server.ts.md#ForkServer.start), [`forkKernel`](fork-server.ts.md#forkKernel), [`<constructor>`](fork-server.ts.md#ForkServer.-constructor), [`keyFor`](fork-server.ts.md#keyFor), [`params`](fork-server.ts.md#ForkServer.params)

### `ForkServerUnavailable`  ·  implements/extends Error
- def: [`packages/coding-agent/src/core/kernel/fork-server.ts:35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L35)
- signature: `class ForkServerUnavailable`
- members:
  - `<constructor>(message: string)` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L36)
- used by: [`doStart`](index.ts.md#KernelManager.doStart), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-kernel-index.ts), [`start`](fork-server.ts.md#ForkServer.start), [`forkKernel`](fork-server.ts.md#forkKernel), [`spawnKernel`](fork-server.ts.md#ForkServer.spawnKernel), [`onData`](fork-server.ts.md#ForkServer.onData), [`ensureReady`](fork-server.ts.md#ForkServer.ensureReady), [`rejectPending`](fork-server.ts.md#ForkServer.rejectPending)  (1 test-only)

### `PendingSpawn`
- def: [`packages/coding-agent/src/core/kernel/fork-server.ts:64`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L64)
- signature: `type PendingSpawn`
- members:
  - `reject` — [`L66`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L66)
  - `resolve` — [`L65`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L65)
  - `timer` — [`L67`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L67)
- used by: [`spawnKernel`](fork-server.ts.md#ForkServer.spawnKernel), [`onData`](fork-server.ts.md#ForkServer.onData), [`rejectPending`](fork-server.ts.md#ForkServer.rejectPending), [`pending`](fork-server.ts.md#ForkServer.pending)

### `SpawnParams`
- def: [`packages/coding-agent/src/core/kernel/fork-server.ts:56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L56)
- signature: `interface SpawnParams`
- members:
  - `connectionPath` — [`L57`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L57)
  - `cwd` — [`L58`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L58)
  - `env` — [`L61`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L61)
- used by: [`doStart`](index.ts.md#KernelManager.doStart), [`forkKernel`](fork-server.ts.md#forkKernel), [`spawnKernel`](fork-server.ts.md#ForkServer.spawnKernel), [`needsStartupEnvNotInTemplate`](fork-server.ts.md#ForkServer.needsStartupEnvNotInTemplate)  (1 test-only)

## Functions
- `affectsInterpreterStartup(key: string)` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L31)
- `disposeAllForkServers()` — [`L360`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L360)
- `forkKernel(python: string, spawn: SpawnParams)` — [`L335`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L335) — Fork a kernel onto `spawn.connectionPath` from the shared template for this — documented in [packages-coding-agent-src-core-kernel-index.ts](../../../../../../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
- `isForkServerEnabled()` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L44)
- `keyFor(params: ForkServerParams)` — [`L308`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L308)
- `registerForkServerCleanupOnce()` — [`L312`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L312)

## Module values
- `INTERPRETER_STARTUP_ENV_EXACT` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L29)
- `READY_TIMEOUT_MS` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L17)
- `SPAWN_TIMEOUT_MS` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L18)
- `STDERR_TAIL_MAX` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L19)
- `cleanupRegistered` — [`L306`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L306)
- `servers` — [`L305`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/fork-server.ts#L305)


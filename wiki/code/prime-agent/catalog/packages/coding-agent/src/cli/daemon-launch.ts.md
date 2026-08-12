---
title: 'Module: packages/coding-agent/src/cli/daemon-launch.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/daemon-launch.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`daemon-launch.ts`/
symbols:
  ensureDaemonRunning: ensureDaemonRunning().
  probeDaemonVersion: probeDaemonVersion().
  probeRunningDaemonSessions: probeRunningDaemonSessions().
  StaleDaemonError.-constructor: StaleDaemonError#`<constructor>`().
  shutdownStaleDaemonIfNotBusy: shutdownStaleDaemonIfNotBusy().
  shutdownDaemonAndWait: shutdownDaemonAndWait().
  ensureInteractiveDaemonRunning: ensureInteractiveDaemonRunning().
  shutdownConnectedDaemonAndWait: shutdownConnectedDaemonAndWait().
  RunningDaemonProbe: RunningDaemonProbe#
  shouldStartDaemonEarly: shouldStartDaemonEarly().
  waitForDaemonGone: waitForDaemonGone().
  listActiveDaemonSessionSummaries: listActiveDaemonSessionSummaries().
  maybeStartDaemonEarly: maybeStartDaemonEarly().
  hasProcessIdentityExited: hasProcessIdentityExited().
  queryActiveDaemonSessions.Promise.typeLiteral45.busyClientOwnedSessionCount: queryActiveDaemonSessions().Promise:typeLiteral45:busyClientOwnedSessionCount.
  isSessionBusy: isSessionBusy().
  isDaemonSessionSummary: isDaemonSessionSummary().
  canConnectToDaemon: canConnectToDaemon().
  logDaemonLaunch: logDaemonLaunch().
  processIdentityFromDaemonHello: processIdentityFromDaemonHello().
  readDaemonLogTail: readDaemonLogTail().
  queryActiveDaemonSessions.Promise.typeLiteral45.sessions: queryActiveDaemonSessions().Promise:typeLiteral45:sessions.
  queryActiveDaemonSessions: queryActiveDaemonSessions().
  ensurePromises: ensurePromises.
  DaemonVersionProbe: DaemonVersionProbe#
  currentDaemonLogSize: currentDaemonLogSize().
  findFirstEarlyLaunchPositional: findFirstEarlyLaunchPositional().
  DaemonProcessIdentity: DaemonProcessIdentity#
  delay: delay().
  StaleDaemonError: StaleDaemonError#
  DaemonProcessIdentity.pid: DaemonProcessIdentity#pid.
  DaemonProcessIdentity.processStartId: DaemonProcessIdentity#processStartId.
  DAEMON_STARTUP_TIMEOUT_MS: DAEMON_STARTUP_TIMEOUT_MS.
  DAEMON_STARTUP_LOG_TAIL_BYTES: DAEMON_STARTUP_LOG_TAIL_BYTES.
  DAEMON_STARTUP_EXIT_GRACE_MS: DAEMON_STARTUP_EXIT_GRACE_MS.
  queryActiveDaemonSessions.options-typeLiteral46.includeClientOwned: queryActiveDaemonSessions().(options)typeLiteral46:includeClientOwned.
  PROCESS_START_ID_POLL_INTERVAL_MS: PROCESS_START_ID_POLL_INTERVAL_MS.
  EARLY_LAUNCH_EXCLUDED_FLAGS: EARLY_LAUNCH_EXCLUDED_FLAGS.
  EARLY_LAUNCH_VALUE_FLAGS: EARLY_LAUNCH_VALUE_FLAGS.
  listActiveDaemonSessionSummaries.options-typeLiteral44.includeClientOwned: listActiveDaemonSessionSummaries().(options)typeLiteral44:includeClientOwned.
---
# Module: [`packages/coding-agent/src/cli/daemon-launch.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts)

## Classes
### `DaemonProcessIdentity`
- def: [`packages/coding-agent/src/cli/daemon-launch.ts:171`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L171)
- signature: `interface DaemonProcessIdentity`
- members:
  - `pid` — [`L172`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L172)
  - `processStartId` — [`L173`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L173)
- used by: [`waitForDaemonGone`](daemon-launch.ts.md#waitForDaemonGone), [`hasProcessIdentityExited`](daemon-launch.ts.md#hasProcessIdentityExited), [`processIdentityFromDaemonHello`](daemon-launch.ts.md#processIdentityFromDaemonHello)

### `DaemonVersionProbe`
- def: [`packages/coding-agent/src/cli/daemon-launch.ts:64`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L64)
- signature: `type DaemonVersionProbe`
- uses (calls/refs, reference-scoped): [`DaemonHello`](../modes/daemon/daemon-client.ts.md#DaemonHello)
- used by: [`probeDaemonVersion`](daemon-launch.ts.md#probeDaemonVersion)

### `RunningDaemonProbe`
- def: [`packages/coding-agent/src/cli/daemon-launch.ts:270`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L270)
- signature: `type RunningDaemonProbe`
- uses (calls/refs, reference-scoped): [`SessionSummary`](../modes/daemon/daemon-session-list.ts.md#SessionSummary)
- used by: [`package-manager-cli.ts`](../package-manager-cli.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-package-manager-cli.ts), [`confirmDaemonSessionLoss`](daemon-stop-confirm.ts.md#confirmDaemonSessionLoss), [`probeRunningDaemonSessions`](daemon-launch.ts.md#probeRunningDaemonSessions), [`confirmDaemonSessionLossBeforeUpdate`](../package-manager-cli.ts.md#confirmDaemonSessionLossBeforeUpdate), [`daemon-stop-confirm.ts`](daemon-stop-confirm.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-daemon-stop-confirm.ts), [`daemonProbeMayHaveBusySessions`](../package-manager-cli.ts.md#daemonProbeMayHaveBusySessions)  (1 test-only)

### `StaleDaemonError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/cli/daemon-launch.ts:150`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L150)
- doc: Thrown when a stale-version daemon can't be replaced. The message is user-facing.
- signature: `class StaleDaemonError`
- members:
  - `<constructor>(socketPath: string, hello?: { type: "daemon_hello"; socketPath: string; protocol: DaemonProtocolInfo; schemaId?: string | undefined; schemaRevision?: number | undefined; ... 8 more ...; serverCapabilities: readonly DaemonServerCapability[]; } | undefined)` — [`L151`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L151) — Thrown when a stale-version daemon can't be replaced. The message is user-facing.
- uses (calls/refs, reference-scoped): [`VERSION`](../config.ts.md#VERSION), [`DAEMON_PROTOCOL_VERSION`](../modes/daemon/daemon-protocol.ts.md#DAEMON_PROTOCOL_VERSION), [`getDaemonRuntimeIdentity`](../modes/daemon/daemon-runtime-identity.ts.md#getDaemonRuntimeIdentity), [`DAEMON_SCHEMA_ID`](../modes/daemon/daemon-protocol.ts.md#DAEMON_SCHEMA_ID), [`DaemonHello`](../modes/daemon/daemon-client.ts.md#DaemonHello), [`version`](../modes/daemon/daemon-protocol.ts.md#DaemonProtocolInfo.version), [`formatCurrentCliCommand`](subprocess-launch.ts.md#formatCurrentCliCommand), [`buildId`](../modes/daemon/daemon-protocol.ts.md#DaemonRuntimeIdentity.buildId), [`entrypointPath`](../modes/daemon/daemon-protocol.ts.md#DaemonRuntimeIdentity.entrypointPath), [`executablePath`](../modes/daemon/daemon-protocol.ts.md#DaemonRuntimeIdentity.executablePath), [`launcherPath`](../modes/daemon/daemon-protocol.ts.md#DaemonRuntimeIdentity.launcherPath)
- used by: [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`ensureDaemonRunning`](daemon-launch.ts.md#ensureDaemonRunning), [`awaitDaemonReady`](../main.ts.md#awaitDaemonReady)

## Functions
- `canConnectToDaemon(socketPath: string, timeoutMs: number)` — [`L52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L52)
- `currentDaemonLogSize(socketPath: string)` — [`L432`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L432)
- `delay(ms: number)` — [`L41`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L41)
- `ensureDaemonRunning(socketPath: string, spawnCwd?: string | undefined)` — [`L340`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L340)
- `ensureInteractiveDaemonRunning(socketPath: string, spawnCwd?: string | undefined)` — [`L466`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L466) — Ensure a current-version daemon is listening on socketPath, spawning one if
- `findFirstEarlyLaunchPositional(args: readonly string[])` — [`L513`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L513)
- `hasProcessIdentityExited(identity: DaemonProcessIdentity | undefined, verifyProcessStartId?: boolean)` — [`L178`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L178)
- `isDaemonSessionSummary(value: unknown)` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L33)
- `isSessionBusy(summary: SessionSummary)` — [`L274`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L274)
- `listActiveDaemonSessionSummaries(client: DaemonClient, options?: { includeClientOwned?: boolean | undefined; })` — [`L111`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L111)
- `logDaemonLaunch(message: string)` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L48)
- `maybeStartDaemonEarly(args: readonly string[])` — [`L565`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L565)
- `probeDaemonVersion(socketPath: string)` — [`L70`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L70) — Connect to a running daemon and check whether it matches this client's protocol and app version.
- `probeRunningDaemonSessions(socketPath: string)` — [`L278`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L278)
- `processIdentityFromDaemonHello(hello: { type: "daemon_hello"; socketPath: string; protocol: DaemonProtocolInfo; schemaId?: string | undefined; schemaRevision?: number | undefined; appVersion?: string | undefined; ... 7 more ...; serverCapabilities: readonly DaemonServerCapability[]; } | undefined)` — [`L226`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L226)
- `queryActiveDaemonSessions(client: DaemonClient, options?: { includeClientOwned?: boolean | undefined; })` — [`L118`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L118)
- `readDaemonLogTail(socketPath: string, offset: number)` — [`L441`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L441) — Reads only log content written after `offset`, so stale content from earlier daemon runs is not misattributed to this startup attempt.
- `shouldStartDaemonEarly(args: readonly string[], startupBenchmark: boolean)` — [`L536`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L536)
- `shutdownConnectedDaemonAndWait(client: DaemonClient, socketPath: string, timeoutMs?: number, hello?: { type: "daemon_hello"; socketPath: string; protocol: DaemonProtocolInfo; schemaId?: string | undefined; ... 9 more ...; serverCapabilities: readonly DaemonServerCapability[]; } | undefined)` — [`L237`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L237)
- `shutdownDaemonAndWait(socketPath: string, timeoutMs?: number)` — [`L256`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L256)
- `shutdownStaleDaemonIfNotBusy(socketPath: string)` — [`L304`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L304)
- `waitForDaemonGone(socketPath: string, timeoutMs?: number, requireSocketCleanup?: boolean, expectedIdentity?: DaemonProcessIdentity | undefined)` — [`L194`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L194)

## Module values
- `DAEMON_STARTUP_EXIT_GRACE_MS` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L31)
- `DAEMON_STARTUP_LOG_TAIL_BYTES` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L30)
- `DAEMON_STARTUP_TIMEOUT_MS` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L29)
- `EARLY_LAUNCH_EXCLUDED_FLAGS` — [`L481`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L481)
- `EARLY_LAUNCH_VALUE_FLAGS` — [`L482`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L482)
- `PROCESS_START_ID_POLL_INTERVAL_MS` — [`L176`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L176)
- `busyClientOwnedSessionCount` — [`L121`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L121)
- `ensurePromises` — [`L458`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L458)
- `includeClientOwned` — [`L113`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L113)
- `includeClientOwned` — [`L120`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L120)
- `sessions` — [`L121`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-launch.ts#L121)


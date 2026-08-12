---
title: 'Module: packages/coding-agent/src/cli/daemon-ps.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/daemon-ps.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`daemon-ps.ts`/
symbols:
  discoverDaemons: discoverDaemons().
  runShutdownAllConverging: runShutdownAllConverging().
  DiscoveredDaemonProcess.pid: DiscoveredDaemonProcess#pid.
  forceStopTrackedWorkers: forceStopTrackedWorkers().
  DaemonInfo.status: DaemonInfo#status.
  DaemonInfo.socketPath: DaemonInfo#socketPath.
  stopHiddenSupervisors.failed-Array.typeLiteral557.reason: stopHiddenSupervisors().(failed)Array:typeLiteral557:reason.
  runReap: runReap().
  terminateVerifiedResiduals.failed-Array.typeLiteral621.reason: terminateVerifiedResiduals().(failed)Array:typeLiteral621:reason.
  probeDaemon: probeDaemon().
  DaemonInfo.pid: DaemonInfo#pid.
  planReap: planReap().
  scanListeningDaemons: scanListeningDaemons().
  DiscoveredDaemonProcess.socketPath: DiscoveredDaemonProcess#socketPath.
  runShutdownAll: runShutdownAll().
  classifyReachable: classifyReachable().
  isTrackedWorkerDescriptor: isTrackedWorkerDescriptor().
  planShutdownAll: planShutdownAll().
  DaemonInfo: DaemonInfo#
  parseSsListeners: parseSsListeners().
  apply: apply().
  DiscoveredDaemonProcess: DiscoveredDaemonProcess#
  shutdownDaemon: shutdownDaemon().
  sortDaemons: sortDaemons().
  stopBackgroundService: stopBackgroundService().
  terminateVerifiedListener.failed-Array.typeLiteral668.reason: terminateVerifiedListener().(failed)Array:typeLiteral668:reason.
  findAllTrackedWorkers: findAllTrackedWorkers().
  reapReachableDaemon: reapReachableDaemon().
  DaemonInfo.isDefault: DaemonInfo#isDefault.
  parseLsofListeners: parseLsofListeners().
  findTrackedWorkers: findTrackedWorkers().
  daemonListenerSignature: daemonListenerSignature().
  recordResidualListenerFailures.failed-Array.typeLiteral652.reason: recordResidualListenerFailures().(failed)Array:typeLiteral652:reason.
  DaemonInfo.sessionCount: DaemonInfo#sessionCount.
  stopTrackedProcess: stopTrackedProcess().
  isWorkerSocketPath: isWorkerSocketPath().
  isDaemonProcessListening: isDaemonProcessListening().
  mergeDiscoveredDaemonProcesses: mergeDiscoveredDaemonProcesses().
  runPs: runPs().
  enrichUptimes: enrichUptimes().
  planShutdownConfirmation: planShutdownConfirmation().
  forceKillDaemon: forceKillDaemon().
  canConnectToSocket: canConnectToSocket().
  removeSocketFile: removeSocketFile().
  normalizeSocketPath: normalizeSocketPath().
  recordShutdownFailure: recordShutdownFailure().
  ReapAction: ReapAction#
  DaemonStatus: DaemonStatus#
  evaluateShutdownQuietPeriod: evaluateShutdownQuietPeriod().
  ProbeResult.runtime: ProbeResult#runtime.
  verifyHelloSupervisorPid: verifyHelloSupervisorPid().
  TrackedWorker.descriptor: TrackedWorker#descriptor.
  scanSocketDir: scanSocketDir().
  ProbeResult.reachable: ProbeResult#reachable.
  isProcessAlive: isProcessAlive().
  delay: delay().
  processNameMatches: processNameMatches().
  parsePrimeAgentProcessIds: parsePrimeAgentProcessIds().
  STATUS_ORDER: STATUS_ORDER.
  SHUTDOWN_ALL_ACTION_ORDER: SHUTDOWN_ALL_ACTION_ORDER.
  recordResidualListenerFailures: recordResidualListenerFailures().
  terminateVerifiedListener: terminateVerifiedListener().
  parsePsEtimes: parsePsEtimes().
  ProbeResult.sessionCount: ProbeResult#sessionCount.
  TrackedWorker: TrackedWorker#
  ReapOutcome: ReapOutcome#
  killDaemon: killDaemon().
  DaemonInfo.uptimeSeconds: DaemonInfo#uptimeSeconds.
  DaemonInfo.version: DaemonInfo#version.
  DaemonInfo.hasTrackedWorkers: DaemonInfo#hasTrackedWorkers.
  ProbeResult: ProbeResult#
  ProbeResult.version: ProbeResult#version.
  ProbeResult.protocolVersion: ProbeResult#protocolVersion.
  ProbeResult.schemaId: ProbeResult#schemaId.
  ProbeResult.supervisorPid: ProbeResult#supervisorPid.
  TrackedWorker.descriptorPath: TrackedWorker#descriptorPath.
  DiscoveredDaemonProcess.uptimeSeconds: DiscoveredDaemonProcess#uptimeSeconds.
  DaemonInfo.protocolVersion: DaemonInfo#protocolVersion.
  SHUTDOWN_QUIET_PERIOD_MS: SHUTDOWN_QUIET_PERIOD_MS.
  SHUTDOWN_CONVERGENCE_TIMEOUT_MS: SHUTDOWN_CONVERGENCE_TIMEOUT_MS.
  MAX_COMM_LENGTH: MAX_COMM_LENGTH.
  ProbeResult.supervisorProcessStartId: ProbeResult#supervisorProcessStartId.
  ShutdownConfirmationPlan: ShutdownConfirmationPlan#
  stopHiddenSupervisors: stopHiddenSupervisors().
  stopHiddenSupervisors.stopped-Array.typeLiteral556.socketPath: stopHiddenSupervisors().(stopped)Array:typeLiteral556:socketPath.
  stopHiddenSupervisors.stopped-Array.typeLiteral556.action: stopHiddenSupervisors().(stopped)Array:typeLiteral556:action.
  terminateVerifiedResiduals: terminateVerifiedResiduals().
  terminateVerifiedResiduals.stopped-Array.typeLiteral620.socketPath: terminateVerifiedResiduals().(stopped)Array:typeLiteral620:socketPath.
  terminateVerifiedResiduals.stopped-Array.typeLiteral620.action: terminateVerifiedResiduals().(stopped)Array:typeLiteral620:action.
  describeDaemonParent: describeDaemonParent().
  recordShutdownFailure.failed-Array.typeLiteral683.socketPath: recordShutdownFailure().(failed)Array:typeLiteral683:socketPath.
  recordShutdownFailure.failed-Array.typeLiteral683.reason: recordShutdownFailure().(failed)Array:typeLiteral683:reason.
  apply.reaped-Array.typeLiteral790.socketPath: apply().(reaped)Array:typeLiteral790:socketPath.
  apply.reaped-Array.typeLiteral790.action: apply().(reaped)Array:typeLiteral790:action.
  apply.skipped-Array.typeLiteral791.socketPath: apply().(skipped)Array:typeLiteral791:socketPath.
  apply.skipped-Array.typeLiteral791.reason: apply().(skipped)Array:typeLiteral791:reason.
  DaemonInfo.schemaId: DaemonInfo#schemaId.
  DaemonInfo.buildId: DaemonInfo#buildId.
  DaemonInfo.executablePath: DaemonInfo#executablePath.
  DaemonInfo.pidSource: DaemonInfo#pidSource.
  stopHiddenSupervisors.failed-Array.typeLiteral557.socketPath: stopHiddenSupervisors().(failed)Array:typeLiteral557:socketPath.
  terminateVerifiedResiduals.failed-Array.typeLiteral621.socketPath: terminateVerifiedResiduals().(failed)Array:typeLiteral621:socketPath.
  recordResidualListenerFailures.failed-Array.typeLiteral652.socketPath: recordResidualListenerFailures().(failed)Array:typeLiteral652:socketPath.
  terminateVerifiedListener.failed-Array.typeLiteral668.socketPath: terminateVerifiedListener().(failed)Array:typeLiteral668:socketPath.
---
# Module: [`packages/coding-agent/src/cli/daemon-ps.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts)

## Classes
### `DaemonInfo`
- def: [`packages/coding-agent/src/cli/daemon-ps.ts:47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L47)
- signature: `interface DaemonInfo`
- members:
  - `buildId` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L54)
  - `executablePath` — [`L55`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L55)
  - `hasTrackedWorkers` — [`L60`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L60)
  - `isDefault` — [`L59`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L59)
  - `pid` — [`L49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L49)
  - `pidSource` — [`L56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L56)
  - `protocolVersion` — [`L52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L52)
  - `schemaId` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L53)
  - `sessionCount` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L57)
  - `socketPath` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L48)
  - `status` — [`L58`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L58)
  - `uptimeSeconds` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L50)
  - `version` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L51)
- uses (calls/refs, reference-scoped): [`DaemonStatus`](daemon-ps.ts.md#DaemonStatus)
- used by: [`discoverDaemons`](daemon-ps.ts.md#discoverDaemons), [`runShutdownAllConverging`](daemon-ps.ts.md#runShutdownAllConverging), [`formatDaemonListTable`](daemon-ps-format.ts.md#formatDaemonListTable), [`runReap`](daemon-ps.ts.md#runReap), [`planReap`](daemon-ps.ts.md#planReap), [`runShutdownAll`](daemon-ps.ts.md#runShutdownAll), [`planShutdownAll`](daemon-ps.ts.md#planShutdownAll), [`sortDaemons`](daemon-ps.ts.md#sortDaemons), [`daemon-ps-format.ts`](daemon-ps-format.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-daemon-ps-format.ts), [`ReapAction`](daemon-ps.ts.md#ReapAction)  (3 test-only)

### `DaemonStatus`
- def: [`packages/coding-agent/src/cli/daemon-ps.ts:39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L39)
- doc: `daemon ps` discovers every prime-agent daemon on the machine, not just the
- signature: `type DaemonStatus`
- used by: [`discoverDaemons`](daemon-ps.ts.md#discoverDaemons), [`status`](daemon-ps.ts.md#DaemonInfo.status), [`classifyReachable`](daemon-ps.ts.md#classifyReachable), [`daemon-ps-format.ts`](daemon-ps-format.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-daemon-ps-format.ts), [`formatDaemonCell`](daemon-ps-format.ts.md#formatDaemonCell), [`STATUS_ORDER`](daemon-ps.ts.md#STATUS_ORDER), [`colorStatus`](daemon-ps-format.ts.md#colorStatus)

### `DiscoveredDaemonProcess`
- def: [`packages/coding-agent/src/cli/daemon-ps.ts:41`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L41)
- signature: `interface DiscoveredDaemonProcess`
- members:
  - `pid` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L42)
  - `socketPath` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L43)
  - `uptimeSeconds` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L44)
- used by: [`discoverDaemons`](daemon-ps.ts.md#discoverDaemons), [`reason`](daemon-ps.ts.md#stopHiddenSupervisors.failed-Array.typeLiteral557.reason), [`reason`](daemon-ps.ts.md#terminateVerifiedResiduals.failed-Array.typeLiteral621.reason), [`scanListeningDaemons`](daemon-ps.ts.md#scanListeningDaemons), [`parseSsListeners`](daemon-ps.ts.md#parseSsListeners), [`reason`](daemon-ps.ts.md#terminateVerifiedListener.failed-Array.typeLiteral668.reason), [`parseLsofListeners`](daemon-ps.ts.md#parseLsofListeners), [`daemonListenerSignature`](daemon-ps.ts.md#daemonListenerSignature), [`reason`](daemon-ps.ts.md#recordResidualListenerFailures.failed-Array.typeLiteral652.reason), [`isDaemonProcessListening`](daemon-ps.ts.md#isDaemonProcessListening), [`mergeDiscoveredDaemonProcesses`](daemon-ps.ts.md#mergeDiscoveredDaemonProcesses), [`enrichUptimes`](daemon-ps.ts.md#enrichUptimes), [`recordResidualListenerFailures`](daemon-ps.ts.md#recordResidualListenerFailures), [`terminateVerifiedListener`](daemon-ps.ts.md#terminateVerifiedListener)  (1 test-only)

### `ProbeResult`
- def: [`packages/coding-agent/src/cli/daemon-ps.ts:244`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L244)
- signature: `interface ProbeResult`
- members:
  - `protocolVersion` — [`L246`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L246)
  - `reachable` — [`L252`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L252)
  - `runtime` — [`L248`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L248)
  - `schemaId` — [`L247`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L247)
  - `sessionCount` — [`L249`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L249)
  - `supervisorPid` — [`L250`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L250)
  - `supervisorProcessStartId` — [`L251`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L251)
  - `version` — [`L245`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L245)
- uses (calls/refs, reference-scoped): [`DaemonRuntimeIdentity`](../modes/daemon/daemon-protocol.ts.md#DaemonRuntimeIdentity)
- used by: [`discoverDaemons`](daemon-ps.ts.md#discoverDaemons), [`runShutdownAllConverging`](daemon-ps.ts.md#runShutdownAllConverging), [`reason`](daemon-ps.ts.md#stopHiddenSupervisors.failed-Array.typeLiteral557.reason), [`runReap`](daemon-ps.ts.md#runReap), [`probeDaemon`](daemon-ps.ts.md#probeDaemon), [`classifyReachable`](daemon-ps.ts.md#classifyReachable), [`reapReachableDaemon`](daemon-ps.ts.md#reapReachableDaemon)

### `ReapAction`
- def: [`packages/coding-agent/src/cli/daemon-ps.ts:420`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L420)
- signature: `type ReapAction`
- uses (calls/refs, reference-scoped): [`DaemonInfo`](daemon-ps.ts.md#DaemonInfo)
- used by: [`planReap`](daemon-ps.ts.md#planReap), [`planShutdownAll`](daemon-ps.ts.md#planShutdownAll), [`SHUTDOWN_ALL_ACTION_ORDER`](daemon-ps.ts.md#SHUTDOWN_ALL_ACTION_ORDER)

### `ReapOutcome`
- def: [`packages/coding-agent/src/cli/daemon-ps.ts:1139`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1139)
- signature: `type ReapOutcome`
- used by: [`apply`](daemon-ps.ts.md#apply), [`stopBackgroundService`](daemon-ps.ts.md#stopBackgroundService), [`reapReachableDaemon`](daemon-ps.ts.md#reapReachableDaemon)

### `ShutdownConfirmationPlan`
- def: [`packages/coding-agent/src/cli/daemon-ps.ts:503`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L503)
- signature: `type ShutdownConfirmationPlan`
- used by: [`planShutdownConfirmation`](daemon-ps.ts.md#planShutdownConfirmation)

### `TrackedWorker`
- def: [`packages/coding-agent/src/cli/daemon-ps.ts:925`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L925)
- signature: `interface TrackedWorker`
- members:
  - `descriptor` — [`L926`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L926)
  - `descriptorPath` — [`L927`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L927)
- uses (calls/refs, reference-scoped): [`DaemonWorkerDescriptor`](../modes/daemon/daemon-worker-protocol.ts.md#DaemonWorkerDescriptor)
- used by: [`discoverDaemons`](daemon-ps.ts.md#discoverDaemons), [`forceStopTrackedWorkers`](daemon-ps.ts.md#forceStopTrackedWorkers), [`findAllTrackedWorkers`](daemon-ps.ts.md#findAllTrackedWorkers), [`findTrackedWorkers`](daemon-ps.ts.md#findTrackedWorkers)

## Functions
- `apply(outcome: ReapOutcome, socketPath: string, reaped: { socketPath: string; action: string; }[], skipped: { socketPath: string; reason: string; }[])` — [`L1141`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1141)
- `canConnectToSocket(socketPath: string, timeoutMs: number)` — [`L1220`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1220)
- `classifyReachable(probe: ProbeResult)` — [`L310`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L310)
- `daemonListenerSignature(listeners: readonly DiscoveredDaemonProcess[])` — [`L862`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L862)
- `delay(ms: number)` — [`L1216`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1216)
- `describeDaemonParent(pid: number)` — [`L808`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L808)
- `discoverDaemons()` — [`L345`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L345) — Discover every daemon on the machine and probe each for version + session count.
- `enrichUptimes(daemons: DiscoveredDaemonProcess[])` — [`L208`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L208)
- `evaluateShutdownQuietPeriod(now: number, quietSince: number | undefined)` — [`L72`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L72)
- `findAllTrackedWorkers()` — [`L981`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L981)
- `findTrackedWorkers(supervisorSocketPath: string)` — [`L974`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L974)
- `forceKillDaemon(pid: number)` — [`L1191`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1191)
- `forceStopTrackedWorkers(supervisorSocketPath: string, assertAdmission: () => Promise<void>)` — [`L930`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L930)
- `isDaemonProcessListening(pid: number, socketPath: string)` — [`L203`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L203)
- `isProcessAlive(pid: number)` — [`L1207`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1207)
- `isTrackedWorkerDescriptor(value: unknown)` — [`L1026`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1026)
- `isWorkerSocketPath(socketPath: string)` — [`L883`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L883)
- `killDaemon(pid: number)` — [`L1183`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1183)
- `mergeDiscoveredDaemonProcesses(...groups: readonly DiscoveredDaemonProcess[][])` — [`L153`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L153)
- `normalizeSocketPath(socketPath: string)` — [`L83`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L83) — Normalize a socket path so process-scan and dir-sweep entries merge cleanly.
- `parseLsofListeners(stdout: string)` — [`L116`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L116) — Parse `lsof -nP -F pn -U -a -c <app>` output into listening unix socket owners (macOS fallback).
- `parsePrimeAgentProcessIds(stdout: string, appName: string)` — [`L137`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L137)
- `parsePsEtimes(stdout: string)` — [`L166`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L166) — Parse `ps -o pid=,etimes=` output into a pid → uptime-seconds map.
- `parseSsListeners(stdout: string, appName: string)` — [`L95`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L95) — Parse `ss -lxp` output into the prime-agent daemons listening on unix sockets.
- `planReap(daemons: readonly DaemonInfo[], force: boolean)` — [`L441`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L441) — Decide what to do with each discovered daemon (pure, no side effects). Reap
- `planShutdownAll(daemons: readonly DaemonInfo[], force: boolean)` — [`L479`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L479)
- `planShutdownConfirmation(daemonCount: number, json: boolean, force: boolean, stdinIsTTY: boolean | undefined)` — [`L505`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L505)
- `probeDaemon(socketPath: string)` — [`L255`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L255)
- `processNameMatches(name: string, appName: string)` — [`L90`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L90)
- `reapReachableDaemon(socketPath: string, pid: number | undefined)` — [`L1159`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1159) — Gracefully stop a daemon, but only after a fresh probe confirms it is idle.
- `recordResidualListenerFailures(listeners: readonly DiscoveredDaemonProcess[], failed: { socketPath: string; reason: string; }[], reportedFailures: Set<string>, reason: string)` — [`L789`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L789)
- `recordShutdownFailure(failed: { socketPath: string; reason: string; }[], reportedFailures: Set<string>, socketPath: string, reason: string)` — [`L869`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L869)
- `removeSocketFile(socketPath: string)` — [`L1172`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1172)
- `runPs(json: boolean)` — [`L407`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L407)
- `runReap(json: boolean, force: boolean)` — [`L1078`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1078)
- `runShutdownAll(json: boolean, force: boolean)` — [`L516`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L516)
- `runShutdownAllConverging(json: boolean, force: boolean, assertAdmission: () => Promise<void>)` — [`L560`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L560)
- `scanListeningDaemons()` — [`L177`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L177)
- `scanSocketDir()` — [`L222`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L222) — Socket files in the default socket dir (may be live daemons or orphaned files).
- `shutdownDaemon(socketPath: string, force: boolean)` — [`L1237`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1237) — Ask a daemon to shut down and confirm it actually stopped listening. The
- `sortDaemons(infos: DaemonInfo[])` — [`L397`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L397)
- `stopBackgroundService(socketPath: string, pid: number | undefined, handledPids: Set<number>, force: boolean, assertAdmission: () => Promise<void>)` — [`L892`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L892)
- `stopHiddenSupervisors(stopped: { socketPath: string; action: string; }[], failed: { socketPath: string; reason: string; }[], handledPids: Set<number>, reportedFailures: Set<string>, assertAdmission: () => Promise<void>)` — [`L681`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L681)
- `stopTrackedProcess(pid: number, expectedStartId: string | undefined, assertAdmission: () => Promise<void>)` — [`L1043`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1043)
- `terminateVerifiedListener(listener: DiscoveredDaemonProcess, failed: { socketPath: string; reason: string; }[], reportedFailures: Set<string>, assertAdmission: () => Promise<void>)` — [`L820`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L820)
- `terminateVerifiedResiduals(stopped: { socketPath: string; action: string; }[], failed: { socketPath: string; reason: string; }[], handledPids: Set<number>, reportedFailures: Set<string>, assertAdmission: () => Promise<void>)` — [`L734`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L734)
- `verifyHelloSupervisorPid(pid: number | undefined, expectedProcessStartId: string | undefined)` — [`L321`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L321)

## Module values
- `MAX_COMM_LENGTH` — [`L80`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L80)
- `SHUTDOWN_ALL_ACTION_ORDER` — [`L496`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L496)
- `SHUTDOWN_CONVERGENCE_TIMEOUT_MS` — [`L70`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L70)
- `SHUTDOWN_QUIET_PERIOD_MS` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L69)
- `STATUS_ORDER` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L63)
- `action` — [`L682`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L682)
- `action` — [`L735`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L735)
- `action` — [`L1144`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1144)
- `reason` — [`L683`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L683)
- `reason` — [`L736`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L736)
- `reason` — [`L791`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L791)
- `reason` — [`L822`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L822)
- `reason` — [`L870`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L870)
- `reason` — [`L1145`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1145)
- `socketPath` — [`L682`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L682)
- `socketPath` — [`L683`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L683)
- `socketPath` — [`L735`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L735)
- `socketPath` — [`L736`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L736)
- `socketPath` — [`L791`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L791)
- `socketPath` — [`L822`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L822)
- `socketPath` — [`L870`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L870)
- `socketPath` — [`L1144`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1144)
- `socketPath` — [`L1145`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps.ts#L1145)


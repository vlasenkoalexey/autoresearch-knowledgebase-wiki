---
title: 'Module: packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/regressions/`4606-update-restart-coordinator.test.ts`/
symbols:
  spawnSupervisor.paths-typeLiteral4.socketPath: spawnSupervisor().(paths)typeLiteral4:socketPath.
  connectEventually: connectEventually().
  stopDaemon: stopDaemon().
  requireSessionSummary: requireSessionSummary().
  harnesses: harnesses.
  withSourceCliEntrypoint: withSourceCliEntrypoint().
  waitForTerminalStatus: waitForTerminalStatus().
  SupervisorHandle.child: SupervisorHandle#child.
  waitForProcessExit: waitForProcessExit().
  requireSessionList: requireSessionList().
  supervisors: supervisors.
  delay: delay().
  tsxPath: tsxPath.
  sockets: sockets.
  waitForFile: waitForFile().
  listSupervisorOwnerRecords: listSupervisorOwnerRecords().
  SupervisorHandle: SupervisorHandle#
  SupervisorHandle.stdout: SupervisorHandle#stdout.
  SupervisorHandle.stderr: SupervisorHandle#stderr.
  cliPath: cliPath.
  spawnSupervisor.paths-typeLiteral4.agentDir: spawnSupervisor().(paths)typeLiteral4:agentDir.
  SupervisorOwnerRecord: SupervisorOwnerRecord#
  tsconfigPath: tsconfigPath.
  waitForExit: waitForExit().
  isProcessAlive: isProcessAlive().
  fauxExtensionPath: fauxExtensionPath.
  launcherFixturePath: launcherFixturePath.
  supervisorRegistryDirEnv: supervisorRegistryDirEnv.
  spawnSupervisor: spawnSupervisor().
  spawnSupervisor.paths-typeLiteral4.completionPath: spawnSupervisor().(paths)typeLiteral4:completionPath.
  spawnSupervisor.paths-typeLiteral4.pidPath: spawnSupervisor().(paths)typeLiteral4:pidPath.
  spawnSupervisor.paths-typeLiteral4.registryDir: spawnSupervisor().(paths)typeLiteral4:registryDir.
  shellQuote: shellQuote().
  SupervisorOwnerRecord.pid: SupervisorOwnerRecord#pid.
  SupervisorOwnerRecord.processStartId: SupervisorOwnerRecord#processStartId.
  SupervisorOwnerRecord.socketPath: SupervisorOwnerRecord#socketPath.
---
# Module: [`packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts)

## Classes
### `SupervisorHandle`
- def: [`packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts:17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L17)
- signature: `interface SupervisorHandle`
- members:
  - `child` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L18)
  - `stderr` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L20)
  - `stdout` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L19)
- used by: (3 test-only callers)

### `SupervisorOwnerRecord`
- def: [`packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts:23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L23)
- signature: `interface SupervisorOwnerRecord`
- members:
  - `pid` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L24)
  - `processStartId` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L25)
  - `socketPath` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L26)
- used by: (1 test-only callers)

## Functions
- `connectEventually(socketPath: string, timeoutMs?: number)` — [`L82`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L82)
- `delay(ms: number)` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L39)
- `isProcessAlive(pid: number)` — [`L211`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L211)
- `listSupervisorOwnerRecords(registryDir: string)` — [`L220`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L220)
- `requireSessionList(response: DaemonResponse)` — [`L170`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L170)
- `requireSessionSummary(response: DaemonResponse)` — [`L156`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L156)
- `shellQuote(value: string)` — [`L184`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L184)
- `spawnSupervisor(paths: { agentDir: string; completionPath: string; pidPath: string; registryDir: string; socketPath: string; })` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L43)
- `stopDaemon(socketPath: string)` — [`L229`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L229)
- `waitForExit(child: ChildProcess, timeoutMs?: number)` — [`L100`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L100)
- `waitForFile(path: string, timeoutMs?: number)` — [`L125`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L125)
- `waitForProcessExit(pid: number, timeoutMs?: number)` — [`L116`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L116)
- `waitForTerminalStatus(agentDir: string, timeoutMs?: number)` — [`L136`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L136)
- `withSourceCliEntrypoint(action: () => Promise<T>)` — [`L188`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L188)

## Module values
- `agentDir` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L44)
- `cliPath` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L29)
- `completionPath` — [`L45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L45)
- `fauxExtensionPath` — [`L30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L30)
- `harnesses` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L36)
- `launcherFixturePath` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L31)
- `pidPath` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L46)
- `registryDir` — [`L47`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L47)
- `socketPath` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L48)
- `sockets` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L37)
- `supervisorRegistryDirEnv` — [`L34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L34)
- `supervisors` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L35)
- `tsconfigPath` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L33)
- `tsxPath` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4606-update-restart-coordinator.test.ts#L32)


---
title: 'Module: packages/coding-agent/test/daemon-supervisor-process.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/daemon-supervisor-process.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`daemon-supervisor-process.test.ts`/
symbols:
  connectEventually: connectEventually().
  spawnSupervisor: spawnSupervisor().
  workerPids: workerPids.
  waitForSocketGone: waitForSocketGone().
  PROCESS_STRESS_WORKERS: PROCESS_STRESS_WORKERS.
  tempDir: tempDir().
  requireSessionList: requireSessionList().
  requireSummary: requireSummary().
  startBlockingBash: startBlockingBash().
  waitForProcessGone: waitForProcessGone().
  children: children.
  countWorkerDescriptors: countWorkerDescriptors().
  waitForCondition: waitForCondition().
  waitForWorkerStopTombstone: waitForWorkerStopTombstone().
  waitForExit: waitForExit().
  readWorkerDescriptor: readWorkerDescriptor().
  daemonSockets: daemonSockets.
  childDiagnostics: childDiagnostics.
  tempDirs: tempDirs.
  cliPath: cliPath.
  tsxPath: tsxPath.
  blockingProcessPath: blockingProcessPath.
  readDaemonLogs: readDaemonLogs().
  readSupervisorConfig: readSupervisorConfig().
  quoteShellArgument: quoteShellArgument().
  readSupervisorConfig.typeLiteral288.defaultSessionConfig: readSupervisorConfig().typeLiteral288:defaultSessionConfig.
  readSupervisorConfig.typeLiteral288.defaultSessionConfig.typeLiteral289.sessionDir: readSupervisorConfig().typeLiteral288:defaultSessionConfig.typeLiteral289:sessionDir.
  readSupervisorConfig.typeLiteral288.defaultSessionConfig.typeLiteral289.noTools: readSupervisorConfig().typeLiteral288:defaultSessionConfig.typeLiteral289:noTools.
---
# Module: [`packages/coding-agent/test/daemon-supervisor-process.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts)

## Functions
- `connectEventually(socketPath: string, child?: ChildProcess | undefined)` — [`L177`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L177)
- `countWorkerDescriptors(agentDir: string)` — [`L135`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L135)
- `quoteShellArgument(argument: string)` — [`L275`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L275)
- `readDaemonLogs(agentDir: string)` — [`L111`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L111)
- `readSupervisorConfig(agentDir: string)` — [`L162`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L162)
- `readWorkerDescriptor(agentDir: string)` — [`L122`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L122)
- `requireSessionList(responseData: unknown)` — [`L225`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L225)
- `requireSummary(responseData: unknown)` — [`L218`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L218)
- `spawnSupervisor(agentDir: string, socketPath: string, cwd: string, extraArgs?: readonly string[])` — [`L78`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L78)
- `startBlockingBash(client: DaemonClient, activeSessionId: string, readyPath: string)` — [`L279`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L279)
- `tempDir()` — [`L72`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L72)
- `waitForCondition(predicate: () => boolean, failureMessage: string, timeoutMs?: number)` — [`L264`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L264)
- `waitForExit(child: ChildProcess)` — [`L236`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L236)
- `waitForProcessGone(pid: number)` — [`L249`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L249)
- `waitForSocketGone(socketPath: string)` — [`L202`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L202)
- `waitForWorkerStopTombstone(agentDir: string)` — [`L146`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L146)

## Module values
- `PROCESS_STRESS_WORKERS` — [`L29`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L29)
- `blockingProcessPath` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L23)
- `childDiagnostics` — [`L28`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L28)
- `children` — [`L25`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L25)
- `cliPath` — [`L21`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L21)
- `daemonSockets` — [`L27`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L27)
- `defaultSessionConfig` — [`L162`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L162)
- `noTools` — [`L162`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L162)
- `sessionDir` — [`L162`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L162)
- `tempDirs` — [`L24`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L24)
- `tsxPath` — [`L22`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L22)
- `workerPids` — [`L26`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-process.test.ts#L26)


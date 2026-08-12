---
title: 'Module: packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/regressions/`4603-worker-recovery.test.ts`/
symbols:
  trackProcess: trackProcess().
  spawnStandaloneWorker: spawnStandaloneWorker().
  spawnSupervisor: spawnSupervisor().
  terminateFixtureProcessTree: terminateFixtureProcessTree().
  ProcessHandle.child: ProcessHandle#child.
  runCli.Promise.typeLiteral556.stderr: runCli().Promise:typeLiteral556:stderr.
  registerFixtureOwnedProcesses: registerFixtureOwnedProcesses().
  fixtureProcessQuietMs: fixtureProcessQuietMs.
  stopFixtureOwnedProcesses: stopFixtureOwnedProcesses().
  createPaths: createPaths().
  terminateTrackedFixtureProcess: terminateTrackedFixtureProcess().
  waitForMessage: waitForMessage().
  fixtureProcessState: fixtureProcessState().
  registerFixtureProcess: registerFixtureProcess().
  waitForFixtureProcessStopped: waitForFixtureProcessStopped().
  connectEventually: connectEventually().
  TestPaths.agentDir: TestPaths#agentDir.
  waitForType: waitForType().
  FixtureProcessIdentity.pid: FixtureProcessIdentity#pid.
  createFrameReader: createFrameReader().
  waitForFixtureProcessExit: waitForFixtureProcessExit().
  createResidentSession: createResidentSession().
  FixtureProcessIdentity: FixtureProcessIdentity#
  signalFixtureProcess: signalFixtureProcess().
  delay: delay().
  TestPaths.registryDir: TestPaths#registryDir.
  waitForExit: waitForExit().
  fixtureProcessKey: fixtureProcessKey().
  decodeResponse: decodeResponse().
  FixtureProcessIdentity.processStartId: FixtureProcessIdentity#processStartId.
  readFixtureProcessSnapshot: readFixtureProcessSnapshot().
  waitForExactProcessExit: waitForExactProcessExit().
  exactProcessIsAlive: exactProcessIsAlive().
  FixtureMessage: FixtureMessage#
  ProcessHandle: ProcessHandle#
  registerFixtureRecord: registerFixtureRecord().
  ProcessHandle.role: ProcessHandle#role.
  TestPaths.socketPath: TestPaths#socketPath.
  ProcessHandle.identity: ProcessHandle#identity.
  fixtureProcesses: fixtureProcesses.
  supervisorRegistryDirEnv: supervisorRegistryDirEnv.
  requireSummary: requireSummary().
  ProcessHandle.messages: ProcessHandle#messages.
  handles: handles.
  ProcessHandle.waiters: ProcessHandle#waiters.
  TestPaths.descriptorDir: TestPaths#descriptorDir.
  fixtureDescendantPids: fixtureDescendantPids().
  isFixtureDescendant: isFixtureDescendant().
  listOwnerRecords: listOwnerRecords().
  readWorkerDescriptor: readWorkerDescriptor().
  harnesses: harnesses.
  runCli: runCli().
  ProcessHandle.stderr: ProcessHandle#stderr.
  FixtureProcessIdentity.role: FixtureProcessIdentity#role.
  FixtureProcessSnapshot.ppid: FixtureProcessSnapshot#ppid.
  waitForType.Promise.Extract.typeLiteral271.type: waitForType().Promise:Extract:typeLiteral271:type.
  ProcessHandle.waiters.Array.typeLiteral10.predicate: ProcessHandle#waiters.Array:typeLiteral10:predicate.
  ProcessHandle.waiters.Array.typeLiteral10.resolve: ProcessHandle#waiters.Array:typeLiteral10:resolve.
  FixtureProcessSnapshot: FixtureProcessSnapshot#
  TestPaths: TestPaths#
  fixturePidIsAlive: fixturePidIsAlive().
  runCli.Promise.typeLiteral556.code: runCli().Promise:typeLiteral556:code.
  createFrameReader.typeLiteral560.waitFor: createFrameReader().typeLiteral560:waitFor.
  waitForPath: waitForPath().
  OwnerRecord: OwnerRecord#
  ProcessHandle.stdout: ProcessHandle#stdout.
  ProcessHandle.waiters.Array.typeLiteral10.timeout: ProcessHandle#waiters.Array:typeLiteral10:timeout.
  tsxPath: tsxPath.
  tsconfigPath: tsconfigPath.
  socketTempDirs: socketTempDirs.
  fixtureDescriptorDirs: fixtureDescriptorDirs.
  fixtureRegistryDirs: fixtureRegistryDirs.
  runCli.Promise.typeLiteral556.stdout: runCli().Promise:typeLiteral556:stdout.
  OwnerRecord.generation: OwnerRecord#generation.
  FixtureProcessSnapshot.state: FixtureProcessSnapshot#state.
  TestPaths.executablePath: TestPaths#executablePath.
  TestPaths.socketTmpDir: TestPaths#socketTmpDir.
  cliPath: cliPath.
  readFixtureDirectory: readFixtureDirectory().
  readFixtureJson: readFixtureJson().
  OwnerRecord.token: OwnerRecord#token.
  OwnerRecord.pid: OwnerRecord#pid.
  OwnerRecord.processStartId: OwnerRecord#processStartId.
  fixturePath: fixturePath.
  fauxExtensionPath: fauxExtensionPath.
  OwnerRecord.socketPath: OwnerRecord#socketPath.
  OwnerRecord.descriptorDir: OwnerRecord#descriptorDir.
  OwnerRecord.agentDir: OwnerRecord#agentDir.
---
# Module: [`packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts)

## Classes
### `FixtureMessage`
- def: [`packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts:53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L53)
- signature: `type FixtureMessage`
- used by: (7 test-only callers)

### `FixtureProcessIdentity`
- def: [`packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts:73`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L73)
- signature: `interface FixtureProcessIdentity`
- members:
  - `pid` — [`L74`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L74)
  - `processStartId` — [`L75`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L75)
  - `role` — [`L76`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L76)
- used by: (13 test-only callers)

### `FixtureProcessSnapshot`
- def: [`packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts:79`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L79)
- signature: `interface FixtureProcessSnapshot`
- members:
  - `ppid` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L80)
  - `state` — [`L81`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L81)
- used by: (4 test-only callers)

### `OwnerRecord`
- def: [`packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts:43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L43)
- signature: `interface OwnerRecord`
- members:
  - `agentDir` — [`L50`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L50)
  - `descriptorDir` — [`L49`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L49)
  - `generation` — [`L45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L45)
  - `pid` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L46)
  - `processStartId` — [`L47`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L47)
  - `socketPath` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L48)
  - `token` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L44)
- used by: (2 test-only callers)

### `ProcessHandle`
- def: [`packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts:59`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L59)
- signature: `interface ProcessHandle`
- members:
  - `child` — [`L60`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L60)
  - `identity` — [`L61`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L61)
  - `messages` — [`L65`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L65)
  - `predicate` — [`L67`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L67)
  - `resolve` — [`L68`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L68)
  - `role` — [`L62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L62)
  - `stderr` — [`L64`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L64)
  - `stdout` — [`L63`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L63)
  - `timeout` — [`L69`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L69)
  - `waiters` — [`L66`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L66)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (11 test-only callers)

### `TestPaths`
- def: [`packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts:84`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L84)
- signature: `interface TestPaths`
- members:
  - `agentDir` — [`L85`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L85)
  - `descriptorDir` — [`L86`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L86)
  - `executablePath` — [`L87`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L87)
  - `registryDir` — [`L88`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L88)
  - `socketPath` — [`L90`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L90)
  - `socketTmpDir` — [`L89`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L89)
- used by: (6 test-only callers)

## Functions
- `connectEventually(socketPath: string)` — [`L579`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L579)
- `createFrameReader(socket: Socket)` — [`L699`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L699)
- `createPaths()` — [`L125`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L125)
- `createResidentSession(client: DaemonClient, agentDir: string)` — [`L648`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L648)
- `decodeResponse(frame: PrivateFrame<DaemonWorkerFrameHeader>)` — [`L744`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L744)
- `delay(ms: number)` — [`L748`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L748)
- `exactProcessIsAlive(pid: number, processStartId: string | undefined)` — [`L627`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L627)
- `fixtureDescendantPids(rootPid: number, processes: Map<number, FixtureProcessSnapshot>)` — [`L312`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L312)
- `fixturePidIsAlive(pid: number)` — [`L456`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L456)
- `fixtureProcessKey(identity: FixtureProcessIdentity)` — [`L227`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L227)
- `fixtureProcessState(identity: FixtureProcessIdentity)` — [`L449`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L449)
- `isFixtureDescendant(pid: number, rootPid: number, processes: Map<number, FixtureProcessSnapshot>)` — [`L331`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L331)
- `listOwnerRecords(registryDir: string)` — [`L597`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L597)
- `readFixtureDirectory(path: string)` — [`L431`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L431)
- `readFixtureJson(path: string)` — [`L440`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L440)
- `readFixtureProcessSnapshot()` — [`L297`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L297)
- `readWorkerDescriptor(descriptorDir: string)` — [`L612`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L612)
- `registerFixtureOwnedProcesses()` — [`L251`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L251)
- `registerFixtureProcess(pid: number | undefined, processStartId: string | undefined, role: "client" | "worker" | "supervisor")` — [`L231`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L231)
- `registerFixtureRecord(value: unknown, role: "worker" | "supervisor", path: string)` — [`L280`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L280)
- `requireSummary(value: unknown)` — [`L620`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L620)
- `runCli(paths: TestPaths, args: string[], timeoutMs?: number, extraEnv?: ProcessEnv)` — [`L673`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L673)
- `signalFixtureProcess(identity: FixtureProcessIdentity, signal: Signals)` — [`L344`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L344)
- `spawnStandaloneWorker(paths: TestPaths, workerSocketPath: string, token: string, extraEnv?: ProcessEnv)` — [`L171`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L171)
- `spawnSupervisor(paths: TestPaths)` — [`L148`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L148)
- `stopFixtureOwnedProcesses()` — [`L468`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L468)
- `terminateFixtureProcessTree(root: FixtureProcessIdentity)` — [`L359`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L359)
- `terminateTrackedFixtureProcess(handle: ProcessHandle)` — [`L497`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L497)
- `trackProcess(child: ChildProcess, role: "client" | "worker" | "supervisor")` — [`L202`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L202)
- `waitForExactProcessExit(pid: number, processStartId: string | undefined, timeoutMs?: number)` — [`L634`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L634)
- `waitForExit(handle: ProcessHandle, timeoutMs?: number)` — [`L553`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L553)
- `waitForFixtureProcessExit(identity: FixtureProcessIdentity)` — [`L509`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L509)
- `waitForFixtureProcessStopped(identity: FixtureProcessIdentity, timeoutMs?: number)` — [`L414`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L414)
- `waitForMessage(handle: ProcessHandle, predicate: (message: FixtureMessage) => boolean, timeoutMs?: number)` — [`L520`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L520)
- `waitForPath(path: string, timeoutMs?: number)` — [`L569`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L569)
- `waitForType(handle: ProcessHandle, type: T, timeoutMs?: number | undefined)` — [`L538`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L538)

## Module values
- `cliPath` — [`L95`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L95)
- `code` — [`L678`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L678)
- `fauxExtensionPath` — [`L94`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L94)
- `fixtureDescriptorDirs` — [`L102`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L102)
- `fixturePath` — [`L93`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L93)
- `fixtureProcessQuietMs` — [`L106`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L106)
- `fixtureProcesses` — [`L103`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L103)
- `fixtureRegistryDirs` — [`L104`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L104)
- `handles` — [`L99`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L99)
- `harnesses` — [`L100`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L100)
- `socketTempDirs` — [`L101`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L101)
- `stderr` — [`L678`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L678)
- `stdout` — [`L678`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L678)
- `supervisorRegistryDirEnv` — [`L98`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L98)
- `tsconfigPath` — [`L97`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L97)
- `tsxPath` — [`L96`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L96)
- `type` — [`L542`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L542)
- `waitFor` — [`L700`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4603-worker-recovery.test.ts#L700)


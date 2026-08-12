---
title: 'Module: packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/regressions/`4600-supervisor-singleton.test.ts`/
symbols:
  createPaths.Promise.typeLiteral123.registryDir: createPaths().Promise:typeLiteral123:registryDir.
  spawnFixture.options-typeLiteral48.generation: spawnFixture().(options)typeLiteral48:generation.
  createPaths.Promise.typeLiteral123.socketPath: createPaths().Promise:typeLiteral123:socketPath.
  spawnRealSupervisor: spawnRealSupervisor().
  waitForType: waitForType().
  cleanupSupervisorSockets: cleanupSupervisorSockets.
  waitForMessage: waitForMessage().
  removeDeadFixtureOwnerRecords: removeDeadFixtureOwnerRecords().
  registerOwnerRecordsForCleanup: registerOwnerRecordsForCleanup().
  createPaths.Promise.typeLiteral123.agentDir: createPaths().Promise:typeLiteral123:agentDir.
  cleanupRegisteredProcesses: cleanupRegisteredProcesses().
  send: send().
  waitForExit: waitForExit().
  waitForCleanupProcessExit: waitForCleanupProcessExit().
  stopSupervisor: stopSupervisor().
  dispatchMessage: dispatchMessage().
  forceShutdownReachableSupervisor: forceShutdownReachableSupervisor().
  captureCleanupProcess: captureCleanupProcess().
  createPaths: createPaths().
  cleanupProcessState: cleanupProcessState().
  OwnerRecord.generation: OwnerRecord#generation.
  writeOwnerRecord: writeOwnerRecord().
  releaseOwnershipHolder: releaseOwnershipHolder().
  connectEventually: connectEventually().
  OwnerRecord.processStartId: OwnerRecord#processStartId.
  spawnFixture: spawnFixture().
  FixtureMessage: FixtureMessage#
  FixtureHandle: FixtureHandle#
  FixtureHandle.child: FixtureHandle#child.
  listOwnerRecords: listOwnerRecords().
  registerCleanupProcess: registerCleanupProcess().
  cleanupIdentityKey: cleanupIdentityKey().
  OwnerRecord.pid: OwnerRecord#pid.
  FixtureHandle.diagnostics: FixtureHandle#diagnostics.
  cleanupProcesses: cleanupProcesses.
  FixtureHandle.messages: FixtureHandle#messages.
  waitForCleanupGracePeriod: waitForCleanupGracePeriod().
  OwnerRecord.token: OwnerRecord#token.
  FixtureHandle.diagnostics.typeLiteral16.stderr: FixtureHandle#diagnostics.typeLiteral16:stderr.
  CleanupProcessIdentity.pid: CleanupProcessIdentity#pid.
  createPaths.Promise.typeLiteral123.descriptorDir: createPaths().Promise:typeLiteral123:descriptorDir.
  readOwnerRecord: readOwnerRecord().
  OwnerRecord: OwnerRecord#
  FixtureHandle.waiters: FixtureHandle#waiters.
  CleanupProcessIdentity: CleanupProcessIdentity#
  waitForConnectionStatus: waitForConnectionStatus().
  requireSessionSummary: requireSessionSummary().
  ownerRecordPath: ownerRecordPath().
  waitForOwnerCount: waitForOwnerCount().
  handles: handles.
  OwnerRecord.socketPath: OwnerRecord#socketPath.
  CleanupProcessIdentity.processStartId: CleanupProcessIdentity#processStartId.
  harnesses: harnesses.
  cleanupRegistryDirs: cleanupRegistryDirs.
  waitForType.Promise.Extract.typeLiteral105.type: waitForType().Promise:Extract:typeLiteral105:type.
  FixtureHandle.waiters.Array.typeLiteral17.predicate: FixtureHandle#waiters.Array:typeLiteral17:predicate.
  FixtureHandle.waiters.Array.typeLiteral17.resolve: FixtureHandle#waiters.Array:typeLiteral17:resolve.
  FixtureHandle.diagnostics.typeLiteral16.stdout: FixtureHandle#diagnostics.typeLiteral16:stdout.
  CleanupProcessIdentity.label: CleanupProcessIdentity#label.
  readStableIdentity: readStableIdentity().
  FixtureHandle.waiters.Array.typeLiteral17.timeout: FixtureHandle#waiters.Array:typeLiteral17:timeout.
  spawnFixture.paths-typeLiteral47.agentDir: spawnFixture().(paths)typeLiteral47:agentDir.
  assertConnectable: assertConnectable().
  tsxPath: tsxPath.
  tsconfigPath: tsconfigPath.
  supervisorRegistryDirEnv: supervisorRegistryDirEnv.
  spawnFixture.paths-typeLiteral47.registryDir: spawnFixture().(paths)typeLiteral47:registryDir.
  spawnRealSupervisor.paths-typeLiteral67.agentDir: spawnRealSupervisor().(paths)typeLiteral67:agentDir.
  OwnerRecord.descriptorDir: OwnerRecord#descriptorDir.
  FixtureHandle.waiters.Array.typeLiteral17.reject: FixtureHandle#waiters.Array:typeLiteral17:reject.
  fixturePath: fixturePath.
  fauxExtensionPath: fauxExtensionPath.
  cliPath: cliPath.
  spawnFixture.paths-typeLiteral47.descriptorDir: spawnFixture().(paths)typeLiteral47:descriptorDir.
  spawnFixture.paths-typeLiteral47.socketPath: spawnFixture().(paths)typeLiteral47:socketPath.
  spawnFixture.options-typeLiteral48.extraEnv: spawnFixture().(options)typeLiteral48:extraEnv.
  spawnRealSupervisor.paths-typeLiteral67.registryDir: spawnRealSupervisor().(paths)typeLiteral67:registryDir.
  spawnRealSupervisor.paths-typeLiteral67.socketPath: spawnRealSupervisor().(paths)typeLiteral67:socketPath.
  ownerScopePath: ownerScopePath().
  waitForPath: waitForPath().
  OwnerRecord.version: OwnerRecord#version.
  OwnerRecord.role: OwnerRecord#role.
  OwnerRecord.agentDir: OwnerRecord#agentDir.
  OwnerRecord.appVersion: OwnerRecord#appVersion.
  OwnerRecord.phase: OwnerRecord#phase.
  OwnerRecord.createdAt: OwnerRecord#createdAt.
  OwnerRecord.updatedAt: OwnerRecord#updatedAt.
---
# Module: [`packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts)

## Classes
### `CleanupProcessIdentity`
- def: [`packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts:64`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L64)
- signature: `interface CleanupProcessIdentity`
- members:
  - `label` — [`L67`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L67)
  - `pid` — [`L65`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L65)
  - `processStartId` — [`L66`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L66)
- used by: (9 test-only callers)

### `FixtureHandle`
- def: [`packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts:52`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L52)
- signature: `interface FixtureHandle`
- members:
  - `child` — [`L53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L53)
  - `diagnostics` — [`L54`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L54)
  - `messages` — [`L55`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L55)
  - `predicate` — [`L57`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L57)
  - `reject` — [`L59`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L59)
  - `resolve` — [`L58`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L58)
  - `stderr` — [`L54`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L54)
  - `stdout` — [`L54`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L54)
  - `timeout` — [`L60`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L60)
  - `waiters` — [`L56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L56)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (12 test-only callers)

### `FixtureMessage`
- def: [`packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts:28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L28)
- signature: `type FixtureMessage`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (8 test-only callers)

### `OwnerRecord`
- def: [`packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts:36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L36)
- signature: `interface OwnerRecord`
- members:
  - `agentDir` — [`L45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L45)
  - `appVersion` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L46)
  - `createdAt` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L48)
  - `descriptorDir` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L44)
  - `generation` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L40)
  - `phase` — [`L47`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L47)
  - `pid` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L41)
  - `processStartId` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L42)
  - `role` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L38)
  - `socketPath` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L43)
  - `token` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L39)
  - `updatedAt` — [`L49`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L49)
  - `version` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L37)
- used by: (8 test-only callers)

## Functions
- `assertConnectable(socketPath: string)` — [`L276`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L276)
- `captureCleanupProcess(pid: number, label: string, timeoutMs?: number)` — [`L387`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L387)
- `cleanupIdentityKey(identity: Pick<CleanupProcessIdentity, "pid" | "processStartId">)` — [`L378`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L378)
- `cleanupProcessState(identity: CleanupProcessIdentity)` — [`L412`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L412)
- `cleanupRegisteredProcesses(existingClient?: DaemonClient | undefined)` — [`L489`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L489)
- `connectEventually(socketPath: string)` — [`L287`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L287)
- `createPaths()` — [`L257`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L257)
- `dispatchMessage(handle: FixtureHandle, message: FixtureMessage)` — [`L112`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L112)
- `forceShutdownReachableSupervisor(socketPath: string, existingClient?: DaemonClient | undefined)` — [`L510`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L510)
- `listOwnerRecords(registryDir: string)` — [`L357`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L357)
- `ownerRecordPath(registryDir: string, generation: string)` — [`L341`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L341)
- `ownerScopePath(registryDir: string, generation: string)` — [`L345`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L345)
- `readOwnerRecord(registryDir: string, generation: string)` — [`L349`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L349)
- `readStableIdentity(target: object, property: "clientId" | "protocolClientId")` — [`L326`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L326)
- `registerCleanupProcess(identity: CleanupProcessIdentity)` — [`L382`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L382)
- `registerOwnerRecordsForCleanup(registryDir: string)` — [`L399`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L399)
- `releaseOwnershipHolder(handle: FixtureHandle)` — [`L545`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L545)
- `removeDeadFixtureOwnerRecords(registryDir: string)` — [`L427`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L427)
- `requireSessionSummary(value: unknown)` — [`L334`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L334)
- `send(handle: FixtureHandle, type: "release" | "shutdown" | "go" | "cleanup" | "probe")` — [`L253`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L253)
- `spawnFixture(mode: "supervisor" | "owner" | "legacy_cleanup", paths: { agentDir: string; descriptorDir: string; registryDir: string; socketPath: string; }, options?: { extraEnv?: ProcessEnv | undefined; generation?: string | undefined; })` — [`L126`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L126)
- `spawnRealSupervisor(paths: { agentDir: string; registryDir: string; socketPath: string; }, extraEnv: ProcessEnv)` — [`L166`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L166)
- `stopSupervisor(handle: FixtureHandle, socketPath: string)` — [`L552`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L552)
- `waitForCleanupGracePeriod(timeoutMs?: number)` — [`L474`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L474)
- `waitForCleanupProcessExit(identity: CleanupProcessIdentity, timeoutMs?: number)` — [`L463`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L463)
- `waitForConnectionStatus(connection: DaemonAgentConnection, status: "reconnecting" | "connected", timeoutMs?: number)` — [`L305`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L305)
- `waitForExit(handle: FixtureHandle, timeoutMs?: number)` — [`L237`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L237)
- `waitForMessage(handle: FixtureHandle, predicate: (message: FixtureMessage) => boolean, timeoutMs?: number)` — [`L202`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L202)
- `waitForOwnerCount(registryDir: string, count: number, timeoutMs?: number)` — [`L366`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L366)
- `waitForPath(path: string, timeoutMs?: number)` — [`L531`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L531)
- `waitForType(handle: FixtureHandle, type: T, timeoutMs?: number | undefined)` — [`L227`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L227)
- `writeOwnerRecord(registryDir: string, owner: OwnerRecord)` — [`L541`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L541)

## Module values
- `agentDir` — [`L128`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L128)
- `agentDir` — [`L167`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L167)
- `agentDir` — [`L258`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L258)
- `cleanupProcesses` — [`L78`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L78)
- `cleanupRegistryDirs` — [`L79`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L79)
- `cleanupSupervisorSockets` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L80)
- `cliPath` — [`L72`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L72)
- `descriptorDir` — [`L128`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L128)
- `descriptorDir` — [`L259`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L259)
- `extraEnv` — [`L129`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L129)
- `fauxExtensionPath` — [`L71`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L71)
- `fixturePath` — [`L70`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L70)
- `generation` — [`L129`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L129)
- `handles` — [`L76`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L76)
- `harnesses` — [`L77`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L77)
- `registryDir` — [`L128`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L128)
- `registryDir` — [`L167`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L167)
- `registryDir` — [`L260`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L260)
- `socketPath` — [`L128`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L128)
- `socketPath` — [`L167`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L167)
- `socketPath` — [`L261`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L261)
- `supervisorRegistryDirEnv` — [`L75`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L75)
- `tsconfigPath` — [`L74`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L74)
- `tsxPath` — [`L73`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L73)
- `type` — [`L231`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4600-supervisor-singleton.test.ts#L231)


---
title: 'Module: packages/coding-agent/src/cli/owned-session-worker.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/owned-session-worker.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`owned-session-worker.ts`/
symbols:
  runOwnedSessionWorkerFrontend: runOwnedSessionWorkerFrontend().
  writeOwnedRecoveryDescriptor: writeOwnedRecoveryDescriptor().
  installOwnedSessionRecoveryTracking: installOwnedSessionRecoveryTracking().
  classifyOwnedSessionWorkerInvocation: classifyOwnedSessionWorkerInvocation().
  readOwnedRecoveryDescriptor: readOwnedRecoveryDescriptor().
  isOwnedSessionWorkerProcess: isOwnedSessionWorkerProcess().
  maybeRunOwnedSessionWorkerFrontend: maybeRunOwnedSessionWorkerFrontend().
  installOwnedSessionWorkerOwnerWatch: installOwnedSessionWorkerOwnerWatch().
  hasNonSessionOperation: hasNonSessionOperation().
  createOwnedWorkerLaunchSpec: createOwnedWorkerLaunchSpec().
  closeOwnedSessionWorkerOwnerWatch: closeOwnedSessionWorkerOwnerWatch().
  NON_SESSION_COMMANDS: NON_SESSION_COMMANDS.
  OwnedSessionWorkerProfile: OwnedSessionWorkerProfile#
  OwnedSessionRecoveryDescriptor.sessionFile: OwnedSessionRecoveryDescriptor#sessionFile.
  exitCodeForSignal: exitCodeForSignal().
  closeOwnerWatch: closeOwnerWatch.
  OwnedSessionRecoveryDescriptor: OwnedSessionRecoveryDescriptor#
  OwnedSessionRecoveryDescriptor.profile: OwnedSessionRecoveryDescriptor#profile.
  OwnedWorkerLaunchSpec: OwnedWorkerLaunchSpec#
  createRpcRecoveryArgs: createRpcRecoveryArgs().
  OWNED_WORKER_ENV: OWNED_WORKER_ENV.
  OWNED_RECOVERY_DESCRIPTOR_ENV: OWNED_RECOVERY_DESCRIPTOR_ENV.
  OWNED_PROFILE_ENV: OWNED_PROFILE_ENV.
  OwnedSessionRecoveryDescriptor.version: OwnedSessionRecoveryDescriptor#version.
  OwnedSessionRecoveryDescriptor.sessionId: OwnedSessionRecoveryDescriptor#sessionId.
  OwnedSessionRecoveryDescriptor.cwd: OwnedSessionRecoveryDescriptor#cwd.
  OwnedSessionRecoveryDescriptor.updatedAt: OwnedSessionRecoveryDescriptor#updatedAt.
  NON_SESSION_FLAGS: NON_SESSION_FLAGS.
  valueAfter: valueAfter().
  isStartupBenchmark: isStartupBenchmark().
  forwardSignal: forwardSignal().
---
# Module: [`packages/coding-agent/src/cli/owned-session-worker.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts)

## Classes
### `OwnedSessionRecoveryDescriptor`
- def: [`packages/coding-agent/src/cli/owned-session-worker.ts:31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L31)
- signature: `interface OwnedSessionRecoveryDescriptor`
- members:
  - `cwd` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L36)
  - `profile` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L33)
  - `sessionFile` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L35)
  - `sessionId` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L34)
  - `updatedAt` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L37)
  - `version` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L32)
- uses (calls/refs, reference-scoped): [`OwnedSessionWorkerProfile`](owned-session-worker.ts.md#OwnedSessionWorkerProfile)
- used by: [`runOwnedSessionWorkerFrontend`](owned-session-worker.ts.md#runOwnedSessionWorkerFrontend), [`writeOwnedRecoveryDescriptor`](owned-session-worker.ts.md#writeOwnedRecoveryDescriptor), [`readOwnedRecoveryDescriptor`](owned-session-worker.ts.md#readOwnedRecoveryDescriptor)

### `OwnedSessionWorkerProfile`
- def: [`packages/coding-agent/src/cli/owned-session-worker.ts:25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L25)
- signature: `type OwnedSessionWorkerProfile`
- used by: [`runOwnedSessionWorkerFrontend`](owned-session-worker.ts.md#runOwnedSessionWorkerFrontend), [`writeOwnedRecoveryDescriptor`](owned-session-worker.ts.md#writeOwnedRecoveryDescriptor), [`installOwnedSessionRecoveryTracking`](owned-session-worker.ts.md#installOwnedSessionRecoveryTracking), [`classifyOwnedSessionWorkerInvocation`](owned-session-worker.ts.md#classifyOwnedSessionWorkerInvocation), [`profile`](owned-session-worker.ts.md#OwnedSessionRecoveryDescriptor.profile)

### `OwnedWorkerLaunchSpec`
- def: [`packages/coding-agent/src/cli/owned-session-worker.ts:93`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L93)
- signature: `type OwnedWorkerLaunchSpec`
- uses (calls/refs, reference-scoped): [`CliSubprocessLaunchSpec`](subprocess-launch.ts.md#CliSubprocessLaunchSpec)
- used by: [`createOwnedWorkerLaunchSpec`](owned-session-worker.ts.md#createOwnedWorkerLaunchSpec)

## Functions
- `classifyOwnedSessionWorkerInvocation(args: readonly string[], stdinIsTTY: boolean | undefined, environment?: ProcessEnv)` — [`L65`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L65)
- `closeOwnedSessionWorkerOwnerWatch()` — [`L538`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L538)
- `createOwnedWorkerLaunchSpec(args: readonly string[], executable?: string, execArgs?: readonly string[], entrypoint?: string)` — [`L95`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L95)
- `createRpcRecoveryArgs(args: readonly string[], sessionPath: string)` — [`L161`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L161)
- `exitCodeForSignal(signal: Signals | null)` — [`L180`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L180)
- `forwardSignal(child: ChildProcess, signal: Signals)` — [`L193`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L193)
- `hasNonSessionOperation(args: readonly string[])` — [`L49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L49)
- `installOwnedSessionRecoveryTracking(runtime: AgentSessionRuntime)` — [`L136`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L136)
- `installOwnedSessionWorkerOwnerWatch()` — [`L494`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L494)
- `isOwnedSessionWorkerProcess(environment?: ProcessEnv)` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L27)
- `isStartupBenchmark(environment: ProcessEnv)` — [`L60`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L60)
- `maybeRunOwnedSessionWorkerFrontend(args: readonly string[], forceLegacyFrontend?: boolean)` — [`L479`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L479)
- `readOwnedRecoveryDescriptor(path: string)` — [`L104`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L104)
- `runOwnedSessionWorkerFrontend(args: readonly string[], profile: OwnedSessionWorkerProfile)` — [`L199`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L199)
- `valueAfter(args: readonly string[], flag: string)` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L44)
- `writeOwnedRecoveryDescriptor(path: string, profile: OwnedSessionWorkerProfile, session: AgentSession)` — [`L121`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L121)

## Module values
- `NON_SESSION_COMMANDS` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L42)
- `NON_SESSION_FLAGS` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L40)
- `OWNED_PROFILE_ENV` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L21)
- `OWNED_RECOVERY_DESCRIPTOR_ENV` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L20)
- `OWNED_WORKER_ENV` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L19)
- `closeOwnerWatch` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/owned-session-worker.ts#L23)


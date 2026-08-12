---
title: 'Module: packages/coding-agent/src/core/session-lease.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/session-lease.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`session-lease.ts`/
symbols:
  acquireSessionLease: acquireSessionLease().
  getProcessStartId: getProcessStartId().
  canonicalSessionPath: canonicalSessionPath().
  SessionLease.release: SessionLease#release().
  SESSION_LEASES_ENABLED_ENV: SESSION_LEASES_ENABLED_ENV.
  SESSION_LEASE_OWNER_ID_ENV: SESSION_LEASE_OWNER_ID_ENV.
  readLeaseOwner: readLeaseOwner().
  isLeaseOwnerAlive: isLeaseOwnerAlive().
  SessionAlreadyActiveError: SessionAlreadyActiveError#
  SessionLease: SessionLease#
  getWindowsProcessStartId: getWindowsProcessStartId().
  getCurrentProcessStartId: getCurrentProcessStartId().
  SessionLeaseOwner: SessionLeaseOwner#
  SessionLeaseOwner.pid: SessionLeaseOwner#pid.
  SessionAlreadyActiveError.-constructor: SessionAlreadyActiveError#`<constructor>`().
  leasesEnabled: leasesEnabled().
  SessionLeaseOwner.token: SessionLeaseOwner#token.
  SessionLeaseOwner.processStartId: SessionLeaseOwner#processStartId.
  SessionLeaseOwner.activeSessionId: SessionLeaseOwner#activeSessionId.
  SessionLeaseOwner.version: SessionLeaseOwner#version.
  SessionLeaseOwner.sessionPath: SessionLeaseOwner#sessionPath.
  SessionLeaseOwner.createdAt: SessionLeaseOwner#createdAt.
  SessionLease.released: SessionLease#released.
  SessionLease.-constructor: SessionLease#`<constructor>`().
  runProcessQuery: runProcessQuery().
  currentProcessStartId: currentProcessStartId.
  currentProcessStartIdRead: currentProcessStartIdRead.
  withLeaseGuard: withLeaseGuard().
  leaseDirectory: leaseDirectory().
  isProcessAlive: isProcessAlive().
  ProcessQuery: ProcessQuery#
  reclaimStaleLease: reclaimStaleLease().
  SessionAlreadyActiveError.code: SessionAlreadyActiveError#code.
---
# Module: [`packages/coding-agent/src/core/session-lease.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts)

## Classes
### `ProcessQuery`
- def: [`packages/coding-agent/src/core/session-lease.ts:113`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L113)
- signature: `type ProcessQuery`
- used by: [`getWindowsProcessStartId`](session-lease.ts.md#getWindowsProcessStartId)

### `SessionAlreadyActiveError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/core/session-lease.ts:20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L20)
- signature: `class SessionAlreadyActiveError`
- members:
  - `<constructor>(sessionPath: string, activeSessionId?: string | undefined)` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L23)
  - `code` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L21)
- used by: [`main`](../main.ts.md#main), [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`daemon-supervisor.ts`](../modes/daemon/daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`daemon-agent-connection.ts`](../modes/agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`acquireSessionLease`](session-lease.ts.md#acquireSessionLease), [`serializeDaemonError`](../modes/daemon/daemon-errors.ts.md#serializeDaemonError), [`daemon-errors.ts`](../modes/daemon/daemon-errors.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-errors.ts), [`deserializeDaemonError`](../modes/daemon/daemon-errors.ts.md#deserializeDaemonError), [`reuseWorkerForCreate`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.reuseWorkerForCreate), [`cancelled`](../modes/agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.switchSession.Promise.typeLiteral664.cancelled)  (2 test-only)

### `SessionLease`
- def: [`packages/coding-agent/src/core/session-lease.ts:36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L36)
- signature: `class SessionLease`
- members:
  - `<constructor>(sessionPath: string, directory: string, token: string)` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L39)
  - `release(method)` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L45)
  - `released` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L37)
- uses (calls/refs, reference-scoped): [`readLeaseOwner`](session-lease.ts.md#readLeaseOwner), [`token`](session-lease.ts.md#SessionLeaseOwner.token), [`withLeaseGuard`](session-lease.ts.md#withLeaseGuard)
- used by: [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`createRuntime`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRuntime), [`rehydrateCompletedRlmSubagentOnce`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.rehydrateCompletedRlmSubagentOnce), [`agent-session-runtime.ts`](agent-session-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-runtime.ts), [`createAgentSessionRuntime`](agent-session-runtime.ts.md#createAgentSessionRuntime), [`acquireSessionLease`](session-lease.ts.md#acquireSessionLease), [`<constructor>`](agent-session-runtime.ts.md#AgentSessionRuntime.-constructor), [`acquireReplacementLease`](agent-session-runtime.ts.md#AgentSessionRuntime.acquireReplacementLease), [`buildAndApplyReplacement`](agent-session-runtime.ts.md#AgentSessionRuntime.buildAndApplyReplacement), [`teardownForReplacement`](agent-session-runtime.ts.md#AgentSessionRuntime.teardownForReplacement), [`releaseUncommittedLease`](agent-session-runtime.ts.md#AgentSessionRuntime.releaseUncommittedLease), [`commitReplacementLease`](agent-session-runtime.ts.md#AgentSessionRuntime.commitReplacementLease), [`releaseSessionLease`](agent-session-runtime.ts.md#AgentSessionRuntime.releaseSessionLease)  (5 test-only)

### `SessionLeaseOwner`
- def: [`packages/coding-agent/src/core/session-lease.ts:10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L10)
- signature: `interface SessionLeaseOwner`
- members:
  - `activeSessionId` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L15)
  - `createdAt` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L17)
  - `pid` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L13)
  - `processStartId` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L14)
  - `sessionPath` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L16)
  - `token` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L12)
  - `version` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L11)
- used by: [`acquireSessionLease`](session-lease.ts.md#acquireSessionLease), [`release`](session-lease.ts.md#SessionLease.release), [`readLeaseOwner`](session-lease.ts.md#readLeaseOwner), [`isLeaseOwnerAlive`](session-lease.ts.md#isLeaseOwnerAlive)

## Functions
- `acquireSessionLease(sessionPath: string | undefined, agentDir: string, environment?: ProcessEnv)` — [`L232`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L232)
- `canonicalSessionPath(sessionPath: string)` — [`L73`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L73)
- `getCurrentProcessStartId()` — [`L169`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L169)
- `getProcessStartId(pid: number)` — [`L140`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L140)
- `getWindowsProcessStartId(pid: number, query?: ProcessQuery)` — [`L122`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L122)
- `isLeaseOwnerAlive(owner: SessionLeaseOwner)` — [`L177`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L177)
- `isProcessAlive(pid: number)` — [`L104`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L104)
- `leaseDirectory(agentDir: string, sessionPath: string)` — [`L68`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L68)
- `leasesEnabled(environment: ProcessEnv)` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L63)
- `readLeaseOwner(directory: string)` — [`L86`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L86)
- `reclaimStaleLease(directory: string)` — [`L218`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L218)
- `runProcessQuery(command: string, args: string[])` — [`L115`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L115)
- `withLeaseGuard(directory: string, action: () => T)` — [`L188`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L188)

## Module values
- `SESSION_LEASES_ENABLED_ENV` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L7)
- `SESSION_LEASE_OWNER_ID_ENV` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L8)
- `currentProcessStartId` — [`L166`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L166)
- `currentProcessStartIdRead` — [`L167`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-lease.ts#L167)


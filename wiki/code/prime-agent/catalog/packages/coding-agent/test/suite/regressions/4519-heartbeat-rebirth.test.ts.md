---
title: 'Module: packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/regressions/`4519-heartbeat-rebirth.test.ts`/
symbols:
  createDaemon: createDaemon().
  createDueHeartbeat.input-typeLiteral4.cwd: createDueHeartbeat().(input)typeLiteral4:cwd.
  AgentDaemonCronInternals.typeLiteral0.cronStore: AgentDaemonCronInternals#typeLiteral0:cronStore.
  runtimeResult: runtimeResult().
  AgentDaemonCronInternals.typeLiteral0.sessions: AgentDaemonCronInternals#typeLiteral0:sessions.
  createDueHeartbeat: createDueHeartbeat().
  AgentDaemonCronInternals: AgentDaemonCronInternals#
  AgentDaemonCronInternals.typeLiteral0.cronScheduler: AgentDaemonCronInternals#typeLiteral0:cronScheduler.
  AgentDaemonCronInternals.typeLiteral0.withAgentMessagePreparingGuard: AgentDaemonCronInternals#typeLiteral0:withAgentMessagePreparingGuard().
  createDueHeartbeat.input-typeLiteral4.activeSessionId: createDueHeartbeat().(input)typeLiteral4:activeSessionId.
  createDueHeartbeat.input-typeLiteral4.sessionId: createDueHeartbeat().(input)typeLiteral4:sessionId.
  createDueHeartbeat.input-typeLiteral4.sessionFile: createDueHeartbeat().(input)typeLiteral4:sessionFile.
  AgentDaemonCronInternals.typeLiteral0.createRuntime.command-typeLiteral1.sessionPath: AgentDaemonCronInternals#typeLiteral0:createRuntime().(command)typeLiteral1:sessionPath.
  AgentDaemonCronInternals.typeLiteral0.runCronJob: AgentDaemonCronInternals#typeLiteral0:runCronJob().
  waitForCondition: waitForCondition().
  AgentDaemonCronInternals.typeLiteral0.agentMessagePreparingTargets: AgentDaemonCronInternals#typeLiteral0:agentMessagePreparingTargets.
  AgentDaemonCronInternals.typeLiteral0.agentMessageTargetLocks: AgentDaemonCronInternals#typeLiteral0:agentMessageTargetLocks.
  AgentDaemonCronInternals.typeLiteral0.createRuntime: AgentDaemonCronInternals#typeLiteral0:createRuntime().
  AgentDaemonCronInternals.typeLiteral0.createRuntime.command-typeLiteral1.type: AgentDaemonCronInternals#typeLiteral0:createRuntime().(command)typeLiteral1:type.
---
# Module: [`packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts)

## Classes
### `AgentDaemonCronInternals`
- def: [`packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts:11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L11)
- signature: `type AgentDaemonCronInternals`
- members:
  - `createRuntime(method)` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L16)
  - `runCronJob(method)` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L18)
  - `withAgentMessagePreparingGuard(method)` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L19)
  - `agentMessagePreparingTargets` — [`L12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L12)
  - `agentMessageTargetLocks` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L13)
  - `cronScheduler` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L15)
  - `cronStore` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L14)
  - `sessionPath` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L16)
  - `sessions` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L17)
  - `type` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L16)
- uses (calls/refs, reference-scoped): [`ActiveSessionState`](../../../src/modes/daemon/active-session-state.ts.md#ActiveSessionState), [`AgentCronJob`](../../../src/core/cron-jobs.ts.md#AgentCronJob), [`AgentSession`](../../../src/core/agent-session.ts.md#AgentSession), [`AgentCronJobStore`](../../../src/core/cron-jobs.ts.md#AgentCronJobStore), [`AgentCronScheduler`](../../../src/core/cron-jobs.ts.md#AgentCronScheduler)
- used by: (1 test-only callers)

## Functions
- `createDaemon(harness: Harness, createRuntime: CreateAgentSessionRuntimeFactory)` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L26)
- `createDueHeartbeat(store: AgentCronJobStore, input: { activeSessionId: string; sessionId: string; sessionFile: string; cwd: string; })` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L37)
- `runtimeResult(harness: Harness, cwd: string, agentDir: string)` — [`L49`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L49)
- `waitForCondition(predicate: () => boolean)` — [`L58`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L58)

## Module values
- `activeSessionId` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L39)
- `cwd` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L39)
- `sessionFile` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L39)
- `sessionId` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4519-heartbeat-rebirth.test.ts#L39)


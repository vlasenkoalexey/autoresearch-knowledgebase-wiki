---
title: 'Module: packages/coding-agent/test/suite/regressions/4657-update-heartbeat-recovery.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/regressions/4657-update-heartbeat-recovery.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/regressions/`4657-update-heartbeat-recovery.test.ts`/
symbols:
  AgentDaemonCronInternals.typeLiteral0.rebindCronJobsToState: AgentDaemonCronInternals#typeLiteral0:rebindCronJobsToState().
  AgentDaemonCronInternals.typeLiteral0.cronStore: AgentDaemonCronInternals#typeLiteral0:cronStore.
  AgentDaemonCronInternals.typeLiteral0.cronScheduler: AgentDaemonCronInternals#typeLiteral0:cronScheduler.
  AgentDaemonCronInternals: AgentDaemonCronInternals#
  AgentDaemonCronInternals.typeLiteral0.sessions: AgentDaemonCronInternals#typeLiteral0:sessions.
  AgentDaemonCronInternals.typeLiteral0.registerCronStoreForState: AgentDaemonCronInternals#typeLiteral0:registerCronStoreForState().
  waitFor: waitFor().
---
# Module: [`packages/coding-agent/test/suite/regressions/4657-update-heartbeat-recovery.test.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4657-update-heartbeat-recovery.test.ts)

## Classes
### `AgentDaemonCronInternals`
- def: [`packages/coding-agent/test/suite/regressions/4657-update-heartbeat-recovery.test.ts:9`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4657-update-heartbeat-recovery.test.ts#L9)
- signature: `type AgentDaemonCronInternals`
- members:
  - `rebindCronJobsToState(method)` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4657-update-heartbeat-recovery.test.ts#L14)
  - `registerCronStoreForState(method)` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4657-update-heartbeat-recovery.test.ts#L13)
  - `cronScheduler` — [`L12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4657-update-heartbeat-recovery.test.ts#L12)
  - `cronStore` — [`L11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4657-update-heartbeat-recovery.test.ts#L11)
  - `sessions` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4657-update-heartbeat-recovery.test.ts#L10)
- uses (calls/refs, reference-scoped): [`activeSessionId`](../../../src/modes/daemon/active-session-state.ts.md#ActiveSessionState.activeSessionId), [`runtime`](../../../src/modes/daemon/active-session-state.ts.md#ActiveSessionState.runtime), [`ActiveSessionState`](../../../src/modes/daemon/active-session-state.ts.md#ActiveSessionState), [`fauxAssistantMessage`](../../../../ai/src/providers/faux.ts.md#fauxAssistantMessage), [`id`](../../../src/core/cron-jobs.ts.md#AgentCronJob.id), [`cwd`](../../../src/core/agent-session-config.ts.md#AgentSessionRuntimeConfig.cwd), [`<constructor>`](../../../src/modes/daemon/daemon-mode.ts.md#AgentDaemon.-constructor), [`agentDir`](../../../src/core/agent-session-config.ts.md#AgentSessionRuntimeConfig.agentDir), [`defaultSessionConfig`](../../../src/modes/daemon/daemon-mode.ts.md#DaemonModeOptions.defaultSessionConfig), [`createRuntime`](../../../src/modes/daemon/daemon-mode.ts.md#DaemonModeOptions.createRuntime), [`<get>sessionFile`](../../../src/core/agent-session.ts.md#AgentSession.-get-sessionFile), [`createHeartbeat`](../../../src/core/cron-jobs.ts.md#AgentCronJobStore.createHeartbeat), [`<get>sessionId`](../../../src/core/agent-session.ts.md#AgentSession.-get-sessionId), [`prompt`](../../../src/core/cron-jobs.ts.md#CreateAgentCronJobInput.prompt), [`activeSessionId`](../../../src/core/cron-jobs.ts.md#CreateAgentCronJobInput.activeSessionId), [`sessionId`](../../../src/core/cron-jobs.ts.md#CreateAgentCronJobInput.sessionId), [`scheduleText`](../../../src/core/cron-jobs.ts.md#CreateAgentCronJobInput.scheduleText), [`cwd`](../../../src/core/cron-jobs.ts.md#CreateAgentCronJobInput.cwd), [`sessionFile`](../../../src/core/cron-jobs.ts.md#CreateAgentCronJobInput.sessionFile), [`now`](../../../src/core/cron-jobs.ts.md#CreateAgentCronJobInput.now), [`AgentSessionRuntime`](../../../src/core/agent-session-runtime.ts.md#AgentSessionRuntime), [`list`](../../../src/core/cron-jobs.ts.md#AgentCronJobStore.list), [`AgentCronJobStore`](../../../src/core/cron-jobs.ts.md#AgentCronJobStore), [`nextRunAt`](../../../src/core/cron-jobs.ts.md#AgentCronJob.nextRunAt), [`clients`](../../../src/modes/daemon/active-session-state.ts.md#ActiveSessionState.clients), [`getSessionArtifactDir`](../../../src/core/session-manager.ts.md#SessionManager.getSessionArtifactDir), [`worker`](../../../src/modes/daemon/daemon-mode.ts.md#DaemonModeOptions.worker), [`registerSessionArtifact`](../../../src/core/cron-jobs.ts.md#AgentCronJobStore.registerSessionArtifact), [`lastEventSequence`](../../../src/modes/daemon/active-session-state.ts.md#ActiveSessionState.lastEventSequence), [`forSessionArtifacts`](../../../src/core/cron-jobs.ts.md#AgentCronJobStore.forSessionArtifacts), [`runCount`](../../../src/core/cron-jobs.ts.md#AgentCronJob.runCount), [`eventGeneration`](../../../src/modes/daemon/active-session-state.ts.md#ActiveSessionState.eventGeneration), [`extensionUiRequests`](../../../src/modes/daemon/active-session-state.ts.md#ActiveSessionState.extensionUiRequests), [`start`](../../../src/core/cron-jobs.ts.md#AgentCronScheduler.start), [`pendingAttaches`](../../../src/modes/daemon/active-session-state.ts.md#ActiveSessionState.pendingAttaches), [`AgentCronScheduler`](../../../src/core/cron-jobs.ts.md#AgentCronScheduler), [`stop`](../../../src/core/cron-jobs.ts.md#AgentCronScheduler.stop)  (8 test-only)

## Functions
- `waitFor(predicate: () => boolean)` — [`L94`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4657-update-heartbeat-recovery.test.ts#L94)


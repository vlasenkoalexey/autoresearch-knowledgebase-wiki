---
title: 'Module: packages/coding-agent/src/core/cron-jobs.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/cron-jobs.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`cron-jobs.ts`/
symbols:
  AgentCronJob.id: AgentCronJob#id.
  AgentCronJob: AgentCronJob#
  AgentCronJobStore.createHeartbeat: AgentCronJobStore#createHeartbeat().
  AgentCronJobStore.createRlmHeartbeat: AgentCronJobStore#createRlmHeartbeat().
  AgentCronJobStore.create: AgentCronJobStore#create().
  AgentCronJob.status: AgentCronJob#status.
  CreateAgentCronJobInput.prompt: CreateAgentCronJobInput#prompt.
  CreateAgentCronJobInput.activeSessionId: CreateAgentCronJobInput#activeSessionId.
  CreateAgentCronJobInput.sessionId: CreateAgentCronJobInput#sessionId.
  CreateAgentCronJobInput.scheduleText: CreateAgentCronJobInput#scheduleText.
  CreateAgentCronJobInput.sessionFile: CreateAgentCronJobInput#sessionFile.
  CreateAgentCronJobInput.cwd: CreateAgentCronJobInput#cwd.
  CreateAgentCronJobInput.now: CreateAgentCronJobInput#now.
  AgentCronJobStore.list: AgentCronJobStore#list().
  AgentCronJobStore.updateRlmHeartbeat.update-typeLiteral153.now: AgentCronJobStore#updateRlmHeartbeat().(update)typeLiteral153:now.
  AgentCronJob.activeSessionId: AgentCronJob#activeSessionId.
  AgentCronJobStore: AgentCronJobStore#
  AgentCronJob.nextRunAt: AgentCronJob#nextRunAt.
  AgentCronJobStore.writeJobs: AgentCronJobStore#writeJobs().
  AgentCronJob.source: AgentCronJob#source.
  AgentCronJob.schedule: AgentCronJob#schedule.
  claimDueInState: claimDueInState().
  isAgentCronJob: isAgentCronJob().
  shouldDeferHeartbeatCronJob: shouldDeferHeartbeatCronJob().
  parseHeartbeatCommand: parseHeartbeatCommand().
  AgentCronScheduler.runDue: AgentCronScheduler#runDue().
  AgentCronJobStore.recordDispatchResult.result-typeLiteral336.error: AgentCronJobStore#recordDispatchResult().(result)typeLiteral336:error.
  heartbeatCatalogSignature: heartbeatCatalogSignature().
  AgentCronScheduler.queueDispatch: AgentCronScheduler#queueDispatch().
  AgentCronJob.prompt: AgentCronJob#prompt.
  AgentCronJobStore.listRlmHeartbeats: AgentCronJobStore#listRlmHeartbeats().
  AgentCronJobStore.manageHeartbeat: AgentCronJobStore#manageHeartbeat().
  AgentCronJob.sessionFile: AgentCronJob#sessionFile.
  AgentCronJobStore.-constructor: AgentCronJobStore#`<constructor>`().
  AgentCronJobStore.getHeartbeat: AgentCronJobStore#getHeartbeat().
  parseAgentCronSchedule.typeLiteral70.nextRunAt: parseAgentCronSchedule().typeLiteral70:nextRunAt.
  AgentCronJobStore.readJobs: AgentCronJobStore#readJobs().
  AgentCronJobStore.cancelJobsForSession: AgentCronJobStore#cancelJobsForSession().
  AgentCronJobStore.rebindSessionJobs.input-typeLiteral71.cwd: AgentCronJobStore#rebindSessionJobs().(input)typeLiteral71:cwd.
  migrateLegacyCronJobsToSessionArtifacts.options-typeLiteral536.now: migrateLegacyCronJobsToSessionArtifacts().(options)typeLiteral536:now.
  AgentCronSchedule.kind: AgentCronSchedule#kind.
  formatAgentCronJob: formatAgentCronJob().
  AgentHeartbeatDeliveryMode: AgentHeartbeatDeliveryMode#
  AgentCronJob.sessionId: AgentCronJob#sessionId.
  AgentCronJob.updatedAt: AgentCronJob#updatedAt.
  AgentCronJobStore.recordRunResult: AgentCronJobStore#recordRunResult().
  AgentCronJobStore.registerSessionArtifact: AgentCronJobStore#registerSessionArtifact().
  AgentCronJobStore.mutateStates: AgentCronJobStore#mutateStates().
  recoverInterruptedInState: recoverInterruptedInState().
  AgentCronJobStore.deleteRlmHeartbeat: AgentCronJobStore#deleteRlmHeartbeat().
  AgentHeartbeatManagementAction: AgentHeartbeatManagementAction#
  readJobsState: readJobsState().
  AgentCronJobStore.forSessionArtifacts: AgentCronJobStore#forSessionArtifacts().
  AgentCronJob.runCount: AgentCronJob#runCount.
  AgentCronSchedule.expression: AgentCronSchedule#expression.
  AgentCronJob.deliveryMode: AgentCronJob#deliveryMode.
  AgentCronJobStore.getClaimedJob: AgentCronJobStore#getClaimedJob().
  AgentCronJobStore.cancelRlmHeartbeatsForSession: AgentCronJobStore#cancelRlmHeartbeatsForSession().
  CreateAgentCronJobInput.runtimeKind: CreateAgentCronJobInput#runtimeKind.
  AgentCronJob.createdAt: AgentCronJob#createdAt.
  nextRunAtForSchedule: nextRunAtForSchedule().
  AgentCronJobStore.recordSkipResult: AgentCronJobStore#recordSkipResult().
  AgentCronJobStore.resumeHeartbeat: AgentCronJobStore#resumeHeartbeat().
  AgentCronJobStore.cancel: AgentCronJobStore#cancel().
  AgentCronSchedule.intervalMs: AgentCronSchedule#intervalMs.
  AgentCronScheduler.wake: AgentCronScheduler#wake().
  AgentCronJobStore.recoverSessionArtifact: AgentCronJobStore#recoverSessionArtifact().
  AgentCronJobStore.pauseHeartbeat: AgentCronJobStore#pauseHeartbeat().
  parseCronExpression: parseCronExpression().
  AgentCronJob.cwd: AgentCronJob#cwd.
  AgentCronSchedulerHooks.runJob: AgentCronSchedulerHooks#runJob.
  isHeartbeatCronJob: isHeartbeatCronJob().
  AgentCronJobStore.claimDue: AgentCronJobStore#claimDue().
  AgentCronScheduler.-constructor: AgentCronScheduler#`<constructor>`().
  writeJobsFile: writeJobsFile().
  CronJobsState.jobs: CronJobsState#jobs.
  AgentCronScheduler.start: AgentCronScheduler#start().
  parseAgentCronSchedule.typeLiteral70.schedule: parseAgentCronSchedule().typeLiteral70:schedule.
  CronJobsState.dispatches: CronJobsState#dispatches.
  matchesCronFields: matchesCronFields().
  AgentCronScheduler.scheduleNext: AgentCronScheduler#scheduleNext().
  consumeDeliveryOption: consumeDeliveryOption().
  CreateAgentCronJobInput.label: CreateAgentCronJobInput#label.
  AgentCronJobStore.getLatestHeartbeat: AgentCronJobStore#getLatestHeartbeat().
  AgentCronJobStore.clearHeartbeat: AgentCronJobStore#clearHeartbeat().
  AgentHeartbeatUpdateAction: AgentHeartbeatUpdateAction#
  withoutNextRunAt: withoutNextRunAt().
  normalizeHeartbeatDeliveryMode: normalizeHeartbeatDeliveryMode().
  isAgentCronDispatchRecord: isAgentCronDispatchRecord().
  HeartbeatCronSessionActivity.isStreaming: HeartbeatCronSessionActivity#isStreaming.
  AgentCronDispatch: AgentCronDispatch#
  AgentCronJob.label: AgentCronJob#label.
  HeartbeatCronSessionActivity.isBashRunning: HeartbeatCronSessionActivity#isBashRunning.
  HeartbeatCronSessionActivity.hasPendingSessionWork: HeartbeatCronSessionActivity#hasPendingSessionWork.
  HeartbeatCronSessionActivity.unfinishedActionCount: HeartbeatCronSessionActivity#unfinishedActionCount.
  AgentCronJobStore.getDueJob: AgentCronJobStore#getDueJob().
  AgentCronJobStore.readStates: AgentCronJobStore#readStates().
  resolveHeartbeatStreamingBehavior: resolveHeartbeatStreamingBehavior().
  AgentCronJob.runtimeKind: AgentCronJob#runtimeKind.
  AgentCronJobStore.updateRlmHeartbeat: AgentCronJobStore#updateRlmHeartbeat().
  AgentCronJobStore.updateRlmHeartbeat.update-typeLiteral153.status: AgentCronJobStore#updateRlmHeartbeat().(update)typeLiteral153:status.
  AgentCronJobStore.nextActiveRunAt: AgentCronJobStore#nextActiveRunAt().
  isDueJob: isDueJob().
  AgentCronJob.lastRunAt: AgentCronJob#lastRunAt.
  AgentCronSchedulerHooks.now: AgentCronSchedulerHooks#now.
  SESSION_SCHEDULED_JOBS_FILENAME: SESSION_SCHEDULED_JOBS_FILENAME.
  AgentCronScheduler: AgentCronScheduler#
  parseAgentCronSchedule: parseAgentCronSchedule().
  AgentCronJobStore.recordDispatchResult.result-typeLiteral336.outcome: AgentCronJobStore#recordDispatchResult().(result)typeLiteral336:outcome.
  AgentCronJobStore.recoverInterruptedDispatches: AgentCronJobStore#recoverInterruptedDispatches().
  AgentCronScheduler.now: AgentCronScheduler#now().
  nextCronRunAfter: nextCronRunAfter().
  mergeFreshJobs: mergeFreshJobs().
  AgentCronJobStore.sessionArtifactFiles: AgentCronJobStore#sessionArtifactFiles.
  AgentCronScheduler.stop: AgentCronScheduler#stop().
  CreateAgentCronJobInput.deliveryMode: CreateAgentCronJobInput#deliveryMode.
  CronJobsState: CronJobsState#
  DEFAULT_HEARTBEAT_DELIVERY_MODE: DEFAULT_HEARTBEAT_DELIVERY_MODE.
  AgentCronJobStore.recoverInterruptedDispatchesById: AgentCronJobStore#recoverInterruptedDispatchesById().
  normalizeHeartbeatSchedule: normalizeHeartbeatSchedule().
  AgentCronJob.lastError: AgentCronJob#lastError.
  AgentCronDispatch.id: AgentCronDispatch#id.
  AgentRlmHeartbeatController: AgentRlmHeartbeatController#
  AgentCronJobStore.updateRlmHeartbeat.update-typeLiteral153.prompt: AgentCronJobStore#updateRlmHeartbeat().(update)typeLiteral153:prompt.
  AgentCronJobStore.due: AgentCronJobStore#due().
  parseCronField: parseCronField().
  AgentCronDispatchRecord.id: AgentCronDispatchRecord#id.
  AgentCronDispatchRecord.jobId: AgentCronDispatchRecord#jobId.
  AgentCronJobStore.rebindSessionJobs.input-typeLiteral71.activeSessionId: AgentCronJobStore#rebindSessionJobs().(input)typeLiteral71:activeSessionId.
  AgentCronScheduler.timer: AgentCronScheduler#timer.
  consumeLeadingDeliveryFlag: consumeLeadingDeliveryFlag().
  consumeTrailingDeliveryFlag: consumeTrailingDeliveryFlag().
  AgentCronJobStore.updateRlmHeartbeat.update-typeLiteral153.deliveryMode: AgentCronJobStore#updateRlmHeartbeat().(update)typeLiteral153:deliveryMode.
  consumeDeliveryOption.typeLiteral693.deliveryMode: consumeDeliveryOption().typeLiteral693:deliveryMode.
  parseDeliveryModeToken: parseDeliveryModeToken().
  writeJobsState: writeJobsState().
  ONE_MINUTE_MS: ONE_MINUTE_MS.
  AgentRlmHeartbeatController.createRlmHeartbeat.input-typeLiteral22.deliveryMode: AgentRlmHeartbeatController#createRlmHeartbeat().(input)typeLiteral22:deliveryMode.
  AgentRlmHeartbeatController.updateRlmHeartbeat.input-typeLiteral23.deliveryMode: AgentRlmHeartbeatController#updateRlmHeartbeat().(input)typeLiteral23:deliveryMode.
  AgentCronJobStore.rebindSessionJobs.input-typeLiteral71.sessionId: AgentCronJobStore#rebindSessionJobs().(input)typeLiteral71:sessionId.
  AgentCronJobStore.rebindSessionJobs.input-typeLiteral71.sessionFile: AgentCronJobStore#rebindSessionJobs().(input)typeLiteral71:sessionFile.
  AgentCronJobStore.recordDispatchResult: AgentCronJobStore#recordDispatchResult().
  AgentCronJobStore.recordDispatchResult.result-typeLiteral336.now: AgentCronJobStore#recordDispatchResult().(result)typeLiteral336:now.
  consumeDeliveryOption.typeLiteral693.rest: consumeDeliveryOption().typeLiteral693:rest.
  isAtLeastAsFresh: isAtLeastAsFresh().
  AgentCronSchedulerHooks.beginDispatch: AgentCronSchedulerHooks#beginDispatch.
  AgentCronJobStore.notifyHeartbeatChange: AgentCronJobStore#notifyHeartbeatChange().
  AgentCronJob.lastSkippedAt: AgentCronJob#lastSkippedAt.
  AgentCronJobRunResult: AgentCronJobRunResult#
  migrateLegacyCronJobsToSessionArtifacts: migrateLegacyCronJobsToSessionArtifacts().
  AgentCronScheduler.stopped: AgentCronScheduler#stopped.
  AgentCronSchedulerHooks.onError: AgentCronSchedulerHooks#onError.
  AgentRlmHeartbeatController.deleteRlmHeartbeat: AgentRlmHeartbeatController#deleteRlmHeartbeat().
  AgentCronJobStore.onHeartbeatChange: AgentCronJobStore#onHeartbeatChange().
  migrateLegacyCronJobsToSessionArtifacts.options-typeLiteral536.isSessionOwned: migrateLegacyCronJobsToSessionArtifacts().(options)typeLiteral536:isSessionOwned.
  AgentRlmHeartbeatStatusUpdate: AgentRlmHeartbeatStatusUpdate#
  AgentCronDispatch.job: AgentCronDispatch#job.
  AgentCronDispatchRecord: AgentCronDispatchRecord#
  DEFAULT_HEARTBEAT_SCHEDULE: DEFAULT_HEARTBEAT_SCHEDULE.
  AgentCronJobStore.rebindSessionJobs: AgentCronJobStore#rebindSessionJobs().
  AgentCronJobStore.updateRlmHeartbeat.update-typeLiteral153.label: AgentCronJobStore#updateRlmHeartbeat().(update)typeLiteral153:label.
  AgentCronJobStore.updateRlmHeartbeat.update-typeLiteral153.scheduleText: AgentCronJobStore#updateRlmHeartbeat().(update)typeLiteral153:scheduleText.
  AgentCronJobStore.cancelJobsForSession.input-typeLiteral202.sessionId: AgentCronJobStore#cancelJobsForSession().(input)typeLiteral202:sessionId.
  AgentCronJobStore.cancelJobsForSession.input-typeLiteral202.sessionFile: AgentCronJobStore#cancelJobsForSession().(input)typeLiteral202:sessionFile.
  AgentCronScheduler.dispatchLanes: AgentCronScheduler#dispatchLanes.
  parseCronNumber: parseCronNumber().
  withCronJobsStateLocks: withCronJobsStateLocks().
  normalizeOptionalLabel: normalizeOptionalLabel().
  CreateAgentCronJobInput.source: CreateAgentCronJobInput#source.
  ParsedHeartbeatCommand: ParsedHeartbeatCommand#
  AgentRlmHeartbeatController.updateRlmHeartbeat.input-typeLiteral23.status: AgentRlmHeartbeatController#updateRlmHeartbeat().(input)typeLiteral23:status.
  AgentCronSchedule: AgentCronSchedule#
  CreateAgentCronJobInput: CreateAgentCronJobInput#
  AgentCronJobStore.heartbeatChangeListeners: AgentCronJobStore#heartbeatChangeListeners.
  AgentCronJobStore.requireFilePath: AgentCronJobStore#requireFilePath().
  AgentCronScheduler.running: AgentCronScheduler#running.
  AgentCronScheduler.hasStarted: AgentCronScheduler#hasStarted.
  CronFields.dayOfWeek: CronFields#dayOfWeek.
  AgentRlmHeartbeatController.listRlmHeartbeats.options-typeLiteral21.includeInactive: AgentRlmHeartbeatController#listRlmHeartbeats().(options)typeLiteral21:includeInactive.
  AgentCronJobSource: AgentCronJobSource#
  AgentCronJobRuntimeKind: AgentCronJobRuntimeKind#
  HeartbeatCronSessionActivity.isCompacting: HeartbeatCronSessionActivity#isCompacting.
  HeartbeatCronSessionActivity.isRetrying: HeartbeatCronSessionActivity#isRetrying.
  CronJobsFile.jobs: CronJobsFile#jobs.
  CronJobsFile.dispatches: CronJobsFile#dispatches.
  AgentCronDispatchRecord.claimedAt: AgentCronDispatchRecord#claimedAt.
  AgentCronDispatchRecord.scheduledFor: AgentCronDispatchRecord#scheduledFor.
  ONE_SECOND_MS: ONE_SECOND_MS.
  AgentRlmHeartbeatController.listRlmHeartbeats: AgentRlmHeartbeatController#listRlmHeartbeats().
  AgentRlmHeartbeatController.createRlmHeartbeat: AgentRlmHeartbeatController#createRlmHeartbeat().
  AgentRlmHeartbeatController.updateRlmHeartbeat: AgentRlmHeartbeatController#updateRlmHeartbeat().
  AgentCronJobStore.cancelJobsForSession.input-typeLiteral202.activeSessionId: AgentCronJobStore#cancelJobsForSession().(input)typeLiteral202:activeSessionId.
  AgentCronJobStore.recordRunResult.result-typeLiteral281.error: AgentCronJobStore#recordRunResult().(result)typeLiteral281:error.
  CronFields: CronFields#
  CronFields.minute: CronFields#minute.
  CronFields.hour: CronFields#hour.
  CronFields.dayOfMonth: CronFields#dayOfMonth.
  CronFields.month: CronFields#month.
  compareOptionalIso: compareOptionalIso().
  errorMessage: errorMessage().
  AgentCronJobStatus: AgentCronJobStatus#
  AgentCronScheduleKind: AgentCronScheduleKind#
  AgentCronSchedulerHooks: AgentCronSchedulerHooks#
  HeartbeatCronSessionActivity: HeartbeatCronSessionActivity#
  CronJobsFile: CronJobsFile#
  MAX_TIMEOUT_MS: MAX_TIMEOUT_MS.
  AgentRlmHeartbeatController.createRlmHeartbeat.input-typeLiteral22.instruction: AgentRlmHeartbeatController#createRlmHeartbeat().(input)typeLiteral22:instruction.
  AgentRlmHeartbeatController.createRlmHeartbeat.input-typeLiteral22.interval: AgentRlmHeartbeatController#createRlmHeartbeat().(input)typeLiteral22:interval.
  AgentRlmHeartbeatController.createRlmHeartbeat.input-typeLiteral22.label: AgentRlmHeartbeatController#createRlmHeartbeat().(input)typeLiteral22:label.
  AgentRlmHeartbeatController.updateRlmHeartbeat.input-typeLiteral23.id: AgentRlmHeartbeatController#updateRlmHeartbeat().(input)typeLiteral23:id.
  AgentRlmHeartbeatController.updateRlmHeartbeat.input-typeLiteral23.instruction: AgentRlmHeartbeatController#updateRlmHeartbeat().(input)typeLiteral23:instruction.
  AgentRlmHeartbeatController.updateRlmHeartbeat.input-typeLiteral23.interval: AgentRlmHeartbeatController#updateRlmHeartbeat().(input)typeLiteral23:interval.
  AgentRlmHeartbeatController.updateRlmHeartbeat.input-typeLiteral23.label: AgentRlmHeartbeatController#updateRlmHeartbeat().(input)typeLiteral23:label.
  AgentCronJobStore.listRlmHeartbeats.options-typeLiteral128.includeInactive: AgentCronJobStore#listRlmHeartbeats().(options)typeLiteral128:includeInactive.
  AgentCronJobStore.recordRunResult.result-typeLiteral281.now: AgentCronJobStore#recordRunResult().(result)typeLiteral281:now.
  AgentCronJobStore.recordSkipResult.result-typeLiteral300.now: AgentCronJobStore#recordSkipResult().(result)typeLiteral300:now.
  consumeEveryOption: consumeEveryOption().
  consumeLeadingEverySchedule: consumeLeadingEverySchedule().
  normalizeCronAlias: normalizeCronAlias().
  stripMatchingQuotes: stripMatchingQuotes().
---
# Module: [`packages/coding-agent/src/core/cron-jobs.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts)

## Classes
### `AgentCronDispatch`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:73`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L73)
- signature: `interface AgentCronDispatch`
- members:
  - `id` — [`L74`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L74)
  - `job` — [`L75`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L75)
- uses (calls/refs, reference-scoped): [`AgentCronJob`](cron-jobs.ts.md#AgentCronJob)
- used by: [`claimDueInState`](cron-jobs.ts.md#claimDueInState), [`runDue`](cron-jobs.ts.md#AgentCronScheduler.runDue), [`queueDispatch`](cron-jobs.ts.md#AgentCronScheduler.queueDispatch), [`mutateStates`](cron-jobs.ts.md#AgentCronJobStore.mutateStates), [`claimDue`](cron-jobs.ts.md#AgentCronJobStore.claimDue), [`beginDispatch`](cron-jobs.ts.md#AgentCronSchedulerHooks.beginDispatch)  (2 test-only)

### `AgentCronDispatchRecord`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:99`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L99)
- signature: `interface AgentCronDispatchRecord`
- members:
  - `claimedAt` — [`L102`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L102)
  - `id` — [`L100`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L100)
  - `jobId` — [`L101`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L101)
  - `scheduledFor` — [`L103`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L103)
- used by: [`writeJobs`](cron-jobs.ts.md#AgentCronJobStore.writeJobs), [`claimDueInState`](cron-jobs.ts.md#claimDueInState), [`error`](cron-jobs.ts.md#AgentCronJobStore.recordDispatchResult.result-typeLiteral336.error), [`recoverInterruptedInState`](cron-jobs.ts.md#recoverInterruptedInState), [`getClaimedJob`](cron-jobs.ts.md#AgentCronJobStore.getClaimedJob), [`isAgentCronDispatchRecord`](cron-jobs.ts.md#isAgentCronDispatchRecord), [`CronJobsState`](cron-jobs.ts.md#CronJobsState)

### `AgentCronJob`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L34) — documented in [packages-coding-agent-src-core-cron-jobs.ts](../../../../../concepts/packages-coding-agent-src-core-cron-jobs.ts.md)
- signature: `interface AgentCronJob`
- members:
  - `activeSessionId` — [`L41`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L41)
  - `createdAt` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L48)
  - `cwd` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L44)
  - `deliveryMode` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L40) — Delivery mode for heartbeat/rlm_heartbeat jobs when the session is busy. Defaults to "steer".
  - `id` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L35)
  - `label` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L45)
  - `lastError` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L53)
  - `lastRunAt` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L51)
  - `lastSkippedAt` — [`L52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L52)
  - `nextRunAt` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L50)
  - `prompt` — [`L46`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L46)
  - `runCount` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L54)
  - `runtimeKind` — [`L38`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L38)
  - `schedule` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L47)
  - `sessionFile` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L43)
  - `sessionId` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L42)
  - `source` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L37)
  - `status` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L36)
  - `updatedAt` — [`L49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L49)
- uses (calls/refs, reference-scoped): [`AgentHeartbeatDeliveryMode`](cron-jobs.ts.md#AgentHeartbeatDeliveryMode), [`AgentCronSchedule`](cron-jobs.ts.md#AgentCronSchedule), [`AgentCronJobRuntimeKind`](cron-jobs.ts.md#AgentCronJobRuntimeKind), [`AgentCronJobSource`](cron-jobs.ts.md#AgentCronJobSource), [`AgentCronJobStatus`](cron-jobs.ts.md#AgentCronJobStatus)
- used by: [`interactive-mode.ts`](../modes/interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`handleCommand`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.handleCommand), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`daemon-supervisor.ts`](../modes/daemon/daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`handleCommand`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.handleCommand), [`daemon-agent-connection.ts`](../modes/agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](../modes/agent-connection/in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`<constructor>`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.-constructor), [`daemon-protocol.ts`](../modes/daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`createHeartbeat`](cron-jobs.ts.md#AgentCronJobStore.createHeartbeat), [`start`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.start), [`createRlmHeartbeat`](cron-jobs.ts.md#AgentCronJobStore.createRlmHeartbeat), [`create`](cron-jobs.ts.md#AgentCronJobStore.create), [`createAgentMessageAgentSummary`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentMessageAgentSummary), [`daemon-session-list.ts`](../modes/daemon/daemon-session-list.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-session-list.ts), [`rpc-client.ts`](../modes/rpc/rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`daemon-command.ts`](../cli/daemon-command.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-daemon-command.ts), [`sessionPassivationSnapshot`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.sessionPassivationSnapshot), [`rpc-types.ts`](../modes/rpc/rpc-types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-types.ts), [`buildSessionListWithPassiveRlmSubagents`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.buildSessionListWithPassiveRlmSubagents), [`list`](cron-jobs.ts.md#AgentCronJobStore.list), [`deliveryMode`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRlmHeartbeatForState.input-typeLiteral666.deliveryMode), [`createActionPanel`](../modes/interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.createActionPanel), [`now`](cron-jobs.ts.md#AgentCronJobStore.updateRlmHeartbeat.update-typeLiteral153.now), [`createHeartbeatForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createHeartbeatForState), [`populateHeartbeatList`](../modes/interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.populateHeartbeatList), [`messages.ts`](messages.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-messages.ts), [`runCronJob`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.runCronJob), [`getOrCreateCronJobSession`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.getOrCreateCronJobSession), [`restoreRlmHeartbeatSession`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.restoreRlmHeartbeatSession), [`job`](../modes/agent-connection/types.ts.md#AgentConnectionHeartbeat.job), [`writeJobs`](cron-jobs.ts.md#AgentCronJobStore.writeJobs), [`createHeartbeatPromptMessage`](messages.ts.md#createHeartbeatPromptMessage), [`buildSessionList`](../modes/daemon/daemon-session-list.ts.md#buildSessionList), [`createCronJobForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createCronJobForState), [`showHeartbeat`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.showHeartbeat), [`deliveryMode`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.updateRlmHeartbeatForState.input-typeLiteral676.deliveryMode), [`rebindCronJobsToState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.rebindCronJobsToState)  (+113 more; 34 test-only)

### `AgentCronJobRunResult`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:71`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L71)
- signature: `type AgentCronJobRunResult`
- used by: [`queueDispatch`](cron-jobs.ts.md#AgentCronScheduler.queueDispatch), [`runJob`](cron-jobs.ts.md#AgentCronSchedulerHooks.runJob), [`outcome`](cron-jobs.ts.md#AgentCronJobStore.recordDispatchResult.result-typeLiteral336.outcome)

### `AgentCronJobRuntimeKind`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L18)
- signature: `type AgentCronJobRuntimeKind`
- used by: [`runtimeKind`](cron-jobs.ts.md#CreateAgentCronJobInput.runtimeKind), [`runtimeKind`](cron-jobs.ts.md#AgentCronJob.runtimeKind)

### `AgentCronJobSource`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L17)
- signature: `type AgentCronJobSource`
- used by: [`source`](cron-jobs.ts.md#AgentCronJob.source), [`source`](cron-jobs.ts.md#CreateAgentCronJobInput.source)

### `AgentCronJobStatus`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L15)
- signature: `type AgentCronJobStatus`
- used by: [`status`](cron-jobs.ts.md#AgentCronJob.status)

### `AgentCronJobStore`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:168`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L168)
- signature: `class AgentCronJobStore`
- members:
  - `<constructor>(filePath?: string | undefined, sessionArtifactMode?: boolean)` — [`L172`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L172)
  - `cancel(method)` — [`L621`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L621)
  - `cancelJobsForSession(method)` — [`L502`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L502)
  - `cancelRlmHeartbeatsForSession(method)` — [`L482`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L482)
  - `claimDue(method)` — [`L701`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L701)
  - `clearHeartbeat(method)` — [`L564`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L564)
  - `create(method)` — [`L222`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L222)
  - `createHeartbeat(method)` — [`L312`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L312) — documented in [packages-coding-agent-src-core-cron-jobs.ts](../../../../../concepts/packages-coding-agent-src-core-cron-jobs.ts.md)
  - `createRlmHeartbeat(method)` — [`L369`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L369)
  - `deleteRlmHeartbeat(method)` — [`L467`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L467)
  - `due(method)` — [`L697`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L697)
  - `forSessionArtifacts(method)` — [`L181`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L181)
  - `getClaimedJob(method)` — [`L705`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L705)
  - `getDueJob(method)` — [`L776`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L776)
  - `getHeartbeat(method)` — [`L294`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L294)
  - `getLatestHeartbeat(method)` — [`L306`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L306)
  - `list(method)` — [`L218`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L218)
  - `listRlmHeartbeats(method)` — [`L355`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L355)
  - `manageHeartbeat(method)` — [`L581`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L581)
  - `mutateStates(method)` — [`L800`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L800)
  - `nextActiveRunAt(method)` — [`L780`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L780)
  - `notifyHeartbeatChange(method)` — [`L880`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L880)
  - `onHeartbeatChange(method)` — [`L185`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L185)
  - `pauseHeartbeat(method)` — [`L526`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L526)
  - `readJobs(method)` — [`L789`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L789)
  - `readStates(method)` — [`L793`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L793)
  - `rebindSessionJobs(method)` — [`L258`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L258) — Active session ids are daemon-local. When a persisted session is restored,
  - `recordDispatchResult(method)` — [`L715`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L715)
  - `recordRunResult(method)` — [`L636`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L636)
  - `recordSkipResult(method)` — [`L671`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L671)
  - `recoverInterruptedDispatches(method)` — [`L757`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L757)
  - `recoverInterruptedDispatchesById(method)` — [`L766`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L766)
  - `recoverSessionArtifact(method)` — [`L202`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L202)
  - `registerSessionArtifact(method)` — [`L190`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L190)
  - `requireFilePath(method)` — [`L886`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L886)
  - `resumeHeartbeat(method)` — [`L543`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L543)
  - `updateRlmHeartbeat(method)` — [`L402`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L402)
  - `writeJobs(method)` — [`L823`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L823)
  - `activeSessionId` — [`L259`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L259)
  - `activeSessionId` — [`L503`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L503)
  - `cwd` — [`L262`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L262)
  - `deliveryMode` — [`L410`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L410)
  - `error` — [`L636`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L636)
  - `error` — [`L717`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L717)
  - `heartbeatChangeListeners` — [`L170`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L170)
  - `includeInactive` — [`L355`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L355)
  - `label` — [`L406`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L406)
  - `now` — [`L411`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L411)
  - `now` — [`L636`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L636)
  - `now` — [`L671`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L671)
  - `now` — [`L717`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L717)
  - `outcome` — [`L717`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L717)
  - `prompt` — [`L407`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L407)
  - `scheduleText` — [`L408`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L408)
  - `sessionArtifactFiles` — [`L169`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L169)
  - `sessionFile` — [`L261`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L261)
  - `sessionFile` — [`L503`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L503)
  - `sessionId` — [`L260`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L260)
  - `sessionId` — [`L503`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L503)
  - `status` — [`L409`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L409)
- uses (calls/refs, reference-scoped): [`id`](cron-jobs.ts.md#AgentCronJob.id), [`AgentCronJob`](cron-jobs.ts.md#AgentCronJob), [`status`](cron-jobs.ts.md#AgentCronJob.status), [`prompt`](cron-jobs.ts.md#CreateAgentCronJobInput.prompt), [`activeSessionId`](cron-jobs.ts.md#CreateAgentCronJobInput.activeSessionId), [`sessionId`](cron-jobs.ts.md#CreateAgentCronJobInput.sessionId), [`scheduleText`](cron-jobs.ts.md#CreateAgentCronJobInput.scheduleText), [`cwd`](cron-jobs.ts.md#CreateAgentCronJobInput.cwd), [`sessionFile`](cron-jobs.ts.md#CreateAgentCronJobInput.sessionFile), [`now`](cron-jobs.ts.md#CreateAgentCronJobInput.now), [`activeSessionId`](cron-jobs.ts.md#AgentCronJob.activeSessionId), [`nextRunAt`](cron-jobs.ts.md#AgentCronJob.nextRunAt), [`source`](cron-jobs.ts.md#AgentCronJob.source), [`schedule`](cron-jobs.ts.md#AgentCronJob.schedule), [`claimDueInState`](cron-jobs.ts.md#claimDueInState), [`heartbeatCatalogSignature`](cron-jobs.ts.md#heartbeatCatalogSignature), [`prompt`](cron-jobs.ts.md#AgentCronJob.prompt), [`nextRunAt`](cron-jobs.ts.md#parseAgentCronSchedule.typeLiteral70.nextRunAt), [`sessionFile`](cron-jobs.ts.md#AgentCronJob.sessionFile), [`kind`](cron-jobs.ts.md#AgentCronSchedule.kind), [`AgentHeartbeatDeliveryMode`](cron-jobs.ts.md#AgentHeartbeatDeliveryMode), [`sessionId`](cron-jobs.ts.md#AgentCronJob.sessionId), [`updatedAt`](cron-jobs.ts.md#AgentCronJob.updatedAt), [`recoverInterruptedInState`](cron-jobs.ts.md#recoverInterruptedInState), [`AgentHeartbeatManagementAction`](cron-jobs.ts.md#AgentHeartbeatManagementAction), [`readJobsState`](cron-jobs.ts.md#readJobsState), [`runCount`](cron-jobs.ts.md#AgentCronJob.runCount), [`deliveryMode`](cron-jobs.ts.md#AgentCronJob.deliveryMode), [`runtimeKind`](cron-jobs.ts.md#CreateAgentCronJobInput.runtimeKind), [`createdAt`](cron-jobs.ts.md#AgentCronJob.createdAt), [`nextRunAtForSchedule`](cron-jobs.ts.md#nextRunAtForSchedule), [`cwd`](cron-jobs.ts.md#AgentCronJob.cwd), [`isHeartbeatCronJob`](cron-jobs.ts.md#isHeartbeatCronJob), [`writeJobsFile`](cron-jobs.ts.md#writeJobsFile), [`jobs`](cron-jobs.ts.md#CronJobsState.jobs), [`schedule`](cron-jobs.ts.md#parseAgentCronSchedule.typeLiteral70.schedule), [`dispatches`](cron-jobs.ts.md#CronJobsState.dispatches), [`label`](cron-jobs.ts.md#CreateAgentCronJobInput.label), [`withoutNextRunAt`](cron-jobs.ts.md#withoutNextRunAt), [`AgentCronDispatch`](cron-jobs.ts.md#AgentCronDispatch)  (+20 more)
- used by: [`handleCommand`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.handleCommand), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`daemon-supervisor.ts`](../modes/daemon/daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`<constructor>`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.-constructor), [`createRlmSubagentRuntime`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRlmSubagentRuntime), [`createRuntime`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRuntime), [`rehydrateCompletedRlmSubagentOnce`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.rehydrateCompletedRlmSubagentOnce), [`createAgentMessageAgentSummary`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentMessageAgentSummary), [`sessionPassivationSnapshot`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.sessionPassivationSnapshot), [`deliveryMode`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRlmHeartbeatForState.input-typeLiteral666.deliveryMode), [`createHeartbeatForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createHeartbeatForState), [`runCronJob`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.runCronJob), [`createCronJobForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createCronJobForState), [`deliveryMode`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.updateRlmHeartbeatForState.input-typeLiteral676.deliveryMode), [`rebindCronJobsToState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.rebindCronJobsToState), [`runDue`](cron-jobs.ts.md#AgentCronScheduler.runDue), [`cronStore`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.cronStore), [`queueDispatch`](cron-jobs.ts.md#AgentCronScheduler.queueDispatch), [`registerCronStoreForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.registerCronStoreForState), [`finalizeArchivedWorkerStop`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.finalizeArchivedWorkerStop), [`cancelScheduledJobsForSession`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.cancelScheduledJobsForSession), [`updateHeartbeatForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.updateHeartbeatForState), [`createConnectionState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createConnectionState), [`cancelSubagentRlmHeartbeats`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.cancelSubagentRlmHeartbeats), [`listHeartbeats`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.listHeartbeats), [`deleteRlmHeartbeatForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.deleteRlmHeartbeatForState), [`getRunnableCronJob`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.getRunnableCronJob), [`manageHeartbeat`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.manageHeartbeat), [`<constructor>`](cron-jobs.ts.md#AgentCronScheduler.-constructor), [`start`](cron-jobs.ts.md#AgentCronScheduler.start), [`cancelScheduledJobsForSessionFile`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.cancelScheduledJobsForSessionFile), [`scheduleNext`](cron-jobs.ts.md#AgentCronScheduler.scheduleNext), [`cancelRlmHeartbeat`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.cancelRlmHeartbeat), [`hasScheduledJobsForSession`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.hasScheduledJobsForSession)  (16 test-only)

### `AgentCronSchedule`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L28)
- signature: `interface AgentCronSchedule`
- members:
  - `expression` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L30)
  - `intervalMs` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L31)
  - `kind` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L29)
- uses (calls/refs, reference-scoped): [`AgentCronScheduleKind`](cron-jobs.ts.md#AgentCronScheduleKind)
- used by: [`createHeartbeat`](cron-jobs.ts.md#AgentCronJobStore.createHeartbeat), [`createRlmHeartbeat`](cron-jobs.ts.md#AgentCronJobStore.createRlmHeartbeat), [`now`](cron-jobs.ts.md#AgentCronJobStore.updateRlmHeartbeat.update-typeLiteral153.now), [`populateHeartbeatList`](../modes/interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.populateHeartbeatList), [`createHeartbeatPromptMessage`](messages.ts.md#createHeartbeatPromptMessage), [`showHeartbeat`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.showHeartbeat), [`schedule`](cron-jobs.ts.md#AgentCronJob.schedule), [`isAgentCronJob`](cron-jobs.ts.md#isAgentCronJob), [`error`](cron-jobs.ts.md#AgentCronJobStore.recordDispatchResult.result-typeLiteral336.error), [`nextRunAt`](cron-jobs.ts.md#parseAgentCronSchedule.typeLiteral70.nextRunAt), [`formatAgentCronJob`](cron-jobs.ts.md#formatAgentCronJob), [`recordRunResult`](cron-jobs.ts.md#AgentCronJobStore.recordRunResult), [`recoverInterruptedInState`](cron-jobs.ts.md#recoverInterruptedInState), [`formatHeartbeatDetails`](../modes/interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.formatHeartbeatDetails), [`nextRunAtForSchedule`](cron-jobs.ts.md#nextRunAtForSchedule), [`schedule`](cron-jobs.ts.md#parseAgentCronSchedule.typeLiteral70.schedule), [`heartbeatLegacyPromptToleranceMs`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.heartbeatLegacyPromptToleranceMs)  (11 test-only)

### `AgentCronScheduleKind`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L16)
- signature: `type AgentCronScheduleKind`
- used by: [`kind`](cron-jobs.ts.md#AgentCronSchedule.kind)

### `AgentCronScheduler`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:933`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L933)
- signature: `class AgentCronScheduler`
- members:
  - `<constructor>(store: AgentCronJobStore, hooks: AgentCronSchedulerHooks)` — [`L940`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L940)
  - `now(method)` — [`L1074`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1074)
  - `queueDispatch(method)` — [`L1002`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1002)
  - `runDue(method)` — [`L969`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L969)
  - `scheduleNext(method)` — [`L1048`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1048)
  - `start(method)` — [`L945`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L945)
  - `stop(method)` — [`L954`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L954)
  - `wake(method)` — [`L962`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L962)
  - `dispatchLanes` — [`L938`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L938)
  - `hasStarted` — [`L937`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L937)
  - `running` — [`L935`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L935)
  - `stopped` — [`L936`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L936)
  - `timer` — [`L934`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L934)
- uses (calls/refs, reference-scoped): [`id`](cron-jobs.ts.md#AgentCronJob.id), [`AgentCronJobStore`](cron-jobs.ts.md#AgentCronJobStore), [`activeSessionId`](cron-jobs.ts.md#AgentCronJob.activeSessionId), [`error`](cron-jobs.ts.md#AgentCronJobStore.recordDispatchResult.result-typeLiteral336.error), [`getClaimedJob`](cron-jobs.ts.md#AgentCronJobStore.getClaimedJob), [`runJob`](cron-jobs.ts.md#AgentCronSchedulerHooks.runJob), [`claimDue`](cron-jobs.ts.md#AgentCronJobStore.claimDue), [`AgentCronDispatch`](cron-jobs.ts.md#AgentCronDispatch), [`nextActiveRunAt`](cron-jobs.ts.md#AgentCronJobStore.nextActiveRunAt), [`now`](cron-jobs.ts.md#AgentCronSchedulerHooks.now), [`outcome`](cron-jobs.ts.md#AgentCronJobStore.recordDispatchResult.result-typeLiteral336.outcome), [`recoverInterruptedDispatches`](cron-jobs.ts.md#AgentCronJobStore.recoverInterruptedDispatches), [`recoverInterruptedDispatchesById`](cron-jobs.ts.md#AgentCronJobStore.recoverInterruptedDispatchesById), [`id`](cron-jobs.ts.md#AgentCronDispatch.id), [`now`](cron-jobs.ts.md#AgentCronJobStore.recordDispatchResult.result-typeLiteral336.now), [`recordDispatchResult`](cron-jobs.ts.md#AgentCronJobStore.recordDispatchResult), [`beginDispatch`](cron-jobs.ts.md#AgentCronSchedulerHooks.beginDispatch), [`AgentCronJobRunResult`](cron-jobs.ts.md#AgentCronJobRunResult), [`onError`](cron-jobs.ts.md#AgentCronSchedulerHooks.onError), [`job`](cron-jobs.ts.md#AgentCronDispatch.job), [`AgentCronSchedulerHooks`](cron-jobs.ts.md#AgentCronSchedulerHooks), [`MAX_TIMEOUT_MS`](cron-jobs.ts.md#MAX_TIMEOUT_MS)
- used by: [`handleCommand`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.handleCommand), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`<constructor>`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.-constructor), [`deliveryMode`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRlmHeartbeatForState.input-typeLiteral666.deliveryMode), [`createHeartbeatForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createHeartbeatForState), [`createCronJobForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createCronJobForState), [`shutdown`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.shutdown), [`cancelPreparedUpdateRestart`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.cancelPreparedUpdateRestart), [`deliveryMode`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.updateRlmHeartbeatForState.input-typeLiteral676.deliveryMode), [`rebindCronJobsToState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.rebindCronJobsToState), [`start`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.start), [`beginUpdateRestartTransaction`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.beginUpdateRestartTransaction), [`registerCronStoreForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.registerCronStoreForState), [`cancelScheduledJobsForSession`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.cancelScheduledJobsForSession), [`updateHeartbeatForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.updateHeartbeatForState), [`cancelSubagentRlmHeartbeats`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.cancelSubagentRlmHeartbeats), [`deleteRlmHeartbeatForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.deleteRlmHeartbeatForState), [`cronScheduler`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.cronScheduler), [`manageHeartbeat`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.manageHeartbeat), [`cancelScheduledJobsForSessionFile`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.cancelScheduledJobsForSessionFile), [`cancelRlmHeartbeat`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.cancelRlmHeartbeat)  (10 test-only)

### `AgentCronSchedulerHooks`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:78`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L78)
- signature: `interface AgentCronSchedulerHooks`
- members:
  - `beginDispatch` — [`L80`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L80)
  - `now` — [`L81`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L81)
  - `onError` — [`L82`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L82)
  - `runJob` — [`L79`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L79)
- uses (calls/refs, reference-scoped): [`AgentCronJob`](cron-jobs.ts.md#AgentCronJob), [`AgentCronDispatch`](cron-jobs.ts.md#AgentCronDispatch), [`AgentCronJobRunResult`](cron-jobs.ts.md#AgentCronJobRunResult)
- used by: [`<constructor>`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.-constructor), [`runDue`](cron-jobs.ts.md#AgentCronScheduler.runDue), [`queueDispatch`](cron-jobs.ts.md#AgentCronScheduler.queueDispatch), [`<constructor>`](cron-jobs.ts.md#AgentCronScheduler.-constructor), [`now`](cron-jobs.ts.md#AgentCronScheduler.now)  (2 test-only)

### `AgentHeartbeatDeliveryMode`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L26)
- doc: How a scheduled heartbeat prompt is delivered when the target session is busy:
- signature: `type AgentHeartbeatDeliveryMode`
- used by: [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`DaemonCommand`](../modes/daemon/daemon-protocol.ts.md#DaemonCommand), [`daemon-agent-connection.ts`](../modes/agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](../modes/agent-connection/in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`daemon-protocol.ts`](../modes/daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`rpc-client.ts`](../modes/rpc/rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`rpc-types.ts`](../modes/rpc/rpc-types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-types.ts), [`deliveryMode`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRlmHeartbeatForState.input-typeLiteral666.deliveryMode), [`createHeartbeatForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createHeartbeatForState), [`deliveryMode`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.updateRlmHeartbeatForState.input-typeLiteral676.deliveryMode), [`RpcCommand`](../modes/rpc/rpc-types.ts.md#RpcCommand), [`deliveryMode`](cron-jobs.ts.md#AgentCronJob.deliveryMode), [`consumeDeliveryOption`](cron-jobs.ts.md#consumeDeliveryOption), [`normalizeHeartbeatDeliveryMode`](cron-jobs.ts.md#normalizeHeartbeatDeliveryMode), [`resolveHeartbeatStreamingBehavior`](cron-jobs.ts.md#resolveHeartbeatStreamingBehavior), [`setHeartbeat`](../modes/agent-connection/types.ts.md#AgentConnection.setHeartbeat), [`setHeartbeat`](../modes/agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.setHeartbeat), [`setHeartbeat`](../modes/rpc/rpc-client.ts.md#RpcClient.setHeartbeat), [`DEFAULT_HEARTBEAT_DELIVERY_MODE`](cron-jobs.ts.md#DEFAULT_HEARTBEAT_DELIVERY_MODE), [`deliveryMode`](cron-jobs.ts.md#CreateAgentCronJobInput.deliveryMode), [`consumeLeadingDeliveryFlag`](cron-jobs.ts.md#consumeLeadingDeliveryFlag), [`consumeTrailingDeliveryFlag`](cron-jobs.ts.md#consumeTrailingDeliveryFlag), [`deliveryMode`](cron-jobs.ts.md#AgentCronJobStore.updateRlmHeartbeat.update-typeLiteral153.deliveryMode), [`deliveryMode`](cron-jobs.ts.md#consumeDeliveryOption.typeLiteral693.deliveryMode), [`parseDeliveryModeToken`](cron-jobs.ts.md#parseDeliveryModeToken), [`deliveryMode`](cron-jobs.ts.md#AgentRlmHeartbeatController.createRlmHeartbeat.input-typeLiteral22.deliveryMode), [`deliveryMode`](cron-jobs.ts.md#AgentRlmHeartbeatController.updateRlmHeartbeat.input-typeLiteral23.deliveryMode), [`setHeartbeat`](../modes/agent-connection/in-process-agent-connection.ts.md#InProcessAgentConnection.setHeartbeat), [`ParsedHeartbeatCommand`](cron-jobs.ts.md#ParsedHeartbeatCommand)

### `AgentHeartbeatManagementAction`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L20)
- signature: `type AgentHeartbeatManagementAction`
- used by: [`interactive-mode.ts`](../modes/interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`DaemonCommand`](../modes/daemon/daemon-protocol.ts.md#DaemonCommand), [`daemon-agent-connection.ts`](../modes/agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](../modes/agent-connection/in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`daemon-protocol.ts`](../modes/daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`rpc-client.ts`](../modes/rpc/rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`rpc-types.ts`](../modes/rpc/rpc-types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-types.ts), [`heartbeat-manager.ts`](../modes/interactive/components/heartbeat-manager.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-heartbeat-manager.ts), [`manageHeartbeat`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.manageHeartbeat), [`manageHeartbeat`](cron-jobs.ts.md#AgentCronJobStore.manageHeartbeat), [`RpcCommand`](../modes/rpc/rpc-types.ts.md#RpcCommand), [`manageHeartbeat`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.manageHeartbeat), [`runAction`](../modes/interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.runAction), [`action`](../modes/interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.availableActions.Array.typeLiteral116.action), [`manageHeartbeat`](../modes/agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.manageHeartbeat), [`manageHeartbeat`](../modes/agent-connection/types.ts.md#AgentConnection.manageHeartbeat), [`manageHeartbeat`](../modes/rpc/rpc-client.ts.md#RpcClient.manageHeartbeat), [`onAction`](../modes/interactive/components/heartbeat-manager.ts.md#HeartbeatManagerOptions.onAction), [`manageHeartbeat`](../modes/agent-connection/in-process-agent-connection.ts.md#InProcessAgentConnection.manageHeartbeat), [`actionDescription`](../modes/interactive/components/heartbeat-manager.ts.md#HeartbeatManagerComponent.actionDescription)  (4 test-only)

### `AgentHeartbeatUpdateAction`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L19)
- signature: `type AgentHeartbeatUpdateAction`
- used by: [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`DaemonCommand`](../modes/daemon/daemon-protocol.ts.md#DaemonCommand), [`daemon-agent-connection.ts`](../modes/agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](../modes/agent-connection/in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`daemon-protocol.ts`](../modes/daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`rpc-client.ts`](../modes/rpc/rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`rpc-types.ts`](../modes/rpc/rpc-types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-types.ts), [`updateHeartbeatForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.updateHeartbeatForState), [`RpcCommand`](../modes/rpc/rpc-types.ts.md#RpcCommand), [`updateHeartbeat`](../modes/agent-connection/types.ts.md#AgentConnection.updateHeartbeat), [`updateHeartbeat`](../modes/rpc/rpc-client.ts.md#RpcClient.updateHeartbeat), [`updateHeartbeat`](../modes/agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.updateHeartbeat), [`updateHeartbeat`](../modes/agent-connection/in-process-agent-connection.ts.md#InProcessAgentConnection.updateHeartbeat)

### `AgentRlmHeartbeatController`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:126`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L126)
- signature: `interface AgentRlmHeartbeatController`
- members:
  - `createRlmHeartbeat(method)` — [`L128`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L128)
  - `deleteRlmHeartbeat(method)` — [`L142`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L142)
  - `listRlmHeartbeats(method)` — [`L127`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L127)
  - `updateRlmHeartbeat(method)` — [`L134`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L134)
  - `deliveryMode` — [`L132`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L132)
  - `deliveryMode` — [`L140`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L140)
  - `id` — [`L135`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L135)
  - `includeInactive` — [`L127`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L127)
  - `instruction` — [`L129`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L129)
  - `instruction` — [`L136`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L136)
  - `interval` — [`L130`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L130)
  - `interval` — [`L137`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L137)
  - `label` — [`L131`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L131)
  - `label` — [`L138`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L138)
  - `status` — [`L139`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L139)
- uses (calls/refs, reference-scoped): [`AgentCronJob`](cron-jobs.ts.md#AgentCronJob), [`AgentHeartbeatDeliveryMode`](cron-jobs.ts.md#AgentHeartbeatDeliveryMode), [`AgentRlmHeartbeatStatusUpdate`](cron-jobs.ts.md#AgentRlmHeartbeatStatusUpdate)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`agent-session-services.ts`](agent-session-services.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-services.ts), [`handleRlmHeartbeatHostRequest`](agent-session.ts.md#AgentSession.handleRlmHeartbeatHostRequest), [`setRlmHeartbeatController`](agent-session.ts.md#AgentSession.setRlmHeartbeatController), [`_rlmHeartbeatController`](agent-session.ts.md#AgentSession._rlmHeartbeatController), [`rlmHeartbeatController`](agent-session-services.ts.md#AgentSessionCreationOptions.rlmHeartbeatController), [`rlmHeartbeatController`](agent-session.ts.md#AgentSessionConfig.rlmHeartbeatController)  (2 test-only)

### `AgentRlmHeartbeatStatusUpdate`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L21)
- signature: `type AgentRlmHeartbeatStatusUpdate`
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`status`](cron-jobs.ts.md#AgentCronJobStore.updateRlmHeartbeat.update-typeLiteral153.status), [`isRlmHeartbeatStatusUpdate`](agent-session.ts.md#isRlmHeartbeatStatusUpdate), [`status`](cron-jobs.ts.md#AgentRlmHeartbeatController.updateRlmHeartbeat.input-typeLiteral23.status)

### `CreateAgentCronJobInput`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:57`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L57)
- signature: `interface CreateAgentCronJobInput`
- members:
  - `activeSessionId` — [`L58`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L58)
  - `cwd` — [`L61`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L61)
  - `deliveryMode` — [`L67`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L67)
  - `label` — [`L62`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L62)
  - `now` — [`L68`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L68)
  - `prompt` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L63)
  - `runtimeKind` — [`L66`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L66)
  - `scheduleText` — [`L64`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L64)
  - `sessionFile` — [`L60`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L60)
  - `sessionId` — [`L59`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L59)
  - `source` — [`L65`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L65)
- uses (calls/refs, reference-scoped): [`AgentHeartbeatDeliveryMode`](cron-jobs.ts.md#AgentHeartbeatDeliveryMode), [`AgentCronJobRuntimeKind`](cron-jobs.ts.md#AgentCronJobRuntimeKind), [`AgentCronJobSource`](cron-jobs.ts.md#AgentCronJobSource)
- used by: [`createHeartbeat`](cron-jobs.ts.md#AgentCronJobStore.createHeartbeat), [`createRlmHeartbeat`](cron-jobs.ts.md#AgentCronJobStore.createRlmHeartbeat), [`create`](cron-jobs.ts.md#AgentCronJobStore.create), [`deliveryMode`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createRlmHeartbeatForState.input-typeLiteral666.deliveryMode), [`createHeartbeatForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createHeartbeatForState), [`createCronJobForState`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createCronJobForState)  (9 test-only)

### `CronFields`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:1406`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1406)
- signature: `interface CronFields`
- members:
  - `dayOfMonth` — [`L1409`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1409)
  - `dayOfWeek` — [`L1411`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1411)
  - `hour` — [`L1408`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1408)
  - `minute` — [`L1407`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1407)
  - `month` — [`L1410`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1410)
- used by: [`parseCronExpression`](cron-jobs.ts.md#parseCronExpression), [`matchesCronFields`](cron-jobs.ts.md#matchesCronFields)

### `CronJobsFile`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:94`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L94)
- signature: `interface CronJobsFile`
- members:
  - `dispatches` — [`L96`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L96)
  - `jobs` — [`L95`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L95)
- used by: [`readJobsState`](cron-jobs.ts.md#readJobsState)

### `CronJobsState`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:106`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L106)
- signature: `interface CronJobsState`
- members:
  - `dispatches` — [`L108`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L108)
  - `jobs` — [`L107`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L107)
- uses (calls/refs, reference-scoped): [`AgentCronJob`](cron-jobs.ts.md#AgentCronJob), [`AgentCronDispatchRecord`](cron-jobs.ts.md#AgentCronDispatchRecord)
- used by: [`writeJobs`](cron-jobs.ts.md#AgentCronJobStore.writeJobs), [`claimDueInState`](cron-jobs.ts.md#claimDueInState), [`error`](cron-jobs.ts.md#AgentCronJobStore.recordDispatchResult.result-typeLiteral336.error), [`readJobs`](cron-jobs.ts.md#AgentCronJobStore.readJobs), [`now`](cron-jobs.ts.md#migrateLegacyCronJobsToSessionArtifacts.options-typeLiteral536.now), [`mutateStates`](cron-jobs.ts.md#AgentCronJobStore.mutateStates), [`recoverInterruptedInState`](cron-jobs.ts.md#recoverInterruptedInState), [`readJobsState`](cron-jobs.ts.md#readJobsState), [`getClaimedJob`](cron-jobs.ts.md#AgentCronJobStore.getClaimedJob), [`recoverSessionArtifact`](cron-jobs.ts.md#AgentCronJobStore.recoverSessionArtifact), [`writeJobsFile`](cron-jobs.ts.md#writeJobsFile), [`readStates`](cron-jobs.ts.md#AgentCronJobStore.readStates), [`writeJobsState`](cron-jobs.ts.md#writeJobsState)

### `HeartbeatCronSessionActivity`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:85`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L85)
- signature: `interface HeartbeatCronSessionActivity`
- members:
  - `hasPendingSessionWork` — [`L90`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L90)
  - `isBashRunning` — [`L89`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L89)
  - `isCompacting` — [`L87`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L87)
  - `isRetrying` — [`L88`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L88)
  - `isStreaming` — [`L86`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L86)
  - `unfinishedActionCount` — [`L91`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L91)
- used by: [`shouldDeferHeartbeatCronJob`](cron-jobs.ts.md#shouldDeferHeartbeatCronJob)  (1 test-only)

### `ParsedHeartbeatCommand`
- def: [`packages/coding-agent/src/core/cron-jobs.ts:119`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L119)
- signature: `type ParsedHeartbeatCommand`
- uses (calls/refs, reference-scoped): [`AgentHeartbeatDeliveryMode`](cron-jobs.ts.md#AgentHeartbeatDeliveryMode)
- used by: [`parseHeartbeatCommand`](cron-jobs.ts.md#parseHeartbeatCommand)

## Functions
- `claimDueInState(state: CronJobsState, dueAt: Date, claimedAt: Date)` — [`L1574`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1574)
- `compareOptionalIso(left: string | undefined, right: string | undefined)` — [`L1657`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1657)
- `consumeDeliveryOption(text: string)` — [`L1252`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1252)
- `consumeEveryOption(text: string)` — [`L1316`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1316)
- `consumeLeadingDeliveryFlag(text: string)` — [`L1277`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1277)
- `consumeLeadingEverySchedule(text: string)` — [`L1330`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1330)
- `consumeTrailingDeliveryFlag(text: string)` — [`L1290`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1290)
- `errorMessage(error: unknown)` — [`L1670`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1670)
- `formatAgentCronJob(job: AgentCronJob)` — [`L1242`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1242)
- `heartbeatCatalogSignature(jobs: readonly AgentCronJob[])` — [`L145`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L145)
- `isAgentCronDispatchRecord(value: unknown)` — [`L1725`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1725)
- `isAgentCronJob(value: unknown)` — [`L1684`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1684)
- `isAtLeastAsFresh(candidate: AgentCronJob, current: AgentCronJob)` — [`L1645`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1645)
- `isDueJob(job: AgentCronJob, now: Date)` — [`L1493`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1493)
- `isHeartbeatCronJob(job: AgentCronJob)` — [`L1347`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1347)
- `matchesCronFields(date: Date, fields: CronFields)` — [`L1456`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1456)
- `mergeFreshJobs(currentJobs: readonly AgentCronJob[], nextJobs: readonly AgentCronJob[])` — [`L1631`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1631)
- `migrateLegacyCronJobsToSessionArtifacts(filePath: string, options?: { isSessionOwned?: ((job: AgentCronJob) => boolean) | undefined; now?: Date | undefined; })` — [`L894`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L894)
- `nextCronRunAfter(expression: string, after: Date)` — [`L1374`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1374)
- `nextRunAtForSchedule(schedule: AgentCronSchedule, after: Date)` — [`L1229`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1229)
- `normalizeCronAlias(text: string)` — [`L1468`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1468)
- `normalizeHeartbeatDeliveryMode(value: unknown)` — [`L1152`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1152)
- `normalizeHeartbeatSchedule(input: string | undefined)` — [`L1141`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1141)
- `normalizeOptionalLabel(label: string | undefined)` — [`L1674`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1674)
- `parseAgentCronSchedule(input: string, now?: Date)` — [`L1079`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1079)
- `parseCronExpression(expression: string)` — [`L1390`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1390)
- `parseCronField(field: string, min: number, max: number)` — [`L1414`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1414)
- `parseCronNumber(value: string | undefined, min: number, max: number)` — [`L1445`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1445)
- `parseDeliveryModeToken(token: string)` — [`L1308`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1308)
- `parseHeartbeatCommand(input: string)` — [`L1168`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1168)
- `readJobsState(path: string)` — [`L1531`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1531)
- `recoverInterruptedInState(state: CronJobsState, now: Date, recovered: AgentCronJob[], dispatchIds?: ReadonlySet<string> | undefined)` — [`L1602`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1602)
- `resolveHeartbeatStreamingBehavior(deliveryMode: AgentHeartbeatDeliveryMode | undefined)` — [`L1162`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1162)
- `shouldDeferHeartbeatCronJob(job: AgentCronJob, activity: HeartbeatCronSessionActivity)` — [`L1351`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1351)
- `stripMatchingQuotes(value: string)` — [`L1483`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1483)
- `withCronJobsStateLocks(paths: readonly string[], action: () => T)` — [`L1497`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1497)
- `withoutNextRunAt(job: AgentCronJob)` — [`L1679`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1679)
- `writeJobsFile(path: string, jobs: readonly AgentCronJob[], mergeCurrent: boolean)` — [`L1542`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1542)
- `writeJobsState(path: string, state: CronJobsState)` — [`L1550`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1550)

## Module values
- `DEFAULT_HEARTBEAT_DELIVERY_MODE` — [`L117`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L117)
- `DEFAULT_HEARTBEAT_SCHEDULE` — [`L116`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L116)
- `MAX_TIMEOUT_MS` — [`L113`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L113)
- `ONE_MINUTE_MS` — [`L115`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L115)
- `ONE_SECOND_MS` — [`L114`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L114)
- `SESSION_SCHEDULED_JOBS_FILENAME` — [`L111`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L111)
- `deliveryMode` — [`L1252`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1252)
- `isSessionOwned` — [`L896`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L896)
- `nextRunAt` — [`L1082`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1082)
- `now` — [`L896`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L896)
- `rest` — [`L1252`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1252)
- `schedule` — [`L1082`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/cron-jobs.ts#L1082)


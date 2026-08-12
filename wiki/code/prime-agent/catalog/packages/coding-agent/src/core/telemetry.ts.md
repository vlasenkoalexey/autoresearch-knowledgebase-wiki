---
title: 'Module: packages/coding-agent/src/core/telemetry.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/telemetry.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`telemetry.ts`/
symbols:
  installAgentTelemetry: installAgentTelemetry().
  captureOnboardingCompleted: captureOnboardingCompleted().
  TelemetryClient.-constructor: TelemetryClient#`<constructor>`().
  captureAgentCommandUsed: captureAgentCommandUsed().
  TelemetryClient.capture: TelemetryClient#capture().
  addUsage: addUsage().
  EMPTY_USAGE_TOTALS: EMPTY_USAGE_TOTALS.
  mergeUsage: mergeUsage().
  createActiveRun: createActiveRun().
  getOrCreateTelemetryInstallationId: getOrCreateTelemetryInstallationId().
  TelemetryClient.flush: TelemetryClient#flush().
  assistantMessage: assistantMessage().
  isTelemetryEnabled: isTelemetryEnabled().
  TelemetryClient.drainQueue: TelemetryClient#drainQueue().
  telemetryAuthCategory: telemetryAuthCategory().
  TelemetrySink.capture: TelemetrySink#capture().
  readInstallationId: readInstallationId().
  TelemetryClient.send: TelemetryClient#send().
  baseProperties: baseProperties().
  ActiveRun.usage: ActiveRun#usage.
  TelemetrySink: TelemetrySink#
  SessionTotals.usage: SessionTotals#usage.
  TelemetryClient.queue: TelemetryClient#queue.
  UsageTotals: UsageTotals#
  TelemetryClientOptions.agentDir: TelemetryClientOptions#agentDir.
  TelemetryClientOptions.randomId: TelemetryClientOptions#randomId.
  InstallAgentTelemetryOptions.settingsManager: InstallAgentTelemetryOptions#settingsManager.
  TelemetryClient.scheduleFlush: TelemetryClient#scheduleFlush().
  errorCategory: errorCategory().
  TelemetrySink.flush: TelemetrySink#flush().
  CaptureOnboardingCompletedOptions.authSource: CaptureOnboardingCompletedOptions#authSource.
  CaptureOnboardingCompletedOptions.storedCredentialType: CaptureOnboardingCompletedOptions#storedCredentialType.
  TelemetryProperties: TelemetryProperties#
  InstallAgentTelemetryOptions.sink: InstallAgentTelemetryOptions#sink.
  newUsageTotals: newUsageTotals().
  TelemetryClient.flushTimer: TelemetryClient#flushTimer.
  CaptureAgentCommandUsedOptions.settingsManager: CaptureAgentCommandUsedOptions#settingsManager.
  TelemetryEventName: TelemetryEventName#
  InstallAgentTelemetryOptions.agentDir: InstallAgentTelemetryOptions#agentDir.
  UsageTotals.modelCallCount: UsageTotals#modelCallCount.
  runOutcome: runOutcome().
  InstallAgentTelemetryOptions.executionMode: InstallAgentTelemetryOptions#executionMode.
  CaptureOnboardingCompletedOptions.settingsManager: CaptureOnboardingCompletedOptions#settingsManager.
  CaptureOnboardingCompletedOptions.outcome: CaptureOnboardingCompletedOptions#outcome.
  CaptureAgentCommandUsedOptions.sink: CaptureAgentCommandUsedOptions#sink.
  ActiveRun.lastAssistant: ActiveRun#lastAssistant.
  TelemetryEvent: TelemetryEvent#
  TelemetryClientOptions.now: TelemetryClientOptions#now.
  CaptureAgentCommandUsedOptions.commandName: CaptureAgentCommandUsedOptions#commandName.
  ActiveRun.agentEnded: ActiveRun#agentEnded.
  ActiveRun.firstTurnStartedAt: ActiveRun#firstTurnStartedAt.
  ActiveRun.currentTurnStartedAt: ActiveRun#currentTurnStartedAt.
  TelemetryClient.flushInFlight: TelemetryClient#flushInFlight.
  TelemetryBatch: TelemetryBatch#
  CaptureOnboardingCompletedOptions.sink: CaptureOnboardingCompletedOptions#sink.
  TelemetryClientOptions.fetch: TelemetryClientOptions#fetch.
  CaptureAgentCommandUsedOptions.agentDir: CaptureAgentCommandUsedOptions#agentDir.
  ActiveRun.maxModelLatencyMs: ActiveRun#maxModelLatencyMs.
  ActiveRun.toolCallCount: ActiveRun#toolCallCount.
  ActiveRun.compactionCount: ActiveRun#compactionCount.
  TelemetryClient.installationId: TelemetryClient#installationId.
  TelemetryExecutionMode: TelemetryExecutionMode#
  TelemetryEvent.name: TelemetryEvent#name.
  TelemetryEvent.properties: TelemetryEvent#properties.
  writeTelemetryStateAtomically: writeTelemetryStateAtomically().
  TelemetryClient: TelemetryClient#
  TelemetryOnboardingOutcome: TelemetryOnboardingOutcome#
  TelemetryState: TelemetryState#
  TelemetryState.installationId: TelemetryState#installationId.
  CaptureOnboardingCompletedOptions.agentDir: CaptureOnboardingCompletedOptions#agentDir.
  CaptureOnboardingCompletedOptions.durationMs: CaptureOnboardingCompletedOptions#durationMs.
  CaptureOnboardingCompletedOptions.provider: CaptureOnboardingCompletedOptions#provider.
  ActiveRun.firstModelEventMs: ActiveRun#firstModelEventMs.
  ActiveRun.visibleTtftMs: ActiveRun#visibleTtftMs.
  ActiveRun.modelLatencyMs: ActiveRun#modelLatencyMs.
  ActiveRun.turnCount: ActiveRun#turnCount.
  ActiveRun.toolErrorCount: ActiveRun#toolErrorCount.
  ActiveRun.retryCount: ActiveRun#retryCount.
  SessionTotals.runCount: SessionTotals#runCount.
  SessionTotals.successfulRunCount: SessionTotals#successfulRunCount.
  SessionTotals.failedRunCount: SessionTotals#failedRunCount.
  SessionTotals.abortedRunCount: SessionTotals#abortedRunCount.
  SessionTotals.promptCount: SessionTotals#promptCount.
  SessionTotals.toolCallCount: SessionTotals#toolCallCount.
  SessionTotals.compactionCount: SessionTotals#compactionCount.
  parseBooleanOverride: parseBooleanOverride().
  TelemetryClient.randomId: TelemetryClient#randomId.
  TelemetryClient.batchSize: TelemetryClient#batchSize.
  TELEMETRY_STATE_VERSION: TELEMETRY_STATE_VERSION.
  TelemetryState.version: TelemetryState#version.
  TelemetryClientOptions.endpoint: TelemetryClientOptions#endpoint.
  TelemetryClientOptions.batchSize: TelemetryClientOptions#batchSize.
  InstallAgentTelemetryOptions.now: InstallAgentTelemetryOptions#now.
  InstallAgentTelemetryOptions.randomId: InstallAgentTelemetryOptions#randomId.
  ActiveRun: ActiveRun#
  ActiveRun.startedAt: ActiveRun#startedAt.
  SessionTotals.startedAt: SessionTotals#startedAt.
  isInstallationId: isInstallationId().
  TelemetryClient.endpoint: TelemetryClient#endpoint.
  TelemetryClient.fetchImpl: TelemetryClient#fetchImpl.
  TelemetryClient.now: TelemetryClient#now.
  TelemetryClient.flushIntervalMs: TelemetryClient#flushIntervalMs.
  TelemetryClient.requestTimeoutMs: TelemetryClient#requestTimeoutMs.
  TelemetryClient.disabled: TelemetryClient#disabled.
  telemetryProviderCategory: telemetryProviderCategory().
  DEFAULT_TELEMETRY_ENDPOINT: DEFAULT_TELEMETRY_ENDPOINT.
  TELEMETRY_STATE_FILE: TELEMETRY_STATE_FILE.
  DEFAULT_BATCH_SIZE: DEFAULT_BATCH_SIZE.
  DEFAULT_FLUSH_INTERVAL_MS: DEFAULT_FLUSH_INTERVAL_MS.
  DEFAULT_REQUEST_TIMEOUT_MS: DEFAULT_REQUEST_TIMEOUT_MS.
  TelemetryPrimitive: TelemetryPrimitive#
  TelemetryAuthCategory: TelemetryAuthCategory#
  TelemetryEvent.id: TelemetryEvent#id.
  TelemetryEvent.timestamp: TelemetryEvent#timestamp.
  TelemetryBatch.installation_id: TelemetryBatch#installation_id.
  TelemetryBatch.events: TelemetryBatch#events.
  TelemetryClientOptions: TelemetryClientOptions#
  TelemetryClientOptions.flushIntervalMs: TelemetryClientOptions#flushIntervalMs.
  TelemetryClientOptions.requestTimeoutMs: TelemetryClientOptions#requestTimeoutMs.
  InstallAgentTelemetryOptions: InstallAgentTelemetryOptions#
  CaptureOnboardingCompletedOptions: CaptureOnboardingCompletedOptions#
  CaptureOnboardingCompletedOptions.now: CaptureOnboardingCompletedOptions#now.
  CaptureOnboardingCompletedOptions.randomId: CaptureOnboardingCompletedOptions#randomId.
  CaptureAgentCommandUsedOptions: CaptureAgentCommandUsedOptions#
  CaptureAgentCommandUsedOptions.now: CaptureAgentCommandUsedOptions#now.
  CaptureAgentCommandUsedOptions.randomId: CaptureAgentCommandUsedOptions#randomId.
  SessionTotals: SessionTotals#
  modelCategory: modelCategory().
---
# Module: [`packages/coding-agent/src/core/telemetry.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts)

## Classes
### `ActiveRun`
- def: [`packages/coding-agent/src/core/telemetry.ts:112`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L112)
- signature: `interface ActiveRun`
- members:
  - `agentEnded` — [`L114`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L114)
  - `compactionCount` — [`L124`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L124)
  - `currentTurnStartedAt` — [`L118`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L118)
  - `firstModelEventMs` — [`L116`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L116)
  - `firstTurnStartedAt` — [`L115`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L115)
  - `lastAssistant` — [`L127`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L127)
  - `maxModelLatencyMs` — [`L120`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L120)
  - `modelLatencyMs` — [`L119`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L119)
  - `retryCount` — [`L125`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L125)
  - `startedAt` — [`L113`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L113)
  - `toolCallCount` — [`L122`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L122)
  - `toolErrorCount` — [`L123`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L123)
  - `turnCount` — [`L121`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L121)
  - `usage` — [`L126`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L126)
  - `visibleTtftMs` — [`L117`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L117)
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../../ai/src/types.ts.md#AssistantMessage), [`UsageTotals`](telemetry.ts.md#UsageTotals)
- used by: [`installAgentTelemetry`](telemetry.ts.md#installAgentTelemetry), [`createActiveRun`](telemetry.ts.md#createActiveRun)

### `CaptureAgentCommandUsedOptions`
- def: [`packages/coding-agent/src/core/telemetry.ts:99`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L99)
- signature: `interface CaptureAgentCommandUsedOptions`
- members:
  - `agentDir` — [`L100`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L100)
  - `commandName` — [`L102`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L102)
  - `now` — [`L104`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L104)
  - `randomId` — [`L105`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L105)
  - `settingsManager` — [`L101`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L101)
  - `sink` — [`L103`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L103)
- uses (calls/refs, reference-scoped): [`SettingsManager`](settings-manager.ts.md#SettingsManager), [`TelemetrySink`](telemetry.ts.md#TelemetrySink)
- used by: [`setupEditorSubmitHandler`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.setupEditorSubmitHandler), [`captureAgentCommandUsed`](telemetry.ts.md#captureAgentCommandUsed)  (1 test-only)

### `CaptureOnboardingCompletedOptions`
- def: [`packages/coding-agent/src/core/telemetry.ts:86`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L86)
- signature: `interface CaptureOnboardingCompletedOptions`
- members:
  - `agentDir` — [`L87`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L87)
  - `authSource` — [`L92`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L92)
  - `durationMs` — [`L89`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L89)
  - `now` — [`L95`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L95)
  - `outcome` — [`L90`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L90)
  - `provider` — [`L91`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L91)
  - `randomId` — [`L96`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L96)
  - `settingsManager` — [`L88`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L88)
  - `sink` — [`L94`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L94)
  - `storedCredentialType` — [`L93`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L93)
- uses (calls/refs, reference-scoped): [`SettingsManager`](settings-manager.ts.md#SettingsManager), [`type`](auth-storage.ts.md#ApiKeyCredential.typeLiteral1.type), [`source`](auth-storage.ts.md#AuthStatus.typeLiteral5.source), [`AuthStatus`](auth-storage.ts.md#AuthStatus), [`AuthCredential`](auth-storage.ts.md#AuthCredential), [`TelemetrySink`](telemetry.ts.md#TelemetrySink), [`TelemetryOnboardingOutcome`](telemetry.ts.md#TelemetryOnboardingOutcome)
- used by: [`runStartupOnboarding`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.runStartupOnboarding), [`captureOnboardingCompleted`](telemetry.ts.md#captureOnboardingCompleted)  (1 test-only)

### `InstallAgentTelemetryOptions`
- def: [`packages/coding-agent/src/core/telemetry.ts:77`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L77)
- signature: `interface InstallAgentTelemetryOptions`
- members:
  - `agentDir` — [`L78`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L78)
  - `executionMode` — [`L80`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L80)
  - `now` — [`L82`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L82)
  - `randomId` — [`L83`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L83)
  - `settingsManager` — [`L79`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L79)
  - `sink` — [`L81`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L81)
- uses (calls/refs, reference-scoped): [`SettingsManager`](settings-manager.ts.md#SettingsManager), [`TelemetrySink`](telemetry.ts.md#TelemetrySink), [`AgentExecutionMode`](agent-session-config.ts.md#AgentExecutionMode)
- used by: [`installAgentTelemetry`](telemetry.ts.md#installAgentTelemetry), [`createAgentSessionFromServices`](agent-session-services.ts.md#createAgentSessionFromServices)  (1 test-only)

### `SessionTotals`
- def: [`packages/coding-agent/src/core/telemetry.ts:130`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L130)
- signature: `interface SessionTotals`
- members:
  - `abortedRunCount` — [`L135`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L135)
  - `compactionCount` — [`L138`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L138)
  - `failedRunCount` — [`L134`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L134)
  - `promptCount` — [`L136`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L136)
  - `runCount` — [`L132`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L132)
  - `startedAt` — [`L131`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L131)
  - `successfulRunCount` — [`L133`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L133)
  - `toolCallCount` — [`L137`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L137)
  - `usage` — [`L139`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L139)
- uses (calls/refs, reference-scoped): [`UsageTotals`](telemetry.ts.md#UsageTotals)
- used by: [`installAgentTelemetry`](telemetry.ts.md#installAgentTelemetry)

### `TelemetryAuthCategory`
- def: [`packages/coding-agent/src/core/telemetry.ts:32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L32)
- signature: `type TelemetryAuthCategory`
- used by: [`telemetryAuthCategory`](telemetry.ts.md#telemetryAuthCategory)

### `TelemetryBatch`
- def: [`packages/coding-agent/src/core/telemetry.ts:51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L51)
- signature: `interface TelemetryBatch`
- members:
  - `events` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L53)
  - `installation_id` — [`L52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L52)
- uses (calls/refs, reference-scoped): [`TelemetryEvent`](telemetry.ts.md#TelemetryEvent)
- used by: [`drainQueue`](telemetry.ts.md#TelemetryClient.drainQueue), [`send`](telemetry.ts.md#TelemetryClient.send)

### `TelemetryClient`  ·  implements/extends TelemetrySink
- def: [`packages/coding-agent/src/core/telemetry.ts:312`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L312)
- signature: `class TelemetryClient`
- members:
  - `<constructor>(options: TelemetryClientOptions)` — [`L326`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L326)
  - `capture(method)` — [`L336`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L336)
  - `drainQueue(method)` — [`L401`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L401)
  - `flush(method)` — [`L371`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L371)
  - `scheduleFlush(method)` — [`L360`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L360)
  - `send(method)` — [`L412`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L412)
  - `batchSize` — [`L317`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L317)
  - `disabled` — [`L324`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L324)
  - `endpoint` — [`L313`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L313)
  - `fetchImpl` — [`L314`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L314)
  - `flushInFlight` — [`L323`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L323)
  - `flushIntervalMs` — [`L318`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L318)
  - `flushTimer` — [`L322`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L322)
  - `installationId` — [`L320`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L320)
  - `now` — [`L315`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L315)
  - `queue` — [`L321`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L321)
  - `randomId` — [`L316`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L316)
  - `requestTimeoutMs` — [`L319`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L319)
- uses (calls/refs, reference-scoped): [`VERSION`](../config.ts.md#VERSION), [`getOrCreateTelemetryInstallationId`](telemetry.ts.md#getOrCreateTelemetryInstallationId), [`TelemetrySink`](telemetry.ts.md#TelemetrySink), [`agentDir`](telemetry.ts.md#TelemetryClientOptions.agentDir), [`randomId`](telemetry.ts.md#TelemetryClientOptions.randomId), [`TelemetryProperties`](telemetry.ts.md#TelemetryProperties), [`TelemetryEventName`](telemetry.ts.md#TelemetryEventName), [`TelemetryEvent`](telemetry.ts.md#TelemetryEvent), [`now`](telemetry.ts.md#TelemetryClientOptions.now), [`TelemetryBatch`](telemetry.ts.md#TelemetryBatch), [`fetch`](telemetry.ts.md#TelemetryClientOptions.fetch), [`name`](telemetry.ts.md#TelemetryEvent.name), [`properties`](telemetry.ts.md#TelemetryEvent.properties), [`batchSize`](telemetry.ts.md#TelemetryClientOptions.batchSize), [`endpoint`](telemetry.ts.md#TelemetryClientOptions.endpoint), [`TelemetryClientOptions`](telemetry.ts.md#TelemetryClientOptions), [`DEFAULT_BATCH_SIZE`](telemetry.ts.md#DEFAULT_BATCH_SIZE), [`DEFAULT_FLUSH_INTERVAL_MS`](telemetry.ts.md#DEFAULT_FLUSH_INTERVAL_MS), [`DEFAULT_REQUEST_TIMEOUT_MS`](telemetry.ts.md#DEFAULT_REQUEST_TIMEOUT_MS), [`DEFAULT_TELEMETRY_ENDPOINT`](telemetry.ts.md#DEFAULT_TELEMETRY_ENDPOINT), [`events`](telemetry.ts.md#TelemetryBatch.events), [`flushIntervalMs`](telemetry.ts.md#TelemetryClientOptions.flushIntervalMs), [`id`](telemetry.ts.md#TelemetryEvent.id), [`installation_id`](telemetry.ts.md#TelemetryBatch.installation_id), [`requestTimeoutMs`](telemetry.ts.md#TelemetryClientOptions.requestTimeoutMs), [`timestamp`](telemetry.ts.md#TelemetryEvent.timestamp)
- used by: [`installAgentTelemetry`](telemetry.ts.md#installAgentTelemetry), [`captureOnboardingCompleted`](telemetry.ts.md#captureOnboardingCompleted), [`captureAgentCommandUsed`](telemetry.ts.md#captureAgentCommandUsed), [`capture`](telemetry.ts.md#TelemetrySink.capture), [`TelemetrySink`](telemetry.ts.md#TelemetrySink), [`flush`](telemetry.ts.md#TelemetrySink.flush)  (1 test-only)

### `TelemetryClientOptions`
- def: [`packages/coding-agent/src/core/telemetry.ts:66`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L66)
- signature: `interface TelemetryClientOptions`
- members:
  - `agentDir` — [`L67`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L67)
  - `batchSize` — [`L72`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L72)
  - `endpoint` — [`L68`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L68)
  - `fetch` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L69)
  - `flushIntervalMs` — [`L73`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L73)
  - `now` — [`L70`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L70)
  - `randomId` — [`L71`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L71)
  - `requestTimeoutMs` — [`L74`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L74)
- used by: [`installAgentTelemetry`](telemetry.ts.md#installAgentTelemetry), [`captureOnboardingCompleted`](telemetry.ts.md#captureOnboardingCompleted), [`<constructor>`](telemetry.ts.md#TelemetryClient.-constructor), [`captureAgentCommandUsed`](telemetry.ts.md#captureAgentCommandUsed), [`capture`](telemetry.ts.md#TelemetryClient.capture)  (1 test-only)

### `TelemetryEvent`
- def: [`packages/coding-agent/src/core/telemetry.ts:44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L44)
- signature: `interface TelemetryEvent`
- members:
  - `id` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L45)
  - `name` — [`L46`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L46)
  - `properties` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L48)
  - `timestamp` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L47)
- uses (calls/refs, reference-scoped): [`TelemetryProperties`](telemetry.ts.md#TelemetryProperties), [`TelemetryEventName`](telemetry.ts.md#TelemetryEventName)
- used by: [`capture`](telemetry.ts.md#TelemetryClient.capture), [`queue`](telemetry.ts.md#TelemetryClient.queue), [`TelemetryBatch`](telemetry.ts.md#TelemetryBatch)  (1 test-only)

### `TelemetryEventName`
- def: [`packages/coding-agent/src/core/telemetry.ts:23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L23)
- signature: `type TelemetryEventName`
- used by: [`capture`](telemetry.ts.md#TelemetryClient.capture), [`capture`](telemetry.ts.md#TelemetrySink.capture), [`name`](telemetry.ts.md#TelemetryEvent.name)  (3 test-only)

### `TelemetryExecutionMode`
- def: [`packages/coding-agent/src/core/telemetry.ts:30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L30)
- signature: `type TelemetryExecutionMode`
- uses (calls/refs, reference-scoped): [`AgentExecutionMode`](agent-session-config.ts.md#AgentExecutionMode)
- used by: [`baseProperties`](telemetry.ts.md#baseProperties)

### `TelemetryOnboardingOutcome`
- def: [`packages/coding-agent/src/core/telemetry.ts:31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L31)
- signature: `type TelemetryOnboardingOutcome`
- used by: [`interactive-mode.ts`](../modes/interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`runStartupOnboarding`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.runStartupOnboarding), [`outcome`](telemetry.ts.md#CaptureOnboardingCompletedOptions.outcome)

### `TelemetryPrimitive`
- def: [`packages/coding-agent/src/core/telemetry.ts:20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L20)
- signature: `type TelemetryPrimitive`
- used by: [`TelemetryProperties`](telemetry.ts.md#TelemetryProperties)

### `TelemetryProperties`
- def: [`packages/coding-agent/src/core/telemetry.ts:21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L21)
- signature: `type TelemetryProperties`
- uses (calls/refs, reference-scoped): [`TelemetryPrimitive`](telemetry.ts.md#TelemetryPrimitive)
- used by: [`installAgentTelemetry`](telemetry.ts.md#installAgentTelemetry), [`capture`](telemetry.ts.md#TelemetryClient.capture), [`capture`](telemetry.ts.md#TelemetrySink.capture), [`baseProperties`](telemetry.ts.md#baseProperties), [`properties`](telemetry.ts.md#TelemetryEvent.properties)

### `TelemetrySink`
- def: [`packages/coding-agent/src/core/telemetry.ts:56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L56)
- signature: `interface TelemetrySink`
- members:
  - `capture(method)` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L57)
  - `flush(method)` — [`L58`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L58)
- uses (calls/refs, reference-scoped): [`capture`](telemetry.ts.md#TelemetryClient.capture), [`flush`](telemetry.ts.md#TelemetryClient.flush), [`TelemetryProperties`](telemetry.ts.md#TelemetryProperties), [`TelemetryEventName`](telemetry.ts.md#TelemetryEventName), [`TelemetryClient`](telemetry.ts.md#TelemetryClient)  (3 test-only)
- used by: [`installAgentTelemetry`](telemetry.ts.md#installAgentTelemetry), [`captureOnboardingCompleted`](telemetry.ts.md#captureOnboardingCompleted), [`captureAgentCommandUsed`](telemetry.ts.md#captureAgentCommandUsed), [`sink`](telemetry.ts.md#InstallAgentTelemetryOptions.sink), [`sink`](telemetry.ts.md#CaptureAgentCommandUsedOptions.sink), [`sink`](telemetry.ts.md#CaptureOnboardingCompletedOptions.sink), [`TelemetryClient`](telemetry.ts.md#TelemetryClient)  (2 test-only)

### `TelemetryState`
- def: [`packages/coding-agent/src/core/telemetry.ts:61`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L61)
- signature: `interface TelemetryState`
- members:
  - `installationId` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L63)
  - `version` — [`L62`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L62)
- used by: [`getOrCreateTelemetryInstallationId`](telemetry.ts.md#getOrCreateTelemetryInstallationId), [`readInstallationId`](telemetry.ts.md#readInstallationId), [`writeTelemetryStateAtomically`](telemetry.ts.md#writeTelemetryStateAtomically)

### `UsageTotals`
- def: [`packages/coding-agent/src/core/telemetry.ts:108`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L108)
- signature: `interface UsageTotals`
- members:
  - `modelCallCount` — [`L109`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L109)
- uses (calls/refs, reference-scoped): [`Usage`](../../../ai/src/types.ts.md#Usage)
- used by: [`installAgentTelemetry`](telemetry.ts.md#installAgentTelemetry), [`addUsage`](telemetry.ts.md#addUsage), [`EMPTY_USAGE_TOTALS`](telemetry.ts.md#EMPTY_USAGE_TOTALS), [`mergeUsage`](telemetry.ts.md#mergeUsage), [`usage`](telemetry.ts.md#ActiveRun.usage), [`usage`](telemetry.ts.md#SessionTotals.usage), [`newUsageTotals`](telemetry.ts.md#newUsageTotals)

## Functions
- `addUsage(target: UsageTotals, usage: Usage)` — [`L162`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L162)
- `assistantMessage(event: AgentSessionEvent)` — [`L585`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L585)
- `baseProperties(executionMode: TelemetryExecutionMode)` — [`L493`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L493)
- `captureAgentCommandUsed(options: CaptureAgentCommandUsedOptions)` — [`L527`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L527)
- `captureOnboardingCompleted(options: CaptureOnboardingCompletedOptions)` — [`L503`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L503)
- `createActiveRun(now: () => number)` — [`L592`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L592)
- `errorCategory(message: AssistantMessage | undefined)` — [`L549`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L549)
- `getOrCreateTelemetryInstallationId(agentDir: string, randomId?: () => string)` — [`L257`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L257)
- `installAgentTelemetry(session: AgentSession, options: InstallAgentTelemetryOptions)` — [`L607`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L607)
- `isInstallationId(value: unknown)` — [`L221`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L221)
- `isTelemetryEnabled(settingsManager: SettingsManager)` — [`L204`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L204)
- `mergeUsage(target: UsageTotals, usage: UsageTotals)` — [`L176`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L176)
- `modelCategory(model: string)` — [`L429`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L429)
- `newUsageTotals()` — [`L158`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L158)
- `parseBooleanOverride(value: string | undefined)` — [`L190`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L190)
- `readInstallationId(path: string)` — [`L228`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L228)
- `runOutcome(message: AssistantMessage | undefined)` — [`L575`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L575)
- `telemetryAuthCategory(source: "runtime" | "stale" | "stored" | "environment" | "prime_cli" | "fallback" | "models_json_key" | "models_json_command" | undefined, storedCredentialType?: "oauth" | "api_key" | undefined)` — [`L468`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L468)
- `telemetryProviderCategory(provider: string | undefined)` — [`L448`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L448)
- `writeTelemetryStateAtomically(path: string, state: TelemetryState)` — [`L239`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L239)

## Module values
- `DEFAULT_BATCH_SIZE` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L16)
- `DEFAULT_FLUSH_INTERVAL_MS` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L17)
- `DEFAULT_REQUEST_TIMEOUT_MS` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L18)
- `DEFAULT_TELEMETRY_ENDPOINT` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L13)
- `EMPTY_USAGE_TOTALS` — [`L142`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L142)
- `TELEMETRY_STATE_FILE` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L14)
- `TELEMETRY_STATE_VERSION` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/telemetry.ts#L15)


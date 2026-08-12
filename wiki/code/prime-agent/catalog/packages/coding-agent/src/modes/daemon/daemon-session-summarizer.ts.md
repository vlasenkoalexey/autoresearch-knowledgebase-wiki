---
title: 'Module: packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`daemon-session-summarizer.ts`/
symbols:
  generateAgentStatus: generateAgentStatus().
  DaemonSessionSummarizer.summarize: DaemonSessionSummarizer#summarize().
  buildStatusContext: buildStatusContext().
  parseAgentStatusResponse: parseAgentStatusResponse().
  DaemonSessionSummarizer.notifyActivity: DaemonSessionSummarizer#notifyActivity().
  agentStatusChanged: agentStatusChanged().
  DaemonSessionSummarizer.-constructor: DaemonSessionSummarizer#`<constructor>`().
  resolveSummaryModel: resolveSummaryModel().
  DaemonSessionSummarizer.seed: DaemonSessionSummarizer#seed().
  isSessionWorking: isSessionWorking().
  DaemonSessionSummarizer.stop: DaemonSessionSummarizer#stop().
  DaemonSessionSummarizer.forget: DaemonSessionSummarizer#forget().
  AgentStatusResult.taskState: AgentStatusResult#taskState.
  cleanRecap: cleanRecap().
  DaemonSessionSummarizer.start: DaemonSessionSummarizer#start().
  DaemonSessionSummarizer.debounceTimers: DaemonSessionSummarizer#debounceTimers.
  AgentStatusResult: AgentStatusResult#
  AgentStatusResult.summary: AgentStatusResult#summary.
  messageText: messageText().
  DaemonSessionSummarizer.interval: DaemonSessionSummarizer#interval.
  DaemonSessionSummarizer.inFlight: DaemonSessionSummarizer#inFlight.
  GenerateAgentStatusParams.registry: GenerateAgentStatusParams#registry.
  GenerateAgentStatusParams.messages: GenerateAgentStatusParams#messages.
  messageText.typeLiteral3.text: messageText().typeLiteral3:text.
  messageText.typeLiteral3.tools: messageText().typeLiteral3:tools.
  DaemonSessionSummarizer.rerunRequested: DaemonSessionSummarizer#rerunRequested.
  DaemonSessionSummarizer: DaemonSessionSummarizer#
  GenerateAgentStatusParams: GenerateAgentStatusParams#
  GenerateAgentStatusParams.isWorking: GenerateAgentStatusParams#isWorking.
  GenerateAgentStatusParams.signal: GenerateAgentStatusParams#signal.
  SWEEP_INTERVAL_MS: SWEEP_INTERVAL_MS.
  SETTLE_DEBOUNCE_MS: SETTLE_DEBOUNCE_MS.
  SUMMARY_MODEL_PROVIDER: SUMMARY_MODEL_PROVIDER.
  SUMMARY_MODEL_ID: SUMMARY_MODEL_ID.
  SUMMARY_CONTEXT_MESSAGES: SUMMARY_CONTEXT_MESSAGES.
  SUMMARY_MAX_CHARS_PER_MESSAGE: SUMMARY_MAX_CHARS_PER_MESSAGE.
  SUMMARY_MAX_TOKENS: SUMMARY_MAX_TOKENS.
  AGENT_STATUS_SYSTEM_PROMPT: AGENT_STATUS_SYSTEM_PROMPT.
  clamp: clamp().
  REASONING_TRAILER: REASONING_TRAILER.
  COUNTING_ARTIFACT: COUNTING_ARTIFACT.
  MAX_RECAP_WORDS: MAX_RECAP_WORDS.
---
# Module: [`packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts)

## Classes
### `AgentStatusResult`
- def: [`packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts:35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L35)
- signature: `interface AgentStatusResult`
- members:
  - `summary` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L36)
  - `taskState` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L37)
- uses (calls/refs, reference-scoped): [`AgentTaskState`](../../core/session-manager.ts.md#AgentTaskState)
- used by: [`generateAgentStatus`](daemon-session-summarizer.ts.md#generateAgentStatus), [`summarize`](daemon-session-summarizer.ts.md#DaemonSessionSummarizer.summarize), [`parseAgentStatusResponse`](daemon-session-summarizer.ts.md#parseAgentStatusResponse), [`<constructor>`](daemon-session-summarizer.ts.md#DaemonSessionSummarizer.-constructor), [`agentStatusChanged`](daemon-session-summarizer.ts.md#agentStatusChanged)  (1 test-only)

### `DaemonSessionSummarizer`
- def: [`packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts:211`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L211)
- doc: Background status summarization for daemon-hosted sessions, top-level and
- signature: `class DaemonSessionSummarizer`
- members:
  - `<constructor>(listSessions: () => readonly ActiveSessionState[], onStatusChanged?: ((state: ActiveSessionState) => void) | undefined, generate?: (params: GenerateAgentStatusParams) => Promise<...>)` — [`L219`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L219) — Background status summarization for daemon-hosted sessions, top-level and
  - `forget(method)` — [`L256`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L256) — Drop any pending work for a session that is closing.
  - `notifyActivity(method)` — [`L278`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L278) — Called when a session finishes a turn; debounce until the agent settles.
  - `seed(method)` — [`L267`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L267) — Seed in-memory status from the persisted entry when a session is added.
  - `start(method)` — [`L228`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L228)
  - `stop(method)` — [`L240`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L240)
  - `summarize(method)` — [`L292`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L292)
  - `debounceTimers` — [`L213`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L213)
  - `inFlight` — [`L215`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L215)
  - `interval` — [`L212`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L212)
  - `rerunRequested` — [`L217`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L217)
- uses (calls/refs, reference-scoped): [`activeSessionId`](active-session-state.ts.md#ActiveSessionState.activeSessionId), [`runtime`](active-session-state.ts.md#ActiveSessionState.runtime), [`ActiveSessionState`](active-session-state.ts.md#ActiveSessionState), [`<get>session`](../../core/agent-session-runtime.ts.md#AgentSessionRuntime.-get-session), [`<get>messages`](../../core/agent-session.ts.md#AgentSession.-get-messages), [`sessionManager`](../../core/agent-session.ts.md#AgentSession.sessionManager), [`generateAgentStatus`](daemon-session-summarizer.ts.md#generateAgentStatus), [`getLatestAgentStatus`](../../core/session-manager.ts.md#SessionManager.getLatestAgentStatus), [`<get>modelRegistry`](../../core/agent-session.ts.md#AgentSession.-get-modelRegistry), [`appendAgentStatus`](../../core/session-manager.ts.md#SessionManager.appendAgentStatus), [`summaryState`](active-session-state.ts.md#ActiveSessionState.summaryState), [`summary`](../../core/session-manager.ts.md#AgentStatus.summary), [`<get>state`](../../core/agent-session.ts.md#AgentSession.-get-state), [`taskState`](../../core/session-manager.ts.md#AgentStatus.taskState), [`basedOnMessageCount`](../../core/session-manager.ts.md#AgentStatus.basedOnMessageCount), [`AgentStatus`](../../core/session-manager.ts.md#AgentStatus), [`isSessionWorking`](daemon-session-summarizer.ts.md#isSessionWorking), [`streamingMessage`](../../../../agent/src/types.ts.md#AgentState.streamingMessage), [`taskState`](daemon-session-summarizer.ts.md#AgentStatusResult.taskState), [`AgentStatusResult`](daemon-session-summarizer.ts.md#AgentStatusResult), [`summary`](daemon-session-summarizer.ts.md#AgentStatusResult.summary), [`messages`](daemon-session-summarizer.ts.md#GenerateAgentStatusParams.messages), [`registry`](daemon-session-summarizer.ts.md#GenerateAgentStatusParams.registry), [`GenerateAgentStatusParams`](daemon-session-summarizer.ts.md#GenerateAgentStatusParams), [`isWorking`](daemon-session-summarizer.ts.md#GenerateAgentStatusParams.isWorking), [`signal`](daemon-session-summarizer.ts.md#GenerateAgentStatusParams.signal), [`SETTLE_DEBOUNCE_MS`](daemon-session-summarizer.ts.md#SETTLE_DEBOUNCE_MS), [`SWEEP_INTERVAL_MS`](daemon-session-summarizer.ts.md#SWEEP_INTERVAL_MS)
- used by: [`daemon-mode.ts`](daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`addRuntime`](daemon-mode.ts.md#AgentDaemon.addRuntime), [`closeSessionOnce`](daemon-mode.ts.md#AgentDaemon.closeSessionOnce), [`broadcastToSession`](daemon-mode.ts.md#AgentDaemon.broadcastToSession), [`shutdown`](daemon-mode.ts.md#AgentDaemon.shutdown), [`start`](daemon-mode.ts.md#AgentDaemon.start), [`refreshReplacedSessionState`](daemon-mode.ts.md#AgentDaemon.refreshReplacedSessionState), [`summarizer`](daemon-mode.ts.md#AgentDaemon.summarizer)  (1 test-only)

### `GenerateAgentStatusParams`
- def: [`packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts:143`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L143)
- signature: `interface GenerateAgentStatusParams`
- members:
  - `isWorking` — [`L146`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L146)
  - `messages` — [`L145`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L145)
  - `registry` — [`L144`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L144)
  - `signal` — [`L147`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L147)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage), [`ModelRegistry`](../../core/model-registry.ts.md#ModelRegistry)
- used by: [`generateAgentStatus`](daemon-session-summarizer.ts.md#generateAgentStatus), [`summarize`](daemon-session-summarizer.ts.md#DaemonSessionSummarizer.summarize), [`<constructor>`](daemon-session-summarizer.ts.md#DaemonSessionSummarizer.-constructor)

## Functions
- `agentStatusChanged(previous: AgentStatus | undefined, next: AgentStatusResult)` — [`L193`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L193) — True when the new status differs enough from the stored one to be worth broadcasting.
- `buildStatusContext(messages: readonly AgentMessage[], isWorking: boolean)` — [`L81`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L81) — Serialize the trailing messages into a compact prompt body (tool calls by name only).
- `clamp(text: string, max: number)` — [`L75`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L75)
- `cleanRecap(raw: string)` — [`L108`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L108)
- `generateAgentStatus(params: GenerateAgentStatusParams)` — [`L151`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L151) — One cheap model call for a fresh status, or undefined if unavailable/empty/failed.
- `isSessionWorking(state: ActiveSessionState)` — [`L200`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L200)
- `messageText(content: unknown)` — [`L49`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L49)
- `parseAgentStatusResponse(text: string, isWorking: boolean)` — [`L125`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L125) — Take the content of the last `<recap>` and `<status>` tags; idle verdicts default to needs_input.
- `resolveSummaryModel(registry: ModelRegistry)` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L41) — Resolve the cheap summary model, or undefined when it has no configured auth.

## Module values
- `AGENT_STATUS_SYSTEM_PROMPT` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L20)
- `COUNTING_ARTIFACT` — [`L105`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L105)
- `MAX_RECAP_WORDS` — [`L106`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L106)
- `REASONING_TRAILER` — [`L104`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L104)
- `SETTLE_DEBOUNCE_MS` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L10)
- `SUMMARY_CONTEXT_MESSAGES` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L15)
- `SUMMARY_MAX_CHARS_PER_MESSAGE` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L16)
- `SUMMARY_MAX_TOKENS` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L18)
- `SUMMARY_MODEL_ID` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L13)
- `SUMMARY_MODEL_PROVIDER` — [`L12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L12)
- `SWEEP_INTERVAL_MS` — [`L8`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L8)
- `text` — [`L49`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L49)
- `tools` — [`L49`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-session-summarizer.ts#L49)


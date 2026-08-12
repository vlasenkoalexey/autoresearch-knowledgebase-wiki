---
title: 'Module: packages/coding-agent/src/core/autonomous.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/autonomous.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`autonomous.ts`/
symbols:
  createAutonomousRuntimeState: createAutonomousRuntimeState().
  runAutonomousQualityGates: runAutonomousQualityGates().
  autonomousStatus: autonomousStatus().
  nextAutonomousContinuation: nextAutonomousContinuation().
  AgentAutonomousGateConfig.commands: AgentAutonomousGateConfig#commands.
  AgentAutonomousStatus: AgentAutonomousStatus#
  AgentAutonomousStatus.continuationsUsed: AgentAutonomousStatus#continuationsUsed.
  runChildProcess.options-typeLiteral75.signal: runChildProcess().(options)typeLiteral75:signal.
  AgentAutonomousGateConfig.maxRetries: AgentAutonomousGateConfig#maxRetries.
  AgentAutonomousStatus.enabled: AgentAutonomousStatus#enabled.
  autonomousLimitReason: autonomousLimitReason().
  AgentAutonomousStatus.limits: AgentAutonomousStatus#limits.
  AgentAutonomousConfig.maxContinuations: AgentAutonomousConfig#maxContinuations.
  AgentAutonomousConfig.maxTurns: AgentAutonomousConfig#maxTurns.
  AgentAutonomousConfig.maxTokens: AgentAutonomousConfig#maxTokens.
  AgentAutonomousConfig.timeoutMs: AgentAutonomousConfig#timeoutMs.
  AgentAutonomousGateConfig.timeoutMs: AgentAutonomousGateConfig#timeoutMs.
  AgentAutonomousStatus.gates: AgentAutonomousStatus#gates.
  AutonomousRuntimeState.lastGateFailure: AutonomousRuntimeState#lastGateFailure.
  AgentAutonomousStatus.lastGateFailure: AgentAutonomousStatus#lastGateFailure.
  shouldAutonomouslyContinue: shouldAutonomouslyContinue().
  AgentAutonomousStatus.turnsUsed: AgentAutonomousStatus#turnsUsed.
  AgentAutonomousStatus.tokensUsed: AgentAutonomousStatus#tokensUsed.
  refreshAutonomousQualityGates: refreshAutonomousQualityGates().
  AgentAutonomousStatus.startedAt: AgentAutonomousStatus#startedAt.
  AgentAutonomousStatus.gateAttempts: AgentAutonomousStatus#gateAttempts.
  captureGitWorktreeSnapshot: captureGitWorktreeSnapshot().
  AgentAutonomousConfig: AgentAutonomousConfig#
  setAutonomousEnabled._options-typeLiteral4.cwd: setAutonomousEnabled().(_options)typeLiteral4:cwd.
  addAutonomousUsage: addAutonomousUsage().
  DEFAULT_AUTONOMOUS_LIMITS: DEFAULT_AUTONOMOUS_LIMITS.
  AutonomousRuntimeState.lastGateFailureSnapshot: AutonomousRuntimeState#lastGateFailureSnapshot.
  AutonomousRuntimeState.gateAttempts: AutonomousRuntimeState#gateAttempts.
  buildAutonomousGateFailureContinuation: buildAutonomousGateFailureContinuation().
  AutonomousRuntimeState: AutonomousRuntimeState#
  buildGateFailureContinuation: buildGateFailureContinuation().
  formatProcessExit: formatProcessExit().
  DEFAULT_AUTONOMOUS_GATES: DEFAULT_AUTONOMOUS_GATES.
  AgentAutonomousConfig.gates: AgentAutonomousConfig#gates.
  AutonomousRuntimeState.gates: AutonomousRuntimeState#gates.
  autonomousTokenDelta: autonomousTokenDelta().
  gitWorktreeSnapshotsEqual: gitWorktreeSnapshotsEqual().
  AutonomousRuntimeState.continuationsUsed: AutonomousRuntimeState#continuationsUsed.
  addAutonomousContinuation: addAutonomousContinuation().
  AutonomousRuntimeState.enabled: AutonomousRuntimeState#enabled.
  DEFAULT_AUTONOMOUS_CONTINUATION_PROMPT: DEFAULT_AUTONOMOUS_CONTINUATION_PROMPT.
  AutonomousOperationOptions.signal: AutonomousOperationOptions#signal.
  hashUntrackedFiles: hashUntrackedFiles().
  ChildProcessResult.status: ChildProcessResult#status.
  normalizeLimit: normalizeLimit().
  setAutonomousEnabled: setAutonomousEnabled().
  AgentAutonomousGateFailure.exitText: AgentAutonomousGateFailure#exitText.
  AutonomousRuntimeState.turnsUsed: AutonomousRuntimeState#turnsUsed.
  AutonomousRuntimeState.tokensUsed: AutonomousRuntimeState#tokensUsed.
  ChildProcessResult.error: ChildProcessResult#error.
  AutonomousRuntimeState.limits: AutonomousRuntimeState#limits.
  AgentAutonomousGateConfig: AgentAutonomousGateConfig#
  AgentAutonomousGateFailure.attempt: AgentAutonomousGateFailure#attempt.
  AgentAutonomousGateFailure.output: AgentAutonomousGateFailure#output.
  AutonomousRuntimeState.startedAt: AutonomousRuntimeState#startedAt.
  GitWorktreeSnapshot: GitWorktreeSnapshot#
  ChildProcessResult.signal: ChildProcessResult#signal.
  ChildProcessResult.stdout: ChildProcessResult#stdout.
  ChildProcessResult.timedOut: ChildProcessResult#timedOut.
  AutonomousLimitState: AutonomousLimitState#
  GateFailure: GateFailure#
  truncateGateOutput: truncateGateOutput().
  AgentAutonomousGateFailure: AgentAutonomousGateFailure#
  AgentAutonomousGateFailure.command: AgentAutonomousGateFailure#command.
  AutonomousRuntimeState.continuationPrompt: AutonomousRuntimeState#continuationPrompt.
  AutonomousLimitReason: AutonomousLimitReason#
  AutonomousOperationOptions: AutonomousOperationOptions#
  ChildProcessResult: ChildProcessResult#
  ChildProcessResult.outputTruncated: ChildProcessResult#outputTruncated.
  runChildProcess: runChildProcess().
  MAX_GATE_OUTPUT_CHARS: MAX_GATE_OUTPUT_CHARS.
  AutonomousGateResult: AutonomousGateResult#
  GitWorktreeSnapshot.status: GitWorktreeSnapshot#status.
  GitWorktreeSnapshot.diff: GitWorktreeSnapshot#diff.
  GitWorktreeSnapshot.untrackedHash: GitWorktreeSnapshot#untrackedHash.
  runChildProcess.options-typeLiteral75.timeoutMs: runChildProcess().(options)typeLiteral75:timeoutMs.
  AgentAutonomousConfig.enabled: AgentAutonomousConfig#enabled.
  AgentAutonomousConfig.continuationPrompt: AgentAutonomousConfig#continuationPrompt.
  MAX_CHILD_PROCESS_OUTPUT_CHARS: MAX_CHILD_PROCESS_OUTPUT_CHARS.
  AutonomousDecision: AutonomousDecision#
  AutonomousDecision.shouldContinue: AutonomousDecision#shouldContinue.
  AutonomousDecision.reason: AutonomousDecision#reason.
  AutonomousOperationOptions.cwd: AutonomousOperationOptions#cwd.
  untrackedPathsFromStatus: untrackedPathsFromStatus().
  hashUntrackedPath: hashUntrackedPath().
  ChildProcessResult.stderr: ChildProcessResult#stderr.
  runChildProcess.options-typeLiteral75.cwd: runChildProcess().(options)typeLiteral75:cwd.
  runChildProcess.options-typeLiteral75.shell: runChildProcess().(options)typeLiteral75:shell.
  runChildProcess.options-typeLiteral75.maxOutputChars: runChildProcess().(options)typeLiteral75:maxOutputChars.
  createAutonomousRuntimeState._options-typeLiteral0.cwd: createAutonomousRuntimeState().(_options)typeLiteral0:cwd.
---
# Module: [`packages/coding-agent/src/core/autonomous.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts)

## Classes
### `AgentAutonomousConfig`
- def: [`packages/coding-agent/src/core/autonomous.ts:10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L10)
- signature: `interface AgentAutonomousConfig`
- members:
  - `continuationPrompt` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L16)
  - `enabled` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L11)
  - `gates` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L17)
  - `maxContinuations` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L12)
  - `maxTokens` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L14)
  - `maxTurns` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L13)
  - `timeoutMs` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L15)
- uses (calls/refs, reference-scoped): [`AgentAutonomousGateConfig`](autonomous.ts.md#AgentAutonomousGateConfig)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`sdk.ts`](sdk.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-sdk.ts), [`agent-session-services.ts`](agent-session-services.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-services.ts), [`createAutonomousRuntimeState`](autonomous.ts.md#createAutonomousRuntimeState), [`autonomousLimitReason`](autonomous.ts.md#autonomousLimitReason), [`limits`](autonomous.ts.md#AgentAutonomousStatus.limits), [`describeAutonomousLimit`](../modes/print-mode.ts.md#describeAutonomousLimit), [`agent-session-config.ts`](agent-session-config.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-config.ts), [`_formatAutonomousStatus`](agent-session.ts.md#AgentSession._formatAutonomousStatus), [`DEFAULT_AUTONOMOUS_LIMITS`](autonomous.ts.md#DEFAULT_AUTONOMOUS_LIMITS), [`autonomous`](agent-session-config.ts.md#AgentSessionRuntimeConfig.autonomous), [`autonomous`](sdk.ts.md#CreateAgentSessionOptions.autonomous), [`mergeAutonomousConfig`](agent-session-config.ts.md#mergeAutonomousConfig), [`mergeAutonomousGateConfig`](agent-session-config.ts.md#mergeAutonomousGateConfig), [`autonomous`](agent-session.ts.md#AgentSessionConfig.autonomous), [`limits`](autonomous.ts.md#AutonomousRuntimeState.limits), [`autonomous`](agent-session-services.ts.md#AgentSessionCreationOptions.autonomous)  (6 test-only)

### `AgentAutonomousGateConfig`
- def: [`packages/coding-agent/src/core/autonomous.ts:20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L20)
- signature: `interface AgentAutonomousGateConfig`
- members:
  - `commands` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L21)
  - `maxRetries` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L22)
  - `timeoutMs` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L23)
- used by: [`runPrintModeWithConnectionInternal`](../modes/print-mode.ts.md#runPrintModeWithConnectionInternal), [`createAutonomousRuntimeState`](autonomous.ts.md#createAutonomousRuntimeState), [`waitForHeadlessCompletion`](../modes/headless-completion.ts.md#waitForHeadlessCompletion), [`runAutonomousQualityGates`](autonomous.ts.md#runAutonomousQualityGates), [`autonomousStatus`](autonomous.ts.md#autonomousStatus), [`gates`](autonomous.ts.md#AgentAutonomousStatus.gates), [`refreshAutonomousQualityGates`](autonomous.ts.md#refreshAutonomousQualityGates), [`shouldContinueAutonomousGates`](../modes/headless-completion.ts.md#shouldContinueAutonomousGates), [`buildGateFailureContinuation`](autonomous.ts.md#buildGateFailureContinuation), [`DEFAULT_AUTONOMOUS_GATES`](autonomous.ts.md#DEFAULT_AUTONOMOUS_GATES), [`gates`](autonomous.ts.md#AgentAutonomousConfig.gates), [`gates`](autonomous.ts.md#AutonomousRuntimeState.gates), [`mergeAutonomousGateConfig`](agent-session-config.ts.md#mergeAutonomousGateConfig)  (4 test-only)

### `AgentAutonomousGateFailure`
- def: [`packages/coding-agent/src/core/autonomous.ts:26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L26)
- signature: `interface AgentAutonomousGateFailure`
- members:
  - `attempt` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L28)
  - `command` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L27)
  - `exitText` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L29)
  - `output` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L30)
- used by: [`runPrintModeWithConnectionInternal`](../modes/print-mode.ts.md#runPrintModeWithConnectionInternal), [`waitForHeadlessCompletion`](../modes/headless-completion.ts.md#waitForHeadlessCompletion), [`runAutonomousQualityGates`](autonomous.ts.md#runAutonomousQualityGates), [`lastGateFailure`](autonomous.ts.md#AgentAutonomousStatus.lastGateFailure), [`autonomousMeta`](../modes/acp/acp-mode.ts.md#autonomousMeta), [`autonomousProgressKey`](../modes/headless-completion.ts.md#autonomousProgressKey), [`latestAutonomousGateAttempt`](../modes/headless-completion.ts.md#latestAutonomousGateAttempt), [`buildAutonomousGateFailureContinuation`](autonomous.ts.md#buildAutonomousGateFailureContinuation), [`GateFailure`](autonomous.ts.md#GateFailure)  (1 test-only)

### `AgentAutonomousStatus`
- def: [`packages/coding-agent/src/core/autonomous.ts:33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L33)
- signature: `interface AgentAutonomousStatus`
- members:
  - `continuationsUsed` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L35)
  - `enabled` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L34)
  - `gateAttempts` — [`L41`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L41)
  - `gates` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L40)
  - `lastGateFailure` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L42)
  - `limits` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L39)
  - `startedAt` — [`L38`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L38)
  - `tokensUsed` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L37)
  - `turnsUsed` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L36)
- uses (calls/refs, reference-scoped): [`AgentAutonomousConfig`](autonomous.ts.md#AgentAutonomousConfig), [`AgentAutonomousGateConfig`](autonomous.ts.md#AgentAutonomousGateConfig), [`AgentAutonomousGateFailure`](autonomous.ts.md#AgentAutonomousGateFailure)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`daemon-agent-connection.ts`](../modes/agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](../modes/agent-connection/in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`daemon-protocol.ts`](../modes/daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`runPrintModeWithConnectionInternal`](../modes/print-mode.ts.md#runPrintModeWithConnectionInternal), [`acp-mode.ts`](../modes/acp/acp-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-acp-acp-mode.ts), [`waitForHeadlessCompletion`](../modes/headless-completion.ts.md#waitForHeadlessCompletion), [`autonomousStatus`](autonomous.ts.md#autonomousStatus), [`print-mode.ts`](../modes/print-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-print-mode.ts), [`headless-completion.ts`](../modes/headless-completion.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-headless-completion.ts), [`_emitAutonomousStatus`](agent-session.ts.md#AgentSession._emitAutonomousStatus), [`getAutonomousStatus`](agent-session.ts.md#AgentSession.getAutonomousStatus), [`autonomousLimitReason`](autonomous.ts.md#autonomousLimitReason), [`describeAutonomousLimit`](../modes/print-mode.ts.md#describeAutonomousLimit), [`acpStopReason`](../modes/acp/acp-stop-reason.ts.md#acpStopReason), [`autonomousMeta`](../modes/acp/acp-mode.ts.md#autonomousMeta), [`_formatAutonomousStatus`](agent-session.ts.md#AgentSession._formatAutonomousStatus), [`shouldContinueAutonomousGates`](../modes/headless-completion.ts.md#shouldContinueAutonomousGates), [`autonomousProgressKey`](../modes/headless-completion.ts.md#autonomousProgressKey), [`latestAutonomousGateAttempt`](../modes/headless-completion.ts.md#latestAutonomousGateAttempt), [`acp-stop-reason.ts`](../modes/acp/acp-stop-reason.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-acp-acp-stop-reason.ts), [`waitForHeadlessCompletion`](../modes/agent-connection/types.ts.md#AgentConnection.waitForHeadlessCompletion), [`waitForHeadlessCompletion`](../modes/agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.waitForHeadlessCompletion), [`waitForHeadlessCompletion`](../modes/agent-connection/in-process-agent-connection.ts.md#InProcessAgentConnection.waitForHeadlessCompletion), [`AutonomousLimitState`](autonomous.ts.md#AutonomousLimitState), [`DaemonAutonomousStatus`](../modes/daemon/daemon-protocol.ts.md#DaemonAutonomousStatus)  (8 test-only)

### `AutonomousDecision`
- def: [`packages/coding-agent/src/core/autonomous.ts:88`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L88)
- signature: `interface AutonomousDecision`
- members:
  - `reason` — [`L90`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L90)
  - `shouldContinue` — [`L89`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L89)
- used by: [`nextAutonomousContinuation`](autonomous.ts.md#nextAutonomousContinuation), [`shouldAutonomouslyContinue`](autonomous.ts.md#shouldAutonomouslyContinue)

### `AutonomousGateResult`
- def: [`packages/coding-agent/src/core/autonomous.ts:81`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L81)
- signature: `type AutonomousGateResult`
- used by: [`runAutonomousQualityGates`](autonomous.ts.md#runAutonomousQualityGates), [`refreshAutonomousQualityGates`](autonomous.ts.md#refreshAutonomousQualityGates)

### `AutonomousLimitReason`
- def: [`packages/coding-agent/src/core/autonomous.ts:80`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L80)
- signature: `type AutonomousLimitReason`
- used by: [`print-mode.ts`](../modes/print-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-print-mode.ts), [`autonomousLimitReason`](autonomous.ts.md#autonomousLimitReason), [`describeAutonomousLimit`](../modes/print-mode.ts.md#describeAutonomousLimit)

### `AutonomousLimitState`
- def: [`packages/coding-agent/src/core/autonomous.ts:83`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L83)
- signature: `type AutonomousLimitState`
- uses (calls/refs, reference-scoped): [`AgentAutonomousStatus`](autonomous.ts.md#AgentAutonomousStatus)
- used by: [`autonomousLimitReason`](autonomous.ts.md#autonomousLimitReason)

### `AutonomousOperationOptions`
- def: [`packages/coding-agent/src/core/autonomous.ts:99`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L99)
- signature: `interface AutonomousOperationOptions`
- members:
  - `cwd` — [`L100`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L100)
  - `signal` — [`L101`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L101)
- used by: [`nextAutonomousContinuation`](autonomous.ts.md#nextAutonomousContinuation), [`shouldAutonomouslyContinue`](autonomous.ts.md#shouldAutonomouslyContinue), [`refreshAutonomousQualityGates`](autonomous.ts.md#refreshAutonomousQualityGates)

### `AutonomousRuntimeState`
- def: [`packages/coding-agent/src/core/autonomous.ts:66`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L66)
- signature: `interface AutonomousRuntimeState`
- members:
  - `continuationPrompt` — [`L73`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L73)
  - `continuationsUsed` — [`L68`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L68)
  - `enabled` — [`L67`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L67)
  - `gateAttempts` — [`L75`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L75)
  - `gates` — [`L74`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L74)
  - `lastGateFailure` — [`L76`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L76)
  - `lastGateFailureSnapshot` — [`L77`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L77)
  - `limits` — [`L72`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L72)
  - `startedAt` — [`L71`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L71)
  - `tokensUsed` — [`L70`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L70)
  - `turnsUsed` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L69)
- uses (calls/refs, reference-scoped): [`AgentAutonomousConfig`](autonomous.ts.md#AgentAutonomousConfig), [`AgentAutonomousGateConfig`](autonomous.ts.md#AgentAutonomousGateConfig), [`GitWorktreeSnapshot`](autonomous.ts.md#GitWorktreeSnapshot), [`GateFailure`](autonomous.ts.md#GateFailure)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`createAutonomousRuntimeState`](autonomous.ts.md#createAutonomousRuntimeState), [`runAutonomousQualityGates`](autonomous.ts.md#runAutonomousQualityGates), [`autonomousStatus`](autonomous.ts.md#autonomousStatus), [`nextAutonomousContinuation`](autonomous.ts.md#nextAutonomousContinuation), [`shouldAutonomouslyContinue`](autonomous.ts.md#shouldAutonomouslyContinue), [`refreshAutonomousQualityGates`](autonomous.ts.md#refreshAutonomousQualityGates), [`_autonomousState`](agent-session.ts.md#AgentSession._autonomousState), [`cwd`](autonomous.ts.md#setAutonomousEnabled._options-typeLiteral4.cwd), [`addAutonomousUsage`](autonomous.ts.md#addAutonomousUsage), [`_restoreAutonomousRuntimeSnapshot`](agent-session.ts.md#AgentSession._restoreAutonomousRuntimeSnapshot), [`_snapshotAutonomousRuntimeState`](agent-session.ts.md#AgentSession._snapshotAutonomousRuntimeState), [`buildGateFailureContinuation`](autonomous.ts.md#buildGateFailureContinuation), [`addAutonomousContinuation`](autonomous.ts.md#addAutonomousContinuation), [`AutonomousRuntimeSnapshot`](agent-session.ts.md#AutonomousRuntimeSnapshot), [`setAutonomousEnabled`](autonomous.ts.md#setAutonomousEnabled)  (2 test-only)

### `ChildProcessResult`
- def: [`packages/coding-agent/src/core/autonomous.ts:471`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L471)
- signature: `interface ChildProcessResult`
- members:
  - `error` — [`L476`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L476)
  - `outputTruncated` — [`L478`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L478)
  - `signal` — [`L473`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L473)
  - `status` — [`L472`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L472)
  - `stderr` — [`L475`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L475)
  - `stdout` — [`L474`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L474)
  - `timedOut` — [`L477`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L477)
- used by: [`runAutonomousQualityGates`](autonomous.ts.md#runAutonomousQualityGates), [`signal`](autonomous.ts.md#runChildProcess.options-typeLiteral75.signal), [`captureGitWorktreeSnapshot`](autonomous.ts.md#captureGitWorktreeSnapshot), [`formatProcessExit`](autonomous.ts.md#formatProcessExit)

### `GateFailure`
- def: [`packages/coding-agent/src/core/autonomous.ts:104`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L104)
- signature: `type GateFailure`
- uses (calls/refs, reference-scoped): [`AgentAutonomousGateFailure`](autonomous.ts.md#AgentAutonomousGateFailure)
- used by: [`lastGateFailure`](autonomous.ts.md#AutonomousRuntimeState.lastGateFailure)

### `GitWorktreeSnapshot`
- def: [`packages/coding-agent/src/core/autonomous.ts:93`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L93)
- signature: `interface GitWorktreeSnapshot`
- members:
  - `diff` — [`L95`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L95)
  - `status` — [`L94`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L94)
  - `untrackedHash` — [`L96`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L96)
- used by: [`captureGitWorktreeSnapshot`](autonomous.ts.md#captureGitWorktreeSnapshot), [`lastGateFailureSnapshot`](autonomous.ts.md#AutonomousRuntimeState.lastGateFailureSnapshot), [`gitWorktreeSnapshotsEqual`](autonomous.ts.md#gitWorktreeSnapshotsEqual)

## Functions
- `addAutonomousContinuation(state: AutonomousRuntimeState)` — [`L179`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L179)
- `addAutonomousUsage(state: AutonomousRuntimeState, usage: Usage | undefined)` — [`L171`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L171)
- `autonomousLimitReason(state: AutonomousLimitState, now?: number)` — [`L254`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L254)
- `autonomousStatus(state: AutonomousRuntimeState)` — [`L157`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L157)
- `autonomousTokenDelta(usage: Usage | undefined)` — [`L186`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L186)
- `buildAutonomousGateFailureContinuation(failure: AgentAutonomousGateFailure, maxRetries: number, timestamp?: number)` — [`L350`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L350)
- `buildGateFailureContinuation(state: AutonomousRuntimeState, timestamp: number)` — [`L362`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L362)
- `captureGitWorktreeSnapshot(cwd: string | undefined, signal?: AbortSignal | undefined)` — [`L374`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L374)
- `createAutonomousRuntimeState(config?: AgentAutonomousConfig | undefined, _options?: { cwd?: string | undefined; })` — [`L106`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L106)
- `formatProcessExit(result: ChildProcessResult)` — [`L571`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L571)
- `gitWorktreeSnapshotsEqual(a: GitWorktreeSnapshot | undefined, b: GitWorktreeSnapshot | undefined)` — [`L370`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L370)
- `hashUntrackedFiles(cwd: string, status: string, signal?: AbortSignal | undefined)` — [`L433`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L433)
- `hashUntrackedPath(path: string, signal?: AbortSignal | undefined)` — [`L446`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L446)
- `nextAutonomousContinuation(state: AutonomousRuntimeState, message: AssistantMessage, options?: AutonomousOperationOptions, now?: number)` — [`L196`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L196)
- `normalizeLimit(value: number | undefined, fallback: number)` — [`L588`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L588)
- `refreshAutonomousQualityGates(state: AutonomousRuntimeState, options?: AutonomousOperationOptions)` — [`L273`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L273)
- `runAutonomousQualityGates(state: AutonomousRuntimeState, cwd: string | undefined, signal: AbortSignal | undefined)` — [`L284`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L284)
- `runChildProcess(command: string, args: string[], options?: { cwd?: string | undefined; shell?: boolean | undefined; timeoutMs?: number | undefined; maxOutputChars?: number | undefined; signal?: AbortSignal | undefined; })` — [`L481`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L481)
- `setAutonomousEnabled(state: AutonomousRuntimeState, enabled: boolean, _options?: { cwd?: string | undefined; })` — [`L135`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L135)
- `shouldAutonomouslyContinue(state: AutonomousRuntimeState, message: AssistantMessage, options?: AutonomousOperationOptions, now?: number)` — [`L227`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L227)
- `truncateGateOutput(output: string, outputAlreadyTruncated?: boolean, maxChars?: number)` — [`L581`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L581)
- `untrackedPathsFromStatus(status: string)` — [`L425`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L425)

## Module values
- `DEFAULT_AUTONOMOUS_CONTINUATION_PROMPT` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L45)
- `DEFAULT_AUTONOMOUS_GATES` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L57)
- `DEFAULT_AUTONOMOUS_LIMITS` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L48)
- `MAX_CHILD_PROCESS_OUTPUT_CHARS` — [`L64`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L64)
- `MAX_GATE_OUTPUT_CHARS` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L63)
- `cwd` — [`L108`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L108)
- `cwd` — [`L138`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L138)
- `cwd` — [`L485`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L485)
- `maxOutputChars` — [`L488`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L488)
- `shell` — [`L486`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L486)
- `signal` — [`L489`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L489)
- `timeoutMs` — [`L487`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/autonomous.ts#L487)


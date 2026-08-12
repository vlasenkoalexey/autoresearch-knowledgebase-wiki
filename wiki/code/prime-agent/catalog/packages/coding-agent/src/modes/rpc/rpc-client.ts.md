---
title: 'Module: packages/coding-agent/src/modes/rpc/rpc-client.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/rpc/rpc-client.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/rpc/`rpc-client.ts`/
symbols:
  RpcClient.send: RpcClient#send().
  RpcClient.start: RpcClient#start().
  RpcClient.getData: RpcClient#getData().
  RpcClient.promptAndWait: RpcClient#promptAndWait().
  RpcClient.refine: RpcClient#refine().
  RpcClient.handleLine: RpcClient#handleLine().
  RpcClient.getState: RpcClient#getState().
  RpcClient.process: RpcClient#process.
  RpcClient.stop: RpcClient#stop().
  RpcClient.bash: RpcClient#bash().
  RpcClient.setHeartbeat: RpcClient#setHeartbeat().
  RpcClient.updateHeartbeat: RpcClient#updateHeartbeat().
  RpcClient.manageHeartbeat: RpcClient#manageHeartbeat().
  RpcClient.getAvailableModels: RpcClient#getAvailableModels().
  RpcClient.cycleThinkingLevel: RpcClient#cycleThinkingLevel().
  RpcClient.compact: RpcClient#compact().
  RpcClient.getSessionStats: RpcClient#getSessionStats().
  RpcClient.collectEvents: RpcClient#collectEvents().
  RpcClient: RpcClient#
  RpcClient.onEvent: RpcClient#onEvent().
  RpcClient.-constructor: RpcClient#`<constructor>`().
  RpcClient.cycleModel: RpcClient#cycleModel().
  RpcClient.getMessages: RpcClient#getMessages().
  RpcClient.sendAgentMessage: RpcClient#sendAgentMessage().
  RpcClient.getAgentMessageStatus: RpcClient#getAgentMessageStatus().
  RpcClient.pauseAgentMessages: RpcClient#pauseAgentMessages().
  RpcClient.resumeAgentMessages: RpcClient#resumeAgentMessages().
  RpcClient.listSchedules: RpcClient#listSchedules().
  RpcClient.addSchedule: RpcClient#addSchedule().
  RpcClient.cancelSchedule: RpcClient#cancelSchedule().
  RpcClient.listHeartbeats: RpcClient#listHeartbeats().
  RpcClient.getHeartbeat: RpcClient#getHeartbeat().
  RpcClient.observe: RpcClient#observe().
  RpcClient.getCommands: RpcClient#getCommands().
  RpcClient.pendingRequests: RpcClient#pendingRequests.
  RpcClient.onObservedSessionEvent: RpcClient#onObservedSessionEvent().
  RpcClient.getLastAssistantText: RpcClient#getLastAssistantText().
  RpcEventListener: RpcEventListener#
  RpcClient.eventListeners: RpcClient#eventListeners.
  RpcClient.observedSessionListeners: RpcClient#observedSessionListeners.
  RpcCommandBody: RpcCommandBody#
  RpcClient.stderr: RpcClient#stderr.
  RpcClient.prompt: RpcClient#prompt().
  RpcClient.newSession: RpcClient#newSession().
  RpcClient.setThinkingLevel: RpcClient#setThinkingLevel().
  RpcClient.exportHtml: RpcClient#exportHtml().
  RpcClient.clone: RpcClient#clone().
  RpcClient.pendingRequests.Map.typeLiteral4.resolve: RpcClient#pendingRequests.Map:typeLiteral4:resolve.
  RpcClient.steer: RpcClient#steer().
  RpcClient.followUp: RpcClient#followUp().
  RpcClient.setModel: RpcClient#setModel().
  RpcClient.switchSession: RpcClient#switchSession().
  RpcClient.fork: RpcClient#fork().
  RpcClient.getForkMessages: RpcClient#getForkMessages().
  RpcClient.clearAgentMessages: RpcClient#clearAgentMessages().
  RpcClient.waitForIdle: RpcClient#waitForIdle().
  RpcObservedSessionListener: RpcObservedSessionListener#
  REFINE_REQUEST_TIMEOUT_MS: REFINE_REQUEST_TIMEOUT_MS.
  ModelInfo: ModelInfo#
  RpcClient.abort: RpcClient#abort().
  RpcClient.setSessionName: RpcClient#setSessionName().
  RpcClientOptions: RpcClientOptions#
  RpcClient.stopReadingStdout: RpcClient#stopReadingStdout.
  RpcClient.exportHtml.Promise.typeLiteral192.path: RpcClient#exportHtml().Promise:typeLiteral192:path.
  RpcClient.getStderr: RpcClient#getStderr().
  RpcClient.setSteeringMode: RpcClient#setSteeringMode().
  RpcClient.setFollowUpMode: RpcClient#setFollowUpMode().
  RpcClient.setAutoCompaction: RpcClient#setAutoCompaction().
  RpcClient.setAutoRetry: RpcClient#setAutoRetry().
  RpcClient.abortRetry: RpcClient#abortRetry().
  RpcClient.abortBash: RpcClient#abortBash().
  RpcClient.unobserve: RpcClient#unobserve().
  RpcClientOptions.provider: RpcClientOptions#provider.
  RpcClientOptions.model: RpcClientOptions#model.
  RpcClientOptions.args: RpcClientOptions#args.
  RpcClient.pendingRequests.Map.typeLiteral4.reject: RpcClient#pendingRequests.Map:typeLiteral4:reject.
  RpcClient.refine.options-typeLiteral173.global: RpcClient#refine().(options)typeLiteral173:global.
  DistributiveOmit: DistributiveOmit#
  RpcClientOptions.cliPath: RpcClientOptions#cliPath.
  RpcClientOptions.cwd: RpcClientOptions#cwd.
  RpcClientOptions.env: RpcClientOptions#env.
  ModelInfo.provider: ModelInfo#provider.
  ModelInfo.id: ModelInfo#id.
  ModelInfo.contextWindow: ModelInfo#contextWindow.
  ModelInfo.reasoning: ModelInfo#reasoning.
  RpcClient.requestId: RpcClient#requestId.
  RpcClient.refine.options-typeLiteral173.instructions: RpcClient#refine().(options)typeLiteral173:instructions.
  RpcClient.refine.options-typeLiteral173.rollbackId: RpcClient#refine().(options)typeLiteral173:rollbackId.
  RpcClient.newSession.Promise.typeLiteral134.cancelled: RpcClient#newSession().Promise:typeLiteral134:cancelled.
  RpcClient.setModel.Promise.typeLiteral141.provider: RpcClient#setModel().Promise:typeLiteral141:provider.
  RpcClient.setModel.Promise.typeLiteral141.id: RpcClient#setModel().Promise:typeLiteral141:id.
  RpcClient.switchSession.Promise.typeLiteral196.cancelled: RpcClient#switchSession().Promise:typeLiteral196:cancelled.
  RpcClient.fork.Promise.typeLiteral200.text: RpcClient#fork().Promise:typeLiteral200:text.
  RpcClient.fork.Promise.typeLiteral200.cancelled: RpcClient#fork().Promise:typeLiteral200:cancelled.
  RpcClient.clone.Promise.typeLiteral204.cancelled: RpcClient#clone().Promise:typeLiteral204:cancelled.
  RpcClient.getForkMessages.Promise.Array.typeLiteral208.entryId: RpcClient#getForkMessages().Promise:Array:typeLiteral208:entryId.
  RpcClient.getForkMessages.Promise.Array.typeLiteral208.text: RpcClient#getForkMessages().Promise:Array:typeLiteral208:text.
---
# Module: [`packages/coding-agent/src/modes/rpc/rpc-client.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts)

## Classes
### `DistributiveOmit`
- def: [`packages/coding-agent/src/modes/rpc/rpc-client.ts:39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L39)
- doc: Distributive Omit that works with union types
- signature: `type DistributiveOmit`
- used by: [`RpcCommandBody`](rpc-client.ts.md#RpcCommandBody)

### `ModelInfo`
- def: [`packages/coding-agent/src/modes/rpc/rpc-client.ts:59`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L59)
- signature: `interface ModelInfo`
- members:
  - `contextWindow` — [`L62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L62)
  - `id` — [`L61`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L61)
  - `provider` — [`L60`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L60)
  - `reasoning` — [`L63`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L63)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`getAvailableModels`](rpc-client.ts.md#RpcClient.getAvailableModels)  (1 test-only)

### `RpcClient`
- def: [`packages/coding-agent/src/modes/rpc/rpc-client.ts:73`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L73)
- signature: `class RpcClient`
- members:
  - `<constructor>(options?: RpcClientOptions)` — [`L83`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L83)
  - `abort(method)` — [`L218`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L218) — Abort current operation.
  - `abortBash(method)` — [`L358`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L358) — Abort running bash command.
  - `abortRetry(method)` — [`L343`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L343) — Abort in-progress retry.
  - `addSchedule(method)` — [`L467`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L467)
  - `bash(method)` — [`L350`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L350) — Execute a bash command.
  - `cancelSchedule(method)` — [`L472`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L472)
  - `clearAgentMessages(method)` — [`L457`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L457)
  - `clone(method)` — [`L400`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L400) — Clone the current active branch into a new session.
  - `collectEvents(method)` — [`L563`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L563) — Collect events until agent becomes idle.
  - `compact(method)` — [`L300`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L300) — Compact session context.
  - `cycleModel(method)` — [`L251`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L251) — Cycle to next model.
  - `cycleThinkingLevel(method)` — [`L278`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L278) — Cycle thinking level.
  - `exportHtml(method)` — [`L373`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L373) — Export session to HTML.
  - `followUp(method)` — [`L211`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L211) — Queue a follow-up message to be processed after the agent finishes.
  - `fork(method)` — [`L391`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L391) — Fork from a specific message.
  - `getAgentMessageStatus(method)` — [`L445`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L445)
  - `getAvailableModels(method)` — [`L263`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L263) — Get list of available models.
  - `getCommands(method)` — [`L530`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L530) — Get available commands (extension commands, prompt templates, skills).
  - `getData(method)` — [`L661`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L661)
  - `getForkMessages(method)` — [`L408`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L408) — Get messages available for forking.
  - `getHeartbeat(method)` — [`L482`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L482)
  - `getLastAssistantText(method)` — [`L416`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L416) — Get text of last assistant message.
  - `getMessages(method)` — [`L431`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L431) — Get all messages in the session.
  - `getSessionStats(method)` — [`L365`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L365) — Get session statistics.
  - `getState(method)` — [`L235`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L235) — Get current session state.
  - `getStderr(method)` — [`L184`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L184) — Get collected stderr output (useful for debugging).
  - `handleLine(method)` — [`L595`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L595)
  - `listHeartbeats(method)` — [`L477`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L477)
  - `listSchedules(method)` — [`L462`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L462)
  - `manageHeartbeat(method)` — [`L505`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L505)
  - `newSession(method)` — [`L227`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L227) — Start a new session, optionally with parent tracking.
  - `observe(method)` — [`L518`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L518)
  - `onEvent(method)` — [`L161`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L161) — Subscribe to agent events.
  - `onObservedSessionEvent(method)` — [`L171`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L171)
  - `pauseAgentMessages(method)` — [`L449`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L449)
  - `prompt(method)` — [`L197`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L197) — Send a prompt to the agent.
  - `promptAndWait(method)` — [`L585`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L585) — Send prompt and wait for completion, returning all events.
  - `refine(method)` — [`L308`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L308) — Refine editable continual harness state.
  - `resumeAgentMessages(method)` — [`L453`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L453)
  - `send(method)` — [`L630`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L630)
  - `sendAgentMessage(method)` — [`L436`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L436)
  - `setAutoCompaction(method)` — [`L329`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L329) — Set auto-compaction enabled/disabled.
  - `setAutoRetry(method)` — [`L336`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L336) — Set auto-retry enabled/disabled.
  - `setFollowUpMode(method)` — [`L293`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L293) — Set follow-up mode.
  - `setHeartbeat(method)` — [`L487`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L487)
  - `setModel(method)` — [`L243`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L243) — Set model by provider and ID.
  - `setSessionName(method)` — [`L424`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L424) — Set the session display name.
  - `setSteeringMode(method)` — [`L286`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L286) — Set steering mode.
  - `setThinkingLevel(method)` — [`L271`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L271) — Set thinking level.
  - `start(method)` — [`L88`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L88) — Start the RPC agent process.
  - `steer(method)` — [`L204`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L204) — Queue a steering message to interrupt the agent mid-run.
  - `stop(method)` — [`L134`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L134) — Stop the RPC agent process.
  - `switchSession(method)` — [`L382`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L382) — Switch to a different session file.
  - `unobserve(method)` — [`L523`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L523)
  - `updateHeartbeat(method)` — [`L500`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L500)
  - `waitForIdle(method)` — [`L543`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L543) — Wait for agent to become idle (no streaming).
  - `cancelled` — [`L227`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L227)
  - `cancelled` — [`L382`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L382)
  - `cancelled` — [`L391`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L391)
  - `cancelled` — [`L400`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L400)
  - `entryId` — [`L408`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L408)
  - `eventListeners` — [`L76`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L76)
  - `global` — [`L309`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L309)
  - `id` — [`L243`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L243)
  - `instructions` — [`L309`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L309)
  - `observedSessionListeners` — [`L77`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L77)
  - `path` — [`L373`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L373)
  - `pendingRequests` — [`L78`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L78)
  - `process` — [`L74`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L74)
  - `provider` — [`L243`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L243)
  - `reject` — [`L78`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L78)
  - `requestId` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L80)
  - `resolve` — [`L78`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L78)
  - `rollbackId` — [`L309`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L309)
  - `stderr` — [`L81`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L81)
  - `stopReadingStdout` — [`L75`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L75)
  - `text` — [`L391`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L391)
  - `text` — [`L408`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L408)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage), [`AgentCronJob`](../../core/cron-jobs.ts.md#AgentCronJob), [`ImageContent`](../../../../ai/src/types.ts.md#ImageContent), [`ThinkingLevel`](../../../../agent/src/types.ts.md#ThinkingLevel), [`AgentEvent`](../../../../agent/src/types.ts.md#AgentEvent), [`AgentConnectionHeartbeat`](../agent-connection/types.ts.md#AgentConnectionHeartbeat), [`RpcResponse`](rpc-types.ts.md#RpcResponse), [`RefinementResult`](../../core/refinement/refinement.ts.md#RefinementResult), [`serializeJsonLine`](jsonl.ts.md#serializeJsonLine), [`AgentHeartbeatDeliveryMode`](../../core/cron-jobs.ts.md#AgentHeartbeatDeliveryMode), [`attachJsonlLineReader`](jsonl.ts.md#attachJsonlLineReader), [`AgentHeartbeatManagementAction`](../../core/cron-jobs.ts.md#AgentHeartbeatManagementAction), [`RpcCommand`](rpc-types.ts.md#RpcCommand), [`SessionStats`](../../core/session-stats.ts.md#SessionStats), [`AgentSessionMessageSafetyStatus`](../../core/agent-messages.ts.md#AgentSessionMessageSafetyStatus), [`BashResult`](../../core/bash-executor.ts.md#BashResult), [`CompactionResult`](../../core/compaction/compaction.ts.md#CompactionResult), [`AgentSessionMessageReceipt`](../../core/agent-messages.ts.md#AgentSessionMessageReceipt), [`AgentHeartbeatUpdateAction`](../../core/cron-jobs.ts.md#AgentHeartbeatUpdateAction), [`RpcSessionState`](rpc-types.ts.md#RpcSessionState), [`RpcEventListener`](rpc-client.ts.md#RpcEventListener), [`RpcObservedSessionEvent`](rpc-types.ts.md#RpcObservedSessionEvent), [`RpcCommandBody`](rpc-client.ts.md#RpcCommandBody), [`RpcSlashCommand`](rpc-types.ts.md#RpcSlashCommand), [`RpcObservedSessionListener`](rpc-client.ts.md#RpcObservedSessionListener), [`ModelInfo`](rpc-client.ts.md#ModelInfo), [`REFINE_REQUEST_TIMEOUT_MS`](rpc-client.ts.md#REFINE_REQUEST_TIMEOUT_MS), [`RpcClientOptions`](rpc-client.ts.md#RpcClientOptions), [`args`](rpc-client.ts.md#RpcClientOptions.args), [`model`](rpc-client.ts.md#RpcClientOptions.model), [`provider`](rpc-client.ts.md#RpcClientOptions.provider), [`cliPath`](rpc-client.ts.md#RpcClientOptions.cliPath), [`cwd`](rpc-client.ts.md#RpcClientOptions.cwd), [`env`](rpc-client.ts.md#RpcClientOptions.env)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts)  (6 test-only)

### `RpcClientOptions`
- def: [`packages/coding-agent/src/modes/rpc/rpc-client.ts:44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L44)
- signature: `interface RpcClientOptions`
- members:
  - `args` — [`L56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L56) — Additional CLI arguments
  - `cliPath` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L46) — Path to the CLI entry point (default: searches for dist/cli.js)
  - `cwd` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L48) — Working directory for the agent
  - `env` — [`L50`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L50) — Environment variables
  - `model` — [`L54`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L54) — Model ID to use
  - `provider` — [`L52`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L52) — Provider to use
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`start`](rpc-client.ts.md#RpcClient.start), [`<constructor>`](rpc-client.ts.md#RpcClient.-constructor)

### `RpcCommandBody`
- def: [`packages/coding-agent/src/modes/rpc/rpc-client.ts:42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L42)
- doc: RpcCommand without the id field (for internal send)
- signature: `type RpcCommandBody`
- uses (calls/refs, reference-scoped): [`RpcCommand`](rpc-types.ts.md#RpcCommand), [`DistributiveOmit`](rpc-client.ts.md#DistributiveOmit)
- used by: [`send`](rpc-client.ts.md#RpcClient.send)

### `RpcEventListener`
- def: [`packages/coding-agent/src/modes/rpc/rpc-client.ts:66`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L66)
- signature: `type RpcEventListener`
- uses (calls/refs, reference-scoped): [`AgentEvent`](../../../../agent/src/types.ts.md#AgentEvent)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`onEvent`](rpc-client.ts.md#RpcClient.onEvent), [`eventListeners`](rpc-client.ts.md#RpcClient.eventListeners)

### `RpcObservedSessionListener`
- def: [`packages/coding-agent/src/modes/rpc/rpc-client.ts:67`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L67)
- signature: `type RpcObservedSessionListener`
- uses (calls/refs, reference-scoped): [`RpcObservedSessionEvent`](rpc-types.ts.md#RpcObservedSessionEvent)
- used by: [`onObservedSessionEvent`](rpc-client.ts.md#RpcClient.onObservedSessionEvent), [`observedSessionListeners`](rpc-client.ts.md#RpcClient.observedSessionListeners)

## Module values
- `REFINE_REQUEST_TIMEOUT_MS` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-client.ts#L36) — Extended response timeout for refine requests, which run an LLM pass.


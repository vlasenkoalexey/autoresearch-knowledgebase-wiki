---
title: 'Module: packages/coding-agent/src/modes/rpc/rpc-types.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/rpc/rpc-types.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/rpc/`rpc-types.ts`/Rpc
symbols:
  RpcResponse: Response#
  RpcCommand: Command#
  RpcSessionState.model: SessionState#model.
  RpcSessionState: SessionState#
  RpcSessionState.thinkingLevel: SessionState#thinkingLevel.
  RpcExtensionUIRequest: ExtensionUIRequest#
  RpcExtensionUIResponse: ExtensionUIResponse#
  RpcObservedSessionEvent: ObservedSessionEvent#
  RpcSlashCommand: SlashCommand#
  RpcSessionState.messageCount: SessionState#messageCount.
  RpcSessionState.sessionActions: SessionState#sessionActions.
  RpcSessionState.goal: SessionState#goal.
  RpcSessionState.sessionName: SessionState#sessionName.
  RpcSlashCommand.sourceInfo: SlashCommand#sourceInfo.
  RpcCommandType: CommandType#
  RpcSessionState.isStreaming: SessionState#isStreaming.
  RpcSessionState.isCompacting: SessionState#isCompacting.
  RpcSessionState.steeringMode: SessionState#steeringMode.
  RpcSessionState.followUpMode: SessionState#followUpMode.
  RpcSessionState.sessionFile: SessionState#sessionFile.
  RpcSessionState.sessionId: SessionState#sessionId.
  RpcSessionState.autoCompactionEnabled: SessionState#autoCompactionEnabled.
  RpcSlashCommand.name: SlashCommand#name.
  RpcSlashCommand.description: SlashCommand#description.
  RpcSlashCommand.source: SlashCommand#source.
---
# Module: [`packages/coding-agent/src/modes/rpc/rpc-types.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts)

## Classes
### `RpcCommand`
- def: [`packages/coding-agent/src/modes/rpc/rpc-types.ts:29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L29)
- signature: `type RpcCommand`
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../../ai/src/types.ts.md#ImageContent), [`ThinkingLevel`](../../../../agent/src/types.ts.md#ThinkingLevel), [`AgentHeartbeatDeliveryMode`](../../core/cron-jobs.ts.md#AgentHeartbeatDeliveryMode), [`AgentHeartbeatManagementAction`](../../core/cron-jobs.ts.md#AgentHeartbeatManagementAction), [`AgentHeartbeatUpdateAction`](../../core/cron-jobs.ts.md#AgentHeartbeatUpdateAction)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`runRpcModeWithConnectionInternal`](rpc-mode.ts.md#runRpcModeWithConnectionInternal), [`rpc-client.ts`](rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`send`](rpc-client.ts.md#RpcClient.send), [`rpc-mode.ts`](rpc-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-mode.ts), [`RpcCommandBody`](rpc-client.ts.md#RpcCommandBody), [`RpcCommandType`](rpc-types.ts.md#RpcCommandType)

### `RpcCommandType`
- def: [`packages/coding-agent/src/modes/rpc/rpc-types.ts:352`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L352)
- signature: `type RpcCommandType`
- uses (calls/refs, reference-scoped): [`RpcCommand`](rpc-types.ts.md#RpcCommand)

### `RpcExtensionUIRequest`
- def: [`packages/coding-agent/src/modes/rpc/rpc-types.ts:301`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L301)
- doc: Emitted when an extension needs user input
- signature: `type RpcExtensionUIRequest`
- used by: [`runRpcModeWithConnectionInternal`](rpc-mode.ts.md#runRpcModeWithConnectionInternal), [`createRpcExtensionUiBridge`](rpc-extension-ui-context.ts.md#createRpcExtensionUiBridge), [`rpc-mode.ts`](rpc-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-mode.ts), [`rpc-extension-ui-context.ts`](rpc-extension-ui-context.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-extension-ui-context.ts)

### `RpcExtensionUIResponse`
- def: [`packages/coding-agent/src/modes/rpc/rpc-types.ts:343`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L343)
- doc: Response to an extension UI request
- signature: `type RpcExtensionUIResponse`
- used by: [`runRpcModeWithConnectionInternal`](rpc-mode.ts.md#runRpcModeWithConnectionInternal), [`createRpcExtensionUiBridge`](rpc-extension-ui-context.ts.md#createRpcExtensionUiBridge), [`rpc-mode.ts`](rpc-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-mode.ts), [`rpc-extension-ui-context.ts`](rpc-extension-ui-context.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-extension-ui-context.ts), [`handleResponse`](rpc-extension-ui-context.ts.md#RpcExtensionUiBridge.handleResponse)

### `RpcObservedSessionEvent`
- def: [`packages/coding-agent/src/modes/rpc/rpc-types.ts:354`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L354)
- signature: `type RpcObservedSessionEvent`
- uses (calls/refs, reference-scoped): [`AgentEvent`](../../../../agent/src/types.ts.md#AgentEvent)
- used by: [`rpc-client.ts`](rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`rpc-mode.ts`](rpc-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-mode.ts), [`handleLine`](rpc-client.ts.md#RpcClient.handleLine), [`RpcObservedSessionListener`](rpc-client.ts.md#RpcObservedSessionListener)

### `RpcResponse`
- def: [`packages/coding-agent/src/modes/rpc/rpc-types.ts:159`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L159)
- signature: `type RpcResponse`
- uses (calls/refs, reference-scoped): [`Model`](../../../../ai/src/types.ts.md#Model), [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage), [`AgentCronJob`](../../core/cron-jobs.ts.md#AgentCronJob), [`ThinkingLevel`](../../../../agent/src/types.ts.md#ThinkingLevel), [`AgentConnectionHeartbeat`](../agent-connection/types.ts.md#AgentConnectionHeartbeat), [`RefinementResult`](../../core/refinement/refinement.ts.md#RefinementResult), [`SessionStats`](../../core/session-stats.ts.md#SessionStats), [`AgentSessionMessageSafetyStatus`](../../core/agent-messages.ts.md#AgentSessionMessageSafetyStatus), [`BashResult`](../../core/bash-executor.ts.md#BashResult), [`CompactionResult`](../../core/compaction/compaction.ts.md#CompactionResult), [`AgentSessionMessageReceipt`](../../core/agent-messages.ts.md#AgentSessionMessageReceipt), [`RpcSessionState`](rpc-types.ts.md#RpcSessionState), [`RpcSlashCommand`](rpc-types.ts.md#RpcSlashCommand)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`runRpcModeWithConnectionInternal`](rpc-mode.ts.md#runRpcModeWithConnectionInternal), [`rpc-client.ts`](rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`send`](rpc-client.ts.md#RpcClient.send), [`rpc-mode.ts`](rpc-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-mode.ts), [`getData`](rpc-client.ts.md#RpcClient.getData), [`handleLine`](rpc-client.ts.md#RpcClient.handleLine), [`resolve`](rpc-client.ts.md#RpcClient.pendingRequests.Map.typeLiteral4.resolve)

### `RpcSessionState`
- def: [`packages/coding-agent/src/modes/rpc/rpc-types.ts:138`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L138)
- signature: `interface RpcSessionState`
- members:
  - `autoCompactionEnabled` — [`L148`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L148)
  - `followUpMode` — [`L144`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L144)
  - `goal` — [`L151`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L151)
  - `isCompacting` — [`L142`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L142)
  - `isStreaming` — [`L141`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L141)
  - `messageCount` — [`L149`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L149)
  - `model` — [`L139`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L139)
  - `sessionActions` — [`L150`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L150)
  - `sessionFile` — [`L145`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L145)
  - `sessionId` — [`L146`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L146)
  - `sessionName` — [`L147`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L147)
  - `steeringMode` — [`L143`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L143)
  - `thinkingLevel` — [`L140`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L140)
- uses (calls/refs, reference-scoped): [`Model`](../../../../ai/src/types.ts.md#Model), [`ThinkingLevel`](../../../../agent/src/types.ts.md#ThinkingLevel), [`GoalState`](../../core/goals.ts.md#GoalState), [`SessionActionSnapshot`](../../core/session-action-store.ts.md#SessionActionSnapshot)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`runRpcModeWithConnectionInternal`](rpc-mode.ts.md#runRpcModeWithConnectionInternal), [`rpc-client.ts`](rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`rpc-mode.ts`](rpc-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-mode.ts), [`RpcResponse`](rpc-types.ts.md#RpcResponse), [`getState`](rpc-client.ts.md#RpcClient.getState)  (2 test-only)

### `RpcSlashCommand`
- def: [`packages/coding-agent/src/modes/rpc/rpc-types.ts:123`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L123)
- doc: A command available for invocation via prompt
- signature: `interface RpcSlashCommand`
- members:
  - `description` — [`L127`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L127) — Human-readable description
  - `name` — [`L125`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L125) — Command name (without leading slash)
  - `source` — [`L129`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L129) — What kind of command this is
  - `sourceInfo` — [`L131`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-types.ts#L131) — Source metadata for the owning resource
- uses (calls/refs, reference-scoped): [`AgentConnectionSourceInfo`](../agent-connection/types.ts.md#AgentConnectionSourceInfo)
- used by: [`runRpcModeWithConnectionInternal`](rpc-mode.ts.md#runRpcModeWithConnectionInternal), [`rpc-client.ts`](rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`rpc-mode.ts`](rpc-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-mode.ts), [`RpcResponse`](rpc-types.ts.md#RpcResponse), [`getCommands`](rpc-client.ts.md#RpcClient.getCommands)


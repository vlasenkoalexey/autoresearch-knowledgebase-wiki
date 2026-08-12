---
title: 'Module: packages/coding-agent/src/core/agent-observe.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/agent-observe.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`agent-observe.ts`/
symbols:
  createAgentObserveMessagePreview: createAgentObserveMessagePreview().
  messageText: messageText().
  AgentObserveController: AgentObserveController#
  createAgentObserveHostHandlers: createAgentObserveHostHandlers().
  AgentObserveController.recentMessages: AgentObserveController#recentMessages().
  assistantToolCalls: assistantToolCalls().
  AgentObserveController.getAgent: AgentObserveController#getAgent().
  AgentObserveController.listAgents: AgentObserveController#listAgents().
  AgentObserveListResult: AgentObserveListResult#
  AgentObserveAgentSnapshot: AgentObserveAgentSnapshot#
  normalizeObserveLimit: normalizeObserveLimit().
  normalizeObserveMaxChars: normalizeObserveMaxChars().
  AgentObserveRecentMessagesInput.target: AgentObserveRecentMessagesInput#target.
  AgentObserveRecentMessagesResult: AgentObserveRecentMessagesResult#
  AgentObserveAgentSummary: AgentObserveAgentSummary#
  truncate: truncate().
  AGENT_OBSERVE_SKILL_NAME: AGENT_OBSERVE_SKILL_NAME.
  AgentObserveAgentSummary.activeSessionId: AgentObserveAgentSummary#activeSessionId.
  AgentObserveRecentMessagesInput.limit: AgentObserveRecentMessagesInput#limit.
  AgentObserveRecentMessagesInput.maxChars: AgentObserveRecentMessagesInput#maxChars.
  AgentObserveMessagePreview.text: AgentObserveMessagePreview#text.
  AgentObserveAgentSummary.latestMessage: AgentObserveAgentSummary#latestMessage.
  AgentObserveAgentSummary.sessionId: AgentObserveAgentSummary#sessionId.
  AgentObserveAgentSummary.runtimeKind: AgentObserveAgentSummary#runtimeKind.
  AgentObserveAgentSummary.cwd: AgentObserveAgentSummary#cwd.
  AgentObserveAgentSummary.status: AgentObserveAgentSummary#status.
  AgentObserveAgentSummary.isCurrent: AgentObserveAgentSummary#isCurrent.
  AgentObserveAgentSummary.isStreaming: AgentObserveAgentSummary#isStreaming.
  AgentObserveAgentSummary.isCompacting: AgentObserveAgentSummary#isCompacting.
  AgentObserveAgentSummary.attachedClients: AgentObserveAgentSummary#attachedClients.
  AgentObserveAgentSummary.messageCount: AgentObserveAgentSummary#messageCount.
  AgentObserveAgentSummary.queuedCount: AgentObserveAgentSummary#queuedCount.
  AgentObserveAgentSummary.isSessionActive: AgentObserveAgentSummary#isSessionActive.
  AgentObserveRecentMessagesInput: AgentObserveRecentMessagesInput#
  AgentObserveMessagePreview: AgentObserveMessagePreview#
  truncate.typeLiteral13.text: truncate().typeLiteral13:text.
  truncate.typeLiteral13.truncated: truncate().typeLiteral13:truncated.
  contentText: contentText().
  AgentObserveListResult.current: AgentObserveListResult#current.
  AgentObserveRecentMessagesResult.agent: AgentObserveRecentMessagesResult#agent.
  AgentObserveRecentMessagesResult.messages: AgentObserveRecentMessagesResult#messages.
  ORCHESTRATION_HEARTBEAT_SKILL_NAME: ORCHESTRATION_HEARTBEAT_SKILL_NAME.
  AgentObserveAgentSummary.sessionName: AgentObserveAgentSummary#sessionName.
  AgentObserveAgentSummary.parentActiveSessionId: AgentObserveAgentSummary#parentActiveSessionId.
  AgentObserveAgentSummary.parentSessionId: AgentObserveAgentSummary#parentSessionId.
  AgentObserveAgentSummary.rlmChildId: AgentObserveAgentSummary#rlmChildId.
  AgentObserveAgentSummary.rlmParentNodeId: AgentObserveAgentSummary#rlmParentNodeId.
  AgentObserveAgentSummary.firstMessage: AgentObserveAgentSummary#firstMessage.
  AgentObserveListResult.agents: AgentObserveListResult#agents.
  AgentObserveMessagePreview.truncated: AgentObserveMessagePreview#truncated.
  AgentObserveMessagePreview.toolCalls: AgentObserveMessagePreview#toolCalls.
  normalizeOptionalInteger: normalizeOptionalInteger().
  clampInteger: clampInteger().
  AgentObserveMessagePreview.index: AgentObserveMessagePreview#index.
  AgentObserveMessagePreview.role: AgentObserveMessagePreview#role.
  AgentObserveMessagePreview.timestamp: AgentObserveMessagePreview#timestamp.
  AgentObserveMessagePreview.customType: AgentObserveMessagePreview#customType.
  AGENT_OBSERVE_IMPORT_NAME: AGENT_OBSERVE_IMPORT_NAME.
  AgentObserveAgentSnapshot.agent: AgentObserveAgentSnapshot#agent.
  AgentObserveRecentMessagesResult.limit: AgentObserveRecentMessagesResult#limit.
  AgentObserveRecentMessagesResult.maxChars: AgentObserveRecentMessagesResult#maxChars.
  AgentObserveRecentMessagesResult.truncated: AgentObserveRecentMessagesResult#truncated.
  assistantToolCalls.message-Extract.typeLiteral25.role: assistantToolCalls().(message)Extract:typeLiteral25:role.
---
# Module: [`packages/coding-agent/src/core/agent-observe.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts)

## Classes
### `AgentObserveAgentSnapshot`
- def: [`packages/coding-agent/src/core/agent-observe.ts:34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L34)
- signature: `interface AgentObserveAgentSnapshot`
- members:
  - `agent` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L35)
- uses (calls/refs, reference-scoped): [`AgentObserveAgentSummary`](agent-observe.ts.md#AgentObserveAgentSummary)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`_createKernelHostHandlers`](agent-session.ts.md#AgentSession._createKernelHostHandlers), [`handleAgentObserveHostRequest`](agent-session.ts.md#AgentSession.handleAgentObserveHostRequest), [`getAgent`](agent-observe.ts.md#AgentObserveController.getAgent), [`createAgentObserveAgentSnapshot`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentObserveAgentSnapshot)

### `AgentObserveAgentSummary`
- def: [`packages/coding-agent/src/core/agent-observe.ts:7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L7)
- signature: `interface AgentObserveAgentSummary`
- members:
  - `activeSessionId` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L8)
  - `attachedClients` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L17)
  - `cwd` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L12)
  - `firstMessage` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L25)
  - `isCompacting` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L16)
  - `isCurrent` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L14)
  - `isSessionActive` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L20)
  - `isStreaming` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L15)
  - `latestMessage` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L26)
  - `messageCount` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L18)
  - `parentActiveSessionId` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L21)
  - `parentSessionId` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L22)
  - `queuedCount` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L19)
  - `rlmChildId` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L23)
  - `rlmParentNodeId` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L24)
  - `runtimeKind` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L11)
  - `sessionId` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L9)
  - `sessionName` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L10)
  - `status` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L13)
- uses (calls/refs, reference-scoped): [`AgentObserveMessagePreview`](agent-observe.ts.md#AgentObserveMessagePreview)
- used by: [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`createAgentObserveSummary`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentObserveSummary), [`createAgentObserveListResult`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentObserveListResult), [`AgentObserveAgentSnapshot`](agent-observe.ts.md#AgentObserveAgentSnapshot), [`AgentObserveListResult`](agent-observe.ts.md#AgentObserveListResult), [`agent`](agent-observe.ts.md#AgentObserveRecentMessagesResult.agent), [`current`](agent-observe.ts.md#AgentObserveListResult.current)  (2 test-only)

### `AgentObserveController`
- def: [`packages/coding-agent/src/core/agent-observe.ts:62`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L62)
- signature: `interface AgentObserveController`
- members:
  - `getAgent(method)` — [`L64`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L64)
  - `listAgents(method)` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L63)
  - `recentMessages(method)` — [`L65`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L65)
- uses (calls/refs, reference-scoped): [`AgentObserveAgentSnapshot`](agent-observe.ts.md#AgentObserveAgentSnapshot), [`AgentObserveListResult`](agent-observe.ts.md#AgentObserveListResult), [`AgentObserveRecentMessagesResult`](agent-observe.ts.md#AgentObserveRecentMessagesResult), [`AgentObserveRecentMessagesInput`](agent-observe.ts.md#AgentObserveRecentMessagesInput)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`_createKernelHostHandlers`](agent-session.ts.md#AgentSession._createKernelHostHandlers), [`agent-session-services.ts`](agent-session-services.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-services.ts), [`handleAgentObserveHostRequest`](agent-session.ts.md#AgentSession.handleAgentObserveHostRequest), [`createAgentObserveController`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentObserveController), [`createAgentObserveHostHandlers`](agent-observe.ts.md#createAgentObserveHostHandlers), [`_agentObserveController`](agent-session.ts.md#AgentSession._agentObserveController), [`agentObserveController`](agent-session-services.ts.md#AgentSessionCreationOptions.agentObserveController), [`agentObserveController`](agent-session.ts.md#AgentSessionConfig.agentObserveController)  (6 test-only)

### `AgentObserveListResult`
- def: [`packages/coding-agent/src/core/agent-observe.ts:29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L29)
- signature: `interface AgentObserveListResult`
- members:
  - `agents` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L31)
  - `current` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L30)
- uses (calls/refs, reference-scoped): [`AgentObserveAgentSummary`](agent-observe.ts.md#AgentObserveAgentSummary)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`_createKernelHostHandlers`](agent-session.ts.md#AgentSession._createKernelHostHandlers), [`createAgentObserveListResult`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentObserveListResult), [`handleAgentObserveHostRequest`](agent-session.ts.md#AgentSession.handleAgentObserveHostRequest), [`listAgents`](agent-observe.ts.md#AgentObserveController.listAgents)  (1 test-only)

### `AgentObserveMessagePreview`
- def: [`packages/coding-agent/src/core/agent-observe.ts:52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L52)
- signature: `interface AgentObserveMessagePreview`
- members:
  - `customType` — [`L59`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L59)
  - `index` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L53)
  - `role` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L54)
  - `text` — [`L56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L56)
  - `timestamp` — [`L55`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L55)
  - `toolCalls` — [`L58`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L58)
  - `truncated` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L57)
- used by: [`createAgentObserveMessagePreview`](agent-observe.ts.md#createAgentObserveMessagePreview), [`latestMessage`](agent-observe.ts.md#AgentObserveAgentSummary.latestMessage), [`messages`](agent-observe.ts.md#AgentObserveRecentMessagesResult.messages)  (1 test-only)

### `AgentObserveRecentMessagesInput`
- def: [`packages/coding-agent/src/core/agent-observe.ts:38`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L38)
- signature: `interface AgentObserveRecentMessagesInput`
- members:
  - `limit` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L40)
  - `maxChars` — [`L41`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L41)
  - `target` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L39)
- used by: [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`_createKernelHostHandlers`](agent-session.ts.md#AgentSession._createKernelHostHandlers), [`handleAgentObserveHostRequest`](agent-session.ts.md#AgentSession.handleAgentObserveHostRequest), [`createAgentObserveRecentMessages`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentObserveRecentMessages), [`createAgentObserveHostHandlers`](agent-observe.ts.md#createAgentObserveHostHandlers), [`recentMessages`](agent-observe.ts.md#AgentObserveController.recentMessages)  (1 test-only)

### `AgentObserveRecentMessagesResult`
- def: [`packages/coding-agent/src/core/agent-observe.ts:44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L44)
- signature: `interface AgentObserveRecentMessagesResult`
- members:
  - `agent` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L45)
  - `limit` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L47)
  - `maxChars` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L48)
  - `messages` — [`L46`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L46)
  - `truncated` — [`L49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L49)
- uses (calls/refs, reference-scoped): [`AgentObserveAgentSummary`](agent-observe.ts.md#AgentObserveAgentSummary), [`AgentObserveMessagePreview`](agent-observe.ts.md#AgentObserveMessagePreview)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`_createKernelHostHandlers`](agent-session.ts.md#AgentSession._createKernelHostHandlers), [`handleAgentObserveHostRequest`](agent-session.ts.md#AgentSession.handleAgentObserveHostRequest), [`createAgentObserveRecentMessages`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentObserveRecentMessages), [`recentMessages`](agent-observe.ts.md#AgentObserveController.recentMessages)

## Functions
- `assistantToolCalls(message: AssistantMessage)` — [`L198`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L198)
- `clampInteger(value: number, min: number, max: number, label: string)` — [`L129`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L129)
- `contentText(content: unknown)` — [`L168`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L168)
- `createAgentObserveHostHandlers(controller: AgentObserveController)` — [`L70`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L70)
- `createAgentObserveMessagePreview(message: AgentMessage, index: number, maxChars: number)` — [`L100`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L100)
- `messageText(message: AgentMessage)` — [`L146`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L146)
- `normalizeObserveLimit(limit: number | undefined, defaultLimit?: number)` — [`L92`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L92)
- `normalizeObserveMaxChars(maxChars: number | undefined, defaultMaxChars?: number)` — [`L96`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L96)
- `normalizeOptionalInteger(value: unknown, label: string)` — [`L119`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L119)
- `truncate(text: string, maxChars: number)` — [`L139`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L139)

## Module values
- `AGENT_OBSERVE_IMPORT_NAME` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L4)
- `AGENT_OBSERVE_SKILL_NAME` — [`L3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L3)
- `ORCHESTRATION_HEARTBEAT_SKILL_NAME` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L5)
- `role` — [`L198`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L198)
- `text` — [`L139`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L139)
- `truncated` — [`L139`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/agent-observe.ts#L139)


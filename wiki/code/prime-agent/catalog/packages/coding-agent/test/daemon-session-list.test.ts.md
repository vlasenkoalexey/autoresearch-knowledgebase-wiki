---
title: 'Module: packages/coding-agent/test/daemon-session-list.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/daemon-session-list.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`daemon-session-list.test.ts`/
symbols:
  makeState: makeState().
  makeCronJob: makeCronJob().
  makeSessionInfo: makeSessionInfo().
  StateOptions.activeSessionId: StateOptions#activeSessionId.
  StateOptions.messages: StateOptions#messages.
  StateOptions.sessionFile: StateOptions#sessionFile.
  StateOptions.summaryState: StateOptions#summaryState.
  StateOptions.isStreaming: StateOptions#isStreaming.
  StateOptions.metadata: StateOptions#metadata.
  StateOptions.sessionId: StateOptions#sessionId.
  StateOptions.hasAcceptedPromptInFlight: StateOptions#hasAcceptedPromptInFlight.
  StateOptions.streamingMessage: StateOptions#streamingMessage.
  StateOptions.childRunStatuses: StateOptions#childRunStatuses.
  StateOptions.hasRunningRlmChildren: StateOptions#hasRunningRlmChildren.
  StateOptions.model: StateOptions#model.
  StateOptions.pendingToolCalls: StateOptions#pendingToolCalls.
  StateOptions.clients: StateOptions#clients.
  StateOptions.unfinishedActionCount: StateOptions#unfinishedActionCount.
  StateOptions.contextTokens: StateOptions#contextTokens.
  StateOptions.rlmDepth: StateOptions#rlmDepth.
  StateOptions: StateOptions#
  StateOptions.hasUserContent: StateOptions#hasUserContent.
  StateOptions.model.typeLiteral301.provider: StateOptions#model.typeLiteral301:provider.
  StateOptions.model.typeLiteral301.id: StateOptions#model.typeLiteral301:id.
  StateOptions.metadata.typeLiteral302.kind: StateOptions#metadata.typeLiteral302:kind.
  StateOptions.metadata.typeLiteral302.createdAt: StateOptions#metadata.typeLiteral302:createdAt.
  StateOptions.metadata.typeLiteral302.parentActiveSessionId: StateOptions#metadata.typeLiteral302:parentActiveSessionId.
  StateOptions.metadata.typeLiteral302.parentSessionId: StateOptions#metadata.typeLiteral302:parentSessionId.
  StateOptions.metadata.typeLiteral302.parentSessionFile: StateOptions#metadata.typeLiteral302:parentSessionFile.
  StateOptions.metadata.typeLiteral302.rlmChildId: StateOptions#metadata.typeLiteral302:rlmChildId.
  StateOptions.metadata.typeLiteral302.rlmParentNodeId: StateOptions#metadata.typeLiteral302:rlmParentNodeId.
  StateOptions.metadata.typeLiteral302.prompt: StateOptions#metadata.typeLiteral302:prompt.
  StateOptions.metadata.typeLiteral302.sessionDir: StateOptions#metadata.typeLiteral302:sessionDir.
---
# Module: [`packages/coding-agent/test/daemon-session-list.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts)

## Classes
### `StateOptions`
- def: [`packages/coding-agent/test/daemon-session-list.test.ts:683`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L683)
- signature: `interface StateOptions`
- members:
  - `activeSessionId` — [`L684`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L684)
  - `childRunStatuses` — [`L694`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L694)
  - `clients` — [`L690`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L690)
  - `contextTokens` — [`L698`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L698)
  - `createdAt` — [`L703`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L703)
  - `hasAcceptedPromptInFlight` — [`L696`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L696)
  - `hasRunningRlmChildren` — [`L695`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L695)
  - `hasUserContent` — [`L692`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L692)
  - `id` — [`L685`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L685)
  - `isStreaming` — [`L688`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L688)
  - `kind` — [`L702`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L702)
  - `messages` — [`L691`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L691)
  - `metadata` — [`L701`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L701)
  - `model` — [`L685`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L685)
  - `parentActiveSessionId` — [`L704`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L704)
  - `parentSessionFile` — [`L706`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L706)
  - `parentSessionId` — [`L705`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L705)
  - `pendingToolCalls` — [`L689`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L689)
  - `prompt` — [`L709`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L709)
  - `provider` — [`L685`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L685)
  - `rlmChildId` — [`L707`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L707)
  - `rlmDepth` — [`L700`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L700)
  - `rlmParentNodeId` — [`L708`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L708)
  - `sessionDir` — [`L710`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L710)
  - `sessionFile` — [`L686`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L686)
  - `sessionId` — [`L687`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L687)
  - `streamingMessage` — [`L699`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L699)
  - `summaryState` — [`L693`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L693)
  - `unfinishedActionCount` — [`L697`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L697)
- uses (calls/refs, reference-scoped): [`ActiveSessionState`](../src/modes/daemon/active-session-state.ts.md#ActiveSessionState), [`AgentMessage`](../../agent/src/types.ts.md#AgentMessage), [`summaryState`](../src/modes/daemon/active-session-state.ts.md#ActiveSessionState.summaryState)
- used by: (2 test-only callers)

## Functions
- `makeCronJob(overrides: Pick<AgentCronJob, "id" | "activeSessionId"> & Partial<AgentCronJob>)` — [`L786`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L786)
- `makeSessionInfo(overrides: Pick<SessionInfo, "path" | "id"> & Partial<SessionInfo>)` — [`L768`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L768)
- `makeState(options: StateOptions)` — [`L714`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-session-list.test.ts#L714)


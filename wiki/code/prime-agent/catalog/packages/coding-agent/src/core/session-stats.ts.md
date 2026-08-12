---
title: 'Module: packages/coding-agent/src/core/session-stats.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/session-stats.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`session-stats.ts`/SessionStats#
symbols:
  SessionStats: ''
  SessionStats.contextUsage: contextUsage.
  SessionStats.tokens: tokens.
  SessionStats.sessionFile: sessionFile.
  SessionStats.tokens.typeLiteral0.input: tokens.typeLiteral0:input.
  SessionStats.sessionId: sessionId.
  SessionStats.userMessages: userMessages.
  SessionStats.assistantMessages: assistantMessages.
  SessionStats.tokens.typeLiteral0.output: tokens.typeLiteral0:output.
  SessionStats.tokens.typeLiteral0.total: tokens.typeLiteral0:total.
  SessionStats.cost: cost.
  SessionStats.toolCalls: toolCalls.
  SessionStats.toolResults: toolResults.
  SessionStats.totalMessages: totalMessages.
  SessionStats.tokens.typeLiteral0.cacheRead: tokens.typeLiteral0:cacheRead.
  SessionStats.tokens.typeLiteral0.cacheWrite: tokens.typeLiteral0:cacheWrite.
---
# Module: [`packages/coding-agent/src/core/session-stats.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts)

## Classes
### `SessionStats`
- def: [`packages/coding-agent/src/core/session-stats.ts:4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L4)
- doc: Session statistics for the /session command and connection snapshots.
- signature: `interface SessionStats`
- members:
  - `assistantMessages` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L8)
  - `cacheRead` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L15)
  - `cacheWrite` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L16)
  - `contextUsage` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L20)
  - `cost` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L19)
  - `input` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L13)
  - `output` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L14)
  - `sessionFile` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L5)
  - `sessionId` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L6)
  - `tokens` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L12)
  - `toolCalls` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L9)
  - `toolResults` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L10)
  - `total` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L17)
  - `totalMessages` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L11)
  - `userMessages` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-stats.ts#L7)
- uses (calls/refs, reference-scoped): [`ContextUsage`](extensions/types.ts.md#ContextUsage)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`handleCommand`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.handleCommand), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`daemon-agent-connection.ts`](../modes/agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`in-process-agent-connection.ts`](../modes/agent-connection/in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`getSessionStats`](agent-session.ts.md#AgentSession.getSessionStats), [`rpc-client.ts`](../modes/rpc/rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`rpc-types.ts`](../modes/rpc/rpc-types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-types.ts), [`RpcResponse`](../modes/rpc/rpc-types.ts.md#RpcResponse), [`handleSessionCommand`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleSessionCommand), [`refreshConnectionContextUsage`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.refreshConnectionContextUsage), [`formatResumeHint`](../modes/interactive/resume-hint.ts.md#formatResumeHint), [`contextUsage`](../modes/agent-connection/types.ts.md#AgentConnectionState.contextUsage), [`resume-hint.ts`](../modes/interactive/resume-hint.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-resume-hint.ts), [`getSessionStats`](../modes/agent-connection/types.ts.md#AgentConnection.getSessionStats), [`getSessionStats`](../modes/rpc/rpc-client.ts.md#RpcClient.getSessionStats), [`getSessionStats`](../modes/agent-connection/in-process-agent-connection.ts.md#InProcessAgentConnection.getSessionStats), [`getSessionStats`](../modes/agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.getSessionStats), [`ResumeHintStats`](../modes/interactive/resume-hint.ts.md#ResumeHintStats)  (3 test-only)


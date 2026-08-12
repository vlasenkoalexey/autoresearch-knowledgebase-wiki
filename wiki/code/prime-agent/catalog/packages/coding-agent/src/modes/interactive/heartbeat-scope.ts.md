---
title: 'Module: packages/coding-agent/src/modes/interactive/heartbeat-scope.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/heartbeat-scope.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/`heartbeat-scope.ts`/
symbols:
  scopeHeartbeatsToSession: scopeHeartbeatsToSession().
  HeartbeatSessionIdentity.activeSessionId: HeartbeatSessionIdentity#activeSessionId.
  HeartbeatSessionIdentity: HeartbeatSessionIdentity#
  HeartbeatSessionIdentity.sessionId: HeartbeatSessionIdentity#sessionId.
---
# Module: [`packages/coding-agent/src/modes/interactive/heartbeat-scope.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/heartbeat-scope.ts)

## Classes
### `HeartbeatSessionIdentity`
- def: [`packages/coding-agent/src/modes/interactive/heartbeat-scope.ts:3`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/heartbeat-scope.ts#L3)
- signature: `interface HeartbeatSessionIdentity`
- members:
  - `activeSessionId` — [`L4`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/heartbeat-scope.ts#L4)
  - `sessionId` — [`L5`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/heartbeat-scope.ts#L5)
- used by: [`scopeHeartbeatsToSession`](heartbeat-scope.ts.md#scopeHeartbeatsToSession)

## Functions
- `scopeHeartbeatsToSession(heartbeats: readonly AgentConnectionHeartbeat[], session: HeartbeatSessionIdentity | undefined, children: Iterable<Pick<AgentConnectionRlmChildAgentSnapshot, "activeSessionId">>)` — [`L8`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/heartbeat-scope.ts#L8)


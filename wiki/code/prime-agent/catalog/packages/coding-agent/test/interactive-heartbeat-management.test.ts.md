---
title: 'Module: packages/coding-agent/test/interactive-heartbeat-management.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/interactive-heartbeat-management.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`interactive-heartbeat-management.test.ts`/
symbols:
  heartbeat: heartbeat().
  HeartbeatManagementHarness.agentConnection.typeLiteral0.manageHeartbeat: HeartbeatManagementHarness#agentConnection.typeLiteral0:manageHeartbeat().
  HeartbeatManagementHarness.manageHeartbeat: HeartbeatManagementHarness#manageHeartbeat().
  HeartbeatManagementHarness.heartbeats: HeartbeatManagementHarness#heartbeats.
  HeartbeatManagementHarness.applyHeartbeatCatalog: HeartbeatManagementHarness#applyHeartbeatCatalog().
  HeartbeatManagementHarness.heartbeatCatalog: HeartbeatManagementHarness#heartbeatCatalog.
  HeartbeatScopeHarness.heartbeatCatalog: HeartbeatScopeHarness#heartbeatCatalog.
  HeartbeatScopeHarness.heartbeats: HeartbeatScopeHarness#heartbeats.
  HeartbeatScopeHarness.heartbeatManager: HeartbeatScopeHarness#heartbeatManager.
  ChildIdentityUpdateHarness.subagentSnapshots: ChildIdentityUpdateHarness#subagentSnapshots.
  HeartbeatManagementHarness.refreshHeartbeatCatalog: HeartbeatManagementHarness#refreshHeartbeatCatalog().
  HeartbeatScopeHarness.subagentSnapshots: HeartbeatScopeHarness#subagentSnapshots.
  HeartbeatScopeHarness.applyHeartbeatCatalog: HeartbeatScopeHarness#applyHeartbeatCatalog().
  ChildIdentityUpdateHarness.updateSubagentSummary: ChildIdentityUpdateHarness#updateSubagentSummary().
  HeartbeatRefreshHarness.heartbeats: HeartbeatRefreshHarness#heartbeats.
  HeartbeatManagementHarness.patchConnectionState.patch-typeLiteral2.heartbeat: HeartbeatManagementHarness#patchConnectionState().(patch)typeLiteral2:heartbeat.
  HeartbeatManagementHarness: HeartbeatManagementHarness#
  HeartbeatManagementHarness.agentConnection: HeartbeatManagementHarness#agentConnection.
  HeartbeatManagementHarness.connectionState: HeartbeatManagementHarness#connectionState.
  HeartbeatManagementHarness.connectionState.typeLiteral1.activeSessionId: HeartbeatManagementHarness#connectionState.typeLiteral1:activeSessionId.
  HeartbeatManagementHarness.patchConnectionState: HeartbeatManagementHarness#patchConnectionState().
  HeartbeatScopeHarness.updateSubagentSummaryLine: HeartbeatScopeHarness#updateSubagentSummaryLine().
  ChildIdentityUpdateHarness.refreshSubagentSummary: ChildIdentityUpdateHarness#refreshSubagentSummary().
  HeartbeatRefreshHarness.refreshHeartbeatCatalog: HeartbeatRefreshHarness#refreshHeartbeatCatalog().
  HeartbeatScopeHarness: HeartbeatScopeHarness#
  HeartbeatScopeHarness.connectionState: HeartbeatScopeHarness#connectionState.
  HeartbeatScopeHarness.connectionState.typeLiteral3.activeSessionId: HeartbeatScopeHarness#connectionState.typeLiteral3:activeSessionId.
  HeartbeatScopeHarness.connectionState.typeLiteral3.sessionId: HeartbeatScopeHarness#connectionState.typeLiteral3:sessionId.
  HeartbeatScopeHarness.ui: HeartbeatScopeHarness#ui.
  HeartbeatScopeHarness.ui.typeLiteral8.requestRender: HeartbeatScopeHarness#ui.typeLiteral8:requestRender().
  HeartbeatScopeHarness.scheduleHeartbeatManagerRefresh: HeartbeatScopeHarness#scheduleHeartbeatManagerRefresh().
  ChildIdentityUpdateHarness: ChildIdentityUpdateHarness#
  HeartbeatRefreshHarness: HeartbeatRefreshHarness#
  HeartbeatRefreshHarness.heartbeatManager: HeartbeatRefreshHarness#heartbeatManager.
  HeartbeatRefreshHarness.heartbeatManagerRefreshTimer: HeartbeatRefreshHarness#heartbeatManagerRefreshTimer.
  HeartbeatRefreshHarness.scheduleHeartbeatManagerRefresh: HeartbeatRefreshHarness#scheduleHeartbeatManagerRefresh().
---
# Module: [`packages/coding-agent/test/interactive-heartbeat-management.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts)

## Classes
### `ChildIdentityUpdateHarness`
- def: [`packages/coding-agent/test/interactive-heartbeat-management.test.ts:38`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L38)
- signature: `interface ChildIdentityUpdateHarness`
- members:
  - `refreshSubagentSummary(method)` — [`L40`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L40)
  - `updateSubagentSummary(method)` — [`L41`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L41)
  - `subagentSnapshots` — [`L39`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L39)
- uses (calls/refs, reference-scoped): [`AgentConnectionRlmChildAgentSnapshot`](../src/modes/agent-connection/types.ts.md#AgentConnectionRlmChildAgentSnapshot)
- used by: (1 test-only callers)

### `HeartbeatManagementHarness`
- def: [`packages/coding-agent/test/interactive-heartbeat-management.test.ts:9`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L9)
- signature: `interface HeartbeatManagementHarness`
- members:
  - `applyHeartbeatCatalog(method)` — [`L21`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L21)
  - `manageHeartbeat(method)` — [`L13`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L13)
  - `manageHeartbeat(method)` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L23)
  - `patchConnectionState(method)` — [`L20`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L20)
  - `refreshHeartbeatCatalog(method)` — [`L22`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L22)
  - `activeSessionId` — [`L19`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L19)
  - `agentConnection` — [`L12`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L12)
  - `connectionState` — [`L19`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L19)
  - `heartbeat` — [`L20`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L20)
  - `heartbeatCatalog` — [`L10`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L10)
  - `heartbeats` — [`L11`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L11)
- uses (calls/refs, reference-scoped): [`AgentCronJob`](../src/core/cron-jobs.ts.md#AgentCronJob), [`AgentConnectionHeartbeat`](../src/modes/agent-connection/types.ts.md#AgentConnectionHeartbeat), [`AgentHeartbeatManagementAction`](../src/core/cron-jobs.ts.md#AgentHeartbeatManagementAction)
- used by: (1 test-only callers)

### `HeartbeatRefreshHarness`
- def: [`packages/coding-agent/test/interactive-heartbeat-management.test.ts:44`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L44)
- signature: `interface HeartbeatRefreshHarness`
- members:
  - `refreshHeartbeatCatalog(method)` — [`L48`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L48)
  - `scheduleHeartbeatManagerRefresh(method)` — [`L49`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L49)
  - `heartbeatManager` — [`L46`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L46)
  - `heartbeatManagerRefreshTimer` — [`L47`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L47)
  - `heartbeats` — [`L45`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L45)
- uses (calls/refs, reference-scoped): [`AgentConnectionHeartbeat`](../src/modes/agent-connection/types.ts.md#AgentConnectionHeartbeat)
- used by: (1 test-only callers)

### `HeartbeatScopeHarness`
- def: [`packages/coding-agent/test/interactive-heartbeat-management.test.ts:26`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L26)
- signature: `interface HeartbeatScopeHarness`
- members:
  - `applyHeartbeatCatalog(method)` — [`L35`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L35)
  - `requestRender(method)` — [`L32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L32)
  - `scheduleHeartbeatManagerRefresh(method)` — [`L33`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L33)
  - `updateSubagentSummaryLine(method)` — [`L34`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L34)
  - `activeSessionId` — [`L29`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L29)
  - `connectionState` — [`L29`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L29)
  - `heartbeatCatalog` — [`L27`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L27)
  - `heartbeatManager` — [`L31`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L31)
  - `heartbeats` — [`L28`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L28)
  - `sessionId` — [`L29`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L29)
  - `subagentSnapshots` — [`L30`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L30)
  - `ui` — [`L32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L32)
- uses (calls/refs, reference-scoped): [`AgentConnectionHeartbeat`](../src/modes/agent-connection/types.ts.md#AgentConnectionHeartbeat), [`AgentConnectionRlmChildAgentSnapshot`](../src/modes/agent-connection/types.ts.md#AgentConnectionRlmChildAgentSnapshot)
- used by: (1 test-only callers)

## Functions
- `heartbeat(overrides?: Partial<AgentCronJob>)` — [`L52`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-heartbeat-management.test.ts#L52)


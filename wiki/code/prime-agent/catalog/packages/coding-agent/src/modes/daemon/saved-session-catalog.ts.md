---
title: 'Module: packages/coding-agent/src/modes/daemon/saved-session-catalog.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/saved-session-catalog.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`saved-session-catalog.ts`/
symbols:
  listDaemonSavedSessions: listDaemonSavedSessions().
  deleteDaemonSavedSession: deleteDaemonSavedSession().
  renameDaemonSavedSession: renameDaemonSavedSession().
  DaemonSavedSessionCatalogContext: DaemonSavedSessionCatalogContext#
---
# Module: [`packages/coding-agent/src/modes/daemon/saved-session-catalog.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/saved-session-catalog.ts)

## Classes
### `DaemonSavedSessionCatalogContext`
- def: [`packages/coding-agent/src/modes/daemon/saved-session-catalog.ts:19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/saved-session-catalog.ts#L19)
- signature: `type DaemonSavedSessionCatalogContext`
- used by: [`agents-view-mode.ts`](../agents-view/agents-view-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agents-view-agents-view-mode.ts), [`listDaemonSavedSessions`](saved-session-catalog.ts.md#listDaemonSavedSessions), [`deleteDaemonSavedSession`](saved-session-catalog.ts.md#deleteDaemonSavedSession), [`renameDaemonSavedSession`](saved-session-catalog.ts.md#renameDaemonSavedSession), [`getSavedSessionCatalogContext`](../agents-view/agents-view-mode.ts.md#AgentsViewMode.getSavedSessionCatalogContext)

## Functions
- `deleteDaemonSavedSession(client: DaemonClient, context: DaemonSavedSessionCatalogContext, sessionPath: string)` — [`L63`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/saved-session-catalog.ts#L63)
- `listDaemonSavedSessions(client: DaemonClient, context: DaemonSavedSessionCatalogContext, scope: AgentConnectionSavedSessionScope, callbacks?: AgentConnectionSessionListCallbacks | undefined)` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/saved-session-catalog.ts#L21)
- `renameDaemonSavedSession(client: DaemonClient, context: DaemonSavedSessionCatalogContext, sessionPath: string, name: string)` — [`L47`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/saved-session-catalog.ts#L47)


---
title: 'Module: packages/coding-agent/src/core/session-file-actions.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/session-file-actions.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`session-file-actions.ts`/
symbols:
  deleteSessionFile: deleteSessionFile().
  DeleteSessionFileResult: DeleteSessionFileResult#
  removeSessionFile: removeSessionFile().
  DeleteSessionFileOptions: DeleteSessionFileOptions#
  DeleteSessionFileOptions.afterFileRemoved: DeleteSessionFileOptions#afterFileRemoved.
  deleteSessionArtifacts: deleteSessionArtifacts().
---
# Module: [`packages/coding-agent/src/core/session-file-actions.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-file-actions.ts)

## Classes
### `DeleteSessionFileOptions`
- def: [`packages/coding-agent/src/core/session-file-actions.ts:8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-file-actions.ts#L8)
- signature: `interface DeleteSessionFileOptions`
- members:
  - `afterFileRemoved` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-file-actions.ts#L9)
- used by: [`deleteSessionFile`](session-file-actions.ts.md#deleteSessionFile)

### `DeleteSessionFileResult`
- def: [`packages/coding-agent/src/core/session-file-actions.ts:6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-file-actions.ts#L6)
- signature: `type DeleteSessionFileResult`
- used by: [`daemon-agent-connection.ts`](../modes/agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](../modes/agent-connection/in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`daemon-protocol.ts`](../modes/daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`saved-session-catalog.ts`](../modes/daemon/saved-session-catalog.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-saved-session-catalog.ts), [`daemon-catalog-process.ts`](../modes/daemon/daemon-catalog-process.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-catalog-process.ts), [`deleteSessionFile`](session-file-actions.ts.md#deleteSessionFile), [`deleteDaemonSavedSession`](../modes/daemon/saved-session-catalog.ts.md#deleteDaemonSavedSession), [`deleteSavedSession`](../modes/agent-connection/types.ts.md#AgentConnection.deleteSavedSession), [`delete`](../modes/daemon/daemon-catalog-process.ts.md#DaemonCatalogClient.delete), [`deleteSavedSession`](../modes/agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.deleteSavedSession), [`deleteSavedSession`](../modes/agent-connection/in-process-agent-connection.ts.md#InProcessAgentConnection.deleteSavedSession), [`DaemonDeleteSavedSessionResult`](../modes/daemon/daemon-protocol.ts.md#DaemonDeleteSavedSessionResult), [`removeSessionFile`](session-file-actions.ts.md#removeSessionFile)

## Functions
- `deleteSessionArtifacts(sessionPath: string)` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-file-actions.ts#L18) — Permanently remove a session's artifact directory (durable schedule state,
- `deleteSessionFile(sessionPath: string, options?: DeleteSessionFileOptions)` — [`L64`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-file-actions.ts#L64) — Delete a session file, trying the `trash` CLI first, then falling back to unlink.
- `removeSessionFile(sessionPath: string)` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-file-actions.ts#L26) — Remove the session `.jsonl`, trying the `trash` CLI first, then falling back to unlink.


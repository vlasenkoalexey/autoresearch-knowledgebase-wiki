---
title: 'Module: packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`daemon-catalog-process.ts`/
symbols:
  handleCatalogRequest: handleCatalogRequest().
  listSavedSessionSiblings: listSavedSessionSiblings().
  DaemonCatalogClient.spawnCatalog: DaemonCatalogClient#spawnCatalog().
  DaemonCatalogClient.request: DaemonCatalogClient#request().
  serializeSessionInfo: serializeSessionInfo().
  deserializeSessionInfo: deserializeSessionInfo().
  sendCatalogMessage: sendCatalogMessage().
  DaemonCatalogClient.list: DaemonCatalogClient#list().
  DaemonCatalogClient.handleMessage: DaemonCatalogClient#handleMessage().
  DaemonCatalogClient.siblings: DaemonCatalogClient#siblings().
  resolveCatalogSessionMatch: resolveCatalogSessionMatch().
  runDaemonCatalogProcess: runDaemonCatalogProcess().
  DaemonCatalogClient.pending: DaemonCatalogClient#pending.
  DaemonCatalogClient.start: DaemonCatalogClient#start().
  DaemonCatalogClient.handleClose: DaemonCatalogClient#handleClose().
  SessionInfoWire: SessionInfoWire#
  DaemonCatalogClient.child: DaemonCatalogClient#child.
  DaemonCatalogClient.stop: DaemonCatalogClient#stop().
  isDaemonCatalogProcess: isDaemonCatalogProcess().
  DaemonCatalogClient: DaemonCatalogClient#
  DaemonCatalogClient.delete: DaemonCatalogClient#delete().
  CatalogListCallbacks: CatalogListCallbacks#
  DaemonCatalogClient.starting: DaemonCatalogClient#starting.
  CatalogOutbound: CatalogOutbound#
  isCatalogOutbound: isCatalogOutbound().
  DaemonCatalogClient.resolve: DaemonCatalogClient#resolve().
  DAEMON_CATALOG_ROLE_ENV: DAEMON_CATALOG_ROLE_ENV.
  isCatalogRequest: isCatalogRequest().
  DaemonCatalogClient.rename: DaemonCatalogClient#rename().
  DaemonCatalogClient.archive: DaemonCatalogClient#archive().
  DaemonCatalogClient.markInterrupted: DaemonCatalogClient#markInterrupted().
  CatalogRequest: CatalogRequest#
  SessionInfoWire.created: SessionInfoWire#created.
  SessionInfoWire.modified: SessionInfoWire#modified.
  SavedRlmSubagentRegistryEntry: SavedRlmSubagentRegistryEntry#
  SavedRlmSubagentRegistryEntry.childId: SavedRlmSubagentRegistryEntry#childId.
  SavedRlmSubagentRegistryEntry.sessionFile: SavedRlmSubagentRegistryEntry#sessionFile.
  CatalogListCallbacks.onProgress: CatalogListCallbacks#onProgress.
  CatalogListCallbacks.onSession: CatalogListCallbacks#onSession.
  SavedRlmSubagentRegistryEntry.type: SavedRlmSubagentRegistryEntry#type.
  SavedRlmSubagentRegistryEntry.status: SavedRlmSubagentRegistryEntry#status.
  DaemonCatalogClient.-constructor: DaemonCatalogClient#`<constructor>`().
---
# Module: [`packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts)

## Classes
### `CatalogListCallbacks`
- def: [`packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts:41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L41)
- signature: `interface CatalogListCallbacks`
- members:
  - `onProgress` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L42)
  - `onSession` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L43)
- uses (calls/refs, reference-scoped): [`SessionInfo`](../../core/session-manager.ts.md#SessionInfo)
- used by: [`request`](daemon-catalog-process.ts.md#DaemonCatalogClient.request), [`list`](daemon-catalog-process.ts.md#DaemonCatalogClient.list), [`handleMessage`](daemon-catalog-process.ts.md#DaemonCatalogClient.handleMessage), [`pending`](daemon-catalog-process.ts.md#DaemonCatalogClient.pending)

### `CatalogOutbound`
- def: [`packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts:34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L34)
- signature: `type CatalogOutbound`
- uses (calls/refs, reference-scoped): [`SessionInfoWire`](daemon-catalog-process.ts.md#SessionInfoWire)
- used by: [`sendCatalogMessage`](daemon-catalog-process.ts.md#sendCatalogMessage), [`isCatalogOutbound`](daemon-catalog-process.ts.md#isCatalogOutbound)

### `CatalogRequest`
- def: [`packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts:17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L17)
- signature: `type CatalogRequest`
- used by: [`handleCatalogRequest`](daemon-catalog-process.ts.md#handleCatalogRequest), [`request`](daemon-catalog-process.ts.md#DaemonCatalogClient.request), [`isCatalogRequest`](daemon-catalog-process.ts.md#isCatalogRequest)

### `DaemonCatalogClient`
- def: [`packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts:295`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L295)
- signature: `class DaemonCatalogClient`
- members:
  - `<constructor>(onDiagnostic: (message: string) => void)` — [`L308`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L308)
  - `archive(method)` — [`L361`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L361)
  - `delete(method)` — [`L357`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L357)
  - `handleClose(method)` — [`L499`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L499)
  - `handleMessage(method)` — [`L474`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L474)
  - `list(method)` — [`L323`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L323)
  - `markInterrupted(method)` — [`L372`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L372)
  - `rename(method)` — [`L341`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L341)
  - `request(method)` — [`L437`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L437)
  - `resolve(method)` — [`L345`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L345)
  - `siblings(method)` — [`L331`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L331)
  - `spawnCatalog(method)` — [`L393`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L393)
  - `start(method)` — [`L310`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L310)
  - `stop(method)` — [`L383`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L383)
  - `child` — [`L296`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L296)
  - `pending` — [`L298`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L298)
  - `starting` — [`L297`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L297)
- uses (calls/refs, reference-scoped): [`SessionInfo`](../../core/session-manager.ts.md#SessionInfo), [`createCliSubprocessLaunchSpec`](../../cli/subprocess-launch.ts.md#createCliSubprocessLaunchSpec), [`deserializeSessionInfo`](daemon-catalog-process.ts.md#deserializeSessionInfo), [`DeleteSessionFileResult`](../../core/session-file-actions.ts.md#DeleteSessionFileResult), [`createCliSubprocessEnv`](../../cli/subprocess-launch.ts.md#createCliSubprocessEnv), [`args`](../../cli/subprocess-launch.ts.md#CliSubprocessLaunchSpec.args), [`command`](../../cli/subprocess-launch.ts.md#CliSubprocessLaunchSpec.command), [`SessionInfoWire`](daemon-catalog-process.ts.md#SessionInfoWire), [`CatalogListCallbacks`](daemon-catalog-process.ts.md#CatalogListCallbacks), [`isCatalogOutbound`](daemon-catalog-process.ts.md#isCatalogOutbound), [`DAEMON_CATALOG_ROLE_ENV`](daemon-catalog-process.ts.md#DAEMON_CATALOG_ROLE_ENV), [`CatalogRequest`](daemon-catalog-process.ts.md#CatalogRequest), [`onProgress`](daemon-catalog-process.ts.md#CatalogListCallbacks.onProgress), [`onSession`](daemon-catalog-process.ts.md#CatalogListCallbacks.onSession)
- used by: [`daemon-supervisor.ts`](daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`handleCommand`](daemon-supervisor.ts.md#DaemonSupervisor.handleCommand), [`start`](daemon-supervisor.ts.md#DaemonSupervisor.start), [`shutdown`](daemon-supervisor.ts.md#DaemonSupervisor.shutdown), [`cleanupSupervisorResourcesOnce`](daemon-supervisor.ts.md#DaemonSupervisor.cleanupSupervisorResourcesOnce), [`<constructor>`](daemon-supervisor.ts.md#DaemonSupervisor.-constructor), [`createOrReuseWorker`](daemon-supervisor.ts.md#DaemonSupervisor.createOrReuseWorker), [`recoverUncertainWorkerOperations`](daemon-supervisor.ts.md#DaemonSupervisor.recoverUncertainWorkerOperations), [`type`](daemon-supervisor.ts.md#DaemonSupervisor.handleList.command-Extract.typeLiteral1418.type), [`type`](daemon-supervisor.ts.md#DaemonSupervisor.handleSavedSessionList.command-Extract.typeLiteral1475.type), [`assertSupervisorSavedSessionNameAvailable`](daemon-supervisor.ts.md#DaemonSupervisor.assertSupervisorSavedSessionNameAvailable), [`familyCatalogEntries`](daemon-supervisor.ts.md#DaemonSupervisor.familyCatalogEntries), [`finalizeArchivedWorkerStop`](daemon-supervisor.ts.md#DaemonSupervisor.finalizeArchivedWorkerStop), [`parentSessionPath`](daemon-supervisor.ts.md#DaemonSupervisor.savedSessionNameReservationInput.Promise.typeLiteral1261.parentSessionPath), [`catalog`](daemon-supervisor.ts.md#DaemonSupervisor.catalog)  (2 test-only)

### `SavedRlmSubagentRegistryEntry`
- def: [`packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts:62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L62)
- signature: `interface SavedRlmSubagentRegistryEntry`
- members:
  - `childId` — [`L64`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L64)
  - `sessionFile` — [`L65`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L65)
  - `status` — [`L66`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L66)
  - `type` — [`L63`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L63)
- used by: [`listSavedSessionSiblings`](daemon-catalog-process.ts.md#listSavedSessionSiblings)

### `SessionInfoWire`
- def: [`packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts:12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L12)
- signature: `interface SessionInfoWire`
- members:
  - `created` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L13)
  - `modified` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L14)
- uses (calls/refs, reference-scoped): [`SessionInfo`](../../core/session-manager.ts.md#SessionInfo)
- used by: [`deserializeSessionInfo`](daemon-catalog-process.ts.md#deserializeSessionInfo), [`serializeSessionInfo`](daemon-catalog-process.ts.md#serializeSessionInfo), [`list`](daemon-catalog-process.ts.md#DaemonCatalogClient.list), [`siblings`](daemon-catalog-process.ts.md#DaemonCatalogClient.siblings), [`CatalogOutbound`](daemon-catalog-process.ts.md#CatalogOutbound)

## Functions
- `deserializeSessionInfo(session: SessionInfoWire)` — [`L54`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L54)
- `handleCatalogRequest(request: CatalogRequest)` — [`L176`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L176)
- `isCatalogOutbound(value: unknown)` — [`L123`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L123)
- `isCatalogRequest(value: unknown)` — [`L135`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L135)
- `isDaemonCatalogProcess(environment?: ProcessEnv)` — [`L160`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L160)
- `listSavedSessionSiblings(sessionPath: string)` — [`L69`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L69)
- `resolveCatalogSessionMatch(sessions: readonly SessionInfo[], selector: string)` — [`L109`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L109)
- `runDaemonCatalogProcess()` — [`L164`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L164)
- `sendCatalogMessage(message: CatalogOutbound)` — [`L154`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L154)
- `serializeSessionInfo(session: SessionInfo)` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L46)

## Module values
- `DAEMON_CATALOG_ROLE_ENV` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-catalog-process.ts#L10)


---
title: 'Module: packages/coding-agent/test/saved-session-catalog.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/saved-session-catalog.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`saved-session-catalog.test.ts`/
symbols:
  FakeDaemonClient.request: FakeDaemonClient#request().
  asDaemonClient: asDaemonClient().
  FakeDaemonClient.commands: FakeDaemonClient#commands.
  FakeDaemonClient: FakeDaemonClient#
---
# Module: [`packages/coding-agent/test/saved-session-catalog.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/saved-session-catalog.test.ts)

## Classes
### `FakeDaemonClient`
- def: [`packages/coding-agent/test/saved-session-catalog.test.ts:10`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/saved-session-catalog.test.ts#L10)
- signature: `class FakeDaemonClient`
- members:
  - `request(method)` — [`L13`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/saved-session-catalog.test.ts#L13)
  - `commands` — [`L11`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/saved-session-catalog.test.ts#L11)
- uses (calls/refs, reference-scoped): [`DaemonCommand`](../src/modes/daemon/daemon-protocol.ts.md#DaemonCommand), [`DaemonResponse`](../src/modes/daemon/daemon-protocol.ts.md#DaemonResponse), [`DaemonClientRequestOptions`](../src/modes/daemon/daemon-client.ts.md#DaemonClientRequestOptions), [`agentStatus`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.agentStatus), [`onProgress`](../src/modes/daemon/daemon-client.ts.md#DaemonClientRequestOptions.onProgress), [`id`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.id), [`allMessagesText`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.allMessagesText), [`created`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.created), [`cwd`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.cwd), [`firstMessage`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.firstMessage), [`messageCount`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.messageCount), [`modified`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.modified), [`path`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.path), [`parentSessionPath`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.parentSessionPath), [`rlmDepth`](../src/modes/daemon/daemon-protocol.ts.md#DaemonSavedSessionInfo.rlmDepth)
- used by: (2 test-only callers)

## Functions
- `asDaemonClient(client: FakeDaemonClient)` — [`L86`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/saved-session-catalog.test.ts#L86)


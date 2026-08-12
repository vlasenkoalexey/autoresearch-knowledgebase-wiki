---
title: 'Module: packages/coding-agent/src/modes/rpc/rpc-mode.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/rpc/rpc-mode.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/rpc/`rpc-mode.ts`/
symbols:
  runRpcModeWithConnectionInternal: runRpcModeWithConnectionInternal().
  runRpcMode: runRpcMode().
  runRpcModeWithConnection: runRpcModeWithConnection().
  RpcModeConnectionOptions: RpcModeConnectionOptions#
  RpcModeConnectionOptions.bindHeadlessExtensions: RpcModeConnectionOptions#bindHeadlessExtensions.
---
# Module: [`packages/coding-agent/src/modes/rpc/rpc-mode.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-mode.ts)

## Classes
### `RpcModeConnectionOptions`
- def: [`packages/coding-agent/src/modes/rpc/rpc-mode.ts:34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-mode.ts#L34)
- signature: `interface RpcModeConnectionOptions`
- members:
  - `bindHeadlessExtensions` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-mode.ts#L35)
- uses (calls/refs, reference-scoped): [`createRpcExtensionUiBridge`](rpc-extension-ui-context.ts.md#createRpcExtensionUiBridge), [`uiContext`](rpc-extension-ui-context.ts.md#RpcExtensionUiBridge.uiContext)
- used by: [`runRpcModeWithConnectionInternal`](rpc-mode.ts.md#runRpcModeWithConnectionInternal)

## Functions
- `runRpcMode(runtimeHost: AgentSessionRuntime)` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-mode.ts#L41)
- `runRpcModeWithConnection(connection: AgentConnection)` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-mode.ts#L48)
- `runRpcModeWithConnectionInternal(connection: AgentConnection, options?: RpcModeConnectionOptions)` — [`L52`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-mode.ts#L52)


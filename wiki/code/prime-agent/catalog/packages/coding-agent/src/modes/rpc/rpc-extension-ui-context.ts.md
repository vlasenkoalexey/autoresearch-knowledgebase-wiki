---
title: 'Module: packages/coding-agent/src/modes/rpc/rpc-extension-ui-context.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/rpc/rpc-extension-ui-context.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/rpc/`rpc-extension-ui-context.ts`/
symbols:
  createRpcExtensionUiBridge: createRpcExtensionUiBridge().
  RpcExtensionUiBridge.uiContext: RpcExtensionUiBridge#uiContext.
  RpcExtensionUiBridge.handleResponse: RpcExtensionUiBridge#handleResponse().
  RpcExtensionUiBridge.close: RpcExtensionUiBridge#close().
  RpcExtensionUiBridge: RpcExtensionUiBridge#
---
# Module: [`packages/coding-agent/src/modes/rpc/rpc-extension-ui-context.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-extension-ui-context.ts)

## Classes
### `RpcExtensionUiBridge`
- def: [`packages/coding-agent/src/modes/rpc/rpc-extension-ui-context.ts:11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-extension-ui-context.ts#L11)
- signature: `interface RpcExtensionUiBridge`
- members:
  - `close(method)` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-extension-ui-context.ts#L14)
  - `handleResponse(method)` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-extension-ui-context.ts#L13)
  - `uiContext` — [`L12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-extension-ui-context.ts#L12)
- uses (calls/refs, reference-scoped): [`ExtensionUIContext`](../../core/extensions/types.ts.md#ExtensionUIContext), [`RpcExtensionUIResponse`](rpc-types.ts.md#RpcExtensionUIResponse)
- used by: [`runRpcModeWithConnectionInternal`](rpc-mode.ts.md#runRpcModeWithConnectionInternal), [`createRpcExtensionUiBridge`](rpc-extension-ui-context.ts.md#createRpcExtensionUiBridge), [`RpcModeConnectionOptions`](rpc-mode.ts.md#RpcModeConnectionOptions)  (1 test-only)

## Functions
- `createRpcExtensionUiBridge(output: (request: RpcExtensionUIRequest) => void)` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/rpc-extension-ui-context.ts#L17)


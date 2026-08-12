---
title: 'Module: packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`daemon-extension-binding.ts`/
symbols:
  createExtensionUIContext: createExtensionUIContext().
  bindActiveSessionState: bindActiveSessionState().
  createCommandContextActions: createCommandContextActions().
  ActiveSessionBindingCallbacks.broadcast: ActiveSessionBindingCallbacks#broadcast.
  hasExtensionUiClientForMethod: hasExtensionUiClientForMethod().
  ActiveSessionBindingCallbacks.createConnectionState: ActiveSessionBindingCallbacks#createConnectionState.
  ActiveSessionBindingCallbacks.subagentRuntimeHost: ActiveSessionBindingCallbacks#subagentRuntimeHost.
  ActiveSessionBindingCallbacks.sessionReplaced: ActiveSessionBindingCallbacks#sessionReplaced.
  BroadcastSessionEvent: BroadcastSessionEvent#
  ActiveSessionBindingCallbacks.shutdown: ActiveSessionBindingCallbacks#shutdown.
  slimSessionEventForWire: slimSessionEventForWire().
  ActiveSessionBindingCallbacks: ActiveSessionBindingCallbacks#
---
# Module: [`packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts)

## Classes
### `ActiveSessionBindingCallbacks`
- def: [`packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts:21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts#L21)
- signature: `interface ActiveSessionBindingCallbacks`
- members:
  - `broadcast` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts#L22)
  - `createConnectionState` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts#L23)
  - `sessionReplaced` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts#L24)
  - `shutdown` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts#L25)
  - `subagentRuntimeHost` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts#L26)
- uses (calls/refs, reference-scoped): [`ActiveSessionState`](active-session-state.ts.md#ActiveSessionState), [`DaemonOutbound`](daemon-protocol.ts.md#DaemonOutbound), [`AgentConnectionState`](../agent-connection/types.ts.md#AgentConnectionState), [`SubagentRuntimeHost`](../../core/rlm-runtime.ts.md#SubagentRuntimeHost)  (1 test-only)
- used by: [`createExtensionUIContext`](daemon-extension-binding.ts.md#createExtensionUIContext), [`addRuntime`](daemon-mode.ts.md#AgentDaemon.addRuntime), [`bindActiveSessionState`](daemon-extension-binding.ts.md#bindActiveSessionState)  (1 test-only)

### `BroadcastSessionEvent`
- def: [`packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts:29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts#L29)
- signature: `type BroadcastSessionEvent`
- uses (calls/refs, reference-scoped): [`DaemonOutbound`](daemon-protocol.ts.md#DaemonOutbound)
- used by: [`slimSessionEventForWire`](daemon-extension-binding.ts.md#slimSessionEventForWire)

## Functions
- `bindActiveSessionState(state: ActiveSessionState, callbacks: ActiveSessionBindingCallbacks)` — [`L49`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts#L49)
- `createCommandContextActions(state: ActiveSessionState)` — [`L99`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts#L99)
- `createExtensionUIContext(state: ActiveSessionState, broadcast: (state: ActiveSessionState, message: DaemonOutbound) => void)` — [`L125`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts#L125)
- `hasExtensionUiClientForMethod(state: ActiveSessionState, method: string)` — [`L249`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts#L249)
- `slimSessionEventForWire(event: AgentConnectionSessionEvent)` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-extension-binding.ts#L38) — message_update events carry the full partial assistant message twice: once


---
title: 'Module: packages/coding-agent/test/legacy-rlm-host-types.d.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/legacy-rlm-host-types.d.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`legacy-rlm-host-types.d.ts`/`"../src/core/rlm-runtime.js"`/SubagentRuntimeHost#
symbols:
  SubagentRuntimeHost: ''
  SubagentRuntimeHost.releaseRlmSubagentRuntime: releaseRlmSubagentRuntime.
---
# Module: [`packages/coding-agent/test/legacy-rlm-host-types.d.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/legacy-rlm-host-types.d.ts)

## Classes
### `SubagentRuntimeHost`
- def: [`packages/coding-agent/test/legacy-rlm-host-types.d.ts:4`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/legacy-rlm-host-types.d.ts#L4)
- signature: `interface SubagentRuntimeHost`
- members:
  - `releaseRlmSubagentRuntime` — [`L6`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/legacy-rlm-host-types.d.ts#L6) — Release a host-owned child after its detached initial task settles.
- uses (calls/refs, reference-scoped): [`AgentSessionRuntime`](../src/core/agent-session-runtime.ts.md#AgentSessionRuntime), [`CreateRlmSubagentRuntimeOptions`](../src/core/rlm-runtime.ts.md#CreateRlmSubagentRuntimeOptions), [`RlmSubagentRuntime`](../src/core/rlm-runtime.ts.md#RlmSubagentRuntime)
- used by: [`index.ts`](../src/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](../src/core/agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`daemon-mode.ts`](../src/modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`_startRlmChildRun`](../src/core/agent-session.ts.md#AgentSession._startRlmChildRun), [`index.ts`](../src/core/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`agent-session-runtime.ts`](../src/core/agent-session-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-runtime.ts), [`createSubagentRuntimeHost`](../src/modes/daemon/daemon-mode.ts.md#AgentDaemon.createSubagentRuntimeHost), [`agent-session-services.ts`](../src/core/agent-session-services.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-services.ts), [`AgentSessionRuntime`](../src/core/agent-session-runtime.ts.md#AgentSessionRuntime), [`modelFallbackMessage`](../src/core/sdk.ts.md#CreateAgentSessionResult.modelFallbackMessage), [`daemon-extension-binding.ts`](../src/modes/daemon/daemon-extension-binding.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-extension-binding.ts), [`_subagentRuntimeHost`](../src/core/agent-session.ts.md#AgentSession._subagentRuntimeHost), [`setSubagentRuntimeHost`](../src/core/agent-session-runtime.ts.md#AgentSessionRuntime.setSubagentRuntimeHost), [`subagentRuntimeHost`](../src/core/agent-session-services.ts.md#AgentSessionCreationOptions.subagentRuntimeHost), [`subagentRuntimeHost`](../src/core/agent-session.ts.md#AgentSessionConfig.subagentRuntimeHost), [`setSubagentRuntimeHost`](../src/core/agent-session.ts.md#AgentSession.setSubagentRuntimeHost), [`subagentRuntimeHost`](../src/core/agent-session-runtime.ts.md#AgentSessionRuntime.subagentRuntimeHost), [`subagentRuntimeHost`](../src/modes/daemon/daemon-extension-binding.ts.md#ActiveSessionBindingCallbacks.subagentRuntimeHost)  (5 test-only)


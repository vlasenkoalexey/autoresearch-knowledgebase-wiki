---
title: 'Module: packages/coding-agent/src/core/bash-executor.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/bash-executor.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`bash-executor.ts`/
symbols:
  executeBashWithOperations: executeBashWithOperations().
  BashResult: BashResult#
  BashResult.output: BashResult#output.
  BashResult.cancelled: BashResult#cancelled.
  BashResult.exitCode: BashResult#exitCode.
  BashResult.truncated: BashResult#truncated.
  BashResult.fullOutputPath: BashResult#fullOutputPath.
  BashExecutorOptions.signal: BashExecutorOptions#signal.
  BashExecutorOptions: BashExecutorOptions#
  BashExecutorOptions.onChunk: BashExecutorOptions#onChunk.
---
# Module: [`packages/coding-agent/src/core/bash-executor.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/bash-executor.ts)

## Classes
### `BashExecutorOptions`
- def: [`packages/coding-agent/src/core/bash-executor.ts:22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/bash-executor.ts#L22)
- signature: `interface BashExecutorOptions`
- members:
  - `onChunk` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/bash-executor.ts#L24) — Callback for streaming output chunks (already sanitized)
  - `signal` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/bash-executor.ts#L26) — AbortSignal for cancellation
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`executeBashWithOperations`](bash-executor.ts.md#executeBashWithOperations)

### `BashResult`
- def: [`packages/coding-agent/src/core/bash-executor.ts:29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/bash-executor.ts#L29)
- signature: `interface BashResult`
- members:
  - `cancelled` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/bash-executor.ts#L35) — Whether the command was cancelled via signal
  - `exitCode` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/bash-executor.ts#L33) — Process exit code (undefined if killed/cancelled)
  - `fullOutputPath` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/bash-executor.ts#L39) — Path to temp file containing full output (if output exceeded truncation threshold)
  - `output` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/bash-executor.ts#L31) — Combined stdout + stderr output (sanitized, possibly truncated)
  - `truncated` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/bash-executor.ts#L37) — Whether the output was truncated
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`daemon-agent-connection.ts`](../modes/agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`in-process-agent-connection.ts`](../modes/agent-connection/in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`daemon-protocol.ts`](../modes/daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`rpc-client.ts`](../modes/rpc/rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`rpc-types.ts`](../modes/rpc/rpc-types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-types.ts), [`recordBashResult`](agent-session.ts.md#AgentSession.recordBashResult), [`runUserBashLocked`](agent-session.ts.md#AgentSession.runUserBashLocked), [`RpcResponse`](../modes/rpc/rpc-types.ts.md#RpcResponse), [`executeBash`](agent-session.ts.md#AgentSession.executeBash), [`executeBashWithOperations`](bash-executor.ts.md#executeBashWithOperations), [`bash`](../modes/rpc/rpc-client.ts.md#RpcClient.bash), [`executeBashAndWait`](../modes/agent-connection/types.ts.md#AgentConnection.executeBashAndWait), [`executeBashAndWait`](../modes/agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.executeBashAndWait), [`executeBashAndWait`](../modes/agent-connection/in-process-agent-connection.ts.md#InProcessAgentConnection.executeBashAndWait), [`result`](extensions/types.ts.md#UserBashEventResult.result), [`DaemonBashResult`](../modes/daemon/daemon-protocol.ts.md#DaemonBashResult)  (6 test-only)

## Functions
- `executeBashWithOperations(command: string, cwd: string, operations: BashOperations, options?: BashExecutorOptions | undefined)` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/bash-executor.ts#L50) — Execute a bash command using custom BashOperations.


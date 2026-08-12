---
title: 'Module: packages/coding-agent/src/core/exec.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/exec.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`exec.ts`/
symbols:
  execCommand: execCommand().
  ExecOptions: ExecOptions#
  ExecResult.code: ExecResult#code.
  ExecResult: ExecResult#
  ExecResult.stdout: ExecResult#stdout.
  ExecOptions.signal: ExecOptions#signal.
  ExecOptions.timeout: ExecOptions#timeout.
  ExecOptions.env: ExecOptions#env.
  ExecResult.stderr: ExecResult#stderr.
  ExecOptions.cwd: ExecOptions#cwd.
  ExecResult.killed: ExecResult#killed.
  mergeExecEnv: mergeExecEnv().
---
# Module: [`packages/coding-agent/src/core/exec.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/exec.ts)

## Classes
### `ExecOptions`
- def: [`packages/coding-agent/src/core/exec.ts:11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/exec.ts#L11)
- doc: Options for executing shell commands.
- signature: `interface ExecOptions`
- members:
  - `cwd` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/exec.ts#L17) — Working directory
  - `env` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/exec.ts#L22) — Extra env vars merged over the parent process env for this command.
  - `signal` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/exec.ts#L13) — AbortSignal to cancel the command
  - `timeout` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/exec.ts#L15) — Timeout in milliseconds
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](extensions/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`createExtensionAPI`](extensions/loader.ts.md#createExtensionAPI), [`loader.ts`](extensions/loader.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-loader.ts), [`execCommand`](exec.ts.md#execCommand), [`exec`](extensions/types.ts.md#ExtensionAPI.exec)

### `ExecResult`
- def: [`packages/coding-agent/src/core/exec.ts:28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/exec.ts#L28)
- doc: Result of executing a shell command.
- signature: `interface ExecResult`
- members:
  - `code` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/exec.ts#L31)
  - `killed` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/exec.ts#L32)
  - `stderr` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/exec.ts#L30)
  - `stdout` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/exec.ts#L29)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](extensions/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`execCommand`](exec.ts.md#execCommand), [`exec`](extensions/types.ts.md#ExtensionAPI.exec)  (8 test-only)

## Functions
- `execCommand(command: string, args: string[], cwd: string, options?: ExecOptions | undefined)` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/exec.ts#L54) — Execute a shell command and return stdout/stderr/code.
- `mergeExecEnv(env?: Record<string, string | undefined> | undefined)` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/exec.ts#L35)


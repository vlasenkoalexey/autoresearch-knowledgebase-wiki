---
title: 'Module: packages/coding-agent/src/utils/shell.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/utils/shell.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/utils/`shell.ts`/
symbols:
  killTrackedDetachedChildren: killTrackedDetachedChildren().
  getShellConfig: getShellConfig().
  untrackDetachedChildPid: untrackDetachedChildPid().
  ShellConfig.shell: ShellConfig#shell.
  ShellConfig.args: ShellConfig#args.
  trackDetachedChildPid: trackDetachedChildPid().
  killProcessTree: killProcessTree().
  getShellEnv: getShellEnv().
  sanitizeBinaryOutput: sanitizeBinaryOutput().
  trackedDetachedChildPids: trackedDetachedChildPids.
  findBashOnPath: findBashOnPath().
  ShellConfig: ShellConfig#
---
# Module: [`packages/coding-agent/src/utils/shell.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/shell.ts)

## Classes
### `ShellConfig`
- def: [`packages/coding-agent/src/utils/shell.ts:7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/shell.ts#L7)
- signature: `interface ShellConfig`
- members:
  - `args` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/shell.ts#L9)
  - `shell` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/shell.ts#L8)
- used by: [`createLocalBashOperations`](../core/tools/bash.ts.md#createLocalBashOperations), [`getShellConfig`](shell.ts.md#getShellConfig), [`executeWithConfiguredShell`](../core/resolve-config-value.ts.md#executeWithConfiguredShell)  (1 test-only)

## Functions
- `findBashOnPath()` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/shell.ts#L15) — Find bash executable on PATH (cross-platform)
- `getShellConfig(customShellPath?: string | undefined)` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/shell.ts#L54) — Resolve shell configuration based on platform and an optional explicit shell path.
- `getShellEnv()` — [`L109`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/shell.ts#L109)
- `killProcessTree(pid: number)` — [`L190`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/shell.ts#L190) — Kill a process and all its children (cross-platform)
- `killTrackedDetachedChildren()` — [`L179`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/shell.ts#L179)
- `sanitizeBinaryOutput(str: string)` — [`L131`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/shell.ts#L131) — Sanitize binary output for display/storage.
- `trackDetachedChildPid(pid: number)` — [`L169`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/shell.ts#L169)
- `untrackDetachedChildPid(pid: number)` — [`L174`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/shell.ts#L174)

## Module values
- `trackedDetachedChildPids` — [`L167`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/shell.ts#L167) — Detached child processes must be tracked so they can be killed on parent


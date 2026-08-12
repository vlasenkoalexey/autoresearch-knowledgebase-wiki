---
title: 'Module: packages/coding-agent/src/utils/child-process.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/utils/child-process.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/utils/`child-process.ts`/
symbols:
  isProcessAlive: isProcessAlive().
  shouldUseWindowsShell: shouldUseWindowsShell().
  waitForChildProcess: waitForChildProcess().
  signalProcessGroupOrProcess: signalProcessGroupOrProcess().
  normalizedExitCode: normalizedExitCode().
  isZombieProcess: isZombieProcess().
  processIdExists: processIdExists().
  EXIT_STDIO_GRACE_MS: EXIT_STDIO_GRACE_MS.
  WINDOWS_SHELL_COMMANDS: WINDOWS_SHELL_COMMANDS.
  signalExitCode: signalExitCode().
---
# Module: [`packages/coding-agent/src/utils/child-process.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/child-process.ts)

## Functions
- `isProcessAlive(pid: number)` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/child-process.ts#L50) — True only for a process that is actually running: zombies do not count.
- `isZombieProcess(pid: number)` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/child-process.ts#L27) — A zombie has already exited; it only lingers until its parent reaps it.
- `normalizedExitCode(code: number | null, signal: Signals | null)` — [`L82`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/child-process.ts#L82)
- `processIdExists(pid: number)` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/child-process.ts#L17) — Cheap kill(0) existence probe; counts zombies as existing.
- `shouldUseWindowsShell(command: string)` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/child-process.ts#L10)
- `signalExitCode(signal: Signals | null)` — [`L76`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/child-process.ts#L76) — Wait for a child process to terminate without hanging on inherited stdio handles.
- `signalProcessGroupOrProcess(pid: number, signal: Signals)` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/child-process.ts#L54)
- `waitForChildProcess(child: ChildProcess)` — [`L86`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/child-process.ts#L86)

## Module values
- `EXIT_STDIO_GRACE_MS` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/child-process.ts#L6)
- `WINDOWS_SHELL_COMMANDS` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/child-process.ts#L8)


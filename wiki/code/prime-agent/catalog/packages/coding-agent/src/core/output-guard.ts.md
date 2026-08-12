---
title: 'Module: packages/coding-agent/src/core/output-guard.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/output-guard.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`output-guard.ts`/
symbols:
  takeOverStdout: takeOverStdout().
  writeRawStdout: writeRawStdout().
  stdoutTakeoverState: stdoutTakeoverState.
  restoreStdout: restoreStdout().
  flushRawStdout: flushRawStdout().
  isStdoutTakenOver: isStdoutTakenOver().
  StdoutTakeoverState: StdoutTakeoverState#
  StdoutTakeoverState.rawStdoutWrite: StdoutTakeoverState#rawStdoutWrite.
  StdoutTakeoverState.rawStderrWrite: StdoutTakeoverState#rawStderrWrite.
  StdoutTakeoverState.originalStdoutWrite: StdoutTakeoverState#originalStdoutWrite.
---
# Module: [`packages/coding-agent/src/core/output-guard.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/output-guard.ts)

## Classes
### `StdoutTakeoverState`
- def: [`packages/coding-agent/src/core/output-guard.ts:1`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/output-guard.ts#L1)
- signature: `interface StdoutTakeoverState`
- members:
  - `originalStdoutWrite` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/output-guard.ts#L4)
  - `rawStderrWrite` — [`L3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/output-guard.ts#L3)
  - `rawStdoutWrite` — [`L2`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/output-guard.ts#L2)
- used by: [`takeOverStdout`](output-guard.ts.md#takeOverStdout), [`writeRawStdout`](output-guard.ts.md#writeRawStdout), [`stdoutTakeoverState`](output-guard.ts.md#stdoutTakeoverState), [`restoreStdout`](output-guard.ts.md#restoreStdout), [`flushRawStdout`](output-guard.ts.md#flushRawStdout)

## Functions
- `flushRawStdout()` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/output-guard.ts#L57)
- `isStdoutTakenOver()` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/output-guard.ts#L45)
- `restoreStdout()` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/output-guard.ts#L36)
- `takeOverStdout()` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/output-guard.ts#L9)
- `writeRawStdout(text: string)` — [`L49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/output-guard.ts#L49)

## Module values
- `stdoutTakeoverState` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/output-guard.ts#L7)


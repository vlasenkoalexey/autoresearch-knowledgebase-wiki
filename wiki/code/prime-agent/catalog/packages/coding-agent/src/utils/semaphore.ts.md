---
title: 'Module: packages/coding-agent/src/utils/semaphore.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/utils/semaphore.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/utils/`semaphore.ts`/Semaphore#
symbols:
  Semaphore.run: run().
  Semaphore.-constructor: '`<constructor>`().'
  Semaphore.acquire: acquire().
  Semaphore.release: release().
  Semaphore.-get-queueLength: '`<get>queueLength`().'
  Semaphore.waiters: waiters.
  Semaphore.available: available.
  Semaphore: ''
---
# Module: [`packages/coding-agent/src/utils/semaphore.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/semaphore.ts)

## Classes
### `Semaphore`
- def: [`packages/coding-agent/src/utils/semaphore.ts:5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/semaphore.ts#L5)
- doc: Counting semaphore for bounding async concurrency. FIFO: waiters acquire in
- signature: `class Semaphore`
- members:
  - `<constructor>(permits: number)` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/semaphore.ts#L9) — Counting semaphore for bounding async concurrency. FIFO: waiters acquire in
  - `<get>queueLength` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/semaphore.ts#L16)
  - `acquire(method)` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/semaphore.ts#L20)
  - `release(method)` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/semaphore.ts#L45)
  - `run(method)` — [`L55`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/semaphore.ts#L55) — Run `fn` while holding a permit, releasing it even if `fn` throws. Rejects without running if `signal` aborts while queued.
  - `available` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/semaphore.ts#L6)
  - `waiters` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/semaphore.ts#L7)
- used by: [`boot-gate.ts`](../core/kernel/boot-gate.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-kernel-boot-gate.ts), [`withKernelBootPermit`](../core/kernel/boot-gate.ts.md#withKernelBootPermit), [`kernelBootSemaphore`](../core/kernel/boot-gate.ts.md#kernelBootSemaphore)  (1 test-only)


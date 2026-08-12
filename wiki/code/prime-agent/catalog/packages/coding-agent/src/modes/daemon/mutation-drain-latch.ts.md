---
title: 'Module: packages/coding-agent/src/modes/daemon/mutation-drain-latch.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/mutation-drain-latch.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`mutation-drain-latch.ts`/MutationDrainLatch#
symbols:
  MutationDrainLatch: ''
  MutationDrainLatch.waitForDrain: waitForDrain().
  MutationDrainLatch.end: end().
  MutationDrainLatch.begin: begin().
  MutationDrainLatch.waiters: waiters.
  MutationDrainLatch.active: active.
---
# Module: [`packages/coding-agent/src/modes/daemon/mutation-drain-latch.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/mutation-drain-latch.ts)

## Classes
### `MutationDrainLatch`
- def: [`packages/coding-agent/src/modes/daemon/mutation-drain-latch.ts:2`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/mutation-drain-latch.ts#L2)
- doc: Counts in-flight mutating commands so update-restart preparation can wait for them to drain.
- signature: `class MutationDrainLatch`
- members:
  - `begin(method)` — [`L6`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/mutation-drain-latch.ts#L6)
  - `end(method)` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/mutation-drain-latch.ts#L10)
  - `waitForDrain(method)` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/mutation-drain-latch.ts#L16)
  - `active` — [`L3`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/mutation-drain-latch.ts#L3)
  - `waiters` — [`L4`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/mutation-drain-latch.ts#L4)
- used by: [`daemon-mode.ts`](daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`daemon-supervisor.ts`](daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`<constructor>`](daemon-mode.ts.md#AgentDaemon.-constructor), [`handleLine`](daemon-supervisor.ts.md#DaemonSupervisor.handleLine), [`handleLine`](daemon-mode.ts.md#AgentDaemon.handleLine), [`runIdleEvictionSweep`](daemon-supervisor.ts.md#DaemonSupervisor.runIdleEvictionSweep), [`runUpdateRestartPreparation`](daemon-mode.ts.md#AgentDaemon.runUpdateRestartPreparation), [`prepareUpdateRestart`](daemon-supervisor.ts.md#DaemonSupervisor.prepareUpdateRestart), [`mutationDrain`](daemon-mode.ts.md#AgentDaemon.mutationDrain), [`mutationDrain`](daemon-supervisor.ts.md#DaemonSupervisor.mutationDrain)  (7 test-only)


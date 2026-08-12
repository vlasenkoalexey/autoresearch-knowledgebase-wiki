---
title: 'Module: packages/coding-agent/test/daemon-supervisor-heartbeats.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/daemon-supervisor-heartbeats.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`daemon-supervisor-heartbeats.test.ts`/
symbols:
  createSupervisorHarness: createSupervisorHarness().
  SupervisorHarness.forwardToWorker: SupervisorHarness#forwardToWorker().
  SupervisorHarness.handleCommand: SupervisorHarness#handleCommand().
  SupervisorHarness.workers: SupervisorHarness#workers.
  worker: worker().
  tempDirs: tempDirs.
  SupervisorHarness: SupervisorHarness#
  SupervisorHarness.handleWorkerFrame: SupervisorHarness#handleWorkerFrame().
---
# Module: [`packages/coding-agent/test/daemon-supervisor-heartbeats.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-heartbeats.test.ts)

## Classes
### `SupervisorHarness`
- def: [`packages/coding-agent/test/daemon-supervisor-heartbeats.test.ts:9`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-heartbeats.test.ts#L9)
- signature: `interface SupervisorHarness`
- members:
  - `forwardToWorker(method)` — [`L11`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-heartbeats.test.ts#L11)
  - `handleCommand(method)` — [`L12`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-heartbeats.test.ts#L12)
  - `handleWorkerFrame(method)` — [`L13`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-heartbeats.test.ts#L13)
  - `workers` — [`L10`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-heartbeats.test.ts#L10)
- uses (calls/refs, reference-scoped): [`DaemonCommand`](../src/modes/daemon/daemon-protocol.ts.md#DaemonCommand), [`DaemonSocketClient`](../src/modes/daemon/active-session-state.ts.md#DaemonSocketClient), [`DaemonResponse`](../src/modes/daemon/daemon-protocol.ts.md#DaemonResponse)
- used by: (2 test-only callers)

## Functions
- `createSupervisorHarness()` — [`L24`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-heartbeats.test.ts#L24)
- `worker(lifecycle: "ready" | "recovering", connected?: boolean)` — [`L33`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-heartbeats.test.ts#L33)

## Module values
- `tempDirs` — [`L16`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/daemon-supervisor-heartbeats.test.ts#L16)


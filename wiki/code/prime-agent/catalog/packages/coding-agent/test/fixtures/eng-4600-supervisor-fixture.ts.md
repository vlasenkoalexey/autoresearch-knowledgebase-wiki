---
title: 'Module: packages/coding-agent/test/fixtures/eng-4600-supervisor-fixture.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/fixtures/eng-4600-supervisor-fixture.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/fixtures/`eng-4600-supervisor-fixture.ts`/
symbols:
  runSupervisor: runSupervisor().
  runOwnershipHolder: runOwnershipHolder().
  main: main().
  requiredEnvironment: requiredEnvironment().
  send: send().
  waitForControl: waitForControl().
  runLegacyCleanup: runLegacyCleanup().
  releaseSupervisorRuntime: releaseSupervisorRuntime().
  ControlMessage: ControlMessage#
  ControlMessage.typeLiteral0.type: ControlMessage#typeLiteral0:type.
---
# Module: [`packages/coding-agent/test/fixtures/eng-4600-supervisor-fixture.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/fixtures/eng-4600-supervisor-fixture.ts)

## Classes
### `ControlMessage`
- def: [`packages/coding-agent/test/fixtures/eng-4600-supervisor-fixture.ts:9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/fixtures/eng-4600-supervisor-fixture.ts#L9)
- signature: `type ControlMessage`
- members:
  - `type` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/fixtures/eng-4600-supervisor-fixture.ts#L9)
- used by: (3 test-only callers)

## Functions
- `main()` — [`L136`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/fixtures/eng-4600-supervisor-fixture.ts#L136)
- `releaseSupervisorRuntime(supervisor: DaemonSupervisor)` — [`L90`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/fixtures/eng-4600-supervisor-fixture.ts#L90)
- `requiredEnvironment(name: string)` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/fixtures/eng-4600-supervisor-fixture.ts#L11)
- `runLegacyCleanup()` — [`L104`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/fixtures/eng-4600-supervisor-fixture.ts#L104)
- `runOwnershipHolder()` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/fixtures/eng-4600-supervisor-fixture.ts#L36)
- `runSupervisor()` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/fixtures/eng-4600-supervisor-fixture.ts#L53)
- `send(message: Record<string, unknown>)` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/fixtures/eng-4600-supervisor-fixture.ts#L19)
- `waitForControl(type: "release" | "shutdown" | "go" | "cleanup" | "probe" | "release_runtime")` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/fixtures/eng-4600-supervisor-fixture.ts#L23)


---
title: 'Module: packages/coding-agent/test/suite/acp-features.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/acp-features.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/`acp-features.test.ts`/
symbols:
  connectAcp: connectAcp().
  AcpFixture.agent: AcpFixture#agent.
  AcpFixture.sessionId: AcpFixture#sessionId.
  withMidTurnRebuild.typeLiteral63.arm: withMidTurnRebuild().typeLiteral63:arm.
  runtimeHostFor: runtimeHostFor().
  AcpFixture.updates: AcpFixture#updates.
  AcpFixture.metaOf: AcpFixture#metaOf.
  withMidTurnRebuild: withMidTurnRebuild().
  waitFor: waitFor().
  withMidTurnRebuild.typeLiteral63.connection: withMidTurnRebuild().typeLiteral63:connection.
  rematerialize: rematerialize().
  AcpFixture: AcpFixture#
  ipythonTool: ipythonTool.
---
# Module: [`packages/coding-agent/test/suite/acp-features.test.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-features.test.ts)

## Classes
### `AcpFixture`
- def: [`packages/coding-agent/test/suite/acp-features.test.ts:33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-features.test.ts#L33)
- signature: `interface AcpFixture`
- members:
  - `agent` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-features.test.ts#L34)
  - `metaOf` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-features.test.ts#L37)
  - `sessionId` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-features.test.ts#L36)
  - `updates` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-features.test.ts#L35)
- used by: (2 test-only callers)

## Functions
- `connectAcp(harness: Harness, existing?: InProcessAgentConnection | undefined)` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-features.test.ts#L54)
- `rematerialize(messages: AgentMessage[])` — [`L142`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-features.test.ts#L142) — Copy messages the way a rebuild from persisted entries does: new objects, same fields.
- `runtimeHostFor(session: unknown)` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-features.test.ts#L24) — Feature-preservation suite for ACP mode.
- `waitFor(predicate: () => boolean, timeoutMs?: number)` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-features.test.ts#L45) — Poll until `predicate` holds. Some turns are admitted rather than awaited
- `withMidTurnRebuild(harness: Harness, rebuild: (messages: AgentMessage[]) => AgentMessage[] | undefined)` — [`L117`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-features.test.ts#L117) — Wrap a connection so a transcript rebuild runs mid-turn, right after

## Module values
- `arm` — [`L120`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-features.test.ts#L120)
- `connection` — [`L120`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-features.test.ts#L120)
- `ipythonTool` — [`L91`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-features.test.ts#L91) — Stand-in for the real IPython tool: the suite harness has no kernel, and this


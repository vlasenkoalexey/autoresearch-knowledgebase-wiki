---
title: 'Module: packages/coding-agent/test/acp-cold-cli.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/acp-cold-cli.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`acp-cold-cli.test.ts`/
symbols:
  driveAcpTurn: driveAcpTurn().
  servers: servers.
  startRejectingProvider: startRejectingProvider().
  tempDirs: tempDirs.
  cliPath: cliPath.
  tsxPath: tsxPath.
  AcpResult: AcpResult#
  AcpResult.responses: AcpResult#responses.
  AcpResult.updates: AcpResult#updates.
---
# Module: [`packages/coding-agent/test/acp-cold-cli.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-cold-cli.test.ts)

## Classes
### `AcpResult`
- def: [`packages/coding-agent/test/acp-cold-cli.test.ts:47`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-cold-cli.test.ts#L47)
- signature: `interface AcpResult`
- members:
  - `responses` — [`L48`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-cold-cli.test.ts#L48)
  - `updates` — [`L49`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-cold-cli.test.ts#L49)
- used by: (2 test-only callers)

## Functions
- `driveAcpTurn(baseUrl: string)` — [`L52`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-cold-cli.test.ts#L52)
- `startRejectingProvider()` — [`L35`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-cold-cli.test.ts#L35) — A provider endpoint that always rejects, so the turn fails for a real reason.

## Module values
- `cliPath` — [`L19`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-cold-cli.test.ts#L19) — Cold real-CLI ACP coverage.
- `servers` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-cold-cli.test.ts#L23)
- `tempDirs` — [`L22`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-cold-cli.test.ts#L22)
- `tsxPath` — [`L20`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/acp-cold-cli.test.ts#L20)


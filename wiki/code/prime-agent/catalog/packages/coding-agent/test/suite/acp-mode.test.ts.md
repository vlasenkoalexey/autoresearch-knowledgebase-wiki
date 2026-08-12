---
title: 'Module: packages/coding-agent/test/suite/acp-mode.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/acp-mode.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/`acp-mode.test.ts`/
symbols:
  connectAcpClient: connectAcpClient().
  runtimeHostFor: runtimeHostFor().
  ClientHarness.client: ClientHarness#client.
  ClientHarness.updates: ClientHarness#updates.
  ClientHarness: ClientHarness#
  ClientHarness.close: ClientHarness#close.
---
# Module: [`packages/coding-agent/test/suite/acp-mode.test.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-mode.test.ts)

## Classes
### `ClientHarness`
- def: [`packages/coding-agent/test/suite/acp-mode.test.ts:26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-mode.test.ts#L26)
- doc: Drives ACP mode with a REAL
- signature: `interface ClientHarness`
- members:
  - `client` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-mode.test.ts#L27)
  - `close` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-mode.test.ts#L29)
  - `updates` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-mode.test.ts#L28)
- used by: (2 test-only callers)

## Functions
- `connectAcpClient(connection: any)` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-mode.test.ts#L32)
- `runtimeHostFor(session: unknown)` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/acp-mode.test.ts#L11) — Minimal AgentSessionRuntime host over a real faux-backed AgentSession.


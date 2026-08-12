---
title: 'Module: packages/coding-agent/src/modes/acp/acp-stop-reason.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/acp/acp-stop-reason.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/acp/`acp-stop-reason.ts`/
symbols:
  acpStopReason: acpStopReason().
  acpStopReason.options-typeLiteral0.cancelled: acpStopReason().(options)typeLiteral0:cancelled.
  acpStopReason.options-typeLiteral0.autonomous: acpStopReason().(options)typeLiteral0:autonomous.
  AcpStopReason: AcpStopReason#
---
# Module: [`packages/coding-agent/src/modes/acp/acp-stop-reason.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-stop-reason.ts)

## Classes
### `AcpStopReason`
- def: [`packages/coding-agent/src/modes/acp/acp-stop-reason.ts:8`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-stop-reason.ts#L8)
- doc: ACP stop reasons. `session/prompt` resolves with one of these after the agent
- signature: `type AcpStopReason`
- used by: [`runAcpModeWithConnection`](acp-mode.ts.md#runAcpModeWithConnection), [`acp-mode.ts`](acp-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-acp-acp-mode.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-acp-index.ts), [`acpStopReason`](acp-stop-reason.ts.md#acpStopReason)

## Functions
- `acpStopReason(options: { cancelled: boolean; autonomous?: AgentAutonomousStatus | undefined; })` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-stop-reason.ts#L18) — Map a finished prime-agent turn onto an ACP stop reason.

## Module values
- `autonomous` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-stop-reason.ts#L18)
- `cancelled` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-stop-reason.ts#L18)


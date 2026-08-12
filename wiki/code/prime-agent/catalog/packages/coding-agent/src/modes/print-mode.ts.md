---
title: 'Module: packages/coding-agent/src/modes/print-mode.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/print-mode.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/`print-mode.ts`/
symbols:
  runPrintModeWithConnectionInternal: runPrintModeWithConnectionInternal().
  runPrintMode: runPrintMode().
  describeAutonomousLimit: describeAutonomousLimit().
  PrintModeOptions.mode: PrintModeOptions#mode.
  runPrintModeWithConnection: runPrintModeWithConnection().
  PrintModeOptions.initialImages: PrintModeOptions#initialImages.
  PrintModeOptions: PrintModeOptions#
  PrintModeOptions.initialMessage: PrintModeOptions#initialMessage.
  PrintModeOptions.messages: PrintModeOptions#messages.
---
# Module: [`packages/coding-agent/src/modes/print-mode.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/print-mode.ts)

## Classes
### `PrintModeOptions`
- def: [`packages/coding-agent/src/modes/print-mode.ts:21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/print-mode.ts#L21)
- doc: Options for print mode.
- signature: `interface PrintModeOptions`
- members:
  - `initialImages` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/print-mode.ts#L29) — Images to attach to the initial message
  - `initialMessage` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/print-mode.ts#L27) — First message to send (may contain
  - `messages` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/print-mode.ts#L25) — Array of additional prompts to send after initialMessage
  - `mode` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/print-mode.ts#L23) — Output mode: "text" for final response only, "json" for all events
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../ai/src/types.ts.md#ImageContent)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`main`](../main.ts.md#main), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`runPrintModeWithConnectionInternal`](print-mode.ts.md#runPrintModeWithConnectionInternal), [`runPrintMode`](print-mode.ts.md#runPrintMode), [`runPrintModeWithConnection`](print-mode.ts.md#runPrintModeWithConnection)  (1 test-only)

## Functions
- `describeAutonomousLimit(status: AgentAutonomousStatus, reason: AutonomousLimitReason)` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/print-mode.ts#L32)
- `runPrintMode(runtimeHost: AgentSessionRuntime, options: PrintModeOptions)` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/print-mode.ts#L50) — Run in print (single-shot) mode.
- `runPrintModeWithConnection(connection: AgentConnection, options: PrintModeOptions)` — [`L55`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/print-mode.ts#L55)
- `runPrintModeWithConnectionInternal(connection: AgentConnection, options: PrintModeOptions, bindHeadlessExtensions?: (() => Promise<void>) | undefined)` — [`L62`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/print-mode.ts#L62)


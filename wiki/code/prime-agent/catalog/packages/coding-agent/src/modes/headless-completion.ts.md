---
title: 'Module: packages/coding-agent/src/modes/headless-completion.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/headless-completion.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/`headless-completion.ts`/
symbols:
  waitForHeadlessCompletion: waitForHeadlessCompletion().
  selectHeadlessTerminalResult: selectHeadlessTerminalResult().
  shouldContinueAutonomousGates: shouldContinueAutonomousGates().
  autonomousProgressKey: autonomousProgressKey().
  latestAutonomousGateAttempt: latestAutonomousGateAttempt().
  HeadlessTerminalResultMessage: HeadlessTerminalResultMessage#
  HeadlessTerminalResult.primary: HeadlessTerminalResult#primary.
  HeadlessTerminalResult: HeadlessTerminalResult#
  HeadlessTerminalResult.compactionOutcomes: HeadlessTerminalResult#compactionOutcomes.
---
# Module: [`packages/coding-agent/src/modes/headless-completion.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/headless-completion.ts)

## Classes
### `HeadlessTerminalResult`
- def: [`packages/coding-agent/src/modes/headless-completion.ts:23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/headless-completion.ts#L23)
- signature: `interface HeadlessTerminalResult`
- members:
  - `compactionOutcomes` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/headless-completion.ts#L25)
  - `primary` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/headless-completion.ts#L24)
- uses (calls/refs, reference-scoped): [`CompactionOutcomeMessage`](../core/messages.ts.md#CompactionOutcomeMessage), [`HeadlessTerminalResultMessage`](headless-completion.ts.md#HeadlessTerminalResultMessage)
- used by: [`runPrintModeWithConnectionInternal`](print-mode.ts.md#runPrintModeWithConnectionInternal), [`waitForHeadlessCompletion`](headless-completion.ts.md#waitForHeadlessCompletion), [`selectHeadlessTerminalResult`](headless-completion.ts.md#selectHeadlessTerminalResult)

### `HeadlessTerminalResultMessage`
- def: [`packages/coding-agent/src/modes/headless-completion.ts:21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/headless-completion.ts#L21)
- signature: `type HeadlessTerminalResultMessage`
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../../ai/src/types.ts.md#AssistantMessage), [`SessionSlashCommandResultMessage`](../core/messages.ts.md#SessionSlashCommandResultMessage)
- used by: [`primary`](headless-completion.ts.md#HeadlessTerminalResult.primary)

## Functions
- `autonomousProgressKey(status: AgentAutonomousStatus)` — [`L64`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/headless-completion.ts#L64)
- `latestAutonomousGateAttempt(status: AgentAutonomousStatus)` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/headless-completion.ts#L17)
- `selectHeadlessTerminalResult(messages: readonly AgentMessage[])` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/headless-completion.ts#L28)
- `shouldContinueAutonomousGates(status: AgentAutonomousStatus)` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/headless-completion.ts#L54)
- `waitForHeadlessCompletion(session: AgentSession)` — [`L74`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/headless-completion.ts#L74)


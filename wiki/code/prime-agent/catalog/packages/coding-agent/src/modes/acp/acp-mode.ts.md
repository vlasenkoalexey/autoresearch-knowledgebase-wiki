---
title: 'Module: packages/coding-agent/src/modes/acp/acp-mode.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/acp/acp-mode.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/acp/`acp-mode.ts`/
symbols:
  runAcpModeWithConnection: runAcpModeWithConnection().
  turnFailure: turnFailure().
  autonomousMeta: autonomousMeta().
  promptContent: promptContent().
  runAcpMode: runAcpMode().
  turnBoundary: turnBoundary().
  isPreTurn: isPreTurn().
  AcpSessionEntry.abort: AcpSessionEntry#abort.
  canonicalCwd: canonicalCwd().
  AcpSessionEntry.id: AcpSessionEntry#id.
  AcpSessionEntry.unsubscribe: AcpSessionEntry#unsubscribe.
  rawStdoutSink: rawStdoutSink().
  sameCwd: sameCwd().
  AcpModeOptions: AcpModeOptions#
  AcpModeOptions.stream: AcpModeOptions#stream.
  TurnBoundary: TurnBoundary#
  AcpSessionEntry: AcpSessionEntry#
  promptContent.typeLiteral37.text: promptContent().typeLiteral37:text.
  promptContent.typeLiteral37.images: promptContent().typeLiteral37:images.
  TurnBoundary.identities: TurnBoundary#identities.
  TurnBoundary.keys: TurnBoundary#keys.
  messageKey: messageKey().
  normalizeWindowsDriveLetter: normalizeWindowsDriveLetter().
  AcpModeOptions.bindHeadlessExtensions: AcpModeOptions#bindHeadlessExtensions.
  AcpModeOptions.ownStdout: AcpModeOptions#ownStdout.
---
# Module: [`packages/coding-agent/src/modes/acp/acp-mode.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts)

## Classes
### `AcpModeOptions`
- def: [`packages/coding-agent/src/modes/acp/acp-mode.ts:87`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L87)
- signature: `interface AcpModeOptions`
- members:
  - `bindHeadlessExtensions` — [`L89`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L89) — Bind headless extensions once the connection is live (in-process mode).
  - `ownStdout` — [`L96`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L96) — Skip claiming stdout when the caller supplies its own transport.
  - `stream` — [`L94`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L94) — Transport override. Defaults to NDJSON over stdio; tests supply an
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`runAcpModeWithConnection`](acp-mode.ts.md#runAcpModeWithConnection), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-acp-index.ts)

### `AcpSessionEntry`
- def: [`packages/coding-agent/src/modes/acp/acp-mode.ts:99`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L99)
- signature: `interface AcpSessionEntry`
- members:
  - `abort` — [`L101`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L101)
  - `id` — [`L100`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L100)
  - `unsubscribe` — [`L102`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L102)
- used by: [`runAcpModeWithConnection`](acp-mode.ts.md#runAcpModeWithConnection)

### `TurnBoundary`
- def: [`packages/coding-agent/src/modes/acp/acp-mode.ts:167`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L167)
- doc: The transcript as it stood before a turn started, recorded so the turn's own
- signature: `interface TurnBoundary`
- members:
  - `identities` — [`L168`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L168)
  - `keys` — [`L169`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L169)
- used by: [`turnFailure`](acp-mode.ts.md#turnFailure), [`turnBoundary`](acp-mode.ts.md#turnBoundary), [`isPreTurn`](acp-mode.ts.md#isPreTurn)

## Functions
- `autonomousMeta(status: AgentAutonomousStatus | undefined)` — [`L140`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L140)
- `canonicalCwd(path: string)` — [`L55`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L55)
- `isPreTurn(message: unknown, boundary: TurnBoundary)` — [`L197`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L197)
- `messageKey(message: unknown)` — [`L173`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L173) — Key for a kept message: compaction drops messages, it does not rewrite them.
- `normalizeWindowsDriveLetter(path: string)` — [`L50`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L50)
- `promptContent(blocks: readonly unknown[])` — [`L112`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L112) — Split ACP prompt blocks into the text and images prime-agent accepts.
- `rawStdoutSink()` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L41) — ACP frames must reach real stdout.
- `runAcpMode(runtimeHost: AgentSessionRuntime)` — [`L230`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L230)
- `runAcpModeWithConnection(connection: AgentConnection, options?: AcpModeOptions)` — [`L237`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L237)
- `sameCwd(left: string, right: string)` — [`L67`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L67)
- `turnBoundary(messages: readonly AgentMessage[])` — [`L185`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L185)
- `turnFailure(connection: AgentConnection, boundary: TurnBoundary)` — [`L216`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L216) — Error text from an assistant message this turn produced, when it failed.

## Module values
- `images` — [`L112`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L112)
- `text` — [`L112`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-mode.ts#L112)


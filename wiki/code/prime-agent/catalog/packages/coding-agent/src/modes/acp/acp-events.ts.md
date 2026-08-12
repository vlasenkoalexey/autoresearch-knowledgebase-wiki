---
title: 'Module: packages/coding-agent/src/modes/acp/acp-events.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/acp/acp-events.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/acp/`acp-events.ts`/
symbols:
  acpUpdatesForSessionEvent: acpUpdatesForSessionEvent().
  AcpSessionUpdate.sessionUpdate: AcpSessionUpdate#sessionUpdate.
  bashToolCallId: bashToolCallId().
  assistantDeltaUpdates: assistantDeltaUpdates().
  ipythonRichOutput: ipythonRichOutput().
  acpToolKind: acpToolKind().
  textContent: textContent().
  AcpToolStatus: AcpToolStatus#
  AcpEventMappingState: AcpEventMappingState#
  IPYTHON_TOOL_NAME: IPYTHON_TOOL_NAME.
  AcpEventMappingState.activeBashRunId: AcpEventMappingState#activeBashRunId.
  AcpToolKind: AcpToolKind#
  AcpSessionUpdate: AcpSessionUpdate#
  BASH_TOOL_CALL_PREFIX: BASH_TOOL_CALL_PREFIX.
  base64ByteLength: base64ByteLength().
  textContent.typeLiteral5.type: textContent().typeLiteral5:type.
  textContent.typeLiteral5.text: textContent().typeLiteral5:text.
  ipythonCellSource: ipythonCellSource().
  toolResultText: toolResultText().
---
# Module: [`packages/coding-agent/src/modes/acp/acp-events.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts)

## Classes
### `AcpEventMappingState`
- def: [`packages/coding-agent/src/modes/acp/acp-events.ts:131`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L131)
- doc: Correlates streaming bash output with its run.
- signature: `interface AcpEventMappingState`
- members:
  - `activeBashRunId` — [`L132`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L132)
- used by: [`acpUpdatesForSessionEvent`](acp-events.ts.md#acpUpdatesForSessionEvent), [`runAcpModeWithConnection`](acp-mode.ts.md#runAcpModeWithConnection), [`acp-mode.ts`](acp-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-acp-acp-mode.ts)  (1 test-only)

### `AcpSessionUpdate`
- def: [`packages/coding-agent/src/modes/acp/acp-events.ts:17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L17)
- signature: `interface AcpSessionUpdate`
- members:
  - `sessionUpdate` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L18)
- used by: [`acpUpdatesForSessionEvent`](acp-events.ts.md#acpUpdatesForSessionEvent), [`assistantDeltaUpdates`](acp-events.ts.md#assistantDeltaUpdates)  (1 test-only)

### `AcpToolKind`
- def: [`packages/coding-agent/src/modes/acp/acp-events.ts:14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L14)
- doc: Translate prime-agent session events into ACP `session/update` payloads.
- signature: `type AcpToolKind`
- used by: [`acpUpdatesForSessionEvent`](acp-events.ts.md#acpUpdatesForSessionEvent), [`acpToolKind`](acp-events.ts.md#acpToolKind)

### `AcpToolStatus`
- def: [`packages/coding-agent/src/modes/acp/acp-events.ts:15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L15)
- signature: `type AcpToolStatus`
- used by: [`acpUpdatesForSessionEvent`](acp-events.ts.md#acpUpdatesForSessionEvent)

## Functions
- `acpToolKind(toolName: string)` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L25)
- `acpUpdatesForSessionEvent(event: AgentConnectionSessionEvent, state?: AcpEventMappingState)` — [`L135`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L135)
- `assistantDeltaUpdates(event: AssistantMessageEvent)` — [`L57`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L57) — Map one streaming assistant event to an ACP chunk.
- `base64ByteLength(data: string)` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L41) — Decoded byte length of a base64 payload, without materializing it.
- `bashToolCallId(runId: string | undefined)` — [`L305`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L305)
- `ipythonCellSource(args: unknown)` — [`L68`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L68) — Extract the IPython cell source so a client can show what is executing.
- `ipythonRichOutput(result: unknown)` — [`L100`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L100) — Rich IPython output that ACP has no content type for.
- `textContent(text: string)` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L46)
- `toolResultText(result: unknown)` — [`L74`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L74)

## Module values
- `BASH_TOOL_CALL_PREFIX` — [`L303`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L303)
- `IPYTHON_TOOL_NAME` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L23) — prime-agent's model-facing tool is IPython; bash is the secondary escape hatch.
- `text` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L46)
- `type` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/acp/acp-events.ts#L46)


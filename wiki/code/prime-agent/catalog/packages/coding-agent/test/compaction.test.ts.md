---
title: 'Module: packages/coding-agent/test/compaction.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/compaction.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`compaction.test.ts`/
symbols:
  createMessageEntry: createMessageEntry().
  createUserMessage: createUserMessage().
  createAssistantMessage: createAssistantMessage().
  extractText: extractText().
  loadLargeSessionEntries: loadLargeSessionEntries().
  createMockUsage: createMockUsage().
  createCompactionEntry: createCompactionEntry().
  createModelChangeEntry: createModelChangeEntry().
  createThinkingLevelEntry: createThinkingLevelEntry().
  lastId: lastId.
  resetEntryCounter: resetEntryCounter().
  entryCounter: entryCounter.
---
# Module: [`packages/coding-agent/test/compaction.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/compaction.test.ts)

## Functions
- `createAssistantMessage(text: string, usage?: Usage | undefined)` — [`L57`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/compaction.test.ts#L57)
- `createCompactionEntry(summary: string, firstKeptEntryId: string)` — [`L96`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/compaction.test.ts#L96)
- `createMessageEntry(message: AgentMessage)` — [`L83`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/compaction.test.ts#L83)
- `createMockUsage(input: number, output: number, cacheRead?: number, cacheWrite?: number)` — [`L42`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/compaction.test.ts#L42)
- `createModelChangeEntry(provider: string, modelId: string)` — [`L111`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/compaction.test.ts#L111)
- `createThinkingLevelEntry(thinkingLevel: string)` — [`L125`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/compaction.test.ts#L125)
- `createUserMessage(text: string)` — [`L53`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/compaction.test.ts#L53)
- `extractText(messages: AgentMessage[])` — [`L138`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/compaction.test.ts#L138)
- `loadLargeSessionEntries()` — [`L34`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/compaction.test.ts#L34)
- `resetEntryCounter()` — [`L73`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/compaction.test.ts#L73)

## Module values
- `entryCounter` — [`L70`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/compaction.test.ts#L70)
- `lastId` — [`L71`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/compaction.test.ts#L71)


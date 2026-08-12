---
title: 'Module: packages/coding-agent/src/core/compaction/utils.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/compaction/utils.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/compaction/`utils.ts`/
symbols:
  serializeConversation: serializeConversation().
  extractFileOpsFromMessage: extractFileOpsFromMessage().
  computeFileLists: computeFileLists().
  createFileOps: createFileOps().
  FileOperations: FileOperations#
  FileOperations.edited: FileOperations#edited.
  SUMMARIZATION_SYSTEM_PROMPT: SUMMARIZATION_SYSTEM_PROMPT.
  FileOperations.read: FileOperations#read.
  formatFileOperations: formatFileOperations().
  computeFileLists.typeLiteral9.readFiles: computeFileLists().typeLiteral9:readFiles.
  computeFileLists.typeLiteral9.modifiedFiles: computeFileLists().typeLiteral9:modifiedFiles.
  FileOperations.written: FileOperations#written.
  TOOL_RESULT_MAX_CHARS: TOOL_RESULT_MAX_CHARS.
  truncateForSummary: truncateForSummary().
---
# Module: [`packages/coding-agent/src/core/compaction/utils.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/utils.ts)

## Classes
### `FileOperations`
- def: [`packages/coding-agent/src/core/compaction/utils.ts:12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/utils.ts#L12)
- signature: `interface FileOperations`
- members:
  - `edited` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/utils.ts#L15)
  - `read` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/utils.ts#L13)
  - `written` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/utils.ts#L14)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`prepareBranchEntries`](branch-summarization.ts.md#prepareBranchEntries), [`compaction.ts`](compaction.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-compaction-compaction.ts), [`branch-summarization.ts`](branch-summarization.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-compaction-branch-summarization.ts), [`extractFileOpsFromMessage`](utils.ts.md#extractFileOpsFromMessage), [`extractFileOperations`](compaction.ts.md#extractFileOperations), [`computeFileLists`](utils.ts.md#computeFileLists), [`createFileOps`](utils.ts.md#createFileOps), [`modifiedFiles`](branch-summarization.ts.md#BranchSummaryDetails.modifiedFiles), [`fileOps`](branch-summarization.ts.md#BranchPreparation.fileOps), [`fileOps`](compaction.ts.md#CompactionPreparation.fileOps)

## Functions
- `computeFileLists(fileOps: FileOperations)` — [`L56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/utils.ts#L56) — Compute final file lists from file operations.
- `createFileOps()` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/utils.ts#L18)
- `extractFileOpsFromMessage(message: AgentMessage, fileOps: FileOperations)` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/utils.ts#L29) — Extract file operations from tool calls in an assistant message.
- `formatFileOperations(readFiles: string[], modifiedFiles: string[])` — [`L66`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/utils.ts#L66) — Format file operations as XML tags for summary.
- `serializeConversation(messages: Message[])` — [`L103`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/utils.ts#L103) — Serialize LLM messages to text for summarization.
- `truncateForSummary(text: string, maxChars: number)` — [`L89`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/utils.ts#L89) — Truncate text to a maximum character length for summarization.

## Module values
- `SUMMARIZATION_SYSTEM_PROMPT` — [`L162`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/utils.ts#L162)
- `TOOL_RESULT_MAX_CHARS` — [`L83`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/utils.ts#L83) — Maximum characters for a tool result in serialized summaries.
- `modifiedFiles` — [`L56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/utils.ts#L56)
- `readFiles` — [`L56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/utils.ts#L56)


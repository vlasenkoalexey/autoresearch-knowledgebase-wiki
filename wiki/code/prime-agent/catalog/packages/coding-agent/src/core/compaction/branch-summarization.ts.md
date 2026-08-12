---
title: 'Module: packages/coding-agent/src/core/compaction/branch-summarization.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/compaction/branch-summarization.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/compaction/`branch-summarization.ts`/
symbols:
  getMessageFromEntry: getMessageFromEntry().
  generateBranchSummary: generateBranchSummary().
  prepareBranchEntries: prepareBranchEntries().
  collectEntriesForBranchSummary: collectEntriesForBranchSummary().
  BranchSummaryDetails.modifiedFiles: BranchSummaryDetails#modifiedFiles.
  CollectEntriesResult.entries: CollectEntriesResult#entries.
  BranchPreparation.messages: BranchPreparation#messages.
  BranchPreparation.fileOps: BranchPreparation#fileOps.
  GenerateBranchSummaryOptions.model: GenerateBranchSummaryOptions#model.
  CollectEntriesResult.commonAncestorId: CollectEntriesResult#commonAncestorId.
  BranchSummaryResult: BranchSummaryResult#
  BranchSummaryResult.error: BranchSummaryResult#error.
  BranchSummaryDetails.readFiles: BranchSummaryDetails#readFiles.
  BranchPreparation: BranchPreparation#
  CollectEntriesResult: CollectEntriesResult#
  GenerateBranchSummaryOptions: GenerateBranchSummaryOptions#
  GenerateBranchSummaryOptions.apiKey: GenerateBranchSummaryOptions#apiKey.
  GenerateBranchSummaryOptions.headers: GenerateBranchSummaryOptions#headers.
  GenerateBranchSummaryOptions.signal: GenerateBranchSummaryOptions#signal.
  GenerateBranchSummaryOptions.customInstructions: GenerateBranchSummaryOptions#customInstructions.
  GenerateBranchSummaryOptions.replaceInstructions: GenerateBranchSummaryOptions#replaceInstructions.
  GenerateBranchSummaryOptions.reserveTokens: GenerateBranchSummaryOptions#reserveTokens.
  BRANCH_SUMMARY_PROMPT: BRANCH_SUMMARY_PROMPT.
  BranchSummaryResult.summary: BranchSummaryResult#summary.
  BranchSummaryResult.readFiles: BranchSummaryResult#readFiles.
  BranchSummaryResult.modifiedFiles: BranchSummaryResult#modifiedFiles.
  BranchSummaryResult.aborted: BranchSummaryResult#aborted.
  BranchSummaryDetails: BranchSummaryDetails#
  BranchPreparation.totalTokens: BranchPreparation#totalTokens.
  BRANCH_SUMMARY_PREAMBLE: BRANCH_SUMMARY_PREAMBLE.
---
# Module: [`packages/coding-agent/src/core/compaction/branch-summarization.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts)

## Classes
### `BranchPreparation`
- def: [`packages/coding-agent/src/core/compaction/branch-summarization.ts:49`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L49)
- signature: `interface BranchPreparation`
- members:
  - `fileOps` — [`L53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L53) — File operations extracted from tool calls
  - `messages` — [`L51`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L51) — Messages extracted for summarization, in chronological order
  - `totalTokens` — [`L55`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L55) — Total estimated tokens in messages
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage), [`FileOperations`](utils.ts.md#FileOperations)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`generateBranchSummary`](branch-summarization.ts.md#generateBranchSummary), [`prepareBranchEntries`](branch-summarization.ts.md#prepareBranchEntries)

### `BranchSummaryDetails`
- def: [`packages/coding-agent/src/core/compaction/branch-summarization.ts:42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L42)
- doc: Details stored in BranchSummaryEntry.details for file tracking
- signature: `interface BranchSummaryDetails`
- members:
  - `modifiedFiles` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L44)
  - `readFiles` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L43)
- uses (calls/refs, reference-scoped): [`utils.ts`](utils.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-compaction-utils.ts), [`FileOperations`](utils.ts.md#FileOperations)
- used by: [`prepareBranchEntries`](branch-summarization.ts.md#prepareBranchEntries)

### `BranchSummaryResult`
- def: [`packages/coding-agent/src/core/compaction/branch-summarization.ts:33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L33)
- signature: `interface BranchSummaryResult`
- members:
  - `aborted` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L37)
  - `error` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L38)
  - `modifiedFiles` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L36)
  - `readFiles` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L35)
  - `summary` — [`L34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L34)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`summaryEntry`](../agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`generateBranchSummary`](branch-summarization.ts.md#generateBranchSummary)

### `CollectEntriesResult`
- def: [`packages/coding-agent/src/core/compaction/branch-summarization.ts:58`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L58)
- signature: `interface CollectEntriesResult`
- members:
  - `commonAncestorId` — [`L62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L62) — Common ancestor between old and new position, if any
  - `entries` — [`L60`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L60) — Entries to summarize, in chronological order
- uses (calls/refs, reference-scoped): [`SessionEntry`](../session-manager.ts.md#SessionEntry)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`summaryEntry`](../agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`collectEntriesForBranchSummary`](branch-summarization.ts.md#collectEntriesForBranchSummary)

### `GenerateBranchSummaryOptions`
- def: [`packages/coding-agent/src/core/compaction/branch-summarization.ts:65`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L65)
- signature: `interface GenerateBranchSummaryOptions`
- members:
  - `apiKey` — [`L69`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L69) — API key for the model
  - `customInstructions` — [`L75`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L75) — Optional custom instructions for summarization
  - `headers` — [`L71`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L71) — Request headers for the model
  - `model` — [`L67`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L67) — Model to use for summarization
  - `replaceInstructions` — [`L77`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L77) — If true, customInstructions replaces the default prompt instead of being appended
  - `reserveTokens` — [`L79`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L79) — Tokens reserved for prompt + LLM response (default 16384)
  - `signal` — [`L73`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L73) — Abort signal for cancellation
- uses (calls/refs, reference-scoped): [`Model`](../../../../ai/src/types.ts.md#Model)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`summaryEntry`](../agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`generateBranchSummary`](branch-summarization.ts.md#generateBranchSummary)

## Functions
- `collectEntriesForBranchSummary(session: ReadonlySessionManager, oldLeafId: string | null, targetId: string)` — [`L98`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L98) — Collect entries that should be summarized when navigating from one position to another.
- `generateBranchSummary(entries: SessionEntry[], options: GenerateBranchSummaryOptions)` — [`L288`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L288) — Generate a summary of abandoned branch entries.
- `getMessageFromEntry(entry: SessionEntry)` — [`L146`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L146) — Extract AgentMessage from a session entry.
- `prepareBranchEntries(entries: SessionEntry[], tokenBudget?: number)` — [`L190`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L190) — Prepare entries for summarization with token budget.

## Module values
- `BRANCH_SUMMARY_PREAMBLE` — [`L248`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L248)
- `BRANCH_SUMMARY_PROMPT` — [`L253`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/branch-summarization.ts#L253)


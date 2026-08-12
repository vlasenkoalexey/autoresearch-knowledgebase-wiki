---
title: 'Module: packages/coding-agent/src/core/compaction/compaction.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/compaction/compaction.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/compaction/`compaction.ts`/
symbols:
  prepareCompaction: prepareCompaction().
  findCutPoint: findCutPoint().
  getMessageFromEntry: getMessageFromEntry().
  estimateTokens: estimateTokens().
  compact: compact().
  findTurnStartIndex: findTurnStartIndex().
  findValidCutPoints: findValidCutPoints().
  getLastAssistantUsage: getLastAssistantUsage().
  generateSummary: generateSummary().
  getMessageFromEntryForCompaction: getMessageFromEntryForCompaction().
  generateTurnPrefixSummary: generateTurnPrefixSummary().
  extractFileOperations: extractFileOperations().
  getAssistantUsage: getAssistantUsage().
  estimateContextTokens: estimateContextTokens().
  calculateContextTokens: calculateContextTokens().
  CompactionResult: CompactionResult#
  DEFAULT_COMPACTION_SETTINGS: DEFAULT_COMPACTION_SETTINGS.
  CompactionPreparation.firstKeptEntryId: CompactionPreparation#firstKeptEntryId.
  CompactionPreparation.tokensBefore: CompactionPreparation#tokensBefore.
  shouldCompact: shouldCompact().
  CompactionResult.summary: CompactionResult#summary.
  buildSummarizationPrompt: buildSummarizationPrompt().
  CutPointResult.firstKeptEntryIndex: CutPointResult#firstKeptEntryIndex.
  ContextUsageEstimate.tokens: ContextUsageEstimate#tokens.
  CompactionPreparation.messagesToSummarize: CompactionPreparation#messagesToSummarize.
  CompactionResult.tokensBefore: CompactionResult#tokensBefore.
  CompactionSettings: CompactionSettings#
  getLastAssistantUsageInfo: getLastAssistantUsageInfo().
  CompactionSettings.reserveTokens: CompactionSettings#reserveTokens.
  CompactionPreparation.turnPrefixMessages: CompactionPreparation#turnPrefixMessages.
  CompactionSettings.keepRecentTokens: CompactionSettings#keepRecentTokens.
  CutPointResult.isSplitTurn: CutPointResult#isSplitTurn.
  CompactionResult.firstKeptEntryId: CompactionResult#firstKeptEntryId.
  CompactionSettings.enabled: CompactionSettings#enabled.
  CutPointResult.turnStartIndex: CutPointResult#turnStartIndex.
  ContextUsageEstimate.lastUsageIndex: ContextUsageEstimate#lastUsageIndex.
  CompactionPreparation: CompactionPreparation#
  CompactionPreparation.isSplitTurn: CompactionPreparation#isSplitTurn.
  CompactionPreparation.previousSummary: CompactionPreparation#previousSummary.
  CompactionPreparation.fileOps: CompactionPreparation#fileOps.
  CompactionPreparation.settings: CompactionPreparation#settings.
  CompactionDetails.readFiles: CompactionDetails#readFiles.
  CompactionDetails.modifiedFiles: CompactionDetails#modifiedFiles.
  CompactionDetails: CompactionDetails#
  COMPACT_SKILL_NAME: COMPACT_SKILL_NAME.
  ContextUsageEstimate.usageTokens: ContextUsageEstimate#usageTokens.
  ContextUsageEstimate.trailingTokens: ContextUsageEstimate#trailingTokens.
  CutPointResult: CutPointResult#
  CompactionResult.details: CompactionResult#details.
  ContextUsageEstimate: ContextUsageEstimate#
  SUMMARIZATION_PROMPT: SUMMARIZATION_PROMPT.
  KERNEL_PERSIST_SUMMARY_NOTE: KERNEL_PERSIST_SUMMARY_NOTE.
  UPDATE_SUMMARIZATION_PROMPT: UPDATE_SUMMARIZATION_PROMPT.
  TURN_PREFIX_SUMMARIZATION_PROMPT: TURN_PREFIX_SUMMARIZATION_PROMPT.
---
# Module: [`packages/coding-agent/src/core/compaction/compaction.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts)

## Classes
### `CompactionDetails`
- def: [`packages/coding-agent/src/core/compaction/compaction.ts:33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L33)
- doc: Details stored in CompactionEntry.details for file tracking
- signature: `interface CompactionDetails`
- members:
  - `modifiedFiles` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L35)
  - `readFiles` — [`L34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L34)
- used by: [`compact`](compaction.ts.md#compact), [`extractFileOperations`](compaction.ts.md#extractFileOperations)

### `CompactionPreparation`
- def: [`packages/coding-agent/src/core/compaction/compaction.ts:618`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L618)
- signature: `interface CompactionPreparation`
- members:
  - `fileOps` — [`L631`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L631) — File operations extracted from messagesToSummarize
  - `firstKeptEntryId` — [`L620`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L620) — UUID of first entry to keep
  - `isSplitTurn` — [`L626`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L626) — Whether this is a split turn (cut point in middle of turn)
  - `messagesToSummarize` — [`L622`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L622) — Messages that will be summarized and discarded
  - `previousSummary` — [`L629`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L629) — Summary from previous compaction, for iterative update
  - `settings` — [`L633`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L633) — Compaction settions from settings.jsonl
  - `tokensBefore` — [`L627`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L627)
  - `turnPrefixMessages` — [`L624`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L624) — Messages that will be turned into turn prefix summary (if splitting)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage), [`FileOperations`](utils.ts.md#FileOperations), [`CompactionSettings`](compaction.ts.md#CompactionSettings)
- used by: [`types.ts`](../extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`prepareCompaction`](compaction.ts.md#prepareCompaction), [`compact`](compaction.ts.md#compact), [`preparation`](../extensions/types.ts.md#SessionBeforeCompactEvent.preparation)  (6 test-only)

### `CompactionResult`
- def: [`packages/coding-agent/src/core/compaction/compaction.ts:108`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L108)
- doc: Result from compact() - SessionManager adds uuid/parentUuid when saving
- signature: `interface CompactionResult`
- members:
  - `details` — [`L113`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L113) — Extension-specific data (e.g., ArtifactIndex, version markers for structured compaction)
  - `firstKeptEntryId` — [`L110`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L110)
  - `summary` — [`L109`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L109)
  - `tokensBefore` — [`L111`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L111)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](../agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`daemon-agent-connection.ts`](../../modes/agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`in-process-agent-connection.ts`](../../modes/agent-connection/in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`types.ts`](../extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`acpUpdatesForSessionEvent`](../../modes/acp/acp-events.ts.md#acpUpdatesForSessionEvent), [`types.ts`](../../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`signal`](../agent-session.ts.md#AgentSession._performCompaction.options-typeLiteral2765.signal), [`compact`](../agent-session.ts.md#AgentSession.compact), [`rpc-client.ts`](../../modes/rpc/rpc-client.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-client.ts), [`rpc-types.ts`](../../modes/rpc/rpc-types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-types.ts), [`AgentConnectionSessionEvent`](../../modes/agent-connection/types.ts.md#AgentConnectionSessionEvent), [`compact`](compaction.ts.md#compact), [`AgentSessionEvent`](../agent-session.ts.md#AgentSessionEvent), [`RpcResponse`](../../modes/rpc/rpc-types.ts.md#RpcResponse), [`SessionBeforeCompactResult`](../extensions/types.ts.md#SessionBeforeCompactResult), [`compact`](../../modes/agent-connection/types.ts.md#AgentConnection.compact), [`compact`](../../modes/rpc/rpc-client.ts.md#RpcClient.compact), [`compact`](../../modes/agent-connection/in-process-agent-connection.ts.md#InProcessAgentConnection.compact), [`compact`](../../modes/agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.compact), [`onComplete`](../extensions/types.ts.md#CompactOptions.onComplete)  (5 test-only)

### `CompactionSettings`
- def: [`packages/coding-agent/src/core/compaction/compaction.ts:122`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L122)
- signature: `interface CompactionSettings`
- members:
  - `enabled` — [`L123`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L123)
  - `keepRecentTokens` — [`L125`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L125)
  - `reserveTokens` — [`L124`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L124)
- used by: [`prepareCompaction`](compaction.ts.md#prepareCompaction), [`compact`](compaction.ts.md#compact), [`DEFAULT_COMPACTION_SETTINGS`](compaction.ts.md#DEFAULT_COMPACTION_SETTINGS), [`shouldCompact`](compaction.ts.md#shouldCompact), [`settings`](compaction.ts.md#CompactionPreparation.settings)  (1 test-only)

### `ContextUsageEstimate`
- def: [`packages/coding-agent/src/core/compaction/compaction.ts:177`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L177)
- signature: `interface ContextUsageEstimate`
- members:
  - `lastUsageIndex` — [`L181`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L181)
  - `tokens` — [`L178`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L178)
  - `trailingTokens` — [`L180`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L180)
  - `usageTokens` — [`L179`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L179)
- used by: [`prepareCompaction`](compaction.ts.md#prepareCompaction), [`getContextUsage`](../agent-session.ts.md#AgentSession.getContextUsage), [`computeContextUsageFromEntries`](../context-tree.ts.md#computeContextUsageFromEntries), [`_getThresholdContextTokens`](../agent-session.ts.md#AgentSession._getThresholdContextTokens), [`estimateContextTokens`](compaction.ts.md#estimateContextTokens)  (1 test-only)

### `CutPointResult`
- def: [`packages/coding-agent/src/core/compaction/compaction.ts:372`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L372)
- signature: `interface CutPointResult`
- members:
  - `firstKeptEntryIndex` — [`L374`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L374) — Index of first entry to keep
  - `isSplitTurn` — [`L378`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L378) — Whether this cut splits a turn (cut point is not a user message)
  - `turnStartIndex` — [`L376`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L376) — Index of user message that starts the turn being split, or -1 if not splitting
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`prepareCompaction`](compaction.ts.md#prepareCompaction), [`findCutPoint`](compaction.ts.md#findCutPoint)  (1 test-only)

## Functions
- `buildSummarizationPrompt(customInstructions?: string | undefined, previousSummary?: string | undefined)` — [`L544`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L544) — Build the instruction portion of the summarization prompt: the initial or
- `calculateContextTokens(usage: Usage)` — [`L145`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L145) — Calculate total context tokens from usage.
- `compact(preparation: CompactionPreparation, model: Model<any>, apiKey: string, headers?: Record<string, string> | undefined, customInstructions?: string | undefined, signal?: AbortSignal | undefined, thinkingLevel?: ThinkingLevel | undefined)` — [`L745`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L745) — Generate summaries for compaction using prepared data.
- `estimateContextTokens(messages: AgentMessage[])` — [`L196`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L196) — Estimate context tokens from messages, using the last assistant usage when available.
- `estimateTokens(message: AgentMessage)` — [`L243`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L243) — Estimate token count for a message using chars/4 heuristic.
- `extractFileOperations(messages: AgentMessage[], entries: SessionEntry[], prevCompactionIndex: number)` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L41) — Extract file operations from messages and previous compaction entries.
- `findCutPoint(entries: SessionEntry[], startIndex: number, endIndex: number, keepRecentTokens: number)` — [`L397`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L397) — Find the cut point in session entries that keeps approximately `keepRecentTokens`.
- `findTurnStartIndex(entries: SessionEntry[], entryIndex: number, startIndex: number)` — [`L355`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L355) — Find the user message (or bashExecution) that starts the turn containing the given entry index.
- `findValidCutPoints(entries: SessionEntry[], startIndex: number, endIndex: number)` — [`L310`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L310) — Find valid cut points: indices of user, assistant, custom, or bashExecution messages.
- `generateSummary(currentMessages: AgentMessage[], model: Model<any>, reserveTokens: number, apiKey: string, headers?: Record<string, string> | undefined, signal?: AbortSignal | undefined, customInstructions?: string | undefined, previousSummary?: string | undefined, thinkingLevel?: ThinkingLevel | undefined)` — [`L556`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L556) — Generate a summary of the conversation using the LLM.
- `generateTurnPrefixSummary(messages: AgentMessage[], model: Model<any>, reserveTokens: number, apiKey: string, headers?: Record<string, string> | undefined, signal?: AbortSignal | undefined, thinkingLevel?: ThinkingLevel | undefined)` — [`L830`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L830) — Generate a summary for a turn prefix (when splitting a turn).
- `getAssistantUsage(msg: AgentMessage)` — [`L153`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L153) — Get usage from an assistant message if available.
- `getLastAssistantUsage(entries: SessionEntry[])` — [`L166`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L166) — Find the last non-aborted assistant message usage from session entries.
- `getLastAssistantUsageInfo(messages: AgentMessage[])` — [`L184`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L184)
- `getMessageFromEntry(entry: SessionEntry)` — [`L79`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L79) — Extract AgentMessage from an entry if it produces one.
- `getMessageFromEntryForCompaction(entry: SessionEntry)` — [`L100`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L100)
- `prepareCompaction(pathEntries: SessionEntry[], settings: CompactionSettings)` — [`L636`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L636)
- `shouldCompact(contextTokens: number, contextWindow: number, settings: CompactionSettings)` — [`L229`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L229) — Check if compaction should trigger based on context usage.

## Module values
- `COMPACT_SKILL_NAME` — [`L120`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L120)
- `DEFAULT_COMPACTION_SETTINGS` — [`L128`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L128)
- `KERNEL_PERSIST_SUMMARY_NOTE` — [`L498`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L498)
- `SUMMARIZATION_PROMPT` — [`L465`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L465)
- `TURN_PREFIX_SUMMARIZATION_PROMPT` — [`L723`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L723)
- `UPDATE_SUMMARIZATION_PROMPT` — [`L501`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/compaction/compaction.ts#L501)


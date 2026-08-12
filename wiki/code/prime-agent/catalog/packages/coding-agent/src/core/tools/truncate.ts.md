---
title: 'Module: packages/coding-agent/src/core/tools/truncate.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/tools/truncate.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/tools/`truncate.ts`/
symbols:
  truncateTail: truncateTail().
  truncateHead: truncateHead().
  TruncationResult.truncated: TruncationResult#truncated.
  DEFAULT_MAX_BYTES: DEFAULT_MAX_BYTES.
  TruncationResult: TruncationResult#
  DEFAULT_MAX_LINES: DEFAULT_MAX_LINES.
  TruncationResult.totalLines: TruncationResult#totalLines.
  TruncationResult.content: TruncationResult#content.
  formatSize: formatSize().
  TruncationResult.outputLines: TruncationResult#outputLines.
  truncateLine: truncateLine().
  TruncationResult.truncatedBy: TruncationResult#truncatedBy.
  TruncationResult.totalBytes: TruncationResult#totalBytes.
  TruncationResult.outputBytes: TruncationResult#outputBytes.
  TruncationResult.maxBytes: TruncationResult#maxBytes.
  TruncationResult.lastLinePartial: TruncationResult#lastLinePartial.
  TruncationResult.maxLines: TruncationResult#maxLines.
  TruncationResult.firstLineExceedsLimit: TruncationResult#firstLineExceedsLimit.
  TruncationOptions: TruncationOptions#
  TruncationOptions.maxLines: TruncationOptions#maxLines.
  TruncationOptions.maxBytes: TruncationOptions#maxBytes.
  truncateLine.typeLiteral93.text: truncateLine().typeLiteral93:text.
  truncateLine.typeLiteral93.wasTruncated: truncateLine().typeLiteral93:wasTruncated.
  GREP_MAX_LINE_LENGTH: GREP_MAX_LINE_LENGTH.
  truncateStringToBytesFromEnd: truncateStringToBytesFromEnd().
---
# Module: [`packages/coding-agent/src/core/tools/truncate.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts)

## Classes
### `TruncationOptions`
- def: [`packages/coding-agent/src/core/tools/truncate.ts:40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L40)
- signature: `interface TruncationOptions`
- members:
  - `maxBytes` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L44) — Maximum number of bytes (default: 50KB)
  - `maxLines` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L42) — Maximum number of lines (default: 2000)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`truncateTail`](truncate.ts.md#truncateTail), [`truncateHead`](truncate.ts.md#truncateHead)

### `TruncationResult`
- def: [`packages/coding-agent/src/core/tools/truncate.ts:15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L15)
- signature: `interface TruncationResult`
- members:
  - `content` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L17) — The truncated content
  - `firstLineExceedsLimit` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L33) — Whether the first line exceeded the byte limit (for head truncation)
  - `lastLinePartial` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L31) — Whether the last line was partially truncated (only for tail truncation edge case)
  - `maxBytes` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L37) — The max bytes limit that was applied
  - `maxLines` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L35) — The max lines limit that was applied
  - `outputBytes` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L29) — Number of bytes in the truncated output
  - `outputLines` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L27) — Number of complete lines in the truncated output
  - `totalBytes` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L25) — Total number of bytes in the original content
  - `totalLines` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L23) — Total number of lines in the original content
  - `truncated` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L19) — Whether truncation occurred
  - `truncatedBy` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L21) — Which limit was hit: "lines", "bytes", or null if not truncated
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../../modes/interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`handleEvent`](../../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleEvent), [`addMessageToChat`](../../modes/interactive/interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`createBashToolDefinition`](bash.ts.md#createBashToolDefinition), [`bash.ts`](bash.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-bash.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`details`](bash.ts.md#rebuildBashResultRenderComponent.result-typeLiteral96.details), [`updateDisplay`](../../modes/interactive/components/bash-execution.ts.md#BashExecutionComponent.updateDisplay), [`bash-execution.ts`](../../modes/interactive/components/bash-execution.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-bash-execution.ts), [`truncateTail`](truncate.ts.md#truncateTail), [`snapshot`](output-accumulator.ts.md#OutputAccumulator.snapshot), [`truncateHead`](truncate.ts.md#truncateHead), [`finishSideQuestionBash`](../../modes/interactive/interactive-mode.ts.md#InteractiveMode.finishSideQuestionBash), [`executeBashWithOperations`](../bash-executor.ts.md#executeBashWithOperations), [`setComplete`](../../modes/interactive/components/bash-execution.ts.md#BashExecutionComponent.setComplete), [`output-accumulator.ts`](output-accumulator.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-output-accumulator.ts), [`truncation`](output-accumulator.ts.md#OutputSnapshot.truncation), [`truncation`](bash.ts.md#BashToolDetails.truncation), [`truncationResult`](../../modes/interactive/components/bash-execution.ts.md#BashExecutionComponent.truncationResult)  (3 test-only)

## Functions
- `formatSize(bytes: number)` — [`L50`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L50) — Format bytes as human-readable size.
- `truncateHead(content: string, options?: TruncationOptions)` — [`L67`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L67) — Truncate content from the head (keep first N lines/bytes).
- `truncateLine(line: string, maxChars?: number)` — [`L257`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L257) — Truncate a single line to max characters, adding [truncated] suffix.
- `truncateStringToBytesFromEnd(str: string, maxBytes: number)` — [`L236`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L236) — Truncate a string to fit within a byte limit (from the end).
- `truncateTail(content: string, options?: TruncationOptions)` — [`L157`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L157) — Truncate content from the tail (keep last N lines/bytes).

## Module values
- `DEFAULT_MAX_BYTES` — [`L12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L12)
- `DEFAULT_MAX_LINES` — [`L11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L11) — Shared truncation utilities for tool outputs.
- `GREP_MAX_LINE_LENGTH` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L13)
- `text` — [`L260`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L260)
- `wasTruncated` — [`L260`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/truncate.ts#L260)


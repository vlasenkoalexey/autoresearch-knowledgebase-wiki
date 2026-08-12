---
title: 'Module: packages/coding-agent/src/core/tools/edit-diff.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/tools/edit-diff.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/tools/`edit-diff.ts`/
symbols:
  applyEditsToNormalizedContent: applyEditsToNormalizedContent().
  computeEditsDiff: computeEditsDiff().
  fuzzyFindText: fuzzyFindText().
  computeEditDiff: computeEditDiff().
  Edit: Edit#
  stripBom: stripBom().
  MatchedEdit.matchIndex: MatchedEdit#matchIndex.
  generateDiffString: generateDiffString().
  generateDiffString.typeLiteral100.firstChangedLine: generateDiffString().typeLiteral100:firstChangedLine.
  Edit.oldText: Edit#oldText.
  Edit.newText: Edit#newText.
  EditDiffError.error: EditDiffError#error.
  normalizeToLF: normalizeToLF().
  normalizeForFuzzyMatch: normalizeForFuzzyMatch().
  FuzzyMatchResult.found: FuzzyMatchResult#found.
  FuzzyMatchResult.index: FuzzyMatchResult#index.
  FuzzyMatchResult.matchLength: FuzzyMatchResult#matchLength.
  FuzzyMatchResult.usedFuzzyMatch: FuzzyMatchResult#usedFuzzyMatch.
  stripBom.typeLiteral33.text: stripBom().typeLiteral33:text.
  generateDiffString.typeLiteral100.diff: generateDiffString().typeLiteral100:diff.
  EditDiffResult: EditDiffResult#
  EditDiffResult.diff: EditDiffResult#diff.
  EditDiffError: EditDiffError#
  countOccurrences: countOccurrences().
  FuzzyMatchResult.contentForReplacement: FuzzyMatchResult#contentForReplacement.
  MatchedEdit.editIndex: MatchedEdit#editIndex.
  MatchedEdit.matchLength: MatchedEdit#matchLength.
  AppliedEditsResult.baseContent: AppliedEditsResult#baseContent.
  AppliedEditsResult.newContent: AppliedEditsResult#newContent.
  stripBom.typeLiteral33.bom: stripBom().typeLiteral33:bom.
  detectLineEnding: detectLineEnding().
  restoreLineEndings: restoreLineEndings().
  MatchedEdit.newText: MatchedEdit#newText.
  EditDiffResult.firstChangedLine: EditDiffResult#firstChangedLine.
  FuzzyMatchResult: FuzzyMatchResult#
  MatchedEdit: MatchedEdit#
  AppliedEditsResult: AppliedEditsResult#
  getNotFoundError: getNotFoundError().
  getDuplicateError: getDuplicateError().
  getEmptyOldTextError: getEmptyOldTextError().
  getNoChangeError: getNoChangeError().
---
# Module: [`packages/coding-agent/src/core/tools/edit-diff.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts)

## Classes
### `AppliedEditsResult`
- def: [`packages/coding-agent/src/core/tools/edit-diff.ts:85`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L85)
- signature: `interface AppliedEditsResult`
- members:
  - `baseContent` — [`L86`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L86)
  - `newContent` — [`L87`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L87)
- used by: [`createEditToolDefinition`](edit.ts.md#createEditToolDefinition), [`applyEditsToNormalizedContent`](edit-diff.ts.md#applyEditsToNormalizedContent), [`computeEditsDiff`](edit-diff.ts.md#computeEditsDiff)

### `Edit`
- def: [`packages/coding-agent/src/core/tools/edit-diff.ts:73`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L73)
- signature: `interface Edit`
- members:
  - `newText` — [`L75`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L75)
  - `oldText` — [`L74`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L74)
- used by: [`edit.ts`](edit.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-edit.ts), [`applyEditsToNormalizedContent`](edit-diff.ts.md#applyEditsToNormalizedContent), [`computeEditsDiff`](edit-diff.ts.md#computeEditsDiff), [`getRenderablePreviewInput`](edit.ts.md#getRenderablePreviewInput), [`computeEditDiff`](edit-diff.ts.md#computeEditDiff), [`validateEditInput`](edit.ts.md#validateEditInput), [`edits`](edit.ts.md#RenderableEditArgs.typeLiteral48.edits)  (3 test-only)

### `EditDiffError`
- def: [`packages/coding-agent/src/core/tools/edit-diff.ts:398`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L398)
- signature: `interface EditDiffError`
- members:
  - `error` — [`L399`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L399)
- used by: [`edit.ts`](edit.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-edit.ts), [`formatEditResult`](edit.ts.md#formatEditResult), [`buildEditCallComponent`](edit.ts.md#buildEditCallComponent), [`computeEditsDiff`](edit-diff.ts.md#computeEditsDiff), [`setEditPreview`](edit.ts.md#setEditPreview), [`computeEditDiff`](edit-diff.ts.md#computeEditDiff), [`EditPreview`](edit.ts.md#EditPreview)  (1 test-only)

### `EditDiffResult`
- def: [`packages/coding-agent/src/core/tools/edit-diff.ts:393`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L393)
- signature: `interface EditDiffResult`
- members:
  - `diff` — [`L394`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L394)
  - `firstChangedLine` — [`L395`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L395)
- used by: [`edit.ts`](edit.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-edit.ts), [`formatEditResult`](edit.ts.md#formatEditResult), [`buildEditCallComponent`](edit.ts.md#buildEditCallComponent), [`computeEditsDiff`](edit-diff.ts.md#computeEditsDiff), [`setEditPreview`](edit.ts.md#setEditPreview), [`computeEditDiff`](edit-diff.ts.md#computeEditDiff), [`EditPreview`](edit.ts.md#EditPreview)

### `FuzzyMatchResult`
- def: [`packages/coding-agent/src/core/tools/edit-diff.ts:57`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L57)
- signature: `interface FuzzyMatchResult`
- members:
  - `contentForReplacement` — [`L70`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L70) — The content to use for replacement operations.
  - `found` — [`L59`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L59) — Whether a match was found
  - `index` — [`L61`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L61) — The index where the match starts (in the content that should be used for replacement)
  - `matchLength` — [`L63`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L63) — Length of the matched text
  - `usedFuzzyMatch` — [`L65`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L65) — Whether fuzzy matching was used (false = exact match)
- used by: [`applyEditsToNormalizedContent`](edit-diff.ts.md#applyEditsToNormalizedContent), [`fuzzyFindText`](edit-diff.ts.md#fuzzyFindText)

### `MatchedEdit`
- def: [`packages/coding-agent/src/core/tools/edit-diff.ts:78`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L78)
- signature: `interface MatchedEdit`
- members:
  - `editIndex` — [`L79`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L79)
  - `matchIndex` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L80)
  - `matchLength` — [`L81`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L81)
  - `newText` — [`L82`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L82)
- used by: [`applyEditsToNormalizedContent`](edit-diff.ts.md#applyEditsToNormalizedContent)

## Functions
- `applyEditsToNormalizedContent(normalizedContent: string, edits: Edit[], path: string)` — [`L193`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L193) — Apply one or more exact-text replacements to LF-normalized content.
- `computeEditDiff(path: string, oldText: string, newText: string, cwd: string)` — [`L441`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L441) — Compute the diff for a single edit operation without applying it.
- `computeEditsDiff(path: string, edits: Edit[], cwd: string)` — [`L406`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L406) — Compute the diff for one or more edit operations without applying them.
- `countOccurrences(content: string, oldText: string)` — [`L141`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L141)
- `detectLineEnding(content: string)` — [`L11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L11)
- `fuzzyFindText(content: string, oldText: string)` — [`L96`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L96) — Find oldText in content, trying exact match first, then fuzzy match.
- `generateDiffString(oldContent: string, newContent: string, contextLines?: number, startLine?: number)` — [`L266`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L266) — Generate a unified diff string with line numbers and context.
- `getDuplicateError(path: string, editIndex: number, totalEdits: number, occurrences: number)` — [`L158`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L158)
- `getEmptyOldTextError(path: string, editIndex: number, totalEdits: number)` — [`L169`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L169)
- `getNoChangeError(path: string, totalEdits: number)` — [`L176`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L176)
- `getNotFoundError(path: string, editIndex: number, totalEdits: number)` — [`L147`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L147)
- `normalizeForFuzzyMatch(text: string)` — [`L34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L34) — Normalize text for fuzzy matching. Applies progressive transformations:
- `normalizeToLF(text: string)` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L19)
- `restoreLineEndings(text: string, ending: "\n" | "\r\n")` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L23)
- `stripBom(content: string)` — [`L137`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L137) — Strip UTF-8 BOM if present, return both the BOM (if any) and the text without it

## Module values
- `bom` — [`L137`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L137)
- `diff` — [`L271`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L271)
- `firstChangedLine` — [`L271`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L271)
- `text` — [`L137`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit-diff.ts#L137)


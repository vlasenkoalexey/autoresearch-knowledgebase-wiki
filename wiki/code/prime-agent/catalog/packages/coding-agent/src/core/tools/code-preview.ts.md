---
title: 'Module: packages/coding-agent/src/core/tools/code-preview.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/tools/code-preview.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/tools/`code-preview.ts`/
symbols:
  previewBashCommand: previewBashCommand().
  pythonLineScore: pythonLineScore().
  previewPythonCode: previewPythonCode().
  previewHeredoc: previewHeredoc().
  previewIpythonCode: previewIpythonCode().
  CodePreview.language: CodePreview#language.
  descriptor: descriptor().
  pythonPreviewLine: pythonPreviewLine().
  CodePreview.text: CodePreview#text.
  firstPythonChildLine: firstPythonChildLine().
  isSkippableBashLine: isSkippableBashLine().
  simplifyPythonPreviewLine: simplifyPythonPreviewLine().
  pythonPreviewIndex: pythonPreviewIndex().
  simplifyBashCommandLine: simplifyBashCommandLine().
  stripBashPrefix: stripBashPrefix().
  isSkippablePythonLine: isSkippablePythonLine().
  pathTail: pathTail().
  simplifyRunnerCommand: simplifyRunnerCommand().
  simplifyMutationCommand: simplifyMutationCommand().
  bashLineScore: bashLineScore().
  pythonPathVars: pythonPathVars().
  CodePreview: CodePreview#
  pythonPrintInnerCall: pythonPrintInnerCall().
  pythonFileOperation: pythonFileOperation().
  pythonSubprocessCommand: pythonSubprocessCommand().
  truncateDescriptor: truncateDescriptor().
  PYTHON_DECORATOR_PATTERN: PYTHON_DECORATOR_PATTERN.
  PYTHON_CONTROL_PATTERN: PYTHON_CONTROL_PATTERN.
  PYTHON_CALL_PATTERN: PYTHON_CALL_PATTERN.
  shellWords: shellWords().
  PreviewCandidate.language: PreviewCandidate#language.
  DESCRIPTOR_MAX_WIDTH: DESCRIPTOR_MAX_WIDTH.
  COMMENT_LINE_PATTERN: COMMENT_LINE_PATTERN.
  PYTHON_DEFINITION_PATTERN: PYTHON_DEFINITION_PATTERN.
  PYTHON_LOW_SIGNAL_CALL_PATTERN: PYTHON_LOW_SIGNAL_CALL_PATTERN.
  CodePreviewLanguage: CodePreviewLanguage#
  pythonIndent: pythonIndent().
  MAGIC_LINE_PATTERN: MAGIC_LINE_PATTERN.
  CD_PREFIX_PATTERN: CD_PREFIX_PATTERN.
  BASH_SET_PATTERN: BASH_SET_PATTERN.
  BASH_SETUP_PATTERN: BASH_SETUP_PATTERN.
  PYTHON_IMPORT_PATTERN: PYTHON_IMPORT_PATTERN.
  PYTHON_MAIN_PATTERN: PYTHON_MAIN_PATTERN.
  PYTHON_ASSIGNMENT_CALL_PATTERN: PYTHON_ASSIGNMENT_CALL_PATTERN.
  PYTHON_LOW_SIGNAL_ASSIGNMENT_CALL_PATTERN: PYTHON_LOW_SIGNAL_ASSIGNMENT_CALL_PATTERN.
  PYTHON_EFFECT_CALL_PATTERN: PYTHON_EFFECT_CALL_PATTERN.
  HEREDOC_PATTERN: HEREDOC_PATTERN.
  PATH_ASSIGN_PATTERN: PATH_ASSIGN_PATTERN.
  STRING_ASSIGN_PATTERN: STRING_ASSIGN_PATTERN.
  PreviewCandidate: PreviewCandidate#
  PreviewCandidate.text: PreviewCandidate#text.
  PreviewCandidate.score: PreviewCandidate#score.
  collapseWhitespace: collapseWhitespace().
  redactNoise: redactNoise().
  splitCommandChain: splitCommandChain().
  heredocBody: heredocBody().
  PreviewCandidate.index: PreviewCandidate#index.
---
# Module: [`packages/coding-agent/src/core/tools/code-preview.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts)

## Classes
### `CodePreview`
- def: [`packages/coding-agent/src/core/tools/code-preview.ts:29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L29)
- signature: `interface CodePreview`
- members:
  - `language` — [`L30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L30)
  - `text` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L31)
- uses (calls/refs, reference-scoped): [`CodePreviewLanguage`](code-preview.ts.md#CodePreviewLanguage)
- used by: [`collapsedLine`](../../modes/interactive/components/ipython-cell.ts.md#IPythonCellComponent.collapsedLine), [`previewBashCommand`](code-preview.ts.md#previewBashCommand), [`previewPythonCode`](code-preview.ts.md#previewPythonCode), [`previewHeredoc`](code-preview.ts.md#previewHeredoc), [`formatBashCall`](bash.ts.md#formatBashCall), [`previewIpythonCode`](code-preview.ts.md#previewIpythonCode)

### `CodePreviewLanguage`
- def: [`packages/coding-agent/src/core/tools/code-preview.ts:27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L27)
- signature: `type CodePreviewLanguage`
- used by: [`language`](code-preview.ts.md#CodePreview.language), [`language`](code-preview.ts.md#PreviewCandidate.language)

### `PreviewCandidate`
- def: [`packages/coding-agent/src/core/tools/code-preview.ts:34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L34)
- signature: `interface PreviewCandidate`
- members:
  - `index` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L38)
  - `language` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L35)
  - `score` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L37)
  - `text` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L36)
- uses (calls/refs, reference-scoped): [`CodePreviewLanguage`](code-preview.ts.md#CodePreviewLanguage)
- used by: [`previewBashCommand`](code-preview.ts.md#previewBashCommand)

## Functions
- `bashLineScore(line: string, index: number)` — [`L218`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L218)
- `collapseWhitespace(text: string)` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L41)
- `descriptor(text: string)` — [`L64`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L64)
- `firstPythonChildLine(lines: readonly string[], parentIndex: number)` — [`L344`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L344)
- `heredocBody(lines: readonly string[], startIndex: number, delimiter: string)` — [`L160`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L160)
- `isSkippableBashLine(line: string)` — [`L72`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L72)
- `isSkippablePythonLine(line: string)` — [`L259`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L259)
- `pathTail(path: string)` — [`L91`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L91)
- `previewBashCommand(command: string)` — [`L229`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L229)
- `previewHeredoc(lines: readonly string[])` — [`L173`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L173)
- `previewIpythonCode(code: string)` — [`L436`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L436)
- `previewPythonCode(code: string)` — [`L412`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L412)
- `pythonFileOperation(line: string, paths: ReadonlyMap<string, string>)` — [`L286`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L286)
- `pythonIndent(line: string)` — [`L264`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L264)
- `pythonLineScore(lines: readonly string[], index: number, paths: ReadonlyMap<string, string>)` — [`L359`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L359)
- `pythonPathVars(lines: readonly string[])` — [`L275`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L275)
- `pythonPreviewIndex(lines: readonly string[], index: number)` — [`L403`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L403)
- `pythonPreviewLine(lines: readonly string[], index: number, paths: ReadonlyMap<string, string>)` — [`L327`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L327)
- `pythonPrintInnerCall(line: string)` — [`L269`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L269)
- `pythonSubprocessCommand(line: string)` — [`L309`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L309)
- `redactNoise(text: string)` — [`L52`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L52)
- `shellWords(line: string)` — [`L82`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L82)
- `simplifyBashCommandLine(line: string)` — [`L149`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L149)
- `simplifyMutationCommand(line: string)` — [`L132`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L132)
- `simplifyPythonPreviewLine(line: string, paths: ReadonlyMap<string, string>)` — [`L321`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L321)
- `simplifyRunnerCommand(line: string)` — [`L95`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L95)
- `splitCommandChain(line: string)` — [`L153`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L153)
- `stripBashPrefix(line: string)` — [`L68`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L68)
- `truncateDescriptor(text: string)` — [`L45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L45)

## Module values
- `BASH_SETUP_PATTERN` — [`L9`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L9)
- `BASH_SET_PATTERN` — [`L8`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L8)
- `CD_PREFIX_PATTERN` — [`L7`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L7)
- `COMMENT_LINE_PATTERN` — [`L6`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L6)
- `DESCRIPTOR_MAX_WIDTH` — [`L3`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L3)
- `HEREDOC_PATTERN` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L23)
- `MAGIC_LINE_PATTERN` — [`L5`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L5)
- `PATH_ASSIGN_PATTERN` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L24)
- `PYTHON_ASSIGNMENT_CALL_PATTERN` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L17)
- `PYTHON_CALL_PATTERN` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L15)
- `PYTHON_CONTROL_PATTERN` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L14)
- `PYTHON_DECORATOR_PATTERN` — [`L11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L11)
- `PYTHON_DEFINITION_PATTERN` — [`L12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L12)
- `PYTHON_EFFECT_CALL_PATTERN` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L21)
- `PYTHON_IMPORT_PATTERN` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L10)
- `PYTHON_LOW_SIGNAL_ASSIGNMENT_CALL_PATTERN` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L19)
- `PYTHON_LOW_SIGNAL_CALL_PATTERN` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L16)
- `PYTHON_MAIN_PATTERN` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L13)
- `STRING_ASSIGN_PATTERN` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/code-preview.ts#L25)


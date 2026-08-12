---
title: 'Module: packages/coding-agent/src/cli/file-processor.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/file-processor.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`file-processor.ts`/
symbols:
  processFileArguments: processFileArguments().
  ProcessedFiles.images: ProcessedFiles#images.
  ProcessedFiles: ProcessedFiles#
  ProcessedFiles.text: ProcessedFiles#text.
  ProcessFileOptions: ProcessFileOptions#
  ProcessFileOptions.autoResizeImages: ProcessFileOptions#autoResizeImages.
---
# Module: [`packages/coding-agent/src/cli/file-processor.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/file-processor.ts)

## Classes
### `ProcessFileOptions`
- def: [`packages/coding-agent/src/cli/file-processor.ts:18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/file-processor.ts#L18)
- signature: `interface ProcessFileOptions`
- members:
  - `autoResizeImages` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/file-processor.ts#L20) — Whether to auto-resize images to 2000x2000 max. Default: true
- used by: [`processFileArguments`](file-processor.ts.md#processFileArguments)

### `ProcessedFiles`
- def: [`packages/coding-agent/src/cli/file-processor.ts:13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/file-processor.ts#L13)
- signature: `interface ProcessedFiles`
- members:
  - `images` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/file-processor.ts#L15)
  - `text` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/file-processor.ts#L14)
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../ai/src/types.ts.md#ImageContent)
- used by: [`processFileArguments`](file-processor.ts.md#processFileArguments), [`initialImages`](../main.ts.md#prepareInitialMessage.Promise.typeLiteral38.initialImages)  (2 test-only)

## Functions
- `processFileArguments(fileArgs: string[], options?: ProcessFileOptions | undefined)` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/file-processor.ts#L24) — Process


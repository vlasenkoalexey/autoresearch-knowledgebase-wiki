---
title: 'Module: packages/coding-agent/src/utils/image-resize.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/utils/image-resize.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/utils/`image-resize.ts`/
symbols:
  resizeImage: resizeImage().
  formatDimensionNote: formatDimensionNote().
  DEFAULT_OPTIONS: DEFAULT_OPTIONS.
  encodeCandidate: encodeCandidate().
  ResizedImage.data: ResizedImage#data.
  ResizedImage.originalWidth: ResizedImage#originalWidth.
  ResizedImage.originalHeight: ResizedImage#originalHeight.
  ResizedImage.width: ResizedImage#width.
  ResizedImage.wasResized: ResizedImage#wasResized.
  ImageResizeOptions.maxWidth: ImageResizeOptions#maxWidth.
  ImageResizeOptions.maxHeight: ImageResizeOptions#maxHeight.
  ResizedImage.height: ResizedImage#height.
  ResizedImage.mimeType: ResizedImage#mimeType.
  ImageResizeOptions.maxBytes: ImageResizeOptions#maxBytes.
  EncodedCandidate: EncodedCandidate#
  ImageResizeOptions: ImageResizeOptions#
  ImageResizeOptions.jpegQuality: ImageResizeOptions#jpegQuality.
  ResizedImage: ResizedImage#
  EncodedCandidate.data: EncodedCandidate#data.
  EncodedCandidate.encodedSize: EncodedCandidate#encodedSize.
  EncodedCandidate.mimeType: EncodedCandidate#mimeType.
  DEFAULT_MAX_BYTES: DEFAULT_MAX_BYTES.
---
# Module: [`packages/coding-agent/src/utils/image-resize.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts)

## Classes
### `EncodedCandidate`
- def: [`packages/coding-agent/src/utils/image-resize.ts:32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L32)
- signature: `interface EncodedCandidate`
- members:
  - `data` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L33)
  - `encodedSize` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L34)
  - `mimeType` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L35)
- used by: [`resizeImage`](image-resize.ts.md#resizeImage), [`encodeCandidate`](image-resize.ts.md#encodeCandidate)

### `ImageResizeOptions`
- def: [`packages/coding-agent/src/utils/image-resize.ts:5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L5)
- signature: `interface ImageResizeOptions`
- members:
  - `jpegQuality` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L9)
  - `maxBytes` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L8)
  - `maxHeight` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L7)
  - `maxWidth` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L6)
- used by: [`resizeImage`](image-resize.ts.md#resizeImage), [`DEFAULT_OPTIONS`](image-resize.ts.md#DEFAULT_OPTIONS)

### `ResizedImage`
- def: [`packages/coding-agent/src/utils/image-resize.ts:12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L12)
- signature: `interface ResizedImage`
- members:
  - `data` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L13)
  - `height` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L18)
  - `mimeType` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L14)
  - `originalHeight` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L16)
  - `originalWidth` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L15)
  - `wasResized` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L19)
  - `width` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L17)
- used by: [`resizeImage`](image-resize.ts.md#resizeImage), [`handleClipboardImagePaste`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleClipboardImagePaste), [`processFileArguments`](../cli/file-processor.ts.md#processFileArguments), [`formatDimensionNote`](image-resize.ts.md#formatDimensionNote)  (1 test-only)

## Functions
- `encodeCandidate(buffer: Uint8Array<ArrayBufferLike>, mimeType: string)` — [`L38`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L38)
- `formatDimensionNote(result: ResizedImage)` — [`L169`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L169) — Format a dimension note for resized images.
- `resizeImage(img: ImageContent, options?: ImageResizeOptions | undefined)` — [`L60`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L60) — Resize an image to fit within the specified max dimensions and encoded file size.

## Module values
- `DEFAULT_MAX_BYTES` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L23)
- `DEFAULT_OPTIONS` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/image-resize.ts#L25)


---
title: 'Module: packages/coding-agent/src/utils/exif-orientation.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/utils/exif-orientation.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/utils/`exif-orientation.ts`/
symbols:
  applyExifOrientation: applyExifOrientation().
  rotate90: rotate90().
  getExifOrientation: getExifOrientation().
  findJpegTiffOffset: findJpegTiffOffset().
  findWebpTiffOffset: findWebpTiffOffset().
  Photon: Photon#
  hasExifHeader: hasExifHeader().
  readOrientationFromTiff: readOrientationFromTiff().
  DstIndexFn: DstIndexFn#
---
# Module: [`packages/coding-agent/src/utils/exif-orientation.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/exif-orientation.ts)

## Classes
### `DstIndexFn`
- def: [`packages/coding-agent/src/utils/exif-orientation.ts:124`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/exif-orientation.ts#L124)
- signature: `type DstIndexFn`
- used by: [`rotate90`](exif-orientation.ts.md#rotate90)

### `Photon`
- def: [`packages/coding-agent/src/utils/exif-orientation.ts:3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/exif-orientation.ts#L3)
- signature: `type Photon`
- used by: [`applyExifOrientation`](exif-orientation.ts.md#applyExifOrientation), [`rotate90`](exif-orientation.ts.md#rotate90)

## Functions
- `applyExifOrientation(photon: typeof import("/node_modules/@silvia-odwyer/photon-node/photon_rs"), image: PhotonImage, originalBytes: Uint8Array<...>)` — [`L147`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/exif-orientation.ts#L147)
- `findJpegTiffOffset(bytes: Uint8Array<ArrayBufferLike>)` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/exif-orientation.ts#L39)
- `findWebpTiffOffset(bytes: Uint8Array<ArrayBufferLike>)` — [`L65`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/exif-orientation.ts#L65)
- `getExifOrientation(bytes: Uint8Array<ArrayBufferLike>)` — [`L98`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/exif-orientation.ts#L98)
- `hasExifHeader(bytes: Uint8Array<ArrayBufferLike>, offset: number)` — [`L87`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/exif-orientation.ts#L87)
- `readOrientationFromTiff(bytes: Uint8Array<ArrayBufferLike>, tiffStart: number)` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/exif-orientation.ts#L5)
- `rotate90(photon: typeof import("/node_modules/@silvia-odwyer/photon-node/photon_rs"), image: PhotonImage, dstIndex: DstIndexFn)` — [`L126`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/exif-orientation.ts#L126)


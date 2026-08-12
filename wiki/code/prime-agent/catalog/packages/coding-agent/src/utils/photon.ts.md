---
title: 'Module: packages/coding-agent/src/utils/photon.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/utils/photon.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/utils/`photon.ts`/
symbols:
  patchPhotonWasmRead: patchPhotonWasmRead().
  loadPhoton: loadPhoton().
  fs: fs.
  ReadFileSync: ReadFileSync#
  photonModule: photonModule.
  WASM_FILENAME: WASM_FILENAME.
  loadPromise: loadPromise.
  getFallbackWasmPaths: getFallbackWasmPaths().
  require: require.
  pathOrNull: pathOrNull().
---
# Module: [`packages/coding-agent/src/utils/photon.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/photon.ts)

## Classes
### `ReadFileSync`
- def: [`packages/coding-agent/src/utils/photon.ts:27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/photon.ts#L27)
- signature: `type ReadFileSync`
- uses (calls/refs, reference-scoped): [`fs`](photon.ts.md#fs)
- used by: [`patchPhotonWasmRead`](photon.ts.md#patchPhotonWasmRead)

## Functions
- `getFallbackWasmPaths()` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/photon.ts#L45)
- `loadPhoton()` — [`L116`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/photon.ts#L116) — Load the photon module asynchronously.
- `patchPhotonWasmRead()` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/photon.ts#L54)
- `pathOrNull(file: PathOrFileDescriptor)` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/photon.ts#L35)

## Module values
- `WASM_FILENAME` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/photon.ts#L29)
- `fs` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/photon.ts#L22)
- `loadPromise` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/photon.ts#L33)
- `photonModule` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/photon.ts#L32)
- `require` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/photon.ts#L21)


---
title: 'Module: packages/coding-agent/src/core/tools/output-accumulator.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/tools/output-accumulator.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/tools/`output-accumulator.ts`/
symbols:
  OutputAccumulator.snapshot: OutputAccumulator#snapshot().
  OutputAccumulator.-constructor: OutputAccumulator#`<constructor>`().
  OutputAccumulator.appendDecodedText: OutputAccumulator#appendDecodedText().
  OutputAccumulator.append: OutputAccumulator#append().
  OutputAccumulator.ensureTempFile: OutputAccumulator#ensureTempFile().
  OutputAccumulator.shouldUseTempFile: OutputAccumulator#shouldUseTempFile().
  OutputAccumulator.finish: OutputAccumulator#finish().
  OutputAccumulator.trimTail: OutputAccumulator#trimTail().
  OutputAccumulator.maxBytes: OutputAccumulator#maxBytes.
  OutputAccumulator.tailText: OutputAccumulator#tailText.
  OutputAccumulator.tempFileStream: OutputAccumulator#tempFileStream.
  OutputSnapshot.truncation: OutputSnapshot#truncation.
  OutputSnapshot.fullOutputPath: OutputSnapshot#fullOutputPath.
  OutputAccumulator.getSnapshotText: OutputAccumulator#getSnapshotText().
  OutputAccumulator.maxLines: OutputAccumulator#maxLines.
  OutputAccumulator.totalDecodedBytes: OutputAccumulator#totalDecodedBytes.
  OutputAccumulator.maxRollingBytes: OutputAccumulator#maxRollingBytes.
  OutputAccumulator.tailBytes: OutputAccumulator#tailBytes.
  OutputAccumulator.totalLines: OutputAccumulator#totalLines.
  OutputAccumulator.tempFilePath: OutputAccumulator#tempFilePath.
  OutputAccumulator.closeTempFile: OutputAccumulator#closeTempFile().
  OutputAccumulator.getLastLineBytes: OutputAccumulator#getLastLineBytes().
  OutputSnapshot.content: OutputSnapshot#content.
  byteLength: byteLength().
  OutputAccumulator.rawChunks: OutputAccumulator#rawChunks.
  OutputAccumulator.tailStartsAtLineBoundary: OutputAccumulator#tailStartsAtLineBoundary.
  OutputAccumulator.currentLineBytes: OutputAccumulator#currentLineBytes.
  OutputAccumulator.finished: OutputAccumulator#finished.
  OutputAccumulator.tempFilePrefix: OutputAccumulator#tempFilePrefix.
  OutputAccumulator.decoder: OutputAccumulator#decoder.
  OutputAccumulator.totalRawBytes: OutputAccumulator#totalRawBytes.
  OutputAccumulatorOptions: OutputAccumulatorOptions#
  OutputAccumulatorOptions.maxLines: OutputAccumulatorOptions#maxLines.
  OutputAccumulatorOptions.maxBytes: OutputAccumulatorOptions#maxBytes.
  OutputAccumulatorOptions.tempFilePrefix: OutputAccumulatorOptions#tempFilePrefix.
  OutputSnapshot: OutputSnapshot#
  defaultTempFilePath: defaultTempFilePath().
  OutputAccumulator: OutputAccumulator#
  OutputAccumulator.snapshot.options-typeLiteral3.persistIfTruncated: OutputAccumulator#snapshot().(options)typeLiteral3:persistIfTruncated.
---
# Module: [`packages/coding-agent/src/core/tools/output-accumulator.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts)

## Classes
### `OutputAccumulator`
- def: [`packages/coding-agent/src/core/tools/output-accumulator.ts:35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L35)
- doc: Incrementally tracks streaming output with bounded memory.
- signature: `class OutputAccumulator`
- members:
  - `<constructor>(options?: OutputAccumulatorOptions)` — [`L55`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L55) — Incrementally tracks streaming output with bounded memory.
  - `append(method)` — [`L62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L62)
  - `appendDecodedText(method)` — [`L146`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L146)
  - `closeTempFile(method)` — [`L119`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L119)
  - `ensureTempFile(method)` — [`L205`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L205)
  - `finish(method)` — [`L78`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L78)
  - `getLastLineBytes(method)` — [`L142`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L142)
  - `getSnapshotText(method)` — [`L190`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L190)
  - `shouldUseTempFile(method)` — [`L199`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L199)
  - `snapshot(method)` — [`L89`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L89)
  - `trimTail(method)` — [`L173`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L173)
  - `currentLineBytes` — [`L49`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L49)
  - `decoder` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L40)
  - `finished` — [`L50`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L50)
  - `maxBytes` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L37)
  - `maxLines` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L36)
  - `maxRollingBytes` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L38)
  - `persistIfTruncated` — [`L89`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L89)
  - `rawChunks` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L42)
  - `tailBytes` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L44)
  - `tailStartsAtLineBoundary` — [`L45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L45)
  - `tailText` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L43)
  - `tempFilePath` — [`L52`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L52)
  - `tempFilePrefix` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L39)
  - `tempFileStream` — [`L53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L53)
  - `totalDecodedBytes` — [`L47`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L47)
  - `totalLines` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L48)
  - `totalRawBytes` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L46)
- uses (calls/refs, reference-scoped): [`truncateTail`](truncate.ts.md#truncateTail), [`truncated`](truncate.ts.md#TruncationResult.truncated), [`DEFAULT_MAX_BYTES`](truncate.ts.md#DEFAULT_MAX_BYTES), [`TruncationResult`](truncate.ts.md#TruncationResult), [`DEFAULT_MAX_LINES`](truncate.ts.md#DEFAULT_MAX_LINES), [`totalLines`](truncate.ts.md#TruncationResult.totalLines), [`content`](truncate.ts.md#TruncationResult.content), [`truncatedBy`](truncate.ts.md#TruncationResult.truncatedBy), [`totalBytes`](truncate.ts.md#TruncationResult.totalBytes), [`maxBytes`](truncate.ts.md#TruncationResult.maxBytes), [`truncation`](output-accumulator.ts.md#OutputSnapshot.truncation), [`fullOutputPath`](output-accumulator.ts.md#OutputSnapshot.fullOutputPath), [`maxLines`](truncate.ts.md#TruncationResult.maxLines), [`byteLength`](output-accumulator.ts.md#byteLength), [`content`](output-accumulator.ts.md#OutputSnapshot.content), [`OutputAccumulatorOptions`](output-accumulator.ts.md#OutputAccumulatorOptions), [`OutputSnapshot`](output-accumulator.ts.md#OutputSnapshot), [`defaultTempFilePath`](output-accumulator.ts.md#defaultTempFilePath), [`maxBytes`](output-accumulator.ts.md#OutputAccumulatorOptions.maxBytes), [`maxLines`](output-accumulator.ts.md#OutputAccumulatorOptions.maxLines), [`tempFilePrefix`](output-accumulator.ts.md#OutputAccumulatorOptions.tempFilePrefix)
- used by: [`createBashToolDefinition`](bash.ts.md#createBashToolDefinition), [`bash.ts`](bash.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-bash.ts)

### `OutputAccumulatorOptions`
- def: [`packages/coding-agent/src/core/tools/output-accumulator.ts:7`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L7)
- signature: `interface OutputAccumulatorOptions`
- members:
  - `maxBytes` — [`L9`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L9)
  - `maxLines` — [`L8`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L8)
  - `tempFilePrefix` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L10)
- used by: [`<constructor>`](output-accumulator.ts.md#OutputAccumulator.-constructor)

### `OutputSnapshot`
- def: [`packages/coding-agent/src/core/tools/output-accumulator.ts:13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L13)
- signature: `interface OutputSnapshot`
- members:
  - `content` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L14)
  - `fullOutputPath` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L16)
  - `truncation` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L15)
- uses (calls/refs, reference-scoped): [`TruncationResult`](truncate.ts.md#TruncationResult)
- used by: [`createBashToolDefinition`](bash.ts.md#createBashToolDefinition), [`snapshot`](output-accumulator.ts.md#OutputAccumulator.snapshot)

## Functions
- `byteLength(text: string)` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L24)
- `defaultTempFilePath(prefix: string)` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/output-accumulator.ts#L19)


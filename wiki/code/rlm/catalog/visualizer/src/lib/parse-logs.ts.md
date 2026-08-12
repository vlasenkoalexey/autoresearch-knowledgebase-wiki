---
title: 'Module: visualizer/src/lib/parse-logs.ts'
type: catalog
provenance: extracted
module: visualizer/src/lib/parse-logs.ts
status: fresh
symbol_base: scip-typescript npm visualizer 0.1.0 src/lib/`parse-logs.ts`/
symbols:
  computeMetadata: computeMetadata().
  parseJSONL: parseJSONL().
  parseLogFile: parseLogFile().
  getDefaultConfig: getDefaultConfig().
  extractContextQuestion: extractContextQuestion().
  extractContextVariable: extractContextVariable().
  ParsedJSONL.iterations: ParsedJSONL#iterations.
  ParsedJSONL: ParsedJSONL#
  ParsedJSONL.config: ParsedJSONL#config.
---
# Module: [`visualizer/src/lib/parse-logs.ts`](../../../../../../../raw/code/rlm/visualizer/src/lib/parse-logs.ts)

## Classes
### `ParsedJSONL`
- def: [`visualizer/src/lib/parse-logs.ts:32`](../../../../../../../raw/code/rlm/visualizer/src/lib/parse-logs.ts#L32)
- signature: `interface ParsedJSONL`
- members:
  - `config` — [`L34`](../../../../../../../raw/code/rlm/visualizer/src/lib/parse-logs.ts#L34)
  - `iterations` — [`L33`](../../../../../../../raw/code/rlm/visualizer/src/lib/parse-logs.ts#L33)
- uses (calls/refs, reference-scoped): [`RLMIteration`](types.ts.md#RLMIteration), [`RLMConfigMetadata`](types.ts.md#RLMConfigMetadata)
- used by: [`parseJSONL`](parse-logs.ts.md#parseJSONL), [`parseLogFile`](parse-logs.ts.md#parseLogFile)

## Functions
- `computeMetadata(iterations: RLMIteration[])` — [`L121`](../../../../../../../raw/code/rlm/visualizer/src/lib/parse-logs.ts#L121) — documented in [visualizer-src-lib-types.ts](../../../../concepts/visualizer-src-lib-types.ts.md)
- `extractContextQuestion(iterations: RLMIteration[])` — [`L70`](../../../../../../../raw/code/rlm/visualizer/src/lib/parse-logs.ts#L70) — documented in [visualizer-src-lib-types.ts](../../../../concepts/visualizer-src-lib-types.ts.md)
- `extractContextVariable(iterations: RLMIteration[])` — [`L4`](../../../../../../../raw/code/rlm/visualizer/src/lib/parse-logs.ts#L4)
- `getDefaultConfig()` — [`L19`](../../../../../../../raw/code/rlm/visualizer/src/lib/parse-logs.ts#L19)
- `parseJSONL(content: string)` — [`L37`](../../../../../../../raw/code/rlm/visualizer/src/lib/parse-logs.ts#L37) — documented in [visualizer-src-lib-types.ts](../../../../concepts/visualizer-src-lib-types.ts.md)
- `parseLogFile(fileName: string, content: string)` — [`L169`](../../../../../../../raw/code/rlm/visualizer/src/lib/parse-logs.ts#L169)


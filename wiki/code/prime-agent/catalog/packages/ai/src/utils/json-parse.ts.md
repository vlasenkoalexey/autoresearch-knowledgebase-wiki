---
title: 'Module: packages/ai/src/utils/json-parse.ts'
type: catalog
provenance: extracted
module: packages/ai/src/utils/json-parse.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/utils/`json-parse.ts`/
symbols:
  parseStreamingJson: parseStreamingJson().
  repairJson: repairJson().
  parseJsonWithRepair: parseJsonWithRepair().
  VALID_JSON_ESCAPES: VALID_JSON_ESCAPES.
  isControlCharacter: isControlCharacter().
  escapeControlCharacter: escapeControlCharacter().
---
# Module: [`packages/ai/src/utils/json-parse.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/json-parse.ts)

## Functions
- `escapeControlCharacter(char: string)` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/json-parse.ts#L10)
- `isControlCharacter(char: string)` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/json-parse.ts#L5)
- `parseJsonWithRepair(json: string)` — [`L85`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/json-parse.ts#L85)
- `parseStreamingJson(partialJson: string | undefined)` — [`L104`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/json-parse.ts#L104) — Attempts to parse potentially incomplete JSON during streaming.
- `repairJson(json: string)` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/json-parse.ts#L32) — Repairs malformed JSON string literals by:

## Module values
- `VALID_JSON_ESCAPES` — [`L3`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/json-parse.ts#L3)


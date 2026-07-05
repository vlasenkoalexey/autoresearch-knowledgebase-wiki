---
title: 'Module: extensions/pi-autoresearch-vkf/frontmatter.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/frontmatter.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`frontmatter.ts`/
symbols:
  YamlValue: YamlValue#
  parseBlockMap: parseBlockMap().
  parseBlockList: parseBlockList().
  parseFrontmatter: parseFrontmatter().
  assembleCard: assembleCard().
  parseScalarOrFlow: parseScalarOrFlow().
  emit: emit().
  scalarStr: scalarStr().
  FENCE: FENCE.
  Cursor.value: Cursor#value.
  stringifyFrontmatter: stringifyFrontmatter().
  indentOf: indentOf.
  ParsedCard.data: ParsedCard#data.
  parseScalar: parseScalar().
  Cursor.next: Cursor#next.
  ParsedCard.body: ParsedCard#body.
  Cursor: Cursor#
  findKeyColon: findKeyColon().
  ParsedCard: ParsedCard#
  stripStructuralComments: stripStructuralComments().
  splitFlow: splitFlow().
---
# Module: [`extensions/pi-autoresearch-vkf/frontmatter.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts)

## Classes
### `Cursor`
- def: [`extensions/pi-autoresearch-vkf/frontmatter.ts:68`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L68) — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
- signature: `interface Cursor`
- members:
  - `next` — [`L71`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L71) — Index of the first line not consumed by this block. — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
  - `value` — [`L69`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L69) — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
- used by: [`parseBlockMap`](frontmatter.ts.md#parseBlockMap), [`parseBlockList`](frontmatter.ts.md#parseBlockList), [`parseFrontmatter`](frontmatter.ts.md#parseFrontmatter)

### `ParsedCard`
- def: [`extensions/pi-autoresearch-vkf/frontmatter.ts:24`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L24) — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
- signature: `interface ParsedCard`
- members:
  - `body` — [`L28`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L28) — Everything after the closing `---`, verbatim. — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
  - `data` — [`L26`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L26) — Parsed frontmatter mapping. — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
- uses (calls/refs, reference-scoped): [`YamlValue`](frontmatter.ts.md#YamlValue)
- used by: [`readCardFile`](cards.ts.md#readCardFile), [`parseFrontmatter`](frontmatter.ts.md#parseFrontmatter)

### `YamlValue`
- def: [`extensions/pi-autoresearch-vkf/frontmatter.ts:16`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L16) — documented in [extensions-pi-autoresearch-vkf-cards.ts](../../../concepts/extensions-pi-autoresearch-vkf-cards.ts.md)
- doc: A small YAML-frontmatter reader/writer for VKF cards.
- signature: `type YamlValue`
- used by: [`meta`](cards.ts.md#Card.meta), [`buildExperimentCard`](cards.ts.md#buildExperimentCard), [`losses`](cards.ts.md#transitionCard.opts-typeLiteral158.evidence.typeLiteral159.losses), [`confidence`](cards.ts.md#baseFrontmatter.args-typeLiteral28.confidence), [`writeTransaction`](cards.ts.md#writeTransaction), [`cards.ts`](cards.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-cards.ts), [`parseBlockMap`](frontmatter.ts.md#parseBlockMap), [`parseBlockList`](frontmatter.ts.md#parseBlockList), [`assembleCard`](frontmatter.ts.md#assembleCard), [`parseScalarOrFlow`](frontmatter.ts.md#parseScalarOrFlow), [`emit`](frontmatter.ts.md#emit), [`scalarStr`](frontmatter.ts.md#scalarStr), [`stringifyFrontmatter`](frontmatter.ts.md#stringifyFrontmatter), [`data`](frontmatter.ts.md#ParsedCard.data), [`parseScalar`](frontmatter.ts.md#parseScalar)

## Functions
- `assembleCard(data: Record<string, YamlValue>, body: string)` — [`L268`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L268) — Assemble a complete card: `--- <frontmatter> --- <body>`. — documented in [extensions-pi-autoresearch-vkf-cards.ts](../../../concepts/extensions-pi-autoresearch-vkf-cards.ts.md)
- `emit(key: string, value: YamlValue, indent: number)` — [`L217`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L217) — Emit a value as canonical block YAML at the given indent level. — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
- `findKeyColon(s: string)` — [`L159`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L159) — Locate the colon that separates a key from its value (ignores `://` in URLs). — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
- `parseBlockList(lines: string[], indent: number, start: number)` — [`L118`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L118) — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
- `parseBlockMap(lines: string[], indent: number, start?: number)` — [`L74`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L74) — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
- `parseFrontmatter(text: string)` — [`L34`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L34) — Split a card into `{ data, body }`. Throws if no frontmatter fence is found. — documented in [extensions-pi-autoresearch-vkf-cards.ts](../../../concepts/extensions-pi-autoresearch-vkf-cards.ts.md)
- `parseScalar(s: string)` — [`L201`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L201) — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
- `parseScalarOrFlow(raw: string)` — [`L166`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L166) — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
- `scalarStr(value: YamlValue)` — [`L245`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L245) — Render a scalar, quoting when needed to stay valid YAML. — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
- `splitFlow(inner: string)` — [`L176`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L176) — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
- `stringifyFrontmatter(data: Record<string, YamlValue>)` — [`L261`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L261) — Serialize a frontmatter mapping to canonical block YAML (no fences). — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
- `stripStructuralComments(lines: string[])` — [`L59`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L59) — Drop blank lines and full-line comments; keep everything else verbatim. — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)

## Module values
- `FENCE` — [`L31`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L31) — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)
- `indentOf` — [`L66`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/frontmatter.ts#L66) — documented in [extensions-pi-autoresearch-vkf-frontmatter.ts](../../../concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md)


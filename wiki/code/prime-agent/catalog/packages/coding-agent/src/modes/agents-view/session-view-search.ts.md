---
title: 'Module: packages/coding-agent/src/modes/agents-view/session-view-search.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/agents-view/session-view-search.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/agents-view/`session-view-search.ts`/
symbols:
  matchSearchText: matchSearchText().
  matchesSearchText: matchesSearchText().
  parseSearchQuery: parseSearchQuery().
  ParsedSearchQuery.tokens: ParsedSearchQuery#tokens.
  ParsedSearchQuery.regex: ParsedSearchQuery#regex.
  MatchResult.matches: MatchResult#matches.
  ParsedSearchQuery.mode: ParsedSearchQuery#mode.
  MatchResult.score: MatchResult#score.
  ParsedSearchQuery.error: ParsedSearchQuery#error.
  createSessionSearchText: createSessionSearchText().
  ParsedSearchQuery: ParsedSearchQuery#
  normalizeWhitespaceLower: normalizeWhitespaceLower().
  MatchResult: MatchResult#
  STRICT_FUZZY_MAX_TOKEN_SCORE: STRICT_FUZZY_MAX_TOKEN_SCORE.
---
# Module: [`packages/coding-agent/src/modes/agents-view/session-view-search.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agents-view/session-view-search.ts)

## Classes
### `MatchResult`
- def: [`packages/coding-agent/src/modes/agents-view/session-view-search.ts:10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agents-view/session-view-search.ts#L10)
- signature: `interface MatchResult`
- members:
  - `matches` — [`L11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agents-view/session-view-search.ts#L11)
  - `score` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agents-view/session-view-search.ts#L13) — Lower is better; only meaningful when matches === true
- used by: [`matchSearchText`](session-view-search.ts.md#matchSearchText), [`matchesSearchText`](session-view-search.ts.md#matchesSearchText)

### `ParsedSearchQuery`
- def: [`packages/coding-agent/src/modes/agents-view/session-view-search.ts:2`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agents-view/session-view-search.ts#L2)
- signature: `interface ParsedSearchQuery`
- members:
  - `error` — [`L7`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agents-view/session-view-search.ts#L7) — If set, parsing failed and we should treat query as non-matching.
  - `mode` — [`L3`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agents-view/session-view-search.ts#L3)
  - `regex` — [`L5`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agents-view/session-view-search.ts#L5)
  - `tokens` — [`L4`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agents-view/session-view-search.ts#L4)
- used by: [`matchSearchText`](session-view-search.ts.md#matchSearchText), [`matchesSearchText`](session-view-search.ts.md#matchesSearchText), [`parseSearchQuery`](session-view-search.ts.md#parseSearchQuery)

## Functions
- `createSessionSearchText(parts: readonly (string | null | undefined)[])` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agents-view/session-view-search.ts#L21) — Join arbitrary session fields into the common search corpus.
- `matchSearchText(text: string, parsed: ParsedSearchQuery)` — [`L105`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agents-view/session-view-search.ts#L105) — Match any precomputed search corpus using the resume picker's query language.
- `matchesSearchText(text: string, query: string)` — [`L139`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agents-view/session-view-search.ts#L139)
- `normalizeWhitespaceLower(text: string)` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agents-view/session-view-search.ts#L16)
- `parseSearchQuery(query: string)` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agents-view/session-view-search.ts#L25)

## Module values
- `STRICT_FUZZY_MAX_TOKEN_SCORE` — [`L102`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agents-view/session-view-search.ts#L102)


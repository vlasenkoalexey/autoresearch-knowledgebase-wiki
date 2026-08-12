---
title: 'Module: packages/ai/src/utils/overflow.ts'
type: catalog
provenance: extracted
module: packages/ai/src/utils/overflow.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/utils/`overflow.ts`/
symbols:
  isContextOverflow: isContextOverflow().
  getOverflowPatterns: getOverflowPatterns().
  OVERFLOW_PATTERNS: OVERFLOW_PATTERNS.
  NON_OVERFLOW_PATTERNS: NON_OVERFLOW_PATTERNS.
---
# Module: [`packages/ai/src/utils/overflow.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/overflow.ts)

## Functions
- `getOverflowPatterns()` — [`L151`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/overflow.ts#L151) — Get the overflow patterns for testing purposes.
- `isContextOverflow(message: AssistantMessage, contextWindow?: number | undefined)` — [`L117`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/overflow.ts#L117) — Check if an assistant message represents a context overflow error.

## Module values
- `NON_OVERFLOW_PATTERNS` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/overflow.ts#L63) — Patterns that indicate non-overflow errors (e.g. rate limiting, server errors).
- `OVERFLOW_PATTERNS` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/overflow.ts#L31) — Regex patterns to detect context overflow errors from different providers.


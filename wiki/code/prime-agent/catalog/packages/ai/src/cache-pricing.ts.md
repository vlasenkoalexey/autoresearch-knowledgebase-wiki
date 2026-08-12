---
title: 'Module: packages/ai/src/cache-pricing.ts'
type: catalog
provenance: extracted
module: packages/ai/src/cache-pricing.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/`cache-pricing.ts`/
symbols:
  getAnthropicCacheWriteCost: getAnthropicCacheWriteCost().
  hasStandardAnthropicCachePricing: hasStandardAnthropicCachePricing().
  getAnthropicCacheCosts.typeLiteral12.cacheWrite: getAnthropicCacheCosts().typeLiteral12:cacheWrite.
  getAnthropicCacheCosts: getAnthropicCacheCosts().
  ANTHROPIC_FIVE_MINUTE_CACHE_WRITE_COST_MULTIPLIER: ANTHROPIC_FIVE_MINUTE_CACHE_WRITE_COST_MULTIPLIER.
  AnthropicCacheDuration: AnthropicCacheDuration#
  ANTHROPIC_ONE_HOUR_CACHE_WRITE_COST_MULTIPLIER: ANTHROPIC_ONE_HOUR_CACHE_WRITE_COST_MULTIPLIER.
  AnthropicCacheCreationUsage: AnthropicCacheCreationUsage#
  AnthropicCacheCreationUsage.ephemeral_5m_input_tokens: AnthropicCacheCreationUsage#ephemeral_5m_input_tokens.
  AnthropicCacheCreationUsage.ephemeral_1h_input_tokens: AnthropicCacheCreationUsage#ephemeral_1h_input_tokens.
  ANTHROPIC_CACHE_READ_COST_MULTIPLIER: ANTHROPIC_CACHE_READ_COST_MULTIPLIER.
  getAnthropicCacheCosts.typeLiteral12.cacheRead: getAnthropicCacheCosts().typeLiteral12:cacheRead.
---
# Module: [`packages/ai/src/cache-pricing.ts`](../../../../../../../raw/code/prime-agent/packages/ai/src/cache-pricing.ts)

## Classes
### `AnthropicCacheCreationUsage`
- def: [`packages/ai/src/cache-pricing.ts:5`](../../../../../../../raw/code/prime-agent/packages/ai/src/cache-pricing.ts#L5)
- signature: `interface AnthropicCacheCreationUsage`
- members:
  - `ephemeral_1h_input_tokens` — [`L7`](../../../../../../../raw/code/prime-agent/packages/ai/src/cache-pricing.ts#L7)
  - `ephemeral_5m_input_tokens` — [`L6`](../../../../../../../raw/code/prime-agent/packages/ai/src/cache-pricing.ts#L6)
- used by: [`getAnthropicCacheWriteCost`](cache-pricing.ts.md#getAnthropicCacheWriteCost)

### `AnthropicCacheDuration`
- def: [`packages/ai/src/cache-pricing.ts:3`](../../../../../../../raw/code/prime-agent/packages/ai/src/cache-pricing.ts#L3)
- signature: `type AnthropicCacheDuration`
- used by: [`getAnthropicCacheWriteCost`](cache-pricing.ts.md#getAnthropicCacheWriteCost), [`getAnthropicCacheCosts`](cache-pricing.ts.md#getAnthropicCacheCosts)

## Functions
- `getAnthropicCacheCosts(inputCost: number, duration: AnthropicCacheDuration)` — [`L27`](../../../../../../../raw/code/prime-agent/packages/ai/src/cache-pricing.ts#L27)
- `getAnthropicCacheWriteCost(inputCost: number, duration: AnthropicCacheDuration, cacheCreation?: AnthropicCacheCreationUsage | null | undefined)` — [`L41`](../../../../../../../raw/code/prime-agent/packages/ai/src/cache-pricing.ts#L41)
- `hasStandardAnthropicCachePricing(model: Model<TApi>)` — [`L14`](../../../../../../../raw/code/prime-agent/packages/ai/src/cache-pricing.ts#L14)

## Module values
- `ANTHROPIC_CACHE_READ_COST_MULTIPLIER` — [`L10`](../../../../../../../raw/code/prime-agent/packages/ai/src/cache-pricing.ts#L10)
- `ANTHROPIC_FIVE_MINUTE_CACHE_WRITE_COST_MULTIPLIER` — [`L11`](../../../../../../../raw/code/prime-agent/packages/ai/src/cache-pricing.ts#L11)
- `ANTHROPIC_ONE_HOUR_CACHE_WRITE_COST_MULTIPLIER` — [`L12`](../../../../../../../raw/code/prime-agent/packages/ai/src/cache-pricing.ts#L12)
- `cacheRead` — [`L30`](../../../../../../../raw/code/prime-agent/packages/ai/src/cache-pricing.ts#L30)
- `cacheWrite` — [`L30`](../../../../../../../raw/code/prime-agent/packages/ai/src/cache-pricing.ts#L30)


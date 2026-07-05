---
title: 'Module: extensions/pi-autoresearch-vkf/context_prune.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/context_prune.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`context_prune.ts`/
symbols:
  pruneContext: pruneContext().
  textParts: textParts.
  isPruned: isPruned.
  DEFAULTS: DEFAULTS.
  textChars: textChars.
  PrunableMessage: PrunableMessage#
  TextPart: TextPart#
  pruneContext.typeLiteral17.pruned: pruneContext().typeLiteral17:pruned.
  PRUNE_STUB: PRUNE_STUB.
  PrunableMessage.role: PrunableMessage#role.
  PrunableMessage.content: PrunableMessage#content.
  TextPart.text: TextPart#text.
  pruneContext.typeLiteral17.savedChars: pruneContext().typeLiteral17:savedChars.
  PrunableMessage.toolName: PrunableMessage#toolName.
  PruneOptions: PruneOptions#
  PruneOptions.thresholdChars: PruneOptions#thresholdChars.
  PruneOptions.keepRecentTurns: PruneOptions#keepRecentTurns.
  PruneOptions.minSavingsChars: PruneOptions#minSavingsChars.
  CHATTY_TOOLS: CHATTY_TOOLS.
  TextPart.type: TextPart#type.
---
# Module: [`extensions/pi-autoresearch-vkf/context_prune.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts)

## Classes
### `PrunableMessage`
- def: [`extensions/pi-autoresearch-vkf/context_prune.ts:32`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L32) — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
- doc: Structural slice of pi's AgentMessage that pruning needs.
- signature: `interface PrunableMessage`
- members:
  - `content` — [`L35`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L35) — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
  - `role` — [`L33`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L33)
  - `toolName` — [`L34`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L34) — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
- used by: [`pruneContext`](context_prune.ts.md#pruneContext), [`textParts`](context_prune.ts.md#textParts), [`isPruned`](context_prune.ts.md#isPruned), [`textChars`](context_prune.ts.md#textChars)

### `PruneOptions`
- def: [`extensions/pi-autoresearch-vkf/context_prune.ts:43`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L43) — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
- signature: `interface PruneOptions`
- members:
  - `keepRecentTurns` — [`L47`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L47) — Results within this many assistant turns of the end are kept. — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
  - `minSavingsChars` — [`L49`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L49) — Skip the batch unless it reclaims at least this much (cache-churn guard). — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
  - `thresholdChars` — [`L45`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L45) — Only prune when tool-result text in context exceeds this. — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
- used by: [`pruneContext`](context_prune.ts.md#pruneContext), [`DEFAULTS`](context_prune.ts.md#DEFAULTS)

### `TextPart`
- def: [`extensions/pi-autoresearch-vkf/context_prune.ts:38`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L38) — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
- signature: `interface TextPart`
- members:
  - `text` — [`L40`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L40) — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
  - `type` — [`L39`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L39) — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
- used by: [`textParts`](context_prune.ts.md#textParts), [`isPruned`](context_prune.ts.md#isPruned), [`textChars`](context_prune.ts.md#textChars)

## Functions
- `pruneContext(messages: PrunableMessage[], opts?: PruneOptions | undefined)` — [`L75`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L75) — Replace the text of old chatty tool results with {@link PRUNE_STUB}, in — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)

## Module values
- `CHATTY_TOOLS` — [`L18`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L18) — Tools whose results go stale once their content is carded / logged to disk. — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
- `DEFAULTS` — [`L52`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L52) — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
- `PRUNE_STUB` — [`L28`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L28) — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
- `isPruned` — [`L67`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L67) — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
- `pruned` — [`L75`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L75) — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
- `savedChars` — [`L75`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L75)
- `textChars` — [`L65`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L65) — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)
- `textParts` — [`L58`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/context_prune.ts#L58) — documented in [extensions-pi-autoresearch-vkf-context_prune.ts](../../../concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md)


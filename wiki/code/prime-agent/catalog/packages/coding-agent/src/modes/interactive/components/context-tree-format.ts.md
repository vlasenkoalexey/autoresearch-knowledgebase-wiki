---
title: 'Module: packages/coding-agent/src/modes/interactive/components/context-tree-format.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/context-tree-format.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`context-tree-format.ts`/
symbols:
  formatContextTree: formatContextTree().
  formatContextColumn: formatContextColumn().
  sumOwnUsage: sumOwnUsage().
  spentTokens: spentTokens().
  flattenContextTree: flattenContextTree().
  ContextTreeRow.node: ContextTreeRow#node.
  statusIcon: statusIcon().
  countNodes: countNodes().
  padStartAnsi: padStartAnsi().
  ContextTreeRow.prefix: ContextTreeRow#prefix.
  padEndAnsi: padEndAnsi().
  CONTEXT_BAR_WIDTH: CONTEXT_BAR_WIDTH.
  ContextTreeRow: ContextTreeRow#
  formatCost: formatCost().
  MIN_LABEL_WIDTH: MIN_LABEL_WIDTH.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/context-tree-format.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts)

## Classes
### `ContextTreeRow`
- def: [`packages/coding-agent/src/modes/interactive/components/context-tree-format.ts:12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts#L12)
- signature: `interface ContextTreeRow`
- members:
  - `node` — [`L13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts#L13)
  - `prefix` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts#L15) — Tree-drawing prefix, e.g. "│  └─ ".
- uses (calls/refs, reference-scoped): [`ContextTreeNode`](../../../core/context-tree.ts.md#ContextTreeNode)
- used by: [`formatContextTree`](context-tree-format.ts.md#formatContextTree), [`flattenContextTree`](context-tree-format.ts.md#flattenContextTree)

## Functions
- `countNodes(root: ContextTreeNode)` — [`L90`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts#L90)
- `flattenContextTree(root: ContextTreeNode)` — [`L38`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts#L38)
- `formatContextColumn(contextUsage: ContextUsage | undefined, withBar: boolean)` — [`L60`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts#L60)
- `formatContextTree(root: ContextTreeNode, width: number)` — [`L112`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts#L112) — Render the /context overview: a tree with one row per agent showing its own
- `formatCost(cost: number)` — [`L56`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts#L56)
- `padEndAnsi(text: string, width: number)` — [`L82`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts#L82)
- `padStartAnsi(text: string, width: number)` — [`L86`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts#L86)
- `spentTokens(usage: Usage)` — [`L52`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts#L52) — Spend-relevant token count, matching the "Total" line of /usage.
- `statusIcon(status: "active" | RlmChildAgentStatus)` — [`L18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts#L18)
- `sumOwnUsage(root: ContextTreeNode)` — [`L95`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts#L95) — Own usage summed over the whole tree: exact even while children are mid-run.

## Module values
- `CONTEXT_BAR_WIDTH` — [`L9`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts#L9)
- `MIN_LABEL_WIDTH` — [`L10`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/context-tree-format.ts#L10)


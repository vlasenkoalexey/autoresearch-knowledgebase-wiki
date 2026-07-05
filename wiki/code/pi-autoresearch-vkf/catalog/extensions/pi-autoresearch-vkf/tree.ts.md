---
title: 'Module: extensions/pi-autoresearch-vkf/tree.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/tree.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`tree.ts`/
symbols:
  selectExpansion: selectExpansion().
  depths: depths().
  buildTree: buildTree().
  bestNode: bestNode().
  frontier: frontier().
  resolveParents: resolveParents().
  ExpansionPick.r: ExpansionPick#r.
  TreeNode: TreeNode#
  TreeNode.experiment: TreeNode#experiment.
  TreeNode.children: TreeNode#children.
  selectExpansion.opts-typeLiteral110.direction: selectExpansion().(opts)typeLiteral110:direction.
  TreeNode.depth: TreeNode#depth.
  ExpansionPick: ExpansionPick#
  ExpansionPick.node_kind: ExpansionPick#node_kind.
  ExpansionPick.parent_id: ExpansionPick#parent_id.
  ExpansionPick.idea: ExpansionPick#idea.
  selectExpansion.opts-typeLiteral110.exploreFraction: selectExpansion().(opts)typeLiteral110:exploreFraction.
  selectExpansion.opts-typeLiteral110.k: selectExpansion().(opts)typeLiteral110:k.
  ExpansionPick.slot: ExpansionPick#slot.
---
# Module: [`extensions/pi-autoresearch-vkf/tree.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts)

## Classes
### `ExpansionPick`
- def: [`extensions/pi-autoresearch-vkf/tree.ts:129`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L129) — documented in [extensions-pi-autoresearch-vkf-tree.ts](../../../concepts/extensions-pi-autoresearch-vkf-tree.ts.md)
- signature: `interface ExpansionPick`
- members:
  - `idea` — [`L135`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L135) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `node_kind` — [`L133`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L133) — The move this would be (improve the best node, or branch to explore).
  - `parent_id` — [`L131`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L131) — Id of the node to branch from, or `undefined` to draft a fresh root.
  - `r` — [`L134`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L134)
  - `slot` — [`L136`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L136)
- uses (calls/refs, reference-scoped): [`IdeaInput`](scoring.ts.md#IdeaInput), [`ScoredIdea`](scoring.ts.md#ScoredIdea), [`NodeKind`](experiments.ts.md#NodeKind), [`Slot`](scoring.ts.md#Slot)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`selectExpansion`](tree.ts.md#selectExpansion)

### `TreeNode`
- def: [`extensions/pi-autoresearch-vkf/tree.ts:19`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L19) — documented in [extensions-pi-autoresearch-vkf-tree.ts](../../../concepts/extensions-pi-autoresearch-vkf-tree.ts.md)
- signature: `interface TreeNode`
- members:
  - `children` — [`L21`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L21) — documented in [extensions-pi-autoresearch-vkf-tree.ts](../../../concepts/extensions-pi-autoresearch-vkf-tree.ts.md)
  - `depth` — [`L23`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L23) — Depth from a root (root = 0). — documented in [extensions-pi-autoresearch-vkf-tree.ts](../../../concepts/extensions-pi-autoresearch-vkf-tree.ts.md)
  - `experiment` — [`L20`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L20) — documented in [extensions-pi-autoresearch-vkf-tree.ts](../../../concepts/extensions-pi-autoresearch-vkf-tree.ts.md)
- uses (calls/refs, reference-scoped): [`Experiment`](experiments.ts.md#Experiment)
- used by: [`depths`](tree.ts.md#depths), [`buildTree`](tree.ts.md#buildTree)

## Functions
- `bestNode(experiments: readonly Experiment[], direction: MetricDirection)` — [`L96`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L96) — The best-valued node so far, respecting metric direction. `undefined` if none measured. — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
- `buildTree(experiments: readonly Experiment[])` — [`L53`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L53) — Assemble the experiment forest (usually one root). Order is preserved. — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
- `depths(experiments: readonly Experiment[])` — [`L85`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L85) — Compute the depth of every node by id (root = 0). — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
- `frontier(experiments: readonly Experiment[], direction: MetricDirection)` — [`L113`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L113) — Nodes worth expanding from: the best node plus the current leaves (nodes with no — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
- `resolveParents(experiments: readonly Experiment[])` — [`L32`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L32) — Resolve each experiment's parent id, inferring a linear chain for legacy rows — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
- `selectExpansion(experiments: readonly Experiment[], scored: readonly { r: ScoredIdea; idea: IdeaInput; }[], opts: { direction: MetricDirection; exploreFraction: number; k: number; })` — [`L147`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L147) — Best-first expansion: choose *which node to expand* and *which idea to apply*. — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)

## Module values
- `direction` — [`L150`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L150) — documented in [extensions-pi-autoresearch-vkf-tree.ts](../../../concepts/extensions-pi-autoresearch-vkf-tree.ts.md)
- `exploreFraction` — [`L150`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L150) — documented in [extensions-pi-autoresearch-vkf-tree.ts](../../../concepts/extensions-pi-autoresearch-vkf-tree.ts.md)
- `k` — [`L150`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/tree.ts#L150) — documented in [extensions-pi-autoresearch-vkf-tree.ts](../../../concepts/extensions-pi-autoresearch-vkf-tree.ts.md)


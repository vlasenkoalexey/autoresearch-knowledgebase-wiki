---
title: 'Module: extensions/pi-autoresearch-vkf/experiments.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/experiments.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`experiments.ts`/
symbols:
  summarize: summarize().
  Experiment: Experiment#
  Experiment.id: Experiment#id.
  Experiment.value: Experiment#value.
  readExperiments: readExperiments().
  Experiment.outcome: Experiment#outcome.
  experimentMetrics: experimentMetrics().
  ExperimentSummary.best: ExperimentSummary#best.
  nodeBaseline: nodeBaseline().
  OUTCOME_GLYPH: OUTCOME_GLYPH.
  Experiment.lever: Experiment#lever.
  Experiment.kept: Experiment#kept.
  Outcome: Outcome#
  Experiment.parent_id: Experiment#parent_id.
  Experiment.altitude: Experiment#altitude.
  deriveOutcome: deriveOutcome().
  NodeKind: NodeKind#
  Experiment.description: Experiment#description.
  writeExperiments: writeExperiments().
  Experiment.node_kind: Experiment#node_kind.
  appendExperiment: appendExperiment().
  Experiment.metrics: Experiment#metrics.
  ExperimentSummary.inconclusive: ExperimentSummary#inconclusive.
  GLYPH: GLYPH.
  Experiment.commit: Experiment#commit.
  ExperimentSummary.win: ExperimentSummary#win.
  ExperimentSummary.loss: ExperimentSummary#loss.
  ExperimentSummary.kept: ExperimentSummary#kept.
  ExperimentSummary.discarded: ExperimentSummary#discarded.
  OUTCOMES: OUTCOMES.
  NODE_KINDS: NODE_KINDS.
  Experiment.claim_id: Experiment#claim_id.
  Experiment.branch: Experiment#branch.
  Experiment.commit_url: Experiment#commit_url.
  Experiment.baseline: Experiment#baseline.
  Experiment.memory_card: Experiment#memory_card.
  Experiment.notes: Experiment#notes.
  Experiment.ts: Experiment#ts.
  ExperimentSummary: ExperimentSummary#
  ExperimentSummary.total: ExperimentSummary#total.
  Experiment.depth: Experiment#depth.
  ExperimentSummary.pending: ExperimentSummary#pending.
---
# Module: [`extensions/pi-autoresearch-vkf/experiments.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts)

## Classes
### `Experiment`
- def: [`extensions/pi-autoresearch-vkf/experiments.ts:30`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L30) — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
- signature: `interface Experiment`
- members:
  - `altitude` — [`L60`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L60) — Size of the change, inherited from the tested claim. — documented in [extensions-pi-autoresearch-vkf-progress_data.ts](../../../concepts/extensions-pi-autoresearch-vkf-progress_data.ts.md)
  - `baseline` — [`L62`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L62) — Baseline this run was compared against.
  - `branch` — [`L54`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L54) — Per-idea branch the change was snapshotted onto (`autoresearch-vkf-<idea>`).
  - `claim_id` — [`L46`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L46) — Claim/idea this experiment tested (a VKF id, e.g. "claim:adagc").
  - `commit` — [`L52`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L52) — Short (7-char) commit hash capturing the change, if known. — documented in [extensions-pi-autoresearch-vkf-progress_data.ts](../../../concepts/extensions-pi-autoresearch-vkf-progress_data.ts.md)
  - `commit_url` — [`L56`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L56) — Web URL to the exact snapshot commit (built from `origin`), if resolvable.
  - `depth` — [`L44`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L44) — Depth in the search tree (root = 0). Filled when the node is logged.
  - `description` — [`L34`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L34) — What was changed, in words. — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
  - `id` — [`L32`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L32) — Stable id, e.g. "exp-003-adagc". — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
  - `kept` — [`L66`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L66) — Whether the change was kept (vs reverted). — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
  - `lever` — [`L58`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L58) — System part this experiment touched, inherited from the tested claim. — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
  - `memory_card` — [`L68`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L68) — Memory experiment-card id written back to the bundle, if any.
  - `metrics` — [`L50`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L50) — All `METRIC name=value` pairs recorded for this run, primary metric included.
  - `node_kind` — [`L42`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L42) — What kind of move this node is (draft/improve/debug/branch).
  - `notes` — [`L70`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L70) — Free-form notes: deviations, surprises, next steps.
  - `outcome` — [`L64`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L64) — Outcome relative to the baseline and metric direction. — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
  - `parent_id` — [`L40`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L40) — Id of the experiment this one branched from in the search tree. `undefined` — documented in [extensions-pi-autoresearch-vkf-progress_data.ts](../../../concepts/extensions-pi-autoresearch-vkf-progress_data.ts.md)
  - `ts` — [`L72`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L72) — ISO timestamp.
  - `value` — [`L48`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L48) — Primary metric value obtained (the session's configured metric). — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
- uses (calls/refs, reference-scoped): [`Outcome`](experiments.ts.md#Outcome), [`NodeKind`](experiments.ts.md#NodeKind)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`index.ts`](index.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-index.ts), [`buildDashboardData`](progress_data.ts.md#buildDashboardData), [`dashboard.ts`](dashboard.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-dashboard.ts), [`buildFullscreenLines`](dashboard.ts.md#buildFullscreenLines), [`summarize`](experiments.ts.md#summarize), [`selectExpansion`](tree.ts.md#selectExpansion), [`loopLine`](dashboard.ts.md#loopLine), [`progress_data.ts`](progress_data.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-progress_data.ts), [`runsTable`](dashboard.ts.md#runsTable), [`tree.ts`](tree.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-tree.ts), [`depths`](tree.ts.md#depths), [`buildTree`](tree.ts.md#buildTree), [`coverageLine`](dashboard.ts.md#coverageLine), [`readExperiments`](experiments.ts.md#readExperiments), [`bestNode`](tree.ts.md#bestNode), [`frontier`](tree.ts.md#frontier), [`resolveParents`](tree.ts.md#resolveParents), [`experimentMetrics`](experiments.ts.md#experimentMetrics), [`statusLabel`](dashboard.ts.md#statusLabel), [`nodeBaseline`](experiments.ts.md#nodeBaseline), [`bestValue`](progress_data.ts.md#bestValue), [`experiments`](progress_data.ts.md#BuildDashboardInput.experiments), [`experiment`](tree.ts.md#TreeNode.experiment), [`writeExperiments`](experiments.ts.md#writeExperiments), [`appendExperiment`](experiments.ts.md#appendExperiment)

### `ExperimentSummary`
- def: [`extensions/pi-autoresearch-vkf/experiments.ts:122`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L122) — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
- signature: `interface ExperimentSummary`
- members:
  - `best` — [`L133`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L133) — Best metric value seen, respecting direction. — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
  - `discarded` — [`L131`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L131) — Runs whose change was reverted (`kept === false`). — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
  - `inconclusive` — [`L126`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L126) — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
  - `kept` — [`L129`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L129) — Runs whose change was kept (`kept === true`). — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
  - `loss` — [`L125`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L125) — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
  - `pending` — [`L127`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L127) — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
  - `total` — [`L123`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L123) — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
  - `win` — [`L124`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L124) — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`buildWidgetLines`](dashboard.ts.md#buildWidgetLines), [`summarize`](experiments.ts.md#summarize), [`experimentLine`](dashboard.ts.md#experimentLine), [`loopLine`](dashboard.ts.md#loopLine)

### `NodeKind`
- def: [`extensions/pi-autoresearch-vkf/experiments.ts:26`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L26)
- doc: What kind of move produced this node, in the tree-search sense:
- signature: `type NodeKind`
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`index.ts`](index.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-index.ts), [`tree.ts`](tree.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-tree.ts), [`node_kind`](experiments.ts.md#Experiment.node_kind), [`node_kind`](tree.ts.md#ExpansionPick.node_kind), [`NODE_KINDS`](experiments.ts.md#NODE_KINDS)

### `Outcome`
- def: [`extensions/pi-autoresearch-vkf/experiments.ts:15`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L15) — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
- signature: `type Outcome`
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`index.ts`](index.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-index.ts), [`outcome`](experiments.ts.md#Experiment.outcome), [`deriveOutcome`](experiments.ts.md#deriveOutcome), [`GLYPH`](experiments.ts.md#GLYPH), [`OUTCOMES`](experiments.ts.md#OUTCOMES)

## Functions
- `appendExperiment(experiments: Experiment[], exp: Experiment)` — [`L118`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L118) — Append a new experiment (experiments are immutable once logged). — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
- `deriveOutcome(baseline: number | undefined, value: number, direction: MetricDirection, threshold?: number)` — [`L89`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L89) — Derive an outcome from a measured value vs the baseline. `threshold` is the
- `experimentMetrics(e: Experiment, primaryMetric: string)` — [`L162`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L162) — The metrics map for a run, falling back to the primary value for older records. — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
- `nodeBaseline(experiments: readonly Experiment[], parentId: string | undefined, configBaseline: number | undefined)` — [`L175`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L175) — The baseline a node should be judged against: the value of its parent node in — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)
- `readExperiments(path: string)` — [`L104`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L104) — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
- `summarize(experiments: Experiment[], direction: MetricDirection)` — [`L136`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L136) — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
- `writeExperiments(path: string, experiments: Experiment[])` — [`L113`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L113) — documented in [extensions-pi-autoresearch-vkf-experiments.ts](../../../concepts/extensions-pi-autoresearch-vkf-experiments.ts.md)

## Module values
- `GLYPH` — [`L75`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L75)
- `NODE_KINDS` — [`L28`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L28)
- `OUTCOMES` — [`L17`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L17)
- `OUTCOME_GLYPH` — [`L82`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/experiments.ts#L82) — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)


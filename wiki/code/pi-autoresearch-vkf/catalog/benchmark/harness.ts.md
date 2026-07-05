---
title: 'Module: benchmark/harness.ts'
type: catalog
provenance: extracted
module: benchmark/harness.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 benchmark/`harness.ts`/
symbols:
  runOurs: runOurs().
  runBaseline: runBaseline().
  aggregate: aggregate().
  GroundTruthIdea.id: GroundTruthIdea#id.
  GroundTruthIdea.priorEV: GroundTruthIdea#priorEV.
  renderReport: renderReport().
  runScenario: runScenario().
  GroundTruthIdea.title: GroundTruthIdea#title.
  GroundTruthIdea.mechanism: GroundTruthIdea#mechanism.
  GroundTruthIdea.context: GroundTruthIdea#context.
  GroundTruthIdea.trueDelta: GroundTruthIdea#trueDelta.
  GroundTruthIdea.recency: GroundTruthIdea#recency.
  GroundTruthIdea.reliability: GroundTruthIdea#reliability.
  Combo.id: Combo#id.
  GroundTruthIdea.deadEndGroup: GroundTruthIdea#deadEndGroup.
  observe: observe().
  ScenarioReport.baseline: ScenarioReport#baseline.
  ScenarioReport.ours: ScenarioReport#ours.
  Scenario: Scenario#
  Scenario.ideas: Scenario#ideas.
  GroundTruthIdea.isPlaybook: GroundTruthIdea#isPlaybook.
  isCombo: isCombo.
  Candidate: Candidate#
  Combo.priorEV: Combo#priorEV.
  mean: mean().
  Scenario.combos: Scenario#combos.
  Combo.title: Combo#title.
  Combo.mechanism: Combo#mechanism.
  Combo.context: Combo#context.
  Scenario.budget: Scenario#budget.
  Scenario.optimumImprovement: Scenario#optimumImprovement.
  text: text.
  GroundTruthIdea: GroundTruthIdea#
  Combo: Combo#
  Combo.parents: Combo#parents.
  Combo.trueDelta: Combo#trueDelta.
  Combo.recency: Combo#recency.
  Combo.reliability: Combo#reliability.
  Scenario.name: Scenario#name.
  RunMetrics: RunMetrics#
  RunMetrics.bestImprovement: RunMetrics#bestImprovement.
  RunMetrics.uniqueMechanisms: RunMetrics#uniqueMechanisms.
  RunMetrics.wastedExperiments: RunMetrics#wastedExperiments.
  RunMetrics.deadEndsRetried: RunMetrics#deadEndsRetried.
  RunMetrics.combosDiscovered: RunMetrics#combosDiscovered.
  RunMetrics.foundOptimum: RunMetrics#foundOptimum.
  Aggregate: Aggregate#
  Aggregate.bestImprovement: Aggregate#bestImprovement.
  Aggregate.uniqueMechanisms: Aggregate#uniqueMechanisms.
  Aggregate.wastedExperiments: Aggregate#wastedExperiments.
  Aggregate.deadEndsRetried: Aggregate#deadEndsRetried.
  Aggregate.combosDiscovered: Aggregate#combosDiscovered.
  Aggregate.foundOptimumRate: Aggregate#foundOptimumRate.
  Scenario.baseline: Scenario#baseline.
  hashStr: hashStr().
  mulberry32: mulberry32().
  ScenarioReport: ScenarioReport#
  ScenarioReport.name: ScenarioReport#name.
  GroundTruthIdea.cost: GroundTruthIdea#cost.
  gauss: gauss().
  NOISE_SIGMA: NOISE_SIGMA.
  LOSS_THRESHOLD: LOSS_THRESHOLD.
---
# Module: [`benchmark/harness.ts`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts)

## Classes
### `Aggregate`
- def: [`benchmark/harness.ts:286`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L286)
- signature: `interface Aggregate`
- members:
  - `bestImprovement` — [`L287`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L287)
  - `combosDiscovered` — [`L291`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L291)
  - `deadEndsRetried` — [`L290`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L290)
  - `foundOptimumRate` — [`L292`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L292)
  - `uniqueMechanisms` — [`L288`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L288)
  - `wastedExperiments` — [`L289`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L289)
- used by: (4 test-only callers)

### `Candidate`
- def: [`benchmark/harness.ts:116`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L116)
- signature: `type Candidate`
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

### `Combo`
- def: [`benchmark/harness.ts:44`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L44)
- doc: A synthesized idea unlocked only when both parents have been tried AND the
- signature: `interface Combo`
- members:
  - `context` — [`L48`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L48)
  - `id` — [`L45`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L45)
  - `mechanism` — [`L47`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L47)
  - `parents` — [`L49`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L49)
  - `priorEV` — [`L51`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L51)
  - `recency` — [`L52`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L52)
  - `reliability` — [`L53`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L53)
  - `title` — [`L46`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L46)
  - `trueDelta` — [`L50`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L50)
- used by: (6 test-only callers)

### `GroundTruthIdea`
- def: [`benchmark/harness.ts:25`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L25)
- signature: `interface GroundTruthIdea`
- members:
  - `context` — [`L29`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L29)
  - `cost` — [`L37`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L37)
  - `deadEndGroup` — [`L39`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L39) — Ideas in the same dead-end family share a group id.
  - `id` — [`L26`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L26)
  - `isPlaybook` — [`L32`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L32)
  - `mechanism` — [`L28`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L28)
  - `priorEV` — [`L34`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L34) — Agent's a-priori attraction to this idea, [0,1] (EV proxy).
  - `recency` — [`L35`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L35)
  - `reliability` — [`L36`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L36)
  - `title` — [`L27`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L27)
  - `trueDelta` — [`L31`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L31) — True metric improvement if tried (e.g. loss reduction). 0/negative = dud.
- used by: (6 test-only callers)

### `RunMetrics`
- def: [`benchmark/harness.ts:68`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L68)
- signature: `interface RunMetrics`
- members:
  - `bestImprovement` — [`L69`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L69)
  - `combosDiscovered` — [`L73`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L73)
  - `deadEndsRetried` — [`L72`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L72)
  - `foundOptimum` — [`L74`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L74)
  - `uniqueMechanisms` — [`L70`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L70)
  - `wastedExperiments` — [`L71`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L71)
- used by: (3 test-only callers)

### `Scenario`
- def: [`benchmark/harness.ts:56`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L56)
- signature: `interface Scenario`
- members:
  - `baseline` — [`L59`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L59) — Starting metric (lower is better, e.g. validation loss).
  - `budget` — [`L61`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L61) — Experiment budget (number of runs allowed).
  - `combos` — [`L65`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L65)
  - `ideas` — [`L64`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L64)
  - `name` — [`L57`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L57)
  - `optimumImprovement` — [`L63`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L63) — Improvement at/above which we count the run as finding the optimum.
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (7 test-only callers)

### `ScenarioReport`
- def: [`benchmark/harness.ts:315`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L315)
- signature: `interface ScenarioReport`
- members:
  - `baseline` — [`L317`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L317)
  - `name` — [`L316`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L316)
  - `ours` — [`L318`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L318)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

## Functions
- `aggregate(scenario: Scenario, run: (s: Scenario, seed: number) => RunMetrics, seeds: number)` — [`L299`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L299)
- `gauss(rng: () => number)` — [`L99`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L99)
- `hashStr(s: string)` — [`L79`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L79)
- `mean(xs: number[])` — [`L295`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L295)
- `mulberry32(seed: number)` — [`L88`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L88)
- `observe(trueDelta: number, ideaId: string, seed: number)` — [`L109`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L109) — Deterministic noisy measurement for trying `ideaId` under `seed` — the same
- `renderReport(reports: ScenarioReport[], seeds: number)` — [`L329`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L329)
- `runBaseline(scenario: Scenario, seed: number)` — [`L131`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L131) — Models a loop with no structured memory: it reaches for ideas by apparent value
- `runOurs(scenario: Scenario, seed: number)` — [`L189`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L189) — Durable memory (never repeats), priority ranking via the real `rankIdeas` — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- `runScenario(scenario: Scenario, seeds: number)` — [`L321`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L321)

## Module values
- `LOSS_THRESHOLD` — [`L122`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L122)
- `NOISE_SIGMA` — [`L105`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L105)
- `isCombo` — [`L117`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L117)
- `text` — [`L119`](../../../../../raw/code/pi-autoresearch-vkf/benchmark/harness.ts#L119)


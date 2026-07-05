---
title: Benchmark methodology — VKF memory + synthesis vs. a blind loop
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Benchmark methodology — VKF memory + synthesis vs. a blind loop

## Definition
`npm run bench` runs two policies — "Standard" (a blind loop: EV-greedy, no durable memory, no synthesis) and
"Ours" (VKF memory + novelty scoring + contradiction synthesis, driven through the real `scoring.ts`/`synthesis.ts`) —
over deterministic, ground-truth idea-environments, 500 seeds per scenario, and reports the difference. The
README states the headline result directly: across both scenarios (Tiny-LM validation loss, inference
latency), "ours" finds the scenario's true optimum 100% of the time with zero wasted (repeat) experiments,
versus 0% for the blind loop — because in each scenario the global optimum is a *synthesized* idea (a
combination of two ground-truth ideas) that a blind ranking loop cannot construct on its own.

## In pi-autoresearch-vkf (grounded)
The harness lives in `benchmark/`, not `extensions/`, and is deliberately kept separate from the pi runtime so
it can drive the *real* production modules directly with plain data. [`runOurs`](../catalog/benchmark/harness.ts.md#runOurs)
and [`runBaseline`](../catalog/benchmark/harness.ts.md#runBaseline) are the two policies under test — `runOurs`
is the one that actually calls [`rankIdeas`](../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md) (and, per
its own doc comment, "the real `rankIdeas`" specifically to avoid re-implementing a scoring stand-in) and the
[`synthesis.ts`](../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md) contradiction miner to unlock
[`Combo`](../catalog/benchmark/harness.ts.md#Combo) ideas. Ground-truth environments are
[`GroundTruthIdea`](../catalog/benchmark/harness.ts.md#GroundTruthIdea) and
[`Scenario`](../catalog/benchmark/harness.ts.md#Scenario) records defined in
[`benchmark/scenarios.ts`](../catalog/benchmark/scenarios.ts.md) (`tinyLM`, `inferenceLatency`, collected in
`SCENARIOS`) — each `Scenario` bundles a `baseline`, a `budget`, an `optimumImprovement` threshold, its
`ideas`, and the `combos` only synthesis can unlock. [`observe`](../catalog/benchmark/harness.ts.md#observe) is
the shared, seeded-noise measurement function both policies call, so neither gets a fidelity advantage — only
the *policy* (which idea to try next) differs. [`aggregate`](../catalog/benchmark/harness.ts.md#aggregate) and
[`runScenario`](../catalog/benchmark/harness.ts.md#runScenario) roll many seeded runs into the
[`Aggregate`](../catalog/benchmark/harness.ts.md#Aggregate)/[`ScenarioReport`](../catalog/benchmark/harness.ts.md#ScenarioReport)
metrics the README's table quotes (`bestImprovement`, `uniqueMechanisms`, `wastedExperiments`,
`deadEndsRetried`, `combosDiscovered`, `foundOptimumRate`). `benchmark/run.ts`'s
[`main`](../catalog/benchmark/run.ts.md#main) is the CLI entry point (`--seeds`), and
[`stripTitle`](../catalog/benchmark/run.ts.md#stripTitle) is what lets it rewrite the README's own
`<!-- BENCH:START/END -->` block in place with fresh numbers.

## Why it matters / when it applies
The benchmark isolates *search-policy quality* from everything else an LLM agent brings to a real run (it
never calls an LLM) — [`Combo`](../catalog/benchmark/harness.ts.md#Combo)'s own doc comment is explicit that a
synthesized idea is "unlocked only when both parents have been tried AND the contradiction miner flags the
pair — i.e. discoverable solely by synthesis," which is precisely the property the 0%-vs-100% "found optimum"
numbers are designed to expose. Because the harness re-uses the production `scoring.ts`/`synthesis.ts` modules
rather than a simulated stand-in, a regression in either module's real logic shows up here directly. The
README's own roadmap notes the harness's current limit: it isolates the idea-selection policy but doesn't yet
credit tree-aware behavior like backtracking or node re-expansion (see
[the search tree's design-rationale comparison](../concepts/extensions-pi-autoresearch-vkf-tree.ts.md) for why
that gap exists in the current `tree.ts` implementation too).

## Connections
- Code concepts: [Idea scoring](../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md),
  [Hypothesis synthesis](../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md),
  [The experiment search tree](../concepts/extensions-pi-autoresearch-vkf-tree.ts.md)
- Module catalogs: [benchmark/harness.ts](../catalog/benchmark/harness.ts.md),
  [benchmark/scenarios.ts](../catalog/benchmark/scenarios.ts.md), [benchmark/run.ts](../catalog/benchmark/run.ts.md)
- Related doc-concepts: [Tool reference](tool-reference.md)

## Source
Extracted from `README.md` ("Benchmark" section, including the `<!-- BENCH:START/END -->` results table) and
`CLAUDE.md` (`npm run bench` command description), both kept in place.

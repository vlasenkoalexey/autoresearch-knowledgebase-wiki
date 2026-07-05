---
title: The artifacts feedback loop — turning failures into the next prompt's context
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-05
status: fresh
---
# The artifacts feedback loop — turning failures into the next prompt's context

## Definition

The README's "Artifacts & Debugging" section frames the `EvaluationResult` artifacts side-channel not as
a data structure but as a behavior: an evaluator returns stderr, profiling data, LLM feedback, or build
warnings alongside its metrics, and "the next generation prompt automatically includes" that context
(rendered under a "Previous Execution Feedback" heading), which the README summarizes as "a feedback loop
where each generation learns from previous mistakes." This page grounds that end-to-end loop claim across
the three code concepts that each implement one leg of it.

## In openevolve (grounded)

The loop has three legs, each documented in depth on its own concept page but only visible as a whole
when traced end-to-end:

1. **Produce.** A user's evaluator constructs an
   [`EvaluationResult`](../catalog/openevolve/evaluation_result.md#EvaluationResult) with both `metrics`
   and `artifacts` (see [`openevolve-evaluation_result.md`](../concepts/openevolve-evaluation_result.md)),
   or the [`Evaluator`](../catalog/openevolve/evaluator.md#Evaluator)'s own cascade stages attach
   stderr/traceback artifacts automatically on a timeout or exception (see
   [`openevolve-evaluator.md`](../concepts/openevolve-evaluator.md)). Either way, artifacts never travel
   through [`evaluate_program`](../catalog/openevolve/evaluator.md#Evaluator.evaluate_program)'s own
   `Dict[str, float]` return value — they are captured out-of-band as a side effect, keyed by program id.
2. **Store.** The child `Program`'s artifacts are attached to it in the database (see
   [`openevolve-database.md`](../concepts/openevolve-database.md)) rather than discarded once the
   `combined_score` is computed.
3. **Render.** On a later iteration, when that program (or a descendant sampled alongside it) is chosen
   as a parent or inspiration, [`PromptSampler`](../catalog/openevolve/prompt/sampler.md#PromptSampler)'s
   [`_render_artifacts`](../catalog/openevolve/prompt/sampler.md#PromptSampler._render_artifacts) turns
   the stored artifacts back into prompt text (bounded by
   [`max_artifact_bytes`](../catalog/openevolve/config.md#PromptConfig) and passed through a security
   filter, per [`openevolve-prompt-sampler.md`](../concepts/openevolve-prompt-sampler.md)) — this is the
   concrete mechanism behind the README's "Previous Execution Feedback" prompt section.

## Why it matters / when it applies

The loop only closes because the artifacts channel is deliberately kept separate from the metrics channel
at every step (see the "smuggling mechanism" framing on
[`openevolve-evaluation_result.md`](../concepts/openevolve-evaluation_result.md)) — if failure context had
to be encoded as a numeric metric, there would be no way to hand the LLM *why* a candidate scored `0.0`,
only that it did. The README's own worked example (`stderr: "Warning: suboptimal memory access
pattern"` → rendered as `⚠️ Warning: suboptimal memory access pattern` in the next prompt) is exactly the
render step in the mechanism above, not a separate feature. This is also the mechanism the README's system
message guidance implicitly leans on: "Artifact-Driven Iteration" (refining a system message based on
observed stderr/warning patterns, see [`system-message-design.md`](system-message-design.md)) only works
because the artifacts loop is already surfacing that stderr into every subsequent prompt automatically —
a user tuning their system message is reacting to context the loop, not the user, is responsible for
delivering.

## Connections

- Code concepts: [EvaluationResult — the metrics-plus-artifacts evaluation contract](../concepts/openevolve-evaluation_result.md),
  [Evaluator — cascade evaluation with folded-in LLM judgment](../concepts/openevolve-evaluator.md),
  [Prompt sampler — assembling what the LLM mutation operator sees](../concepts/openevolve-prompt-sampler.md),
  [The program database](../concepts/openevolve-database.md) — where artifacts live between being
  produced and being rendered.
- Module catalogs: [openevolve/evaluation_result.py](../catalog/openevolve/evaluation_result.md),
  [openevolve/evaluator.py](../catalog/openevolve/evaluator.md),
  [openevolve/prompt/sampler.py](../catalog/openevolve/prompt/sampler.md).
- Related doc-concepts: [System message design](system-message-design.md) — the README's guidance on
  reacting to the same feedback this loop already surfaces.

## Source

Extracted from `README.md` (kept in place), "Artifacts & Debugging" section.

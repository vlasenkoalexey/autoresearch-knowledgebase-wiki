---
title: article_opt pipeline stage interface
type: concept
provenance: mixed
concept: domains-article_opt-pipeline-base
updated: 2026-07-05
status: fresh
---

# article_opt pipeline stage interface

## Overview
`domains/article_opt/pipeline/base.py` defines the one interface every Level-1 pipeline stage — and every
Level-2-generated stage — must satisfy:
[`BaseStage`](../catalog/domains/article_opt/pipeline/base.md#BaseStage). It is a small, deliberately
minimal abstract class: one abstract method (`run`), one shared helper for reading outer-loop guidance, and
one shared helper for writing artifacts to disk. Everything domain-specific — prompts, rubric text, LLM
calls — lives in the five concrete stages
([`ArticleAnalysisStage`](../catalog/domains/article_opt/pipeline/article_analysis.md#ArticleAnalysisStage),
[`ImprovementHypothesesStage`](../catalog/domains/article_opt/pipeline/improvement_hypotheses.md#ImprovementHypothesesStage),
[`EditPlanningStage`](../catalog/domains/article_opt/pipeline/edit_planning.md#EditPlanningStage),
[`ImpactAssessmentStage`](../catalog/domains/article_opt/pipeline/impact_assessment.md#ImpactAssessmentStage),
[`RevisedOutputStage`](../catalog/domains/article_opt/pipeline/revised_output.md#RevisedOutputStage)) that
subclass it — and this narrow, uniform contract is exactly what lets Level 2's generated code slot into the
same list without the runner needing to know anything else about it.

## Diagram
```mermaid
classDiagram
    class BaseStage {
        +name: str
        +model: str
        +max_retries: int|None
        +run(context: dict) dict
        #_outer_guidance(context: dict) str
        #_save_artifact(run_dir, filename, content) str
    }
    BaseStage <|-- ArticleAnalysisStage
    BaseStage <|-- EditPlanningStage
    BaseStage <|-- ImpactAssessmentStage
    BaseStage <|-- ImprovementHypothesesStage
    BaseStage <|-- RevisedOutputStage
    BaseStage <|-- GeneratedStage["(Level-2 generated stage)"]
```

## Design rationale (why it's built this way)
The class docstring spells out the entire calling contract in one place — the exact `context` dict keys a
stage may read (`article_id`, `article_content`, `previous_outputs`, `retrieved_lessons`,
`evaluator_feedback`, `run_dir`, `run_number`) and the exact shape a stage must return (`content`,
`artifacts`). Making this contract textual (a docstring) rather than a typed dataclass is what lets the
Level-2 code-generation prompt (see
[domains-article_opt-mechanism_research.md](domains-article_opt-mechanism_research.md)) reproduce it almost
verbatim — the generated-stage interface spec lists the same context keys in the same order, because it's
describing the same interface a human-authored stage already implements.

[`_outer_guidance`](../catalog/domains/article_opt/pipeline/base.md#BaseStage._outer_guidance) is the only
place Level 1.5's `prompt_overrides` re-enters a running stage: it looks up
`context["outer_guidance"].get(self.name, "")` — keyed by the stage's own
[`name`](../catalog/domains/article_opt/pipeline/base.md#BaseStage.name) class attribute — and returns
either an empty string or a formatted `## Outer Loop Guidance` block. Because the lookup is by `name` and
`name` defaults to `"base"` unless a subclass overrides it, a subclass that forgets to set `name` would
silently share (or fail to receive) outer guidance meant for a different stage.

`max_retries: int | None = None` on the class defaults every stage to the runner's global retry count; only
[`EditPlanningStage`](../catalog/domains/article_opt/pipeline/edit_planning.md#EditPlanningStage) overrides
it (to 2), letting one stage opt into a different retry budget without a parallel configuration mechanism.

## Entry points
- [`run`](../catalog/domains/article_opt/pipeline/base.md#BaseStage.run) — the abstract method every
  concrete stage implements; this is the method the runner (see
  [domains-article_opt-runner.md](domains-article_opt-runner.md)) calls once per stage per run.
- [`ArticleAnalysisStage.run`](../catalog/domains/article_opt/pipeline/article_analysis.md#ArticleAnalysisStage.run) —
  the pipeline's first stage; scores the current article against the rubric and extracts per-dimension
  scores via [`parse_json_response`](../catalog/core/llm_client.md#parse_json_response).
- [`RevisedOutputStage.run`](../catalog/domains/article_opt/pipeline/revised_output.md#RevisedOutputStage.run) —
  the pipeline's last stage; this is the stage
  [`inject_stage`](../catalog/domains/article_opt/runner.md#InnerRunner.inject_stage) most commonly targets
  as an `inject_after` point, since it is where the article's final text is produced for the run.

## Mechanism (step-by-step)
1. Every stage is constructed with just a
   [`model`](../catalog/domains/article_opt/pipeline/base.md#BaseStage.model) string (`__init__` stores it on
   `self.model`); stages carry no other constructor-time configuration, so all per-run context flows through
   the `context` dict passed to `run`, not through instance state set at construction.
2. [`ArticleAnalysisStage.run`](../catalog/domains/article_opt/pipeline/article_analysis.md#ArticleAnalysisStage.run)
   reads `article_content` plus any `retrieved_lessons`/`evaluator_feedback` from context, calls
   [`call_llm`](../catalog/core/llm_client.md#call_llm) with the full `RUBRIC` text embedded in the prompt,
   saves the free-text analysis via
   [`_save_artifact`](../catalog/domains/article_opt/pipeline/base.md#BaseStage._save_artifact), then issues a
   *second* `call_llm` call purely to extract structured A–E scores as JSON via
   [`parse_json_response`](../catalog/core/llm_client.md#parse_json_response) — one stage, two LLM round trips.
3. [`ImprovementHypothesesStage.run`](../catalog/domains/article_opt/pipeline/improvement_hypotheses.md#ImprovementHypothesesStage.run)
   and
   [`EditPlanningStage.run`](../catalog/domains/article_opt/pipeline/edit_planning.md#EditPlanningStage.run)
   both call [`_outer_guidance`](../catalog/domains/article_opt/pipeline/base.md#BaseStage._outer_guidance)
   explicitly and splice its output into their prompts alongside the "INJECTION POINT" comment marking where
   `retrieved_lessons` (inner-loop lessons, not outer guidance) goes — the two injection channels
   (outer-loop text and inner-loop lessons) are textually adjacent in the prompt but come from entirely
   different state objects: the outer loop's prompt-override store (see
   [domains-article_opt-outer.md](domains-article_opt-outer.md)) versus the inner loop's per-cycle lesson
   list (see [domains-article_opt-runner.md](domains-article_opt-runner.md)).
4. Only [`ImprovementHypothesesStage.run`](../catalog/domains/article_opt/pipeline/improvement_hypotheses.md#ImprovementHypothesesStage.run)
   and [`EditPlanningStage.run`](../catalog/domains/article_opt/pipeline/edit_planning.md#EditPlanningStage.run)
   call `_outer_guidance` at all — the other three built-in stages
   ([`ArticleAnalysisStage`](../catalog/domains/article_opt/pipeline/article_analysis.md#ArticleAnalysisStage.run),
   [`ImpactAssessmentStage`](../catalog/domains/article_opt/pipeline/impact_assessment.md#ImpactAssessmentStage.run),
   and [`RevisedOutputStage`](../catalog/domains/article_opt/pipeline/revised_output.md#RevisedOutputStage.run))
   never do, so Level 1.5's prompt-override text can only reach those two stages. `ImpactAssessmentStage.run`,
   for instance, reads the prior two stages' outputs (`article_analysis`, `edit_planning`) from
   `previous_outputs` and predicts post-edit scores, but has no outer-loop injection point of its own.
5. [`RevisedOutputStage.run`](../catalog/domains/article_opt/pipeline/revised_output.md#RevisedOutputStage.run)
   branches on article length (`<= 8000` chars: whole-article rewrite via
   [`_revise_whole`](../catalog/domains/article_opt/pipeline/revised_output.md#RevisedOutputStage._revise_whole);
   longer: per-section rewrite via
   [`_revise_by_section`](../catalog/domains/article_opt/pipeline/revised_output.md#RevisedOutputStage._revise_by_section)
   using [`_extract_sections`](../catalog/domains/article_opt/pipeline/revised_output.md#_extract_sections))
   before saving the result via `_save_artifact` and returning it under both `content` and a
   `revised_article` key.
6. Every stage's [`_save_artifact`](../catalog/domains/article_opt/pipeline/base.md#BaseStage._save_artifact)
   call resolves to the same path shape — `run_dir / "stages" / self.name / filename` — so artifacts from a
   Level-2-injected stage land in their own subdirectory automatically, keyed only by whatever
   [`name`](../catalog/domains/article_opt/pipeline/base.md#BaseStage.name) the generated class declares.

## Key data structures
`context: dict` is the only state a stage ever sees — it is rebuilt fresh at the start of every run by the
runner (see [domains-article_opt-runner.md](domains-article_opt-runner.md)), so a stage cannot retain
information across runs except by writing it into its own output text, which then flows into the *next* run
only via `retrieved_lessons` (extracted separately by the runner, not by the stage itself).

## Dynamics (design intent)
Stages execute strictly sequentially in list order — there is no parallelism across stages within a run, and
each stage's output populates `previous_outputs` before the next stage runs, so a later stage always sees an
already-committed (not concurrently-mutating) view of every earlier stage's text.

## Edge cases
`_save_artifact`'s path is built directly from `self.name` with no sanitization — a
Level-2-generated stage whose `name` attribute contains path-separator characters would write outside the
intended `stages/<name>/` subdirectory; nothing in this class checks for that (a similar containment check
exists for the generated *file* itself in the Level-2 generator — see
[domains-article_opt-mechanism_research.md](domains-article_opt-mechanism_research.md) — but not for this
per-run artifact directory).

## Open questions
`max_retries: int | None = None` is read by the runner as "use global config" — this packet's Subgraph
doesn't show that resolution logic directly, only the class-attribute declaration and
`EditPlanningStage`'s override; see [domains-article_opt-runner.md](domains-article_opt-runner.md) for how
the runner actually applies it.

## See also
- [domains-article_opt-runner.md](domains-article_opt-runner.md) — the caller that instantiates the five
  built-in stages and drives `run` on each.
- [domains-article_opt-mechanism_research.md](domains-article_opt-mechanism_research.md) — Level 2, whose
  generated code must subclass this exact `BaseStage` interface to be loadable at all.
- [domains-article_opt-outer.md](domains-article_opt-outer.md) — the source of the `outer_guidance` dict
  `_outer_guidance` reads.
- [domains-article_opt-cli.md](domains-article_opt-cli.md) — where stage instances first get constructed
  (via `make_runner` → `InnerRunner.__init__`).
- [../../../sources/bilevel-autoresearch.md](../../../sources/bilevel-autoresearch.md) — paper framing; this
  page covers this lighter demo domain's Level-1 task machinery, not the paper's own reported experiment
  (`domains/train_opt`).

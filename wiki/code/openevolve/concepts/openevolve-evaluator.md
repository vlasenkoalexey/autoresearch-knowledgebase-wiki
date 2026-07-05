---
title: Evaluator — cascade evaluation with folded-in LLM judgment
type: concept
provenance: mixed
concept: openevolve-evaluator
concepts: [evolutionary-algorithm-discovery]
updated: 2026-07-05
status: fresh
---
# Evaluator — cascade evaluation with folded-in LLM judgment

<!-- connect:up:begin -->
> **Cross-repo concept:** part of [evolutionary-algorithm-discovery](../../../concepts/evolutionary-algorithm-discovery.md) across this wiki's repos.
<!-- connect:up:end -->
## Overview
[`Evaluator`](../catalog/openevolve/evaluator.md#Evaluator) is the "programmatic evaluator" pillar of the
open-source AlphaEvolve recipe: the thing that turns a candidate program's source text into the scalar
fitness the MAP-Elites/island database uses to decide which candidates seed the next generation. Its
docstring states the job plainly — `[`Evaluator`](../catalog/openevolve/evaluator.md#Evaluator) "evaluates
programs and assigns scores... responsible for executing programs, measuring their performance, and
assigning scores based on the evaluation criteria."` The interesting engineering is not "run untrusted code
and score it" in the abstract — it's the specific shape chosen to make that safe and cheap at evolutionary
scale: a **cascade** of increasingly expensive checks that can bail out early on a bad candidate, wrapped in
retry/timeout handling so a broken or slow candidate program can never take down the evaluator process, plus
an optional second pass where an LLM *judges* the code and that judgment is folded back into the same
numeric `metrics` dict the rest of the system already understands — not routed through some separate
qualitative channel.

The evaluation function itself is not part of OpenEvolve — it is user-supplied Python, loaded dynamically
from a path (`evaluation_file`) the caller configures per task, and expected to expose an `evaluate`
function (required) plus, optionally, `evaluate_stage1`/`evaluate_stage2`/`evaluate_stage3` for cascade mode.
`Evaluator` is the machinery around that user code, not the scoring logic itself.

## Diagram
```mermaid
flowchart TD
    EP["evaluate_program(program_code, program_id)"] --> Cascade{cascade_evaluation<br/>config flag?}
    Cascade -- yes --> CE["_cascade_evaluate(program_path)"]
    Cascade -- no --> DE["_direct_evaluate(program_path)"]

    CE --> S1["run evaluate_stage1<br/>(timeout-bounded)"]
    S1 -- timeout/exception --> S1F["return stage1_passed=0.0<br/>+ error artifacts"]
    S1 -- ok --> T1{clears cascade_thresholds[0]?<br/>and evaluate_stage2 exists?}
    T1 -- no --> S1R[return stage1-only result]
    T1 -- yes --> S2["run evaluate_stage2<br/>(timeout-bounded)"]
    S2 -- timeout/exception --> S2F["keep stage1 metrics,<br/>set stage2_passed=0.0"]
    S2 -- ok --> Merge12[merge stage1+stage2<br/>metrics + artifacts]
    Merge12 --> T2{clears cascade_thresholds[1]?<br/>and evaluate_stage3 exists?}
    T2 -- no --> M12R[return stage1+2 merged result]
    T2 -- yes --> S3["run evaluate_stage3<br/>(timeout-bounded)"]
    S3 -- timeout/exception --> S3F["keep stage1+2 metrics,<br/>set stage3_passed=0.0"]
    S3 -- ok --> Merge123[merge stage3 metrics<br/>into final result]

    DE --> PR["_process_evaluation_result<br/>(normalize dict/EvaluationResult)"]
    S1F --> PR
    S1R --> PR
    S2F --> PR
    M12R --> PR
    S3F --> PR
    Merge123 --> PR

    PR --> LLMGate{use_llm_feedback config<br/>and llm_ensemble present?}
    LLMGate -- yes --> LLME["_llm_evaluate(program_code)"]
    LLME --> Blend["blend llm_* metrics in;<br/>recompute combined_score<br/>as 0.7·accuracy + 0.3·llm_average"]
    LLMGate -- no --> Skip[metrics unchanged]
    Blend --> Return["return eval_result.metrics<br/>to caller"]
    Skip --> Return
```

## Design rationale (why it's built this way)
Evolutionary search generates far more bad or broken candidates than good ones — an LLM diff applied to
working code frequently produces a program that doesn't compile, hangs, or crashes. Running every candidate
through a full, expensive evaluation would waste most of the compute budget on programs that were doomed
from the first cheap check. Cascade evaluation exists to spend that budget progressively:
[`_cascade_evaluate`](../catalog/openevolve/evaluator.md#Evaluator._cascade_evaluate) runs only
`evaluate_stage1` first, and only advances to `evaluate_stage2`/`evaluate_stage3` if the cheaper stage's
score already clears a configured threshold. A candidate that fails stage 1 (say, a syntax or import error)
is scored and discarded after the cheapest possible check — the pricier stages simply never run for it.

Crucially, this is opt-in **per evaluation file**, not purely a config toggle: setting
`cascade_evaluation: true` only changes anything if the user's evaluator module actually defines
`evaluate_stage1`. `Evaluator`'s constructor validates this at load time and, if the config says cascade but
the module has no stage functions, only *warns* rather than erroring — the run falls back to
[`_direct_evaluate`](../catalog/openevolve/evaluator.md#Evaluator._direct_evaluate) silently, making the
cascade setting a no-op. The system chooses graceful degradation over hard failure here, consistent with the
same philosophy at the per-stage level: a stage that times out or throws never aborts the whole evaluation
of that candidate — it returns whatever metrics the last successful stage produced, tagged with which stage
failed and why (`error_type`, `error_message`, `failure_stage` via
[`_create_cascade_error_context`](../catalog/openevolve/evaluator.md#Evaluator._create_cascade_error_context)).
A crashing candidate program degrades the *score*, never the evaluator process, because the user's
`evaluate`/`evaluate_stageN` call is executed as an ordinary Python call inside a thread-pool executor under
an `asyncio.wait_for` deadline, and every call site that invokes it is wrapped in its own try/except — there
is no subprocess or OS-level sandbox in this subgraph; isolation is at the level of "catch the exception,
degrade the metrics," not "contain the process."

> [!inferred] `EvaluatorConfig` (`openevolve/config.py`) also declares `memory_limit_mb`/`cpu_limit` fields,
> but the source comments them as not implemented — so cascade's cheap-first-stage design is effectively
> also the *only* real protection against a runaway candidate consuming excessive resources, short of the
> wall-clock `timeout`.

The LLM-judged pass is a genuinely separate concern layered on top, not a fourth cascade stage: it only runs
if `use_llm_feedback` is configured and an `llm_ensemble` was supplied, and it always runs *after* the
programmatic score is final — `[`_llm_evaluate`](../catalog/openevolve/evaluator.md#Evaluator._llm_evaluate)`
exists for the properties a test harness can't easily check programmatically (code clarity, idiomaticity,
approach quality) but that the AlphaEvolve recipe still wants folded into the same fitness signal driving
selection. Rather than inventing a parallel qualitative-scoring pathway, the LLM's JSON response is split
into numeric values (folded into `metrics`, namespaced `llm_*`) and non-numeric values (routed into
`artifacts` instead) — so "qualitative" judgment is deliberately flattened back into the same scalar contract
[`EvaluationResult`](../catalog/openevolve/evaluation_result.md#EvaluationResult) already exposes to the rest
of the system, and any parse failure or generation error is swallowed to an empty result rather than failing
the evaluation — the judge is best-effort, additive signal, never a hard dependency.

## Entry points
- [`evaluate_program`](../catalog/openevolve/evaluator.md#Evaluator.evaluate_program) — the sole public
  entry point external callers use. [`run`](../catalog/openevolve/controller.md#OpenEvolve.run) calls it
  once, synchronously, to score the initial seed program before evolution starts; every subsequent
  generation reaches it indirectly through the iteration workers below.
- [`_run_iteration_worker`](../catalog/openevolve/process_parallel.md#_run_iteration_worker) — the actual
  per-generation execution path: `OpenEvolve.run` is wired exclusively to `ProcessParallelController`
  (`openevolve/process_parallel.py`), whose `ProcessPoolExecutor` submits this worker function once per
  generation, and it calls `evaluate_program` on each LLM-proposed child program.
  [`run_iteration_with_shared_db`](../catalog/openevolve/iteration.md#run_iteration_with_shared_db) has the
  same shape (sample → build prompt → evaluate) but nothing else in this repo — no controller, script, or
  test — calls it, so it reads as an unused/legacy alternate implementation rather than a live second path.
- [`_lazy_init_worker_components`](../catalog/openevolve/process_parallel.md#_lazy_init_worker_components) —
  constructs a fresh [`Evaluator`](../catalog/openevolve/evaluator.md#Evaluator) instance the first time a
  ProcessPoolExecutor worker needs one, wired to its own `evaluator_models` LLM ensemble — a worker's
  evaluator can therefore run a *different* model from the ensemble that proposes mutations.

## Mechanism (step-by-step)
1. **Construction validates, it doesn't just store config.** [`Evaluator`](../catalog/openevolve/evaluator.md#Evaluator)'s
   constructor dynamically imports `evaluation_file` via `importlib`, requires it to define an `evaluate`
   function (raises `ValueError`/`AttributeError` if the file is missing or that function absent), and — if
   `cascade_evaluation` is configured true — checks for `evaluate_stage1`/`evaluate_stage2`/`evaluate_stage3`,
   warning (not raising) when the configured cascade can't actually happen.
2. **`evaluate_program` writes the candidate to a temp file and retries the whole evaluation on failure.**
   [`evaluate_program`](../catalog/openevolve/evaluator.md#Evaluator.evaluate_program) materializes
   `program_code` into a `NamedTemporaryFile` (suffix matches the target language) and loops up to
   `max_retries + 1` attempts, re-writing a fresh temp file each attempt and always deleting it in a
   `finally` block regardless of outcome.
3. **Dispatch to cascade or direct evaluation based on config.** Inside the retry loop,
   `evaluate_program` calls [`_cascade_evaluate`](../catalog/openevolve/evaluator.md#Evaluator._cascade_evaluate)
   when `cascade_evaluation` is set, else
   [`_direct_evaluate`](../catalog/openevolve/evaluator.md#Evaluator._direct_evaluate), which just runs the
   single `evaluate` function under an `asyncio.wait_for(timeout)` deadline.
4. **Cascade stage 1 gates everything downstream.** `_cascade_evaluate` runs `evaluate_stage1` (also
   timeout-bounded); a timeout or exception there returns immediately with failure metrics and rich error
   context from [`_create_cascade_error_context`](../catalog/openevolve/evaluator.md#Evaluator._create_cascade_error_context) —
   stage 2 and 3 never run for that candidate. On success, the result is checked against the configured
   first cascade threshold (preferring a `combined_score` metric if present, else the average of the other
   numeric metrics); failing that check, or the module simply not defining `evaluate_stage2`, ends the
   evaluation here with the stage-1-only result.
5. **Stage 2 and stage 3 merge forward, and each degrades independently on failure.** A successful stage 2
   is merged with stage 1's numeric metrics and artifacts inside
   [`_cascade_evaluate`](../catalog/openevolve/evaluator.md#Evaluator._cascade_evaluate); a timeout or
   exception in stage 2 instead keeps stage 1's metrics intact and just marks `stage2_passed=0.0` — the evaluation
   never drops back to a bare failure once stage 1 has already produced a usable score. The same
   merge-or-degrade pattern repeats for stage 3, gated by the second cascade threshold and whether
   `evaluate_stage3` exists at all.
6. **Every result, whichever path produced it, is normalized to one shape.**
   [`_process_evaluation_result`](../catalog/openevolve/evaluator.md#Evaluator._process_evaluation_result)
   accepts either a plain `dict` (wrapped via `EvaluationResult.from_dict` for backward compatibility with
   older evaluators) or an [`EvaluationResult`](../catalog/openevolve/evaluation_result.md#EvaluationResult)
   directly, so cascade and direct paths, and old- and new-style user evaluator functions, all converge to
   the same object before anything downstream touches `metrics`/`artifacts`.
7. **A genuine timeout short-circuits the retry loop; other exceptions burn one retry each.**
   `evaluate_program` treats `asyncio.TimeoutError` specially — it returns `{"error": 0.0, "timeout": True}`
   immediately without consuming another attempt, while any other exception is caught, logged, given a
   1-second backoff, and retried up to the configured attempt count before giving up with a bare error
   result. Timeout artifacts and failure artifacts (stderr, traceback) are captured into
   [`_pending_artifacts`](../catalog/openevolve/evaluator.md#Evaluator._pending_artifacts) either way, keyed
   by `program_id`.
8. **An optional LLM pass folds a qualitative judgment back into the same metrics dict.** After a
   programmatic result exists, if `use_llm_feedback` is configured and an ensemble is attached,
   `evaluate_program` calls [`_llm_evaluate`](../catalog/openevolve/evaluator.md#Evaluator._llm_evaluate),
   which builds an `"evaluation"`-templated prompt via
   [`build_prompt`](../catalog/openevolve/prompt/sampler.md#PromptSampler.build_prompt) (passing
   [`feature_dimensions`](../catalog/openevolve/config.md#DatabaseConfig.feature_dimensions) from the
   database config so the judge prompt is feature-aware), sends it to every ensemble member, and — per
   response — parses a JSON object out of the reply, routing numeric fields into a weight-averaged
   `metrics` dict (weighted by each model's [`weights`](../catalog/openevolve/llm/ensemble.md#LLMEnsemble.weights))
   and non-numeric fields into `artifacts`. Back in `evaluate_program`, every LLM metric is namespaced
   `llm_<name>`, averaged into `llm_average`, and — if a programmatic `combined_score` already exists —
   `combined_score` is overwritten as `0.7 * accuracy + 0.3 * llm_average`, so the LLM's judgment directly
   changes the fitness value the island database uses for selection, not just a side annotation.
9. **The LLM prompt/response pair is logged to the database only when the evaluator has one attached, and a
   program id is known.** `_llm_evaluate` calls
   [`log_prompt`](../catalog/openevolve/database.md#ProgramDatabase.log_prompt) with the built prompt and raw
   responses, gated on `self.database and program_id` — both must hold. The
   [`_lazy_init_worker_components`](../catalog/openevolve/process_parallel.md#_lazy_init_worker_components) worker path
   constructs its `Evaluator` with `database=None` ("No shared database in worker"), so on the real
   per-generation execution path this logging never fires; only evaluations run through an `Evaluator` that
   was built with a database attached — e.g. the initial seed program scored by
   [`run`](../catalog/openevolve/controller.md#OpenEvolve.run) — actually retain the qualitative judging
   conversation.

## Key data structures
- [`EvaluationResult`](../catalog/openevolve/evaluation_result.md#EvaluationResult) — the dataclass every
  internal evaluation path converges to: a mandatory
  [`metrics`](../catalog/openevolve/evaluation_result.md#EvaluationResult.metrics) `Dict[str, float]` (the
  scalar contract the rest of the system — thresholds, database, prompt sampler — already understands) plus
  an optional [`artifacts`](../catalog/openevolve/evaluation_result.md#EvaluationResult.artifacts)
  `dict[str, str | bytes]` side-channel for anything that isn't a number: stderr, tracebacks, failure-stage
  labels, or the non-numeric fields an LLM judge returned. Its own docstring is explicit that metrics values
  must be *raw continuous scores*, never pre-binned MAP-Elites bin indices — binning is the database's job,
  not the evaluator's.
- [`_pending_artifacts`](../catalog/openevolve/evaluator.md#Evaluator._pending_artifacts) — a
  `program_id`-keyed dict accumulating artifacts across the cascade/direct/LLM sub-evaluations of a single
  `evaluate_program` call before they're handed off to the caller; this is the mechanism by which a failing
  candidate's stderr/traceback/timeout context becomes visible to the prompt-building side of the pipeline
  for the *next* generation, not just logged and discarded.
- [`config`](../catalog/openevolve/evaluator.md#Evaluator.config) (an `EvaluatorConfig`) — carries
  [`cascade_evaluation`](../catalog/openevolve/config.md#EvaluatorConfig.cascade_evaluation) and
  [`timeout`](../catalog/openevolve/config.md#EvaluatorConfig.timeout) (both cited here); the cascade
  threshold list and retry/LLM-feedback-weight fields live alongside them on the same config object and are
  read directly by `_cascade_evaluate`/`evaluate_program` at each decision point in the mechanism above.

## Dynamics (design intent)
The test suite pins down exactly which parts of this are meant to degrade rather than fail. Timeout
behavior is asserted directly:
[`run_test`](../catalog/tests/test_evaluator_timeout.md#TestTimeoutIntegration.run_test) (in
`test_evaluator_timeout.py:399`) constructs an evaluator whose evaluation function sleeps past a 3-second
`timeout` and asserts the call returns in ~3s (not 6+) with `timeout=True` in the result, and
[`_create_evaluator`](../catalog/tests/test_evaluator_timeout.md#TestEvaluatorTimeout._create_evaluator) is
a shared test helper for constructing short-timeout evaluators specifically to keep this class of test fast.
The cascade-validation warning behavior described above is asserted by
[`test_cascade_validation_warning_for_missing_functions`](../catalog/tests/test_cascade_validation.md#TestCascadeValidation.test_cascade_validation_warning_for_missing_functions)
(cascade requested, no stage functions → warns, mentions `evaluate_stage1` in the message),
[`test_cascade_validation_partial_functions`](../catalog/tests/test_cascade_validation.md#TestCascadeValidation.test_cascade_validation_partial_functions)
(only `evaluate_stage1` defined → warns about missing further stages), and
[`test_no_cascade_validation_when_disabled`](../catalog/tests/test_cascade_validation.md#TestCascadeValidation.test_no_cascade_validation_when_disabled)
(cascade off → no validation at all). The dual dict/`EvaluationResult` contract is pinned by
[`test_direct_evaluate_supports_evaluation_result`](../catalog/tests/test_cascade_validation.md#TestCascadeValidation.test_direct_evaluate_supports_evaluation_result)
and
[`test_direct_evaluate_supports_dict_result`](../catalog/tests/test_cascade_validation.md#TestCascadeValidation.test_direct_evaluate_supports_dict_result),
and normalization itself by
[`test_process_evaluation_result_with_artifacts`](../catalog/tests/test_cascade_validation.md#TestCascadeValidation.test_process_evaluation_result_with_artifacts)
/
[`test_process_evaluation_result_with_dict`](../catalog/tests/test_cascade_validation.md#TestCascadeValidation.test_process_evaluation_result_with_dict).

## Edge cases
- A nonexistent `evaluation_file` fails fast at construction — `Evaluator` raises `ValueError` rather than
  deferring the failure to the first `evaluate_program` call, per
  [`test_cascade_validation_nonexistent_file`](../catalog/tests/test_cascade_validation.md#TestCascadeValidation.test_cascade_validation_nonexistent_file).
- A syntax error in the cascade functions themselves (not the candidate program) raises during construction
  too, per
  [`test_cascade_validation_with_syntax_error`](../catalog/tests/test_cascade_validation.md#TestCascadeValidation.test_cascade_validation_with_syntax_error) —
  the evaluator author's own module has to import cleanly before anything can be evaluated.
- Class-based evaluator modules (an `Evaluator` class wrapping stage methods, re-exposed as module-level
  `evaluate_stage1`/`evaluate_stage2`/`evaluate` functions) satisfy cascade validation identically to
  plain-function modules, per
  [`test_cascade_validation_with_class_based_evaluator`](../catalog/tests/test_cascade_validation.md#TestCascadeValidation.test_cascade_validation_with_class_based_evaluator) —
  validation only checks for the module-level function names, not how they're implemented underneath.
- `_llm_evaluate` returns an empty dict (`{}`) on any failure — a bad JSON parse, a generation error, or no
  `llm_ensemble` at all — rather than raising, so a broken or unavailable LLM judge silently contributes no
  extra signal instead of failing the whole `evaluate_program` call.

## Open questions
- The threshold-comparison logic itself (preferring `combined_score`, else averaging the remaining numeric
  metrics excluding `error`) lives in a private helper this packet's subgraph doesn't cite; the description
  above of that gating logic was verified directly against `openevolve/evaluator.py`, but the helper isn't
  linkable here.
- `_cascade_evaluate` re-imports the evaluation module via a fresh `importlib.util` load on every call,
  separately from the module `Evaluator`'s constructor already loaded and cached as `self.evaluate_function`
  for `_direct_evaluate`. Whether this duplication is intentional (e.g., to pick up a changed evaluation
  file mid-run) or incidental isn't shown in this subgraph.
- Artifact capture is gated by `os.environ.get("ENABLE_ARTIFACTS", "true")` — an environment variable read
  at evaluation time — rather than solely by a config field on `EvaluatorConfig`; the interaction between
  this env var and any config-level artifact setting isn't visible in the cited subgraph.

## See also
- [openevolve-controller](openevolve-controller.md) — calls `evaluate_program` once for the seed program
  and owns the `Evaluator` instance for non-parallel runs.
- [openevolve-evaluation_result](openevolve-evaluation_result.md) — the `EvaluationResult` contract every
  evaluation path in this page converges to.
- [openevolve-database](openevolve-database.md) — the MAP-Elites/island store whose selection reads exactly
  the `metrics` (especially `combined_score`) this page's cascade-and-LLM pipeline produces.
- [../../../concepts/evolutionary-algorithm-discovery.md](../../../concepts/evolutionary-algorithm-discovery.md) —
  the cross-repo concept this evaluator is the programmatic-evaluator instance of.
- [../../../sources/alphaevolve.md](../../../sources/alphaevolve.md) — the paper this evaluator's cascade/
  LLM-judgment design implements the open-source recipe for.

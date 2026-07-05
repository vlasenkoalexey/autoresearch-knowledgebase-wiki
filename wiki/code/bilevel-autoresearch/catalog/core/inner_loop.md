---
title: 'Module: core/inner_loop.py'
type: catalog
provenance: extracted
module: core/inner_loop.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `core.inner_loop`/
symbols:
  InnerLoopController.run_cycle: InnerLoopController#run_cycle().
  InnerLoopController._promote_skills: InnerLoopController#_promote_skills().
  InnerLoopController: InnerLoopController#
  logger: logger.
  InnerLoopController.convergence_threshold: InnerLoopController#convergence_threshold.
  InnerLoopController.runner: InnerLoopController#runner.
  InnerLoopController.max_iterations: InnerLoopController#max_iterations.
  InnerLoopController.convergence_consecutive: InnerLoopController#convergence_consecutive.
  InnerLoopController.skill_confidence_min: InnerLoopController#skill_confidence_min.
  InnerLoopController.__init__: InnerLoopController#__init__().
---
# Module: [`core/inner_loop.py`](../../../../../raw/code/bilevel-autoresearch/core/inner_loop.py)

## Classes
### `InnerLoopController`
- def: [`core/inner_loop.py:15`](../../../../../raw/code/bilevel-autoresearch/core/inner_loop.py#L15) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
- doc: Manages one full inner cycle (up to max_iterations runs on one article).
- signature: `class InnerLoopController:`
- members:
  - `_promote_skills(self, inner: InnerLoopState)` — [`L91`](../../../../../raw/code/bilevel-autoresearch/core/inner_loop.py#L91) — Promote high-confidence lessons to stage skills for injection. — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `run_cycle(self, article_id: str, outer_state: OuterLoopState)` — [`L41`](../../../../../raw/code/bilevel-autoresearch/core/inner_loop.py#L41) — Run one full inner cycle for the given article. — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `convergence_consecutive` — [`L38`](../../../../../raw/code/bilevel-autoresearch/core/inner_loop.py#L38) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `convergence_threshold` — [`L37`](../../../../../raw/code/bilevel-autoresearch/core/inner_loop.py#L37) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `max_iterations` — [`L36`](../../../../../raw/code/bilevel-autoresearch/core/inner_loop.py#L36) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `runner` — [`L35`](../../../../../raw/code/bilevel-autoresearch/core/inner_loop.py#L35) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `skill_confidence_min` — [`L39`](../../../../../raw/code/bilevel-autoresearch/core/inner_loop.py#L39) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
- protocol/private: `__init__`[`L27`](../../../../../raw/code/bilevel-autoresearch/core/inner_loop.py#L27)
- uses (calls/refs, reference-scoped): [`inner_lessons`](state.md#InnerLoopState.inner_lessons), [`InnerLoopState`](state.md#InnerLoopState), [`peak_score`](state.md#InnerLoopState.peak_score), [`OuterLoopState`](state.md#OuterLoopState), [`current_cycle`](state.md#OuterLoopState.current_cycle), [`is_converged`](state.md#InnerLoopState.is_converged), [`update_skill`](state.md#InnerLoopState.update_skill), [`confidence`](state.md#InnerLesson.confidence), [`prompt_overrides`](state.md#OuterLoopState.prompt_overrides), [`build_inner_state`](state.md#OuterLoopState.build_inner_state), [`logger`](inner_loop.md#logger), [`stage`](state.md#InnerLesson.stage)
- used by: [`cmd_mechresearch`](../domains/article_opt/cli.md#cmd_mechresearch), [`run`](../domains/article_opt/outer.md#OuterLoopController.run), [`validate`](../domains/article_opt/mechanism_research.md#MechanismResearcher.validate), [`cmd_inner`](../domains/article_opt/cli.md#cmd_inner), [`cmd_run`](../domains/article_opt/cli.md#cmd_run), [`v`](../domains/article_opt/cli.md#v), [`__init__`](../domains/article_opt/outer.md#OuterLoopController.__init__)  (5 test-only)

## Module values
- `logger` — [`L12`](../../../../../raw/code/bilevel-autoresearch/core/inner_loop.py#L12)


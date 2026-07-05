---
title: 'Module: domains/article_opt/outer.py'
type: catalog
provenance: extracted
module: domains/article_opt/outer.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.article_opt.outer`/
symbols:
  OuterLoopController.run: OuterLoopController#run().
  OuterLoopController._save_outer_lessons: OuterLoopController#_save_outer_lessons().
  OuterLoopController.outer_state: OuterLoopController#outer_state.
  OuterAnalyzer.analyze: OuterAnalyzer#analyze().
  OuterLoopController._apply_config_changes: OuterLoopController#_apply_config_changes().
  OuterLoopController._save_cycle_summary: OuterLoopController#_save_cycle_summary().
  logger: logger.
  OuterLoopController.__init__: OuterLoopController#__init__().
  OuterLoopController._last_strategy: OuterLoopController#_last_strategy().
  OuterLoopController.reference_doc: OuterLoopController#reference_doc.
  OuterAnalyzer: OuterAnalyzer#
  OuterLoopController: OuterLoopController#
  OuterLoopController.max_outer_iterations: OuterLoopController#max_outer_iterations.
  OUTER_SYSTEM: OUTER_SYSTEM.
  OuterAnalyzer.model: OuterAnalyzer#model.
  OuterAnalyzer.api_key: OuterAnalyzer#api_key.
  OuterLoopController.inner_controller: OuterLoopController#inner_controller.
  OuterLoopController.analyzer: OuterLoopController#analyzer.
  OuterLoopController.article_ids: OuterLoopController#article_ids.
  OuterAnalyzer.__init__: OuterAnalyzer#__init__().
---
# Module: [`domains/article_opt/outer.py`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py)

## Classes
### `OuterAnalyzer`
- def: [`domains/article_opt/outer.py:29`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L29)
- doc: Calls DeepSeek to analyze an inner cycle trace and produce:
- signature: `class OuterAnalyzer:`
- members:
  - `analyze(self, inner_summary: dict, outer_context: str, reference_doc: str, outer_cycle: int)` — [`L42`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L42) — Run DeepSeek meta-analysis. Returns structured dict with config changes. — documented in [domains-article_opt-outer](../../../concepts/domains-article_opt-outer.md)
  - `api_key` — [`L40`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L40)
  - `model` — [`L39`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L39)
- protocol/private: `__init__`[`L38`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L38)
- uses (calls/refs, reference-scoped): [`parse_json_response`](../../core/llm_client.md#parse_json_response), [`call`](../../core/llm_client.md#LLMClient.call), [`LLMClient`](../../core/llm_client.md#LLMClient), [`logger`](outer.md#logger), [`OUTER_SYSTEM`](outer.md#OUTER_SYSTEM)
- used by: [`run`](outer.md#OuterLoopController.run), [`cmd_run`](cli.md#cmd_run), [`v`](cli.md#v), [`__init__`](outer.md#OuterLoopController.__init__)

### `OuterLoopController`
- def: [`domains/article_opt/outer.py:110`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L110)
- doc: Manages the full dual-layer experiment.
- signature: `class OuterLoopController:`
- members:
  - `_apply_config_changes(self, analysis: dict, cycle: int)` — [`L227`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L227) — Apply prompt_overrides from DeepSeek analysis to outer_state. — documented in [domains-article_opt-outer](../../../concepts/domains-article_opt-outer.md)
  - `_save_cycle_summary(self, cycle: int, results: list[dict])` — [`L276`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L276) — Write per-cycle JSON summary to examples/.
  - `_save_outer_lessons(self, analysis: dict, inner_summary: dict, cycle: int)` — [`L260`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L260) — Convert analysis output to OuterLesson objects and save. — documented in [domains-article_opt-outer](../../../concepts/domains-article_opt-outer.md)
  - `run(self)` — [`L141`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L141) — Run the full dual-layer experiment. — documented in [core-inner_loop](../../../concepts/core-inner_loop.md)
  - `analyzer` — [`L134`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L134)
  - `article_ids` — [`L135`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L135)
  - `inner_controller` — [`L133`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L133)
  - `max_outer_iterations` — [`L136`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L136)
  - `outer_state` — [`L132`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L132)
  - `reference_doc` — [`L137`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L137)
- protocol/private: `__init__`[`L123`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L123), `_last_strategy`[`L222`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L222)
- uses (calls/refs, reference-scoped): [`run_cycle`](../../core/inner_loop.md#InnerLoopController.run_cycle), [`extract_from_inner`](../../core/state.md#OuterLoopState.extract_from_inner), [`analyze`](outer.md#OuterAnalyzer.analyze), [`save_checkpoint`](../../core/state.md#OuterLoopState.save_checkpoint), [`reset`](../../core/state.md#InnerLoopState.reset), [`InnerLoopController`](../../core/inner_loop.md#InnerLoopController), [`OuterLoopState`](../../core/state.md#OuterLoopState), [`current_cycle`](../../core/state.md#OuterLoopState.current_cycle), [`build_outer_context`](../../core/state.md#OuterLoopState.build_outer_context), [`outer_lessons`](../../core/state.md#OuterLoopState.outer_lessons), [`logger`](outer.md#logger), [`add_outer_lesson`](../../core/state.md#OuterLoopState.add_outer_lesson), [`begin_cycle`](../../core/state.md#OuterLoopState.begin_cycle), [`prompt_overrides`](../../core/state.md#OuterLoopState.prompt_overrides), [`_examples_dir`](../../core/state.md#OuterLoopState._examples_dir), [`add_strategy_result`](../../core/state.md#OuterLoopState.add_strategy_result), [`OuterLesson`](../../core/state.md#OuterLesson), [`strategy_history`](../../core/state.md#OuterLoopState.strategy_history), [`lesson_type`](../../core/state.md#OuterLesson.lesson_type), [`summary`](../../core/state.md#OuterLesson.summary), [`is_outer_converged`](../../core/state.md#OuterLoopState.is_outer_converged), [`OuterAnalyzer`](outer.md#OuterAnalyzer), [`confidence`](../../core/state.md#OuterLesson.confidence), [`outer_cycle`](../../core/state.md#OuterLesson.outer_cycle), [`reuse_rule`](../../core/state.md#OuterLesson.reuse_rule), [`stage_affected`](../../core/state.md#OuterLesson.stage_affected), [`strategy_used`](../../core/state.md#OuterLesson.strategy_used)
- used by: [`cmd_run`](cli.md#cmd_run), [`v`](cli.md#v)

## Module values
- `OUTER_SYSTEM` — [`L24`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L24)
- `logger` — [`L22`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/outer.py#L22)


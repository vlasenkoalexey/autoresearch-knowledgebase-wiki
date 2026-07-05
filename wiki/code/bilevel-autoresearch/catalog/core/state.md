---
title: 'Module: core/state.py'
type: catalog
provenance: extracted
module: core/state.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `core.state`/
symbols:
  OuterLoopState.extract_from_inner: OuterLoopState#extract_from_inner().
  OuterLoopState.load_checkpoint: OuterLoopState#load_checkpoint().
  InnerLoopState.run_trace: InnerLoopState#run_trace.
  OuterLoopState._archive_inner: OuterLoopState#_archive_inner().
  OuterLesson.to_dict: OuterLesson#to_dict().
  InnerLoopState.inner_lessons: InnerLoopState#inner_lessons.
  InnerLoopState: InnerLoopState#
  RunResult.to_dict: RunResult#to_dict().
  OuterLoopState.save_checkpoint: OuterLoopState#save_checkpoint().
  RunResult.overall: RunResult#overall.
  InnerLoopState.reset: InnerLoopState#reset().
  InnerLoopState.record_run: InnerLoopState#record_run().
  InnerLoopState.add_lesson: InnerLoopState#add_lesson().
  InnerLoopState.peak_score: InnerLoopState#peak_score().
  RunResult.scores: RunResult#scores.
  RunResult: RunResult#
  OuterLoopState: OuterLoopState#
  RunResult.stage_map: RunResult#stage_map().
  InnerLoopState.runs_to_threshold: InnerLoopState#runs_to_threshold().
  OuterLoopState.current_cycle: OuterLoopState#current_cycle.
  InnerLoopState.lesson_quality_stats: InnerLoopState#lesson_quality_stats().
  StageScore.stage: StageScore#stage.
  StageScore: StageScore#
  InnerLoopState.is_converged: InnerLoopState#is_converged().
  InnerLoopState.convergence_trace: InnerLoopState#convergence_trace().
  InnerLoopState.evaluator_dimension_pattern: InnerLoopState#evaluator_dimension_pattern().
  OuterLoopState.build_outer_context: OuterLoopState#build_outer_context().
  InnerLoopState.update_skill: InnerLoopState#update_skill().
  RunResult.run_number: RunResult#run_number.
  InnerLesson.confidence: InnerLesson#confidence.
  InnerLoopState.inner_skills: InnerLoopState#inner_skills.
  OuterLoopState.outer_lessons: OuterLoopState#outer_lessons.
  StageScore.score: StageScore#score.
  RunResult.article_version: RunResult#article_version.
  InnerLesson: InnerLesson#
  InnerLoopState.stage_failure_pattern: InnerLoopState#stage_failure_pattern().
  OuterLoopState.add_outer_lesson: OuterLoopState#add_outer_lesson().
  OuterLoopState._persist_outer_lessons: OuterLoopState#_persist_outer_lessons().
  OuterLoopState.begin_cycle: OuterLoopState#begin_cycle().
  InnerLoopState.article_id: InnerLoopState#article_id.
  OuterLoopState.prompt_overrides: OuterLoopState#prompt_overrides.
  StageScore.feedback: StageScore#feedback.
  OuterLoopState._examples_dir: OuterLoopState#_examples_dir.
  InnerLoopState.article_working_copy: InnerLoopState#article_working_copy.
  OuterLoopState.add_strategy_result: OuterLoopState#add_strategy_result().
  OuterLoopState.build_inner_state: OuterLoopState#build_inner_state().
  InnerLesson.stage: InnerLesson#stage.
  InnerLesson.run_number: InnerLesson#run_number.
  OuterLesson: OuterLesson#
  InnerLoopState.retry_log: InnerLoopState#retry_log.
  OuterLoopState.strategy_history: OuterLoopState#strategy_history.
  InnerLesson.summary: InnerLesson#summary.
  InnerLesson.reuse_rule: InnerLesson#reuse_rule.
  OuterLesson.lesson_type: OuterLesson#lesson_type.
  OuterLesson.summary: OuterLesson#summary.
  OuterLoopState.iteration_summaries: OuterLoopState#iteration_summaries.
  OuterLoopState.is_outer_converged: OuterLoopState#is_outer_converged().
  InnerLesson.lesson_type: InnerLesson#lesson_type.
  OuterLesson.outer_cycle: OuterLesson#outer_cycle.
  OuterLesson.strategy_used: OuterLesson#strategy_used.
  OuterLesson.reuse_rule: OuterLesson#reuse_rule.
  OuterLesson.confidence: OuterLesson#confidence.
  OuterLesson.stage_affected: OuterLesson#stage_affected.
  OuterLoopState.base_dir: OuterLoopState#base_dir.
  InnerLoopState.log_retry: InnerLoopState#log_retry().
  StageScore.retried: StageScore#retried.
  RunResult.strategy_used: RunResult#strategy_used.
  OuterLesson.inner_convergence_before: OuterLesson#inner_convergence_before.
  OuterLesson.inner_convergence_after: OuterLesson#inner_convergence_after.
  InnerLoopState._original_article: InnerLoopState#_original_article.
  OuterLoopState.original_articles: OuterLoopState#original_articles.
  InnerLoopState.__init__: InnerLoopState#__init__().
  OuterLoopState.__init__: OuterLoopState#__init__().
  OuterLoopState.outer_skills: OuterLoopState#outer_skills.
---
# Module: [`core/state.py`](../../../../../raw/code/bilevel-autoresearch/core/state.py)

## Classes
### `InnerLesson`
- def: [`core/state.py:49`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L49) — documented in [core-state](../../concepts/core-state.md)
- signature: `class InnerLesson:`
- members:
  - `confidence` — [`L54`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L54) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `lesson_type` — [`L50`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L50)
  - `reuse_rule` — [`L53`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L53)
  - `run_number` — [`L55`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L55)
  - `stage` — [`L51`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L51) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `summary` — [`L52`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L52)
- used by: [`_extract_lessons`](../domains/article_opt/runner.md#InnerRunner._extract_lessons), [`inner_lessons`](state.md#InnerLoopState.inner_lessons), [`_build_lessons_text`](../domains/article_opt/runner.md#InnerRunner._build_lessons_text), [`_promote_skills`](inner_loop.md#InnerLoopController._promote_skills), [`add_lesson`](state.md#InnerLoopState.add_lesson), [`lesson_quality_stats`](state.md#InnerLoopState.lesson_quality_stats)  (4 test-only)

### `InnerLoopState`
- def: [`core/state.py:86`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L86) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
- doc: All state that belongs to one inner cycle.
- signature: `class InnerLoopState:`
- members:
  - `add_lesson(self, lesson: InnerLesson)` — [`L112`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L112) — documented in [domains-article_opt-runner](../../concepts/domains-article_opt-runner.md)
  - `convergence_trace(self)` — [`L143`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L143) — documented in [core-state](../../concepts/core-state.md)
  - `evaluator_dimension_pattern(self)` — [`L163`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L163) — Mean score per rubric dimension across all runs. — documented in [core-state](../../concepts/core-state.md)
  - `is_converged(self, threshold: int = 8, consecutive: int = 3)` — [`L123`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L123) — True if the last `consecutive` runs all scored >= threshold overall. — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `lesson_quality_stats(self)` — [`L173`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L173) — documented in [core-state](../../concepts/core-state.md)
  - `log_retry(self, run: int, stage: str, attempt: int, reason: str)` — [`L118`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L118)
  - `peak_score(self)` — [`L136`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L136) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `record_run(self, result: RunResult)` — [`L108`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L108) — documented in [core-state](../../concepts/core-state.md)
  - `reset(self)` — [`L185`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L185) — Restore to outer-iteration-start state. — documented in [core-state](../../concepts/core-state.md)
  - `runs_to_threshold(self, threshold: int = 8)` — [`L129`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L129) — Return the run number when threshold was first reached, or None. — documented in [core-state](../../concepts/core-state.md)
  - `stage_failure_pattern(self)` — [`L146`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L146) — Per-stage stats: mean score, std, retry count. — documented in [core-state](../../concepts/core-state.md)
  - `update_skill(self, stage: str, skill_text: str)` — [`L115`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L115) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `article_id` — [`L98`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L98)
  - `article_working_copy` — [`L100`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L100)
  - `inner_lessons` — [`L101`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L101) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `inner_skills` — [`L102`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L102) — documented in [domains-article_opt-runner](../../concepts/domains-article_opt-runner.md)
  - `retry_log` — [`L104`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L104) — documented in [core-state](../../concepts/core-state.md)
  - `run_trace` — [`L103`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L103) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
- protocol/private: `__init__`[`L97`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L97), `_original_article`[`L99`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L99)
- uses (calls/refs, reference-scoped): [`overall`](state.md#RunResult.overall), [`scores`](state.md#RunResult.scores), [`RunResult`](state.md#RunResult), [`stage_map`](state.md#RunResult.stage_map), [`stage`](state.md#StageScore.stage), [`confidence`](state.md#InnerLesson.confidence), [`run_number`](state.md#RunResult.run_number), [`InnerLesson`](state.md#InnerLesson), [`article_version`](state.md#RunResult.article_version), [`score`](state.md#StageScore.score)
- used by: [`research`](../domains/article_opt/mechanism_research.md#MechanismResearcher.research), [`run_once`](../domains/article_opt/runner.md#InnerRunner.run_once), [`cmd_mechresearch`](../domains/article_opt/cli.md#cmd_mechresearch), [`run`](../domains/article_opt/outer.md#OuterLoopController.run), [`validate`](../domains/article_opt/mechanism_research.md#MechanismResearcher.validate), [`run_cycle`](inner_loop.md#InnerLoopController.run_cycle), [`cmd_inner`](../domains/article_opt/cli.md#cmd_inner), [`extract_from_inner`](state.md#OuterLoopState.extract_from_inner), [`cmd_once`](../domains/article_opt/cli.md#cmd_once), [`v`](../domains/article_opt/cli.md#v), [`_archive_inner`](state.md#OuterLoopState._archive_inner), [`_build_lessons_text`](../domains/article_opt/runner.md#InnerRunner._build_lessons_text), [`_build_trace_summary`](../domains/article_opt/mechanism_research.md#MechanismResearcher._build_trace_summary), [`_promote_skills`](inner_loop.md#InnerLoopController._promote_skills), [`build_inner_state`](state.md#OuterLoopState.build_inner_state)  (28 test-only)

### `OuterLesson`
- def: [`core/state.py:59`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L59) — documented in [core-state](../../concepts/core-state.md)
- signature: `class OuterLesson:`
- members:
  - `to_dict(self)` — [`L70`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L70)
  - `confidence` — [`L65`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L65)
  - `inner_convergence_after` — [`L67`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L67)
  - `inner_convergence_before` — [`L66`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L66)
  - `lesson_type` — [`L61`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L61)
  - `outer_cycle` — [`L60`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L60)
  - `reuse_rule` — [`L64`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L64)
  - `stage_affected` — [`L68`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L68)
  - `strategy_used` — [`L62`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L62)
  - `summary` — [`L63`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L63)
- used by: [`load_checkpoint`](state.md#OuterLoopState.load_checkpoint), [`_save_outer_lessons`](../domains/article_opt/outer.md#OuterLoopController._save_outer_lessons), [`save_checkpoint`](state.md#OuterLoopState.save_checkpoint), [`build_outer_context`](state.md#OuterLoopState.build_outer_context), [`outer_lessons`](state.md#OuterLoopState.outer_lessons), [`_persist_outer_lessons`](state.md#OuterLoopState._persist_outer_lessons), [`add_outer_lesson`](state.md#OuterLoopState.add_outer_lesson)

### `OuterLoopState`
- def: [`core/state.py:200`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L200) — documented in [domains-article_opt-cli](../../concepts/domains-article_opt-cli.md)
- doc: State that persists across all outer iterations.
- signature: `class OuterLoopState:`
- members:
  - `_archive_inner(self, inner: InnerLoopState)` — [`L249`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L249) — Save best article and full trace to examples/ (archival only). — documented in [core-state](../../concepts/core-state.md)
  - `add_outer_lesson(self, lesson: OuterLesson)` — [`L269`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L269) — documented in [domains-article_opt-outer](../../concepts/domains-article_opt-outer.md)
  - `add_strategy_result(self, strategy: str, inner_before: int | None, inner_after: int | None, notes: str)` — [`L273`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L273)
  - `begin_cycle(self)` — [`L344`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L344) — documented in [domains-article_opt-cli](../../concepts/domains-article_opt-cli.md)
  - `build_inner_state(self, article_id: str)` — [`L347`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L347) — Create a fresh inner state for this article, using the original text.
  - `build_outer_context(self, inner_summary: dict, reference_doc: str = "")` — [`L354`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L354) — Build the context string injected into the outer loop's LLM call. — documented in [domains-article_opt-outer](../../concepts/domains-article_opt-outer.md)
  - `extract_from_inner(self, inner: InnerLoopState, strategy_used: str = "")` — [`L222`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L222) — Pull process-level signals from a completed inner cycle. — documented in [core-state](../../concepts/core-state.md)
  - `is_outer_converged(self, target_inner_runs: int = 10)` — [`L293`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L293) — Outer loop converged when inner loop reaches ≥8/10 in ≤target_inner_runs
  - `load_checkpoint(self)` — [`L319`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L319) — Load from checkpoint if it exists. Returns True if loaded. — documented in [core-state](../../concepts/core-state.md)
  - `save_checkpoint(self)` — [`L306`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L306) — Save outer loop state to a checkpoint file after each cycle. — documented in [domains-article_opt-outer](../../concepts/domains-article_opt-outer.md)
  - `base_dir` — [`L207`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L207) — documented in [core-state](../../concepts/core-state.md)
  - `current_cycle` — [`L213`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L213) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `iteration_summaries` — [`L211`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L211) — documented in [core-state](../../concepts/core-state.md)
  - `original_articles` — [`L208`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L208)
  - `outer_lessons` — [`L209`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L209) — documented in [core-state](../../concepts/core-state.md)
  - `outer_skills` — [`L210`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L210)
  - `prompt_overrides` — [`L218`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L218) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `strategy_history` — [`L212`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L212) — documented in [core-state](../../concepts/core-state.md)
- protocol/private: `__init__`[`L206`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L206), `_examples_dir`[`L214`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L214), `_persist_outer_lessons`[`L284`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L284)
- uses (calls/refs, reference-scoped): [`run_trace`](state.md#InnerLoopState.run_trace), [`to_dict`](state.md#OuterLesson.to_dict), [`InnerLoopState`](state.md#InnerLoopState), [`to_dict`](state.md#RunResult.to_dict), [`overall`](state.md#RunResult.overall), [`peak_score`](state.md#InnerLoopState.peak_score), [`runs_to_threshold`](state.md#InnerLoopState.runs_to_threshold), [`lesson_quality_stats`](state.md#InnerLoopState.lesson_quality_stats), [`convergence_trace`](state.md#InnerLoopState.convergence_trace), [`evaluator_dimension_pattern`](state.md#InnerLoopState.evaluator_dimension_pattern), [`is_converged`](state.md#InnerLoopState.is_converged), [`article_version`](state.md#RunResult.article_version), [`stage_failure_pattern`](state.md#InnerLoopState.stage_failure_pattern), [`article_id`](state.md#InnerLoopState.article_id), [`OuterLesson`](state.md#OuterLesson), [`retry_log`](state.md#InnerLoopState.retry_log), [`lesson_type`](state.md#OuterLesson.lesson_type), [`summary`](state.md#OuterLesson.summary), [`confidence`](state.md#OuterLesson.confidence), [`outer_cycle`](state.md#OuterLesson.outer_cycle), [`reuse_rule`](state.md#OuterLesson.reuse_rule), [`stage_affected`](state.md#OuterLesson.stage_affected), [`strategy_used`](state.md#OuterLesson.strategy_used)
- used by: [`cmd_mechresearch`](../domains/article_opt/cli.md#cmd_mechresearch), [`run`](../domains/article_opt/outer.md#OuterLoopController.run), [`validate`](../domains/article_opt/mechanism_research.md#MechanismResearcher.validate), [`run_cycle`](inner_loop.md#InnerLoopController.run_cycle), [`cmd_inner`](../domains/article_opt/cli.md#cmd_inner), [`cmd_run`](../domains/article_opt/cli.md#cmd_run), [`cmd_once`](../domains/article_opt/cli.md#cmd_once), [`v`](../domains/article_opt/cli.md#v), [`_save_outer_lessons`](../domains/article_opt/outer.md#OuterLoopController._save_outer_lessons), [`_apply_config_changes`](../domains/article_opt/outer.md#OuterLoopController._apply_config_changes), [`_save_cycle_summary`](../domains/article_opt/outer.md#OuterLoopController._save_cycle_summary), [`__init__`](../domains/article_opt/outer.md#OuterLoopController.__init__), [`_last_strategy`](../domains/article_opt/outer.md#OuterLoopController._last_strategy)  (1 test-only)

### `RunResult`
- def: [`core/state.py:26`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L26) — documented in [core-state](../../concepts/core-state.md)
- signature: `class RunResult:`
- members:
  - `stage_map(self)` — [`L34`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L34) — documented in [domains-article_opt-outer](../../concepts/domains-article_opt-outer.md)
  - `to_dict(self)` — [`L37`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L37) — documented in [core-state](../../concepts/core-state.md)
  - `article_version` — [`L30`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L30) — documented in [core-state](../../concepts/core-state.md)
  - `overall` — [`L29`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L29)
  - `run_number` — [`L27`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L27)
  - `scores` — [`L28`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L28) — documented in [core-state](../../concepts/core-state.md)
  - `strategy_used` — [`L31`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L31)
- uses (calls/refs, reference-scoped): [`stage`](state.md#StageScore.stage), [`StageScore`](state.md#StageScore), [`score`](state.md#StageScore.score), [`feedback`](state.md#StageScore.feedback), [`retried`](state.md#StageScore.retried)
- used by: [`run_once`](../domains/article_opt/runner.md#InnerRunner.run_once), [`cmd_mechresearch`](../domains/article_opt/cli.md#cmd_mechresearch), [`validate`](../domains/article_opt/mechanism_research.md#MechanismResearcher.validate), [`cmd_inner`](../domains/article_opt/cli.md#cmd_inner), [`cmd_once`](../domains/article_opt/cli.md#cmd_once), [`run_trace`](state.md#InnerLoopState.run_trace), [`_archive_inner`](state.md#OuterLoopState._archive_inner), [`_build_trace_summary`](../domains/article_opt/mechanism_research.md#MechanismResearcher._build_trace_summary), [`record_run`](state.md#InnerLoopState.record_run), [`peak_score`](state.md#InnerLoopState.peak_score), [`runs_to_threshold`](state.md#InnerLoopState.runs_to_threshold), [`convergence_trace`](state.md#InnerLoopState.convergence_trace), [`evaluator_dimension_pattern`](state.md#InnerLoopState.evaluator_dimension_pattern), [`is_converged`](state.md#InnerLoopState.is_converged), [`stage_failure_pattern`](state.md#InnerLoopState.stage_failure_pattern)  (6 test-only)

### `StageScore`
- def: [`core/state.py:18`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L18) — documented in [core-state](../../concepts/core-state.md)
- signature: `class StageScore:`
- members:
  - `feedback` — [`L21`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L21)
  - `retried` — [`L22`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L22)
  - `score` — [`L20`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L20)
  - `stage` — [`L19`](../../../../../raw/code/bilevel-autoresearch/core/state.py#L19)
- used by: [`run_once`](../domains/article_opt/runner.md#InnerRunner.run_once), [`to_dict`](state.md#RunResult.to_dict), [`scores`](state.md#RunResult.scores), [`stage_map`](state.md#RunResult.stage_map), [`evaluator_dimension_pattern`](state.md#InnerLoopState.evaluator_dimension_pattern)  (3 test-only)


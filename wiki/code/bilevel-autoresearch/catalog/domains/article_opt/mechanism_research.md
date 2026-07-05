---
title: 'Module: domains/article_opt/mechanism_research.py'
type: catalog
provenance: extracted
module: domains/article_opt/mechanism_research.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.article_opt.mechanism_research`/
symbols:
  MechanismResearcher.research: MechanismResearcher#research().
  MechanismResearcher.validate: MechanismResearcher#validate().
  MechanismResearcher._generate_with_retries: MechanismResearcher#_generate_with_retries().
  MechanismResearcher._save_summary: MechanismResearcher#_save_summary().
  MechanismResearcher._build_trace_summary: MechanismResearcher#_build_trace_summary().
  logger: logger.
  MechanismResearcher._save_code: MechanismResearcher#_save_code().
  MechanismResearcher._load_stage: MechanismResearcher#_load_stage().
  MechanismResult.session_id: MechanismResult#session_id.
  MechanismResearcher._get_explore_prompt: MechanismResearcher#_get_explore_prompt().
  MechanismResearcher._get_specify_prompt: MechanismResearcher#_get_specify_prompt().
  MechanismResearcher: MechanismResearcher#
  MechanismResult: MechanismResult#
  MechanismResult.article_id: MechanismResult#article_id.
  MechanismResult.stage_name: MechanismResult#stage_name.
  MechanismResult.inject_after: MechanismResult#inject_after.
  MechanismResult.domain_source: MechanismResult#domain_source.
  MechanismResult.stage_path: MechanismResult#stage_path.
  MechanismResult.code_retries: MechanismResult#code_retries.
  MechanismResearcher._generated_dir: MechanismResearcher#_generated_dir.
  MechanismResearcher.__init__: MechanismResearcher#__init__().
  MechanismResearcher._get_codegen_prompt: MechanismResearcher#_get_codegen_prompt().
  MechanismResearcher._get_reference_code: MechanismResearcher#_get_reference_code().
  EXPLORE_SYSTEM: EXPLORE_SYSTEM.
  EXPLORE_PROMPT: EXPLORE_PROMPT.
  SPECIFY_SYSTEM: SPECIFY_SYSTEM.
  SPECIFY_PROMPT: SPECIFY_PROMPT.
  CODEGEN_PROMPT: CODEGEN_PROMPT.
  MechanismResult.stage_class: MechanismResult#stage_class.
  MechanismResearcher._read_reference_stage: MechanismResearcher#_read_reference_stage().
  MechanismResult.hypothesis: MechanismResult#hypothesis.
  MechanismResult.spec: MechanismResult#spec.
  MechanismResult.code: MechanismResult#code.
  MechanismResult.exploration: MechanismResult#exploration.
  MechanismResult.critique: MechanismResult#critique.
  MechanismResult.validation: MechanismResult#validation.
  MechanismResearcher._build_lessons_summary: MechanismResearcher#_build_lessons_summary().
  MechanismResearcher._extract_selected: MechanismResearcher#_extract_selected().
  MechanismResearcher._parse_spec_metadata: MechanismResearcher#_parse_spec_metadata().
---
# Module: [`domains/article_opt/mechanism_research.py`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py)

## Classes
### `MechanismResearcher`  ·  implements/extends BaseMechanismResearcher
- def: [`domains/article_opt/mechanism_research.py:190`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L190) — documented in [core-base_mechanism_research](../../../concepts/core-base_mechanism_research.md)
- doc: Runs one Level-2 research session: produces + validates a new pipeline stage.
- signature: `class MechanismResearcher(BaseMechanismResearcher):`
- members:
  - `_extract_selected(self, exploration: str, critique: str)` — [`L417`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L417) — Pull the selected hypothesis from critique output, fall back to full exploration.
  - `_generate_with_retries(self, spec: str, reference_stage: str, session_dir: Path)` — [`L450`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L450) — Generate code, retrying with error feedback on failure. — documented in [core-base_mechanism_research](../../../concepts/core-base_mechanism_research.md)
  - `_load_stage(self, stage_path: Path, stage_name: str)` — [`L504`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L504) — Dynamically import the generated stage file and return the class. — documented in [domains-article_opt-mechanism_research](../../../concepts/domains-article_opt-mechanism_research.md)
  - `_parse_spec_metadata(self, spec: str, session_id: str)` — [`L426`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L426) — Extract inject_after and stage_name from spec text.
  - `_read_reference_stage(self)` — [`L532`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L532) — Read improvement_hypotheses.py as a style reference for code generation.
  - `_save_code(self, code: str, stage_name: str, session_dir: Path)` — [`L491`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L491) — Write code to the generated/ directory and return the path. — documented in [domains-article_opt-mechanism_research](../../../concepts/domains-article_opt-mechanism_research.md)
  - `research(self, article_id: str, inner_states: list[InnerLoopState], outer_lessons: list[dict])` — [`L223`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L223) — Run one full research session. Returns the result including the loaded stage. — documented in [core-base_mechanism_research](../../../concepts/core-base_mechanism_research.md)
  - `validate(self, result: MechanismResult, article_content: str, runner: InnerRunner, max_inner: int = 5)` — [`L317`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L317) — Run inner loop with the generated stage injected. Returns validation metrics. — documented in [core-inner_loop](../../../concepts/core-inner_loop.md)
- protocol/private: `__init__`[`L202`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L202), `_build_lessons_summary`[`L408`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L408), `_build_trace_summary`[`L397`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L397), `_generated_dir`[`L217`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L217), `_get_codegen_prompt`[`L387`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L387), `_get_explore_prompt`[`L362`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L362), `_get_reference_code`[`L390`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L390), `_get_specify_prompt`[`L373`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L373), `_save_summary`[`L539`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L539)
- uses (calls/refs, reference-scoped): [`call`](../../core/llm_client.md#LLMClient.call), [`run_cycle`](../../core/inner_loop.md#InnerLoopController.run_cycle), [`BaseStage`](pipeline/base.md#BaseStage), [`run_trace`](../../core/state.md#InnerLoopState.run_trace), [`inner_lessons`](../../core/state.md#InnerLoopState.inner_lessons), [`InnerLoopState`](../../core/state.md#InnerLoopState), [`BaseMechanismResearcher`](../../core/base_mechanism_research.md#BaseMechanismResearcher), [`overall`](../../core/state.md#RunResult.overall), [`client`](../../core/base_mechanism_research.md#BaseMechanismResearcher.client), [`inject_stage`](runner.md#InnerRunner.inject_stage), [`peak_score`](../../core/state.md#InnerLoopState.peak_score), [`InnerLoopController`](../../core/inner_loop.md#InnerLoopController), [`OuterLoopState`](../../core/state.md#OuterLoopState), [`runs_to_threshold`](../../core/state.md#InnerLoopState.runs_to_threshold), [`stage_map`](../../core/state.md#RunResult.stage_map), [`InnerRunner`](runner.md#InnerRunner), [`_strip_fences`](../../core/base_mechanism_research.md#BaseMechanismResearcher._strip_fences), [`_syntax_check`](../../core/base_mechanism_research.md#BaseMechanismResearcher._syntax_check), [`logger`](mechanism_research.md#logger), [`is_converged`](../../core/state.md#InnerLoopState.is_converged), [`max_code_retries`](../../core/base_mechanism_research.md#BaseMechanismResearcher.max_code_retries), [`begin_cycle`](../../core/state.md#OuterLoopState.begin_cycle), [`CODEGEN_SYSTEM`](../../core/base_mechanism_research.md#CODEGEN_SYSTEM), [`FIX_PROMPT`](../../core/base_mechanism_research.md#FIX_PROMPT), [`session_id`](mechanism_research.md#MechanismResult.session_id), [`MechanismResult`](mechanism_research.md#MechanismResult), [`article_id`](mechanism_research.md#MechanismResult.article_id), [`inject_after`](mechanism_research.md#MechanismResult.inject_after), [`stage_name`](mechanism_research.md#MechanismResult.stage_name), [`CRITIQUE_PROMPT`](../../core/base_mechanism_research.md#CRITIQUE_PROMPT), [`CRITIQUE_SYSTEM`](../../core/base_mechanism_research.md#CRITIQUE_SYSTEM), [`code_retries`](mechanism_research.md#MechanismResult.code_retries), [`domain_source`](mechanism_research.md#MechanismResult.domain_source), [`stage_path`](mechanism_research.md#MechanismResult.stage_path), [`CODEGEN_PROMPT`](mechanism_research.md#CODEGEN_PROMPT), [`EXPLORE_PROMPT`](mechanism_research.md#EXPLORE_PROMPT), [`EXPLORE_SYSTEM`](mechanism_research.md#EXPLORE_SYSTEM), [`SPECIFY_PROMPT`](mechanism_research.md#SPECIFY_PROMPT), [`SPECIFY_SYSTEM`](mechanism_research.md#SPECIFY_SYSTEM), [`__init__`](../../core/base_mechanism_research.md#BaseMechanismResearcher.__init__)  (+10 more)
- used by: [`cmd_mechresearch`](cli.md#cmd_mechresearch), [`_generate_with_retries`](../../core/base_mechanism_research.md#BaseMechanismResearcher._generate_with_retries), [`BaseMechanismResearcher`](../../core/base_mechanism_research.md#BaseMechanismResearcher), [`_extract_selected`](../../core/base_mechanism_research.md#BaseMechanismResearcher._extract_selected), [`_get_explore_prompt`](../../core/base_mechanism_research.md#BaseMechanismResearcher._get_explore_prompt), [`_get_codegen_prompt`](../../core/base_mechanism_research.md#BaseMechanismResearcher._get_codegen_prompt), [`_get_reference_code`](../../core/base_mechanism_research.md#BaseMechanismResearcher._get_reference_code), [`_get_specify_prompt`](../../core/base_mechanism_research.md#BaseMechanismResearcher._get_specify_prompt), [`_parse_spec_metadata`](../../core/base_mechanism_research.md#BaseMechanismResearcher._parse_spec_metadata)

### `MechanismResult`
- def: [`domains/article_opt/mechanism_research.py:169`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L169) — documented in [domains-article_opt-mechanism_research](../../../concepts/domains-article_opt-mechanism_research.md)
- signature: `class MechanismResult:`
- members:
  - `article_id` — [`L171`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L171)
  - `code` — [`L175`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L175)
  - `code_retries` — [`L182`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L182)
  - `critique` — [`L181`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L181)
  - `domain_source` — [`L173`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L173)
  - `exploration` — [`L180`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L180)
  - `hypothesis` — [`L172`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L172)
  - `inject_after` — [`L177`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L177) — documented in [domains-article_opt-mechanism_research](../../../concepts/domains-article_opt-mechanism_research.md)
  - `session_id` — [`L170`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L170)
  - `spec` — [`L174`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L174)
  - `stage_class` — [`L179`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L179)
  - `stage_name` — [`L176`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L176) — documented in [domains-article_opt-mechanism_research](../../../concepts/domains-article_opt-mechanism_research.md)
  - `stage_path` — [`L178`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L178)
  - `validation` — [`L183`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L183)
- used by: [`research`](mechanism_research.md#MechanismResearcher.research), [`cmd_mechresearch`](cli.md#cmd_mechresearch), [`validate`](mechanism_research.md#MechanismResearcher.validate), [`_save_summary`](mechanism_research.md#MechanismResearcher._save_summary)

## Module values
- `CODEGEN_PROMPT` — [`L111`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L111) — documented in [core-base_mechanism_research](../../../concepts/core-base_mechanism_research.md)
- `EXPLORE_PROMPT` — [`L54`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L54) — documented in [core-base_mechanism_research](../../../concepts/core-base_mechanism_research.md)
- `EXPLORE_SYSTEM` — [`L49`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L49) — documented in [core-base_mechanism_research](../../../concepts/core-base_mechanism_research.md)
- `SPECIFY_PROMPT` — [`L88`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L88) — documented in [core-base_mechanism_research](../../../concepts/core-base_mechanism_research.md)
- `SPECIFY_SYSTEM` — [`L85`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L85) — documented in [core-base_mechanism_research](../../../concepts/core-base_mechanism_research.md)
- `logger` — [`L43`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/mechanism_research.py#L43)


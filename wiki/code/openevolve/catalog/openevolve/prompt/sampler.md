---
title: 'Module: openevolve/prompt/sampler.py'
type: catalog
provenance: extracted
module: openevolve/prompt/sampler.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.prompt.sampler`/
symbols:
  PromptSampler.build_prompt: PromptSampler#build_prompt().
  PromptSampler.template_manager: PromptSampler#template_manager.
  PromptSampler.config: PromptSampler#config.
  PromptSampler._format_evolution_history: PromptSampler#_format_evolution_history().
  PromptSampler._extract_unique_features: PromptSampler#_extract_unique_features().
  PromptSampler._format_inspirations_section: PromptSampler#_format_inspirations_section().
  PromptSampler: PromptSampler#
  PromptSampler._identify_improvement_areas: PromptSampler#_identify_improvement_areas().
  PromptSampler._render_artifacts: PromptSampler#_render_artifacts().
  PromptSampler._determine_program_type: PromptSampler#_determine_program_type().
  PromptSampler._safe_decode_artifact: PromptSampler#_safe_decode_artifact().
  PromptSampler.set_templates: PromptSampler#set_templates().
  PromptSampler._apply_template_variations: PromptSampler#_apply_template_variations().
  PromptSampler.user_template_override: PromptSampler#user_template_override.
  logger: logger.
  PromptSampler.system_template_override: PromptSampler#system_template_override.
  PromptSampler.__init__: PromptSampler#__init__().
  PromptSampler._apply_security_filter: PromptSampler#_apply_security_filter().
  PromptSampler._format_metrics: PromptSampler#_format_metrics().
---
# Module: [`openevolve/prompt/sampler.py`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py)

## Classes
### `PromptSampler`
- def: [`openevolve/prompt/sampler.py:21`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L21)
- doc: Generates prompts for code evolution
- signature: `class PromptSampler:`
- members:
  - `_apply_security_filter(self, text: str)` — [`L662`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L662) — Apply security filtering to artifact text — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `_apply_template_variations(self, template: str)` — [`L595`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L595) — Apply stochastic variations to the template — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `_determine_program_type(self, program: Dict[str, Any], feature_dimensions: Optional[List[str]] = None)` — [`L501`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L501) — Determine the type/category of an inspiration program — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `_extract_unique_features(self, program: Dict[str, Any])` — [`L533`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L533) — Extract unique features of an inspiration program — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `_format_evolution_history(self, previous_programs: List[Dict[str, Any]], top_programs: List[Dict[str, Any]], inspirations: List[Dict[str, Any]], language: str, feature_dimensions: Optional[List[str]] = None)` — [`L248`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L248) — Format the evolution history for the prompt — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `_format_inspirations_section(self, inspirations: List[Dict[str, Any]], language: str, feature_dimensions: Optional[List[str]] = None)` — [`L441`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L441) — Format the inspirations section for the prompt — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `_format_metrics(self, metrics: Dict[str, float])` — [`L174`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L174) — Format metrics for the prompt using safe formatting — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `_identify_improvement_areas(self, current_program: str, parent_program: str, metrics: Dict[str, float], previous_programs: List[Dict[str, Any]], feature_dimensions: Optional[List[str]] = None)` — [`L188`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L188) — Identify improvement areas with proper fitness/feature separation — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `_render_artifacts(self, artifacts: Dict[str, Union[str, bytes]])` — [`L607`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L607) — Render artifacts for prompt inclusion — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `_safe_decode_artifact(self, value: Union[str, bytes])` — [`L636`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L636) — Safely decode an artifact value to string — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `build_prompt(self, current_program: str = "", parent_program: str = "", program_metrics: Dict[str, float] = {}, previous_programs: List[Dict[str, Any]] = [], top_programs: List[Dict[str, Any]] = [], inspirations: List[Dict[str, Any]] = [], language: str = "python", evolution_round: int = 0, diff_based_evolution: bool = True, template_key: Optional[str] = None, program_artifacts: Optional[Dict[str, Union[str, bytes]]] = None, feature_dimensions: Optional[List[str]] = None, current_changes_description: Optional[str] = None, **kwargs: Any)` — [`L51`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L51) — Build a prompt for the LLM — documented in [openevolve-controller](../../../concepts/openevolve-controller.md)
  - `set_templates(self, system_template: Optional[str] = None, user_template: Optional[str] = None)` — [`L37`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L37) — Set custom templates to use for this sampler
  - `config` — [`L25`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L25) — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `system_template_override` — [`L29`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L29) — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `template_manager` — [`L26`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L26) — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `user_template_override` — [`L30`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L30) — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
- protocol/private: `__init__`[`L24`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L24)
- uses (calls/refs, reference-scoped): [`get_fragment`](templates.md#TemplateManager.get_fragment), [`get_fitness_score`](../utils/metrics_utils.md#get_fitness_score), [`programs_as_changes_description`](../config.md#PromptConfig.programs_as_changes_description), [`PromptConfig`](../config.md#PromptConfig), [`get_template`](templates.md#TemplateManager.get_template), [`template_dir`](../config.md#PromptConfig.template_dir), [`num_top_programs`](../config.md#PromptConfig.num_top_programs), [`system_message_changes_description`](../config.md#PromptConfig.system_message_changes_description), [`templates`](templates.md#TemplateManager.templates), [`logger`](sampler.md#logger), [`TemplateManager`](templates.md#TemplateManager), [`format_feature_coordinates`](../utils/metrics_utils.md#format_feature_coordinates), [`num_diverse_programs`](../config.md#PromptConfig.num_diverse_programs), [`artifact_security_filter`](../config.md#PromptConfig.artifact_security_filter), [`comprehensive_implementation_min_lines`](../config.md#PromptConfig.comprehensive_implementation_min_lines), [`concise_implementation_max_lines`](../config.md#PromptConfig.concise_implementation_max_lines), [`include_artifacts`](../config.md#PromptConfig.include_artifacts), [`include_changes_under_chars`](../config.md#PromptConfig.include_changes_under_chars), [`max_artifact_bytes`](../config.md#PromptConfig.max_artifact_bytes), [`system_message`](../config.md#PromptConfig.system_message), [`code_length_threshold`](../config.md#PromptConfig.code_length_threshold), [`suggest_simplification_after_chars`](../config.md#PromptConfig.suggest_simplification_after_chars), [`template_variations`](../config.md#PromptConfig.template_variations), [`use_template_stochasticity`](../config.md#PromptConfig.use_template_stochasticity)
- used by: [`run_iteration_with_shared_db`](../iteration.md#run_iteration_with_shared_db), [`_run_iteration_worker`](../process_parallel.md#_run_iteration_worker), [`_llm_evaluate`](../evaluator.md#Evaluator._llm_evaluate), [`evaluator_prompt_sampler`](../controller.md#OpenEvolve.evaluator_prompt_sampler), [`_lazy_init_worker_components`](../process_parallel.md#_lazy_init_worker_components), [`__init__`](../evaluator.md#Evaluator.__init__), [`prompt_sampler`](../controller.md#OpenEvolve.prompt_sampler)  (26 test-only)

## Module values
- `logger` — [`L18`](../../../../../../raw/code/openevolve/openevolve/prompt/sampler.py#L18)


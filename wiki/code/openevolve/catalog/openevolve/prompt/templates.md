---
title: 'Module: openevolve/prompt/templates.py'
type: catalog
provenance: extracted
module: openevolve/prompt/templates.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.prompt.templates`/
symbols:
  TemplateManager.get_fragment: TemplateManager#get_fragment().
  DEFAULT_TEMPLATES: DEFAULT_TEMPLATES.
  TemplateManager.fragments: TemplateManager#fragments.
  TemplateManager.get_template: TemplateManager#get_template().
  TemplateManager._load_from_directory: TemplateManager#_load_from_directory().
  TemplateManager.templates: TemplateManager#templates.
  TemplateManager: TemplateManager#
  TemplateManager.custom_dir: TemplateManager#custom_dir.
  TemplateManager.add_template: TemplateManager#add_template().
  TemplateManager.add_fragment: TemplateManager#add_fragment().
  logger: logger.
  BASE_SYSTEM_TEMPLATE: BASE_SYSTEM_TEMPLATE.
  BASE_EVALUATOR_SYSTEM_TEMPLATE: BASE_EVALUATOR_SYSTEM_TEMPLATE.
  DIFF_USER_TEMPLATE: DIFF_USER_TEMPLATE.
  FULL_REWRITE_USER_TEMPLATE: FULL_REWRITE_USER_TEMPLATE.
  EVOLUTION_HISTORY_TEMPLATE: EVOLUTION_HISTORY_TEMPLATE.
  PREVIOUS_ATTEMPT_TEMPLATE: PREVIOUS_ATTEMPT_TEMPLATE.
  TOP_PROGRAM_TEMPLATE: TOP_PROGRAM_TEMPLATE.
  INSPIRATIONS_SECTION_TEMPLATE: INSPIRATIONS_SECTION_TEMPLATE.
  INSPIRATION_PROGRAM_TEMPLATE: INSPIRATION_PROGRAM_TEMPLATE.
  EVALUATION_TEMPLATE: EVALUATION_TEMPLATE.
  TemplateManager.default_dir: TemplateManager#default_dir.
  TemplateManager.__init__: TemplateManager#__init__().
---
# Module: [`openevolve/prompt/templates.py`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py)

## Classes
### `TemplateManager`
- def: [`openevolve/prompt/templates.py:175`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L175) — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
- doc: Manages templates with cascading override support
- signature: `class TemplateManager:`
- members:
  - `_load_from_directory(self, directory: Path)` — [`L199`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L199) — Load all templates and fragments from a directory — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `add_fragment(self, fragment_name: str, fragment: str)` — [`L236`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L236) — Add or update a fragment — documented in [openevolve-prompt-templates](../../../concepts/openevolve-prompt-templates.md)
  - `add_template(self, template_name: str, template: str)` — [`L232`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L232) — Add or update a template
  - `get_fragment(self, name: str, **kwargs)` — [`L223`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L223) — Get and format a fragment — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `get_template(self, name: str)` — [`L217`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L217) — Get a template by name — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `custom_dir` — [`L181`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L181) — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `default_dir` — [`L180`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L180) — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `fragments` — [`L185`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L185) — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
  - `templates` — [`L184`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L184) — documented in [openevolve-prompt-sampler](../../../concepts/openevolve-prompt-sampler.md)
- protocol/private: `__init__`[`L178`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L178)
- uses (calls/refs, reference-scoped): [`logger`](templates.md#logger)
- used by: [`build_prompt`](sampler.md#PromptSampler.build_prompt), [`template_manager`](sampler.md#PromptSampler.template_manager), [`_format_evolution_history`](sampler.md#PromptSampler._format_evolution_history), [`_extract_unique_features`](sampler.md#PromptSampler._extract_unique_features), [`_format_inspirations_section`](sampler.md#PromptSampler._format_inspirations_section), [`_identify_improvement_areas`](sampler.md#PromptSampler._identify_improvement_areas), [`_render_artifacts`](sampler.md#PromptSampler._render_artifacts), [`_determine_program_type`](sampler.md#PromptSampler._determine_program_type)

## Module values
- `BASE_EVALUATOR_SYSTEM_TEMPLATE` — [`L19`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L19) — documented in [openevolve-prompt-templates](../../../concepts/openevolve-prompt-templates.md)
- `BASE_SYSTEM_TEMPLATE` — [`L14`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L14) — documented in [openevolve-prompt-templates](../../../concepts/openevolve-prompt-templates.md)
- `DEFAULT_TEMPLATES` — [`L161`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L161) — documented in [openevolve-prompt-templates](../../../concepts/openevolve-prompt-templates.md)
- `DIFF_USER_TEMPLATE` — [`L23`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L23) — documented in [openevolve-prompt-templates](../../../concepts/openevolve-prompt-templates.md)
- `EVALUATION_TEMPLATE` — [`L139`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L139) — documented in [openevolve-prompt-templates](../../../concepts/openevolve-prompt-templates.md)
- `EVOLUTION_HISTORY_TEMPLATE` — [`L96`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L96) — documented in [openevolve-prompt-templates](../../../concepts/openevolve-prompt-templates.md)
- `FULL_REWRITE_USER_TEMPLATE` — [`L69`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L69) — documented in [openevolve-prompt-templates](../../../concepts/openevolve-prompt-templates.md)
- `INSPIRATIONS_SECTION_TEMPLATE` — [`L123`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L123) — documented in [openevolve-prompt-templates](../../../concepts/openevolve-prompt-templates.md)
- `INSPIRATION_PROGRAM_TEMPLATE` — [`L131`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L131) — documented in [openevolve-prompt-templates](../../../concepts/openevolve-prompt-templates.md)
- `PREVIOUS_ATTEMPT_TEMPLATE` — [`L108`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L108) — documented in [openevolve-prompt-templates](../../../concepts/openevolve-prompt-templates.md)
- `TOP_PROGRAM_TEMPLATE` — [`L115`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L115) — documented in [openevolve-prompt-templates](../../../concepts/openevolve-prompt-templates.md)
- `logger` — [`L11`](../../../../../../raw/code/openevolve/openevolve/prompt/templates.py#L11) — documented in [openevolve-prompt-templates](../../../concepts/openevolve-prompt-templates.md)


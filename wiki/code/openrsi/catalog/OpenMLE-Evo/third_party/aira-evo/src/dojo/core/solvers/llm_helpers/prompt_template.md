---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/prompt_template.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/prompt_template.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.core.solvers.llm_helpers.prompt_template`/JinjaPrompt#
symbols:
  JinjaPrompt.format: format().
  JinjaPrompt: ''
  JinjaPrompt.partial_variables: partial_variables.
  JinjaPrompt.template: template.
  JinjaPrompt.__init__: __init__().
  JinjaPrompt.input_variables: input_variables.
  JinjaPrompt.environment: environment.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/prompt_template.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/prompt_template.py)

## Classes
### `JinjaPrompt`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/prompt_template.py:13`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/prompt_template.py#L13)
- doc: This class can be used to generate prompts from jinja templates
- signature: `class JinjaPrompt:`
- members:
  - `format(self, **kwargs)` — [`L35`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/prompt_template.py#L35) — format the template with the given input variables
  - `environment` — [`L33`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/prompt_template.py#L33)
  - `input_variables` — [`L30`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/prompt_template.py#L30)
  - `partial_variables` — [`L31`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/prompt_template.py#L31)
  - `template` — [`L32`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/prompt_template.py#L32)
- protocol/private: `__init__`[`L27`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/prompt_template.py#L27)
- uses (calls/refs, reference-scoped): [`JinjaPromptConfig`](../../../config_dataclasses/llm/jinjaprompt.md#JinjaPromptConfig), [`input_variables`](../../../config_dataclasses/llm/jinjaprompt.md#JinjaPromptConfig.input_variables), [`partial_variables`](../../../config_dataclasses/llm/jinjaprompt.md#JinjaPromptConfig.partial_variables), [`template`](../../../config_dataclasses/llm/jinjaprompt.md#JinjaPromptConfig.template)
- used by: [`__call__`](generic_llm.md#GenericLLM.__call__), [`init_user_message_prompt_template`](generic_llm.md#GenericLLM.init_user_message_prompt_template), [`system_message_prompt_template`](generic_llm.md#GenericLLM.system_message_prompt_template), [`user_message_prompt_template`](generic_llm.md#GenericLLM.user_message_prompt_template)


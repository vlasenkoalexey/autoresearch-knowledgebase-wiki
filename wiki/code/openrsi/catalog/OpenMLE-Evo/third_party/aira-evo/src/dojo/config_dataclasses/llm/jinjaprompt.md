---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/jinjaprompt.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/jinjaprompt.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.config_dataclasses.llm.jinjaprompt`/JinjaPromptConfig#
symbols:
  JinjaPromptConfig: ''
  JinjaPromptConfig.validate: validate().
  JinjaPromptConfig.template: template.
  JinjaPromptConfig.input_variables: input_variables.
  JinjaPromptConfig.partial_variables: partial_variables.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/jinjaprompt.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/jinjaprompt.py)

## Classes
### `JinjaPromptConfig`  ·  implements/extends BaseConfig
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/jinjaprompt.py:15`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/jinjaprompt.py#L15)
- signature: `class JinjaPromptConfig(BaseConfig):`
- members:
  - `validate(self)` — [`L31`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/jinjaprompt.py#L31)
  - `input_variables` — [`L21`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/jinjaprompt.py#L21)
  - `partial_variables` — [`L26`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/jinjaprompt.py#L26)
  - `template` — [`L16`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/jinjaprompt.py#L16)
- uses (calls/refs, reference-scoped): [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate)
- used by: [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate), [`init_user_message_prompt_template`](../operators/base.md#OperatorConfig.init_user_message_prompt_template), [`partial_variables`](../../core/solvers/llm_helpers/prompt_template.md#JinjaPrompt.partial_variables), [`system_message_prompt_template`](../operators/base.md#OperatorConfig.system_message_prompt_template), [`template`](../../core/solvers/llm_helpers/prompt_template.md#JinjaPrompt.template), [`user_message_prompt_template`](../operators/base.md#OperatorConfig.user_message_prompt_template), [`__init__`](../../core/solvers/llm_helpers/prompt_template.md#JinjaPrompt.__init__), [`input_variables`](../../core/solvers/llm_helpers/prompt_template.md#JinjaPrompt.input_variables)


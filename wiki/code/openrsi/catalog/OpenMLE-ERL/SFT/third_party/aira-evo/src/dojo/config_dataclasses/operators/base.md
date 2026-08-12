---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/base.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/base.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.config_dataclasses.operators.base`/OperatorConfig#
symbols:
  OperatorConfig: ''
  OperatorConfig.llm: llm.
  OperatorConfig.system_message_prompt_template: system_message_prompt_template.
  OperatorConfig.init_user_message_prompt_template: init_user_message_prompt_template.
  OperatorConfig.user_message_prompt_template: user_message_prompt_template.
  OperatorConfig.validate: validate().
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/base.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/base.py)

## Classes
### `OperatorConfig`  ·  implements/extends BaseConfig
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/base.py:17`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/base.py#L17)
- signature: `class OperatorConfig(BaseConfig):`
- members:
  - `validate(self)` — [`L30`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/base.py#L30)
  - `init_user_message_prompt_template` — [`L27`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/base.py#L27)
  - `llm` — [`L18`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/base.py#L18)
  - `system_message_prompt_template` — [`L26`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/base.py#L26)
  - `user_message_prompt_template` — [`L28`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/base.py#L28)
- uses (calls/refs, reference-scoped): [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate), [`JinjaPromptConfig`](../llm/jinjaprompt.md#JinjaPromptConfig), [`GenericLLMConfig`](../llm/generic_llm.md#GenericLLMConfig)
- used by: [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate), [`operators`](../solver/base.md#SolverConfig.operators), [`client`](../../core/solvers/llm_helpers/generic_llm.md#GenericLLM.client), [`generation_kwargs`](../../core/solvers/llm_helpers/generic_llm.md#GenericLLM.generation_kwargs), [`init_user_message_prompt_template`](../../core/solvers/llm_helpers/generic_llm.md#GenericLLM.init_user_message_prompt_template), [`system_message_prompt_template`](../../core/solvers/llm_helpers/generic_llm.md#GenericLLM.system_message_prompt_template), [`user_message_prompt_template`](../../core/solvers/llm_helpers/generic_llm.md#GenericLLM.user_message_prompt_template), [`__init__`](../../core/solvers/llm_helpers/generic_llm.md#GenericLLM.__init__)


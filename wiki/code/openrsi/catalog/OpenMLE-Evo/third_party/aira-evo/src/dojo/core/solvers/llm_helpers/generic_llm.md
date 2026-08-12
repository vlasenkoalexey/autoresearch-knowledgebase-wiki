---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.core.solvers.llm_helpers.generic_llm`/
symbols:
  GenericLLM: GenericLLM#
  GenericLLM.__call__: GenericLLM#__call__().
  GenericLLM.client: GenericLLM#client.
  GenericLLM._query_client_with_limit: GenericLLM#_query_client_with_limit().
  GenericLLM.system_message_prompt_template: GenericLLM#system_message_prompt_template.
  GenericLLM.init_user_message_prompt_template: GenericLLM#init_user_message_prompt_template.
  GenericLLM.user_message_prompt_template: GenericLLM#user_message_prompt_template.
  GenericLLM.cfg: GenericLLM#cfg.
  GenericLLM.client_content_key: GenericLLM#client_content_key().
  GenericLLM.call_tracker: GenericLLM#call_tracker.
  GenericLLM.generation_kwargs: GenericLLM#generation_kwargs.
  GenericLLM.__init__: GenericLLM#__init__().
  GenericLLM.logger: GenericLLM#logger.
  log: log.
  GenericLLM._set_up_prompts: GenericLLM#_set_up_prompts().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py)

## Classes
### `GenericLLM`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py:26`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py#L26)
- signature: `class GenericLLM:`
- members:
  - `__call__(self, query_data: Optional[Dict[str, Any]] = None, messages: Optional[List[Dict[str, str]]] = None, no_user_message: bool = False, json_schema: Optional[str] = None, function_name: Optional[str] = None, function_description: Optional[str] = None)` — [`L85`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py#L85) — Makes a call to the LLM client with the provided query data or messages.
  - `__init__(self, cfg: OperatorConfig)` — [`L27`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py#L27) — Initializes the GenericLLM with the provided configuration.
  - `_set_up_prompts(self)` — [`L57`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py#L57) — Sets up the prompt templates by instantiating them using Hydra.
  - `client_content_key(self)` — [`L54`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py#L54)
  - `call_tracker` — [`L51`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py#L51)
  - `cfg` — [`L35`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py#L35)
  - `client` — [`L38`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py#L38)
  - `generation_kwargs` — [`L44`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py#L44)
  - `init_user_message_prompt_template` — [`L65`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py#L65)
  - `logger` — [`L49`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py#L49)
  - `system_message_prompt_template` — [`L64`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py#L64)
  - `user_message_prompt_template` — [`L66`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py#L66)
- protocol/private: `_query_client_with_limit`[`L68`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py#L68)
- uses (calls/refs, reference-scoped): [`get_logger`](../../../utils/logger.md#get_logger), [`query`](backends/open_ai.md#OpenAIClient.query), [`format`](prompt_template.md#JinjaPrompt.format), [`get_client`](backends/utils.md#get_client), [`OperatorConfig`](../../../config_dataclasses/operators/base.md#OperatorConfig), [`client_content_key`](backends/open_ai.md#OpenAIClient.client_content_key), [`JinjaPrompt`](prompt_template.md#JinjaPrompt), [`acquire_llm_slot`](../../../../../../../tts_search/airaevo_concurrency.md#acquire_llm_slot), [`llm`](../../../config_dataclasses/operators/base.md#OperatorConfig.llm), [`client`](../../../config_dataclasses/llm/generic_llm.md#GenericLLMConfig.client), [`init_user_message_prompt_template`](../../../config_dataclasses/operators/base.md#OperatorConfig.init_user_message_prompt_template), [`system_message_prompt_template`](../../../config_dataclasses/operators/base.md#OperatorConfig.system_message_prompt_template), [`user_message_prompt_template`](../../../config_dataclasses/operators/base.md#OperatorConfig.user_message_prompt_template), [`log`](generic_llm.md#log), [`generation_kwargs`](../../../config_dataclasses/llm/generic_llm.md#GenericLLMConfig.generation_kwargs)
- used by: [`improve_op`](../operators/improve.md#improve_op), [`debug_op`](../operators/debug.md#debug_op), [`crossover_op`](../operators/crossover.md#crossover_op), [`analyze_op`](../operators/analyze.md#analyze_op), [`rich_memory_summary_op`](../operators/rich_memory_summary.md#rich_memory_summary_op), [`draft_op`](../operators/draft.md#draft_op), [`setup_operators`](../../../solvers/evo/evo.md#Evolutionary.setup_operators), [`setup_operators`](../../../solvers/greedy/greedy.md#Greedy.setup_operators), [`setup_operators`](../../../solvers/mcts/mcts.md#MCTS.setup_operators)

## Module values
- `log` — [`L20`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/generic_llm.py#L20)


---
title: 'Module: rlm/core/types.py'
type: catalog
provenance: extracted
module: rlm/core/types.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.core.types`/
symbols:
  REPLResult.stderr: REPLResult#stderr.
  REPLResult.stdout: REPLResult#stdout.
  RLMChatCompletion.response: RLMChatCompletion#response.
  RLMChatCompletion: RLMChatCompletion#
  UsageSummary: UsageSummary#
  ModelUsageSummary: ModelUsageSummary#
  REPLResult: REPLResult#
  UsageSummary.model_usage_summaries: UsageSummary#model_usage_summaries.
  REPLResult.rlm_calls: REPLResult#rlm_calls.
  ModelUsageSummary.total_calls: ModelUsageSummary#total_calls.
  ModelUsageSummary.total_input_tokens: ModelUsageSummary#total_input_tokens.
  ModelUsageSummary.total_output_tokens: ModelUsageSummary#total_output_tokens.
  RLMIteration: RLMIteration#
  RLMChatCompletion.metadata: RLMChatCompletion#metadata.
  REPLResult.final_answer: REPLResult#final_answer.
  RLMChatCompletion.usage_summary: RLMChatCompletion#usage_summary.
  RLMChatCompletion.execution_time: RLMChatCompletion#execution_time.
  RLMChatCompletion.to_dict: RLMChatCompletion#to_dict().
  RLMChatCompletion.root_model: RLMChatCompletion#root_model.
  RLMChatCompletion.prompt: RLMChatCompletion#prompt.
  RLMMetadata.to_dict: RLMMetadata#to_dict().
  REPLResult.to_dict: REPLResult#to_dict().
  RLMIteration.code_blocks: RLMIteration#code_blocks.
  CodeBlock.result: CodeBlock#result.
  RLMIteration.response: RLMIteration#response.
  CodeBlock: CodeBlock#
  RLMIteration.to_dict: RLMIteration#to_dict().
  _serialize_value: _serialize_value().
  RLMIteration.prompt: RLMIteration#prompt.
  QueryMetadata.context_lengths: QueryMetadata#context_lengths.
  REPLResult.__init__: REPLResult#__init__().
  REPLResult.__str__: REPLResult#__str__().
  ModelUsageSummary.to_dict: ModelUsageSummary#to_dict().
  UsageSummary.to_dict: UsageSummary#to_dict().
  RLMChatCompletion.from_dict: RLMChatCompletion#from_dict().
  UsageSummary.total_cost: UsageSummary#total_cost().
  REPLResult.locals: REPLResult#locals.
  CodeBlock.code: CodeBlock#code.
  RLMMetadata: RLMMetadata#
  QueryMetadata: QueryMetadata#
  UsageSummary.from_dict: UsageSummary#from_dict().
  CodeBlock.to_dict: CodeBlock#to_dict().
  QueryMetadata.__init__: QueryMetadata#__init__().
  ClientBackend: ClientBackend.
  ModelUsageSummary.total_cost: ModelUsageSummary#total_cost.
  REPLResult.execution_time: REPLResult#execution_time.
  UsageSummary.total_input_tokens: UsageSummary#total_input_tokens().
  UsageSummary.total_output_tokens: UsageSummary#total_output_tokens().
  RLMIteration.final_answer: RLMIteration#final_answer.
  QueryMetadata.context_type: QueryMetadata#context_type.
  RLMChatCompletion.error: RLMChatCompletion#error.
  ModelUsageSummary.from_dict: ModelUsageSummary#from_dict().
  RLMIteration.iteration_time: RLMIteration#iteration_time.
  RLMMetadata.max_depth: RLMMetadata#max_depth.
  RLMMetadata.max_iterations: RLMMetadata#max_iterations.
  RLMMetadata.backend: RLMMetadata#backend.
  RLMMetadata.backend_kwargs: RLMMetadata#backend_kwargs.
  RLMMetadata.environment_type: RLMMetadata#environment_type.
  RLMMetadata.other_backends: RLMMetadata#other_backends.
  RLMMetadata.root_model: RLMMetadata#root_model.
  RLMMetadata.environment_kwargs: RLMMetadata#environment_kwargs.
  QueryMetadata.context_total_length: QueryMetadata#context_total_length.
  REPLResult.llm_calls: REPLResult#llm_calls.
  EnvironmentType: EnvironmentType.
---
# Module: [`rlm/core/types.py`](../../../../../../raw/code/rlm/rlm/core/types.py)

## Classes
### `CodeBlock`
- def: [`rlm/core/types.py:200`](../../../../../../raw/code/rlm/rlm/core/types.py#L200)
- signature: `class CodeBlock:`
- members:
  - `to_dict(self)` — [`L204`](../../../../../../raw/code/rlm/rlm/core/types.py#L204)
  - `code` — [`L201`](../../../../../../raw/code/rlm/rlm/core/types.py#L201)
  - `result` — [`L202`](../../../../../../raw/code/rlm/rlm/core/types.py#L202)
- uses (calls/refs, reference-scoped): [`REPLResult`](types.md#REPLResult), [`to_dict`](types.md#REPLResult.to_dict)
- used by: [`completion`](rlm.md#RLM.completion), [`_check_iteration_limits`](rlm.md#RLM._check_iteration_limits), [`print_iteration`](../logger/verbose.md#VerbosePrinter.print_iteration), [`print_code_execution`](../logger/verbose.md#VerbosePrinter.print_code_execution), [`_completion_turn`](rlm.md#RLM._completion_turn), [`code_blocks`](types.md#RLMIteration.code_blocks), [`format_iteration`](../utils/parsing.md#format_iteration), [`to_dict`](types.md#RLMIteration.to_dict)  (7 test-only)

### `ModelUsageSummary`
- def: [`rlm/core/types.py:43`](../../../../../../raw/code/rlm/rlm/core/types.py#L43) — documented in [rlm-clients-base_lm](../../../concepts/rlm-clients-base_lm.md)
- signature: `class ModelUsageSummary:`
- members:
  - `from_dict(cls, data: dict)` — [`L60`](../../../../../../raw/code/rlm/rlm/core/types.py#L60)
  - `to_dict(self)` — [`L49`](../../../../../../raw/code/rlm/rlm/core/types.py#L49)
  - `total_calls` — [`L44`](../../../../../../raw/code/rlm/rlm/core/types.py#L44)
  - `total_cost` — [`L47`](../../../../../../raw/code/rlm/rlm/core/types.py#L47)
  - `total_input_tokens` — [`L45`](../../../../../../raw/code/rlm/rlm/core/types.py#L45)
  - `total_output_tokens` — [`L46`](../../../../../../raw/code/rlm/rlm/core/types.py#L46)
- used by: [`model_usage_summaries`](types.md#UsageSummary.model_usage_summaries), [`get_last_usage`](../clients/base_lm.md#BaseLM.get_last_usage), [`get_usage_summary`](../clients/openai.md#OpenAIClient.get_usage_summary), [`get_usage_summary`](../clients/gemini.md#GeminiClient.get_usage_summary), [`get_usage_summary`](../clients/anthropic.md#AnthropicClient.get_usage_summary), [`get_usage_summary`](../clients/azure_openai.md#AzureOpenAIClient.get_usage_summary), [`get_usage_summary`](../clients/portkey.md#PortkeyClient.get_usage_summary), [`get_last_usage`](../clients/openai.md#OpenAIClient.get_last_usage), [`get_last_usage`](../clients/gemini.md#GeminiClient.get_last_usage), [`get_last_usage`](../clients/anthropic.md#AnthropicClient.get_last_usage), [`get_last_usage`](../clients/azure_openai.md#AzureOpenAIClient.get_last_usage), [`get_last_usage`](../clients/portkey.md#PortkeyClient.get_last_usage), [`to_dict`](types.md#UsageSummary.to_dict), [`total_cost`](types.md#UsageSummary.total_cost), [`from_dict`](types.md#UsageSummary.from_dict), [`total_input_tokens`](types.md#UsageSummary.total_input_tokens), [`total_output_tokens`](types.md#UsageSummary.total_output_tokens)  (27 test-only)

### `QueryMetadata`
- def: [`rlm/core/types.py:265`](../../../../../../raw/code/rlm/rlm/core/types.py#L265)
- signature: `class QueryMetadata:`
- members:
  - `context_lengths` — [`L266`](../../../../../../raw/code/rlm/rlm/core/types.py#L266)
  - `context_total_length` — [`L267`](../../../../../../raw/code/rlm/rlm/core/types.py#L267)
  - `context_type` — [`L268`](../../../../../../raw/code/rlm/rlm/core/types.py#L268)
- protocol/private: `__init__`[`L270`](../../../../../../raw/code/rlm/rlm/core/types.py#L270)
- used by: [`setup_state`](../../training/src/rlm_train/env.md#RLMTrainEnv.setup_state), [`_setup_prompt`](rlm.md#RLM._setup_prompt), [`build_rlm_system_prompt`](../utils/prompts.md#build_rlm_system_prompt)  (2 test-only)

### `REPLResult`
- def: [`rlm/core/types.py:161`](../../../../../../raw/code/rlm/rlm/core/types.py#L161) — documented in [rlm-core-rlm](../../../concepts/rlm-core-rlm.md)
- signature: `class REPLResult:`
- members:
  - `to_dict(self)` — [`L188`](../../../../../../raw/code/rlm/rlm/core/types.py#L188)
  - `execution_time` — [`L165`](../../../../../../raw/code/rlm/rlm/core/types.py#L165)
  - `final_answer` — [`L167`](../../../../../../raw/code/rlm/rlm/core/types.py#L167)
  - `llm_calls` — [`L166`](../../../../../../raw/code/rlm/rlm/core/types.py#L166)
  - `locals` — [`L164`](../../../../../../raw/code/rlm/rlm/core/types.py#L164)
  - `rlm_calls` — [`L182`](../../../../../../raw/code/rlm/rlm/core/types.py#L182)
  - `stderr` — [`L163`](../../../../../../raw/code/rlm/rlm/core/types.py#L163) — documented in [rlm-core-types](../../../concepts/rlm-core-types.md)
  - `stdout` — [`L162`](../../../../../../raw/code/rlm/rlm/core/types.py#L162) — documented in [rlm-core-types](../../../concepts/rlm-core-types.md)
- protocol/private: `__init__`[`L169`](../../../../../../raw/code/rlm/rlm/core/types.py#L169), `__str__`[`L185`](../../../../../../raw/code/rlm/rlm/core/types.py#L185)
- uses (calls/refs, reference-scoped): [`RLMChatCompletion`](types.md#RLMChatCompletion), [`to_dict`](types.md#RLMChatCompletion.to_dict), [`_serialize_value`](types.md#_serialize_value)
- used by: [`completion`](rlm.md#RLM.completion), [`execute_code`](../environments/local_repl.md#LocalREPL.execute_code), [`execute_code`](../environments/docker_repl.md#DockerREPL.execute_code), [`execute_code`](../environments/ipython_repl.md#IPythonREPL.execute_code), [`_check_iteration_limits`](rlm.md#RLM._check_iteration_limits), [`_setup_subprocess`](../environments/ipython_repl.md#IPythonREPL._setup_subprocess), [`print_iteration`](../logger/verbose.md#VerbosePrinter.print_iteration), [`print_code_execution`](../logger/verbose.md#VerbosePrinter.print_code_execution), [`_completion_turn`](rlm.md#RLM._completion_turn), [`execute_code`](../environments/daytona_repl.md#DaytonaREPL.execute_code), [`execute_code`](../environments/modal_repl.md#ModalREPL.execute_code), [`_execute_in_process`](../environments/ipython_repl.md#IPythonREPL._execute_in_process), [`add_context`](../environments/ipython_repl.md#IPythonREPL.add_context), [`add_history`](../environments/ipython_repl.md#IPythonREPL.add_history), [`execute_code`](../environments/prime_repl.md#PrimeREPL.execute_code), [`_execute_in_kernel_locked`](../environments/ipython_repl.md#IPythonREPL._execute_in_kernel_locked), [`result`](types.md#CodeBlock.result), [`format_execution_result`](../utils/parsing.md#format_execution_result), [`_execute_in_kernel`](../environments/ipython_repl.md#IPythonREPL._execute_in_kernel), [`execute_code`](../environments/e2b_repl.md#E2BREPL.execute_code), [`execute_code`](../environments/base_env.md#IsolatedEnv.execute_code), [`_inject_custom_tools_subprocess`](../environments/ipython_repl.md#IPythonREPL._inject_custom_tools_subprocess), [`execute_code`](../environments/base_env.md#NonIsolatedEnv.execute_code), [`to_dict`](types.md#CodeBlock.to_dict), [`execute_code`](../environments/base_env.md#BaseEnv.execute_code)  (158 test-only)

### `RLMChatCompletion`
- def: [`rlm/core/types.py:118`](../../../../../../raw/code/rlm/rlm/core/types.py#L118) — documented in [rlm-core-lm_handler](../../../concepts/rlm-core-lm_handler.md)
- doc: Record of a single LLM call made from within the environment.
- signature: `class RLMChatCompletion:`
- members:
  - `from_dict(cls, data: dict)` — [`L148`](../../../../../../raw/code/rlm/rlm/core/types.py#L148)
  - `to_dict(self)` — [`L133`](../../../../../../raw/code/rlm/rlm/core/types.py#L133)
  - `error` — [`L129`](../../../../../../raw/code/rlm/rlm/core/types.py#L129)
  - `execution_time` — [`L125`](../../../../../../raw/code/rlm/rlm/core/types.py#L125)
  - `metadata` — [`L126`](../../../../../../raw/code/rlm/rlm/core/types.py#L126)
  - `prompt` — [`L122`](../../../../../../raw/code/rlm/rlm/core/types.py#L122)
  - `response` — [`L123`](../../../../../../raw/code/rlm/rlm/core/types.py#L123) — documented in [rlm-core-types](../../../concepts/rlm-core-types.md)
  - `root_model` — [`L121`](../../../../../../raw/code/rlm/rlm/core/types.py#L121)
  - `usage_summary` — [`L124`](../../../../../../raw/code/rlm/rlm/core/types.py#L124)
- uses (calls/refs, reference-scoped): [`UsageSummary`](types.md#UsageSummary), [`to_dict`](types.md#UsageSummary.to_dict), [`from_dict`](types.md#UsageSummary.from_dict)
- used by: [`completion`](rlm.md#RLM.completion), [`_subcall`](rlm.md#RLM._subcall), [`send_lm_request_batched`](comms_utils.md#send_lm_request_batched), [`_handle_batched`](lm_handler.md#LMRequestHandler._handle_batched), [`_setup_subprocess`](../environments/ipython_repl.md#IPythonREPL._setup_subprocess), [`_handle_single`](lm_handler.md#LMRequestHandler._handle_single), [`print_iteration`](../logger/verbose.md#VerbosePrinter.print_iteration), [`chat_completion`](comms_utils.md#LMResponse.chat_completion), [`_handle_llm_request`](../environments/daytona_repl.md#DaytonaREPL._handle_llm_request), [`_handle_llm_request`](../environments/modal_repl.md#ModalREPL._handle_llm_request), [`_handle_llm_request`](../environments/prime_repl.md#PrimeREPL._handle_llm_request), [`_handle_single`](../environments/docker_repl.md#LLMProxyHandler._handle_single), [`_llm_query`](../environments/ipython_repl.md#IPythonREPL._llm_query), [`_llm_query`](../environments/local_repl.md#LocalREPL._llm_query), [`_handle_llm_request`](../environments/e2b_repl.md#E2BREPL._handle_llm_request), [`_dispatch`](../environments/ipython_repl.md#_SubcallBroker._dispatch), [`_handle_batched`](../environments/docker_repl.md#LLMProxyHandler._handle_batched), [`_llm_query_batched`](../environments/ipython_repl.md#IPythonREPL._llm_query_batched), [`_llm_query_batched`](../environments/local_repl.md#LocalREPL._llm_query_batched), [`_rlm_query_batched`](../environments/ipython_repl.md#IPythonREPL._rlm_query_batched), [`to_dict`](types.md#REPLResult.to_dict), [`_rlm_query_batched`](../environments/local_repl.md#LocalREPL._rlm_query_batched), [`_handle_rlm_batched`](../environments/docker_repl.md#LLMProxyHandler._handle_rlm_batched), [`_rlm_query`](../environments/ipython_repl.md#IPythonREPL._rlm_query), [`_handle_rlm_single`](../environments/docker_repl.md#LLMProxyHandler._handle_rlm_single), [`__init__`](types.md#REPLResult.__init__), [`_rlm_query`](../environments/local_repl.md#LocalREPL._rlm_query), [`_tracked_subcall`](../environments/ipython_repl.md#IPythonREPL._tracked_subcall), [`drain`](../environments/ipython_repl.md#_SubcallBroker.drain), [`to_dict`](comms_utils.md#LMResponse.to_dict), [`_run_inprocess_subcall`](../environments/ipython_repl.md#IPythonREPL._run_inprocess_subcall), [`_pending_llm_calls`](../environments/ipython_repl.md#IPythonREPL._pending_llm_calls), [`_pending_llm_calls`](../environments/local_repl.md#LocalREPL._pending_llm_calls), [`_run_subcall`](../environments/ipython_repl.md#_SubcallBroker._run_subcall), [`from_dict`](comms_utils.md#LMResponse.from_dict), [`__init__`](../environments/ipython_repl.md#IPythonREPL.__init__), [`_completions_by_cell`](../environments/ipython_repl.md#_SubcallBroker._completions_by_cell), [`chat_completions`](comms_utils.md#LMResponse.chat_completions), [`pending_llm_calls`](../environments/daytona_repl.md#DaytonaREPL.pending_llm_calls), [`pending_llm_calls`](../environments/e2b_repl.md#E2BREPL.pending_llm_calls)  (+15 more; 46 test-only)

### `RLMIteration`
- def: [`rlm/core/types.py:209`](../../../../../../raw/code/rlm/rlm/core/types.py#L209) — documented in [rlm-core-rlm](../../../concepts/rlm-core-rlm.md)
- signature: `class RLMIteration:`
- members:
  - `to_dict(self)` — [`L216`](../../../../../../raw/code/rlm/rlm/core/types.py#L216)
  - `code_blocks` — [`L212`](../../../../../../raw/code/rlm/rlm/core/types.py#L212)
  - `final_answer` — [`L213`](../../../../../../raw/code/rlm/rlm/core/types.py#L213)
  - `iteration_time` — [`L214`](../../../../../../raw/code/rlm/rlm/core/types.py#L214)
  - `prompt` — [`L210`](../../../../../../raw/code/rlm/rlm/core/types.py#L210)
  - `response` — [`L211`](../../../../../../raw/code/rlm/rlm/core/types.py#L211)
- uses (calls/refs, reference-scoped): [`CodeBlock`](types.md#CodeBlock), [`to_dict`](types.md#CodeBlock.to_dict)
- used by: [`completion`](rlm.md#RLM.completion), [`_check_iteration_limits`](rlm.md#RLM._check_iteration_limits), [`print_iteration`](../logger/verbose.md#VerbosePrinter.print_iteration), [`_completion_turn`](rlm.md#RLM._completion_turn), [`_default_answer`](rlm.md#RLM._default_answer), [`format_iteration`](../utils/parsing.md#format_iteration), [`log`](../logger/rlm_logger.md#RLMLogger.log)  (11 test-only)

### `RLMMetadata`
- def: [`rlm/core/types.py:232`](../../../../../../raw/code/rlm/rlm/core/types.py#L232)
- doc: Metadata about the RLM configuration.
- signature: `class RLMMetadata:`
- members:
  - `to_dict(self)` — [`L244`](../../../../../../raw/code/rlm/rlm/core/types.py#L244)
  - `backend` — [`L238`](../../../../../../raw/code/rlm/rlm/core/types.py#L238)
  - `backend_kwargs` — [`L239`](../../../../../../raw/code/rlm/rlm/core/types.py#L239)
  - `environment_kwargs` — [`L241`](../../../../../../raw/code/rlm/rlm/core/types.py#L241)
  - `environment_type` — [`L240`](../../../../../../raw/code/rlm/rlm/core/types.py#L240)
  - `max_depth` — [`L236`](../../../../../../raw/code/rlm/rlm/core/types.py#L236)
  - `max_iterations` — [`L237`](../../../../../../raw/code/rlm/rlm/core/types.py#L237)
  - `other_backends` — [`L242`](../../../../../../raw/code/rlm/rlm/core/types.py#L242)
  - `root_model` — [`L235`](../../../../../../raw/code/rlm/rlm/core/types.py#L235)
- uses (calls/refs, reference-scoped): [`_serialize_value`](types.md#_serialize_value)
- used by: [`_persistent_env`](rlm.md#RLM._persistent_env), [`print_metadata`](../logger/verbose.md#VerbosePrinter.print_metadata), [`log_metadata`](../logger/rlm_logger.md#RLMLogger.log_metadata)  (2 test-only)

### `UsageSummary`
- def: [`rlm/core/types.py:70`](../../../../../../raw/code/rlm/rlm/core/types.py#L70) — documented in [rlm-core-rlm](../../../concepts/rlm-core-rlm.md)
- signature: `class UsageSummary:`
- members:
  - `from_dict(cls, data: dict)` — [`L105`](../../../../../../raw/code/rlm/rlm/core/types.py#L105)
  - `to_dict(self)` — [`L93`](../../../../../../raw/code/rlm/rlm/core/types.py#L93)
  - `total_cost(self)` — [`L74`](../../../../../../raw/code/rlm/rlm/core/types.py#L74) — Aggregate cost across all models. Returns None if no cost data available.
  - `total_input_tokens(self)` — [`L84`](../../../../../../raw/code/rlm/rlm/core/types.py#L84) — Aggregate input tokens across all models.
  - `total_output_tokens(self)` — [`L89`](../../../../../../raw/code/rlm/rlm/core/types.py#L89) — Aggregate output tokens across all models.
  - `model_usage_summaries` — [`L71`](../../../../../../raw/code/rlm/rlm/core/types.py#L71)
- uses (calls/refs, reference-scoped): [`ModelUsageSummary`](types.md#ModelUsageSummary), [`total_input_tokens`](types.md#ModelUsageSummary.total_input_tokens), [`total_output_tokens`](types.md#ModelUsageSummary.total_output_tokens), [`to_dict`](types.md#ModelUsageSummary.to_dict), [`total_cost`](types.md#ModelUsageSummary.total_cost), [`from_dict`](types.md#ModelUsageSummary.from_dict)
- used by: [`completion`](rlm.md#RLM.completion), [`_subcall`](rlm.md#RLM._subcall), [`_check_iteration_limits`](rlm.md#RLM._check_iteration_limits), [`_handle_batched`](lm_handler.md#LMRequestHandler._handle_batched), [`_handle_single`](lm_handler.md#LMRequestHandler._handle_single), [`get_usage_summary`](../clients/base_lm.md#BaseLM.get_usage_summary), [`usage_summary`](types.md#RLMChatCompletion.usage_summary), [`get_usage_summary`](../clients/openai.md#OpenAIClient.get_usage_summary), [`to_dict`](types.md#RLMChatCompletion.to_dict), [`get_usage_summary`](../clients/gemini.md#GeminiClient.get_usage_summary), [`get_usage_summary`](../clients/anthropic.md#AnthropicClient.get_usage_summary), [`get_usage_summary`](../clients/azure_openai.md#AzureOpenAIClient.get_usage_summary), [`get_usage_summary`](../clients/portkey.md#PortkeyClient.get_usage_summary), [`get_usage_summary`](lm_handler.md#LMHandler.get_usage_summary), [`from_dict`](types.md#RLMChatCompletion.from_dict)  (28 test-only)

## Functions
- `_serialize_value(value: Any)` — [`L18`](../../../../../../raw/code/rlm/rlm/core/types.py#L18) — Convert a value to a JSON-serializable representation.

## Module values
- `ClientBackend` — [`L5`](../../../../../../raw/code/rlm/rlm/core/types.py#L5)
- `EnvironmentType` — [`L15`](../../../../../../raw/code/rlm/rlm/core/types.py#L15)


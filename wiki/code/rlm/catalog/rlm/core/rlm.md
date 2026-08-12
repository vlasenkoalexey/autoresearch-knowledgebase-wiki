---
title: 'Module: rlm/core/rlm.py'
type: catalog
provenance: extracted
module: rlm/core/rlm.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.core.rlm`/RLM#
symbols:
  RLM.completion: completion().
  RLM: ''
  RLM._subcall: _subcall().
  RLM._spawn_completion_context: _spawn_completion_context().
  RLM._persistent_env: _persistent_env.
  RLM._check_iteration_limits: _check_iteration_limits().
  RLM._completion_turn: _completion_turn().
  RLM.close: close().
  RLM._default_answer: _default_answer().
  RLM.__init__: __init__().
  RLM._setup_prompt: _setup_prompt().
  RLM._check_timeout: _check_timeout().
  RLM.verbose: verbose.
  RLM.logger: logger.
  RLM._fallback_answer: _fallback_answer().
  RLM.backend_kwargs: backend_kwargs.
  RLM._get_compaction_status: _get_compaction_status().
  RLM._consecutive_errors: _consecutive_errors.
  RLM._cumulative_cost: _cumulative_cost.
  RLM.persistent: persistent.
  RLM._compact_history: _compact_history().
  RLM.max_budget: max_budget.
  RLM.max_timeout: max_timeout.
  RLM.environment_type: environment_type.
  RLM.other_backends: other_backends.
  RLM.other_backend_kwargs: other_backend_kwargs.
  RLM.max_tokens: max_tokens.
  RLM.max_errors: max_errors.
  RLM._best_partial_answer: _best_partial_answer.
  RLM._completion_start_time: _completion_start_time.
  RLM._env_supports_persistence: _env_supports_persistence().
  RLM.system_prompt: system_prompt.
  RLM.backend: backend.
  RLM.custom_sub_tools: custom_sub_tools.
  RLM.compaction: compaction.
  RLM.max_depth: max_depth.
  RLM.max_iterations: max_iterations.
  RLM._validate_persistent_environment_support: _validate_persistent_environment_support().
  RLM.custom_tools: custom_tools.
  RLM.depth: depth.
  RLM.on_subcall_start: on_subcall_start.
  RLM.on_subcall_complete: on_subcall_complete.
  RLM._last_error: _last_error.
  RLM._should_compact: _should_compact().
  RLM.__enter__: __enter__().
  RLM.__exit__: __exit__().
  RLM.environment_kwargs: environment_kwargs.
  RLM.max_concurrent_subcalls: max_concurrent_subcalls.
  RLM.user_prologue: user_prologue.
  RLM.compaction_threshold_pct: compaction_threshold_pct.
  RLM.orchestrator: orchestrator.
  RLM.on_iteration_start: on_iteration_start.
  RLM.on_iteration_complete: on_iteration_complete.
---
# Module: [`rlm/core/rlm.py`](../../../../../../raw/code/rlm/rlm/core/rlm.py)

## Classes
### `RLM`
- def: [`rlm/core/rlm.py:41`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L41) — documented in [rlm-core-rlm](../../../concepts/rlm-core-rlm.md)
- doc: Recursive Language Model class that the user instantiates and runs on their tasks.
- signature: `class RLM:`
- members:
  - `__init__(self, backend: ClientBackend = "openai", backend_kwargs: dict[str, Any] | None = None, environment: EnvironmentType = "local", environment_kwargs: dict[str, Any] | None = None, depth: int = 0, max_depth: int = 1, max_iterations: int = 30, max_budget: float | None = None, max_timeout: float | None = None, max_tokens: int | None = None, max_errors: int | None = None, custom_system_prompt: str | None = None, other_backends: list[ClientBackend] | None = None, other_backend_kwargs: list[dict[str, Any]] | None = None, logger: RLMLogger | None = None, verbose: bool = False, persistent: bool = False, custom_tools: dict[str, Any] | None = None, custom_sub_tools: dict[str, Any] | None = None, compaction: bool = False, compaction_threshold_pct: float = 0.85, max_concurrent_subcalls: int = 4, on_subcall_start: Callable[[int, str, str], None] | None = None, on_subcall_complete: Callable[[int, str, float, str | None], None] | None = None, on_iteration_start: Callable[[int, int], None] | None = None, on_iteration_complete: Callable[[int, int, float], None] | None = None, sampling_args: dict[str, Any] | None = None, sub_sampling_args: dict[str, Any] | None = None, orchestrator: bool = True, user_prologue: str | None = None)` — [`L49`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L49) — Args:
  - `_check_iteration_limits(self, iteration: RLMIteration, iteration_num: int, lm_handler: LMHandler)` — [`L512`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L512) — Check error tracking, budget, and token limits after an iteration. — documented in [rlm-core-rlm](../../../concepts/rlm-core-rlm.md)
  - `_check_timeout(self, iteration: int, time_start: float)` — [`L492`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L492) — Raise TimeoutExceededError if the timeout has been exceeded.
  - `_compact_history(self, lm_handler: LMHandler, environment: BaseEnv, message_history: list[dict[str, Any]], compaction_count: int = 1)` — [`L602`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L602) — Summarize current trajectory, append summary to REPL history, and return
  - `_completion_turn(self, prompt: str | dict[str, Any], lm_handler: LMHandler, environment: BaseEnv)` — [`L646`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L646) — Perform a single iteration of the RLM, including prompting the model
  - `_default_answer(self, message_history: list[dict[str, Any]], lm_handler: LMHandler)` — [`L673`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L673) — Default behavior if the RLM runs out of iterations and does not find a final answer. — documented in [rlm-core-rlm](../../../concepts/rlm-core-rlm.md)
  - `_env_supports_persistence(env: BaseEnv)` — [`L898`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L898) — Check if an environment instance supports persistent mode methods.
  - `_fallback_answer(self, message: str | dict[str, Any])` — [`L698`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L698) — Fallback behavior if the RLM is actually at max depth, and should be treated as an LM.
  - `_get_compaction_status(self, message_history: list[dict[str, Any]])` — [`L587`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L587) — Return (current_tokens, threshold_tokens, max_tokens) for compaction.
  - `_setup_prompt(self, prompt: str | dict[str, Any], root_prompt: str | None = None)` — [`L300`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L300) — Setup the system prompt for the RLM. Also include metadata about the prompt and build — documented in [rlm-core-rlm](../../../concepts/rlm-core-rlm.md)
  - `_should_compact(self, message_history: list[dict[str, Any]])` — [`L597`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L597) — True when root message history is at or over the compaction threshold.
  - `_spawn_completion_context(self, prompt: str | dict[str, Any])` — [`L226`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L226) — Spawn an LM handler and environment for a single completion call. — documented in [rlm-core-lm_handler](../../../concepts/rlm-core-lm_handler.md)
  - `_subcall(self, prompt: str, model: str | None = None)` — [`L706`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L706) — Handle a subcall from the environment, potentially spawning a child RLM. — documented in [rlm-core-rlm](../../../concepts/rlm-core-rlm.md)
  - `_validate_persistent_environment_support(self)` — [`L872`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L872) — Validate that the configured environment type supports persistent mode.
  - `close(self)` — [`L902`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L902) — Clean up persistent environment. Call when done with multi-turn conversations. — documented in [rlm-core-rlm](../../../concepts/rlm-core-rlm.md)
  - `completion(self, prompt: str | dict[str, Any], root_prompt: str | None = None)` — [`L326`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L326) — Recursive Language Model completion call. This is the main entry point for querying an RLM, and — documented in [rlm-core-rlm](../../../concepts/rlm-core-rlm.md)
  - `backend` — [`L141`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L141)
  - `backend_kwargs` — [`L142`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L142)
  - `compaction` — [`L163`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L163)
  - `compaction_threshold_pct` — [`L164`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L164)
  - `custom_sub_tools` — [`L161`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L161)
  - `custom_tools` — [`L159`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L159)
  - `depth` — [`L167`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L167)
  - `environment_kwargs` — [`L144`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L144)
  - `environment_type` — [`L143`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L143)
  - `logger` — [`L181`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L181)
  - `max_budget` — [`L170`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L170)
  - `max_concurrent_subcalls` — [`L165`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L165)
  - `max_depth` — [`L168`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L168)
  - `max_errors` — [`L173`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L173)
  - `max_iterations` — [`L169`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L169)
  - `max_timeout` — [`L171`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L171)
  - `max_tokens` — [`L172`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L172)
  - `on_iteration_complete` — [`L188`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L188)
  - `on_iteration_start` — [`L187`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L187)
  - `on_subcall_complete` — [`L186`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L186)
  - `on_subcall_start` — [`L185`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L185)
  - `orchestrator` — [`L175`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L175)
  - `other_backend_kwargs` — [`L156`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L156)
  - `other_backends` — [`L155`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L155)
  - `persistent` — [`L198`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L198)
  - `system_prompt` — [`L174`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L174)
  - `user_prologue` — [`L180`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L180)
  - `verbose` — [`L182`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L182)
- protocol/private: `__enter__`[`L909`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L909), `__exit__`[`L912`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L912), `_best_partial_answer`[`L194`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L194), `_completion_start_time`[`L195`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L195), `_consecutive_errors`[`L192`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L192), `_cumulative_cost`[`L191`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L191), `_last_error`[`L193`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L193), `_persistent_env`[`L199`](../../../../../../raw/code/rlm/rlm/core/rlm.py#L199)
- uses (calls/refs, reference-scoped): [`stderr`](types.md#REPLResult.stderr), [`response`](types.md#RLMChatCompletion.response), [`RLMChatCompletion`](types.md#RLMChatCompletion), [`UsageSummary`](types.md#UsageSummary), [`BaseLM`](../clients/base_lm.md#BaseLM), [`REPLResult`](types.md#REPLResult), [`model_usage_summaries`](types.md#UsageSummary.model_usage_summaries), [`print_iteration`](../logger/verbose.md#VerbosePrinter.print_iteration), [`RLMIteration`](types.md#RLMIteration), [`get_last_usage`](../clients/base_lm.md#BaseLM.get_last_usage), [`metadata`](types.md#RLMChatCompletion.metadata), [`RLMLogger`](../logger/rlm_logger.md#RLMLogger), [`completion`](../clients/base_lm.md#BaseLM.completion), [`final_answer`](types.md#REPLResult.final_answer), [`usage_summary`](types.md#RLMChatCompletion.usage_summary), [`LMHandler`](lm_handler.md#LMHandler), [`execution_time`](types.md#RLMChatCompletion.execution_time), [`get_environment`](../environments/__init__.md#get_environment), [`get_client`](../clients/__init__.md#get_client), [`prompt`](types.md#RLMChatCompletion.prompt), [`root_model`](types.md#RLMChatCompletion.root_model), [`print_metadata`](../logger/verbose.md#VerbosePrinter.print_metadata), [`code_blocks`](types.md#RLMIteration.code_blocks), [`format_iteration`](../utils/parsing.md#format_iteration), [`start`](lm_handler.md#LMHandler.start), [`result`](types.md#CodeBlock.result), [`get_usage_summary`](lm_handler.md#LMHandler.get_usage_summary), [`response`](types.md#RLMIteration.response), [`build_rlm_system_prompt`](../utils/prompts.md#build_rlm_system_prompt), [`BaseEnv`](../environments/base_env.md#BaseEnv), [`CodeBlock`](types.md#CodeBlock), [`log`](../logger/rlm_logger.md#RLMLogger.log), [`print_final_answer`](../logger/verbose.md#VerbosePrinter.print_final_answer), [`log_metadata`](../logger/rlm_logger.md#RLMLogger.log_metadata), [`print_compaction`](../logger/verbose.md#VerbosePrinter.print_compaction), [`print_compaction_status`](../logger/verbose.md#VerbosePrinter.print_compaction_status), [`prompt`](types.md#RLMIteration.prompt), [`print_summary`](../logger/verbose.md#VerbosePrinter.print_summary), [`print_limit_exceeded`](../logger/verbose.md#VerbosePrinter.print_limit_exceeded), [`print_budget_exceeded`](../logger/verbose.md#VerbosePrinter.print_budget_exceeded)  (+45 more; 14 test-only)
- used by: (82 test-only callers)


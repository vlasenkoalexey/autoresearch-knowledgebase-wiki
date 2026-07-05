---
title: 'Module: core/llm_client.py'
type: catalog
provenance: extracted
module: core/llm_client.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `core.llm_client`/
symbols:
  parse_json_response: parse_json_response().
  LLMClient.call: LLMClient#call().
  LLMClient: LLMClient#
  call_llm: call_llm().
  PROVIDERS.PROVIDERS: PROVIDERS.PROVIDERS.
  configure: configure().
  LLMClient._client: LLMClient#_client.
  _strip_thinking_tags: _strip_thinking_tags().
  get_provider_info: get_provider_info().
  _provider_name._provider_name: _provider_name._provider_name.
  _get_openai_client: _get_openai_client().
  _get_anthropic_client: _get_anthropic_client().
  LLMClient._native_sdk: LLMClient#_native_sdk.
  LLMClient._api_key: LLMClient#_api_key.
  LLMClient._model: LLMClient#_model.
  _model_override._model_override: _model_override._model_override.
  _call_openai_compat: _call_openai_compat().
  _call_anthropic: _call_anthropic().
  logger: logger.
  _client_cache._client_cache: _client_cache._client_cache.
  _anthropic_client_cache._anthropic_client_cache: _anthropic_client_cache._anthropic_client_cache.
  _api_key._api_key: _api_key._api_key.
  LLMClient.__init__: LLMClient#__init__().
  LLMClient._base_url: LLMClient#_base_url.
---
# Module: [`core/llm_client.py`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py)

## Classes
### `LLMClient`
- def: [`core/llm_client.py:250`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L250) — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
- doc: Instance-level LLM client.
- signature: `class LLMClient:`
- members:
  - `call(self, prompt: str, system: str = None, max_tokens: int = 4096, max_retries: int = 3, retry_delay: float = 2)` — [`L273`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L273) — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
- protocol/private: `__init__`[`L259`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L259), `_api_key`[`L263`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L263), `_base_url`[`L265`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L265), `_client`[`L269`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L269), `_model`[`L264`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L264), `_native_sdk`[`L266`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L266)
- uses (calls/refs, reference-scoped): [`PROVIDERS`](llm_client.md#PROVIDERS.PROVIDERS), [`_strip_thinking_tags`](llm_client.md#_strip_thinking_tags), [`_get_anthropic_client`](llm_client.md#_get_anthropic_client), [`_get_openai_client`](llm_client.md#_get_openai_client), [`logger`](llm_client.md#logger)
- used by: [`_propose`](../domains/train_opt/runner.md#TrainRunner._propose), [`run_group_d`](../experiments/ablations/paper_ablation/run_ablation.md#run_group_d), [`research`](../domains/article_opt/mechanism_research.md#MechanismResearcher.research), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/05_patched_runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/05_patched_runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_after_cycles_1_2.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_after_cycles_3_4.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_after_cycles_5_6.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C1/runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/05_patched_runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_1_2.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_5_6.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_final.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C2/runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/05_patched_runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C3/runner_after_cycles_1_2.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C3/runner_after_cycles_3_4.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C3/runner_after_cycles_5_6.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C3/runner_final.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.md#TrainRunner._propose), [`research`](../domains/train_opt/mechanism_research.md#TrainMechanismResearcher.research), [`run_group_c`](../experiments/ablations/paper_ablation/run_ablation.md#run_group_c), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_A/A1/runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_A/A2/runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_A/A3/runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_B/B1/runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_B/B2/runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_D/D1/runner_after_batch_1.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_D/D1/runner_after_batch_2.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_D/D1/runner_after_batch_3.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_D/D1/runner_final.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_D/D1/runner.md#TrainRunner._propose), [`_propose`](../experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.md#TrainRunner._propose)  (+72 more)

## Functions
- `_call_anthropic(prompt: str, system: str, model: str, max_tokens: int, api_key: str)` — [`L163`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L163)
- `_call_openai_compat(prompt: str, system: str, model: str, max_tokens: int, api_key: str, base_url: str)` — [`L144`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L144)
- `_get_anthropic_client(api_key: str)` — [`L33`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L33) — Get or create a cached Anthropic client for this api_key.
- `_get_openai_client(api_key: str, base_url: str)` — [`L25`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L25) — Get or create a cached OpenAI client for this (api_key, base_url) pair.
- `_strip_thinking_tags(text: str)` — [`L174`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L174) — Remove <think>...</think> reasoning blocks that some models include in output.
- `call_llm(prompt: str, system: str = None, model: str = "", max_tokens: int = 4096, max_retries: int = 3, retry_delay: float = 2)` — [`L103`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L103) — Call the configured LLM provider with automatic retry. — documented in [core-llm_client](../../concepts/core-llm_client.md)
- `configure(provider: str, api_key: str, model: str = "")` — [`L84`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L84) — Configure the global LLM client. Call once at startup. — documented in [domains-article_opt-cli](../../concepts/domains-article_opt-cli.md)
- `get_provider_info()` — [`L94`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L94) — Return current provider info (for display).
- `parse_json_response(text: str)` — [`L187`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L187) — Robustly parse JSON from an LLM response. — documented in [core-llm_client](../../concepts/core-llm_client.md)

## Module values
- `PROVIDERS` — [`L45`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L45) — documented in [core-llm_client](../../concepts/core-llm_client.md)
- `_anthropic_client_cache` — [`L22`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L22)
- `_api_key` — [`L80`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L80)
- `_client_cache` — [`L21`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L21)
- `_model_override` — [`L81`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L81)
- `_provider_name` — [`L79`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L79)
- `logger` — [`L18`](../../../../../raw/code/bilevel-autoresearch/core/llm_client.py#L18)


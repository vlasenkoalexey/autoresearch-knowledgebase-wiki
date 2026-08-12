---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.core.solvers.llm_helpers.backends.data_types`/
symbols:
  APIStats: APIStats#
  APIStats.__add__: APIStats#__add__().
  APIStats.replace: APIStats#replace().
  ModelArguments: ModelArguments#
  ModelArguments.model_name: ModelArguments#model_name.
  ModelArguments.per_instance_cost_limit: ModelArguments#per_instance_cost_limit.
  ModelArguments.total_cost_limit: ModelArguments#total_cost_limit.
  ModelArguments.temperature: ModelArguments#temperature.
  ModelArguments.top_p: ModelArguments#top_p.
  ModelArguments.replay_path: ModelArguments#replay_path.
  ModelArguments.host_url: ModelArguments#host_url.
  APIStats.total_cost: APIStats#total_cost.
  APIStats.task_cost: APIStats#task_cost.
  APIStats.tokens_sent: APIStats#tokens_sent.
  APIStats.tokens_received: APIStats#tokens_received.
  APIStats.api_calls: APIStats#api_calls.
  ContextWindowExceededError: ContextWindowExceededError#
  CostLimitExceededError: CostLimitExceededError#
  APIError: APIError#
  RateLimitExceededError: RateLimitExceededError#
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py)

## Classes
### `APIError`  ·  implements/extends Exception
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py:71`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L71)
- signature: `class APIError(Exception):`

### `APIStats`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py:39`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L39)
- signature: `class APIStats:`
- members:
  - `replace(self, other)` — [`L55`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L55)
  - `api_calls` — [`L44`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L44)
  - `task_cost` — [`L41`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L41)
  - `tokens_received` — [`L43`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L43)
  - `tokens_sent` — [`L42`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L42)
  - `total_cost` — [`L40`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L40)
- protocol/private: `__add__`[`L46`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L46)

### `ContextWindowExceededError`  ·  implements/extends Exception
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py:63`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L63)
- signature: `class ContextWindowExceededError(Exception):`

### `CostLimitExceededError`  ·  implements/extends Exception
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py:67`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L67)
- signature: `class CostLimitExceededError(Exception):`

### `ModelArguments`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py:19`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L19)
- doc: Arguments configuring the model and it's behavior.
- signature: `class ModelArguments:`
- members:
  - `host_url` — [`L35`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L35)
  - `model_name` — [`L23`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L23)
  - `per_instance_cost_limit` — [`L25`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L25)
  - `replay_path` — [`L33`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L33)
  - `temperature` — [`L29`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L29)
  - `top_p` — [`L31`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L31)
  - `total_cost_limit` — [`L27`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L27)

### `RateLimitExceededError`  ·  implements/extends Exception
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py:75`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/data_types.py#L75)
- signature: `class RateLimitExceededError(Exception):`


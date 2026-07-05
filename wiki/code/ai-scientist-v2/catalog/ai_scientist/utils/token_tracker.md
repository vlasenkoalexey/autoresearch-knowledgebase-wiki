---
title: 'Module: ai_scientist/utils/token_tracker.py'
type: catalog
provenance: extracted
module: ai_scientist/utils/token_tracker.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.utils.token_tracker`/
symbols:
  track_token_usage: track_token_usage().
  token_tracker: token_tracker.
  track_token_usage.async_wrapper: track_token_usage().async_wrapper().
  track_token_usage.sync_wrapper: track_token_usage().sync_wrapper().
  TokenTracker.token_counts: TokenTracker#token_counts.
  TokenTracker.calculate_cost: TokenTracker#calculate_cost().
  TokenTracker.get_summary: TokenTracker#get_summary().
  TokenTracker.reset: TokenTracker#reset().
  TokenTracker.add_tokens: TokenTracker#add_tokens().
  TokenTracker.add_interaction: TokenTracker#add_interaction().
  TokenTracker.interactions: TokenTracker#interactions.
  TokenTracker.get_interactions: TokenTracker#get_interactions().
  TokenTracker.MODEL_PRICES: TokenTracker#MODEL_PRICES.
  TokenTracker: TokenTracker#
  TokenTracker.__init__: TokenTracker#__init__().
---
# Module: [`ai_scientist/utils/token_tracker.py`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py)

## Classes
### `TokenTracker`
- def: [`ai_scientist/utils/token_tracker.py:10`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py#L10) — documented in [ai_scientist-utils-token_tracker](../../../concepts/ai_scientist-utils-token_tracker.md)
- signature: `class TokenTracker:`
- members:
  - `__init__(self)` — [`L11`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py#L11) — Token counts for prompt, completion, reasoning, and cached.
  - `add_interaction(self, model: str, system_message: str, prompt: str, response: str, timestamp: datetime)` — [`L75`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py#L75) — Record a single interaction with the model. — documented in [ai_scientist-llm](../../../concepts/ai_scientist-llm.md)
  - `add_tokens(self, model: str, prompt_tokens: int, completion_tokens: int, reasoning_tokens: int, cached_tokens: int)` — [`L62`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py#L62) — documented in [ai_scientist-llm](../../../concepts/ai_scientist-llm.md)
  - `calculate_cost(self, model: str)` — [`L107`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py#L107) — Calculate the cost for a specific model based on token usage.
  - `get_interactions(self, model: Optional[str] = None)` — [`L93`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py#L93) — Get all interactions, optionally filtered by model.
  - `get_summary(self)` — [`L127`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py#L127) — Get summary of token usage and costs for all models.
  - `reset(self)` — [`L99`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py#L99) — Reset all token counts and interactions.
  - `MODEL_PRICES` — [`L25`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py#L25)
  - `interactions` — [`L23`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py#L23) — documented in [ai_scientist-utils-token_tracker](../../../concepts/ai_scientist-utils-token_tracker.md)
  - `token_counts` — [`L20`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py#L20) — documented in [ai_scientist-utils-token_tracker](../../../concepts/ai_scientist-utils-token_tracker.md)
- used by: [`token_tracker`](token_tracker.md#token_tracker), [`save_token_tracker`](../../launch_scientist_bfts.md#save_token_tracker), [`async_wrapper`](token_tracker.md#track_token_usage.async_wrapper), [`sync_wrapper`](token_tracker.md#track_token_usage.sync_wrapper)

## Functions
- `async_wrapper(*args, **kwargs)` — [`L145`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py#L145) — documented in [ai_scientist-llm](../../../concepts/ai_scientist-llm.md)
- `sync_wrapper(*args, **kwargs)` — [`L185`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py#L185) — documented in [ai_scientist-llm](../../../concepts/ai_scientist-llm.md)
- `track_token_usage(func)` — [`L143`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py#L143) — documented in [ai_scientist-llm](../../../concepts/ai_scientist-llm.md)

## Module values
- `token_tracker` — [`L140`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/utils/token_tracker.py#L140) — documented in [ai_scientist-llm](../../../concepts/ai_scientist-llm.md)


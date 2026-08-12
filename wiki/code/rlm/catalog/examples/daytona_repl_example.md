---
title: 'Module: examples/daytona_repl_example.py'
type: catalog
provenance: extracted
module: examples/daytona_repl_example.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `examples.daytona_repl_example`/
symbols:
  main: main().
  MockLM.get_usage_summary: MockLM#get_usage_summary().
  MockLM: MockLM#
  MockLM.__init__: MockLM#__init__().
  MockLM.acompletion: MockLM#acompletion().
  MockLM.get_last_usage: MockLM#get_last_usage().
  MockLM.completion: MockLM#completion().
---
# Module: [`examples/daytona_repl_example.py`](../../../../../raw/code/rlm/examples/daytona_repl_example.py)

## Classes
### `MockLM`  ·  implements/extends BaseLM
- def: [`examples/daytona_repl_example.py:13`](../../../../../raw/code/rlm/examples/daytona_repl_example.py#L13)
- doc: Simple mock LM that echoes prompts.
- signature: `class MockLM(BaseLM):`
- members:
  - `acompletion(self, prompt)` — [`L22`](../../../../../raw/code/rlm/examples/daytona_repl_example.py#L22)
  - `completion(self, prompt)` — [`L19`](../../../../../raw/code/rlm/examples/daytona_repl_example.py#L19)
  - `get_last_usage(self)` — [`L34`](../../../../../raw/code/rlm/examples/daytona_repl_example.py#L34)
  - `get_usage_summary(self)` — [`L25`](../../../../../raw/code/rlm/examples/daytona_repl_example.py#L25)
- protocol/private: `__init__`[`L16`](../../../../../raw/code/rlm/examples/daytona_repl_example.py#L16)
- uses (calls/refs, reference-scoped): [`UsageSummary`](../rlm/core/types.md#UsageSummary), [`ModelUsageSummary`](../rlm/core/types.md#ModelUsageSummary), [`BaseLM`](../rlm/clients/base_lm.md#BaseLM), [`model_usage_summaries`](../rlm/core/types.md#UsageSummary.model_usage_summaries), [`total_calls`](../rlm/core/types.md#ModelUsageSummary.total_calls), [`total_input_tokens`](../rlm/core/types.md#ModelUsageSummary.total_input_tokens), [`total_output_tokens`](../rlm/core/types.md#ModelUsageSummary.total_output_tokens), [`__init__`](../rlm/clients/base_lm.md#BaseLM.__init__)
- used by: [`BaseLM`](../rlm/clients/base_lm.md#BaseLM), [`get_last_usage`](../rlm/clients/base_lm.md#BaseLM.get_last_usage), [`get_usage_summary`](../rlm/clients/base_lm.md#BaseLM.get_usage_summary), [`completion`](../rlm/clients/base_lm.md#BaseLM.completion), [`acompletion`](../rlm/clients/base_lm.md#BaseLM.acompletion)  (1 test-only)

## Functions
- `main()` — [`L38`](../../../../../raw/code/rlm/examples/daytona_repl_example.py#L38)


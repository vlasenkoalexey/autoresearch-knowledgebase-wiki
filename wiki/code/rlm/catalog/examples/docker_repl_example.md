---
title: 'Module: examples/docker_repl_example.py'
type: catalog
provenance: extracted
module: examples/docker_repl_example.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `examples.docker_repl_example`/
symbols:
  main: main().
  main.mock_subcall: main().mock_subcall().
  MockLM.get_usage_summary: MockLM#get_usage_summary().
  MockLM: MockLM#
  MockLM.__init__: MockLM#__init__().
  MockLM.acompletion: MockLM#acompletion().
  MockLM.get_last_usage: MockLM#get_last_usage().
  MockLM.completion: MockLM#completion().
---
# Module: [`examples/docker_repl_example.py`](../../../../../raw/code/rlm/examples/docker_repl_example.py)

## Classes
### `MockLM`  ·  implements/extends BaseLM
- def: [`examples/docker_repl_example.py:25`](../../../../../raw/code/rlm/examples/docker_repl_example.py#L25)
- signature: `class MockLM(BaseLM):`
- members:
  - `acompletion(self, prompt)` — [`L32`](../../../../../raw/code/rlm/examples/docker_repl_example.py#L32)
  - `completion(self, prompt)` — [`L29`](../../../../../raw/code/rlm/examples/docker_repl_example.py#L29)
  - `get_last_usage(self)` — [`L38`](../../../../../raw/code/rlm/examples/docker_repl_example.py#L38)
  - `get_usage_summary(self)` — [`L35`](../../../../../raw/code/rlm/examples/docker_repl_example.py#L35)
- protocol/private: `__init__`[`L26`](../../../../../raw/code/rlm/examples/docker_repl_example.py#L26)
- uses (calls/refs, reference-scoped): [`UsageSummary`](../rlm/core/types.md#UsageSummary), [`ModelUsageSummary`](../rlm/core/types.md#ModelUsageSummary), [`BaseLM`](../rlm/clients/base_lm.md#BaseLM), [`__init__`](../rlm/clients/base_lm.md#BaseLM.__init__)
- used by: [`BaseLM`](../rlm/clients/base_lm.md#BaseLM), [`get_last_usage`](../rlm/clients/base_lm.md#BaseLM.get_last_usage), [`get_usage_summary`](../rlm/clients/base_lm.md#BaseLM.get_usage_summary), [`completion`](../rlm/clients/base_lm.md#BaseLM.completion), [`acompletion`](../rlm/clients/base_lm.md#BaseLM.acompletion)  (1 test-only)

## Functions
- `main()` — [`L42`](../../../../../raw/code/rlm/examples/docker_repl_example.py#L42)
- `mock_subcall(prompt, model=None)` — [`L75`](../../../../../raw/code/rlm/examples/docker_repl_example.py#L75)


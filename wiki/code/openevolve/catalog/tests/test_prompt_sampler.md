---
title: 'Module: tests/test_prompt_sampler.py'
type: catalog
provenance: extracted
module: tests/test_prompt_sampler.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_prompt_sampler`/TestPromptSampler#
symbols:
  TestPromptSampler.prompt_sampler: prompt_sampler.
  TestPromptSampler.test_build_prompt: test_build_prompt().
  TestPromptSampler.setUp: setUp().
  TestPromptSampler: ''
---
# Module: [`tests/test_prompt_sampler.py`](../../../../../raw/code/openevolve/tests/test_prompt_sampler.py)

## Classes
### `TestPromptSampler`  ·  implements/extends TestCase
- def: [`tests/test_prompt_sampler.py:10`](../../../../../raw/code/openevolve/tests/test_prompt_sampler.py#L10)
- doc: Tests for prompt sampler
- signature: `class TestPromptSampler(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L13`](../../../../../raw/code/openevolve/tests/test_prompt_sampler.py#L13) — Set up test prompt sampler
  - `test_build_prompt(self)` — [`L18`](../../../../../raw/code/openevolve/tests/test_prompt_sampler.py#L18) — Test building a prompt — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `prompt_sampler` — [`L16`](../../../../../raw/code/openevolve/tests/test_prompt_sampler.py#L16)
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`build_prompt`](../openevolve/prompt/sampler.md#PromptSampler.build_prompt), [`prompt`](../openevolve/config.md#Config.prompt), [`PromptSampler`](../openevolve/prompt/sampler.md#PromptSampler)


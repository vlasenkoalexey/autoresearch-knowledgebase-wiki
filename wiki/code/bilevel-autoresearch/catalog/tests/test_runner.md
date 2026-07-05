---
title: 'Module: tests/test_runner.py'
type: catalog
provenance: extracted
module: tests/test_runner.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `tests.test_runner`/
symbols:
  TestInjectStage.test_inject_after_existing_stage: TestInjectStage#test_inject_after_existing_stage().
  TestInjectStage.test_inject_after_first_stage: TestInjectStage#test_inject_after_first_stage().
  TestInjectStage.test_inject_after_last_stage: TestInjectStage#test_inject_after_last_stage().
  TestInjectStage.test_inject_preserves_original_order: TestInjectStage#test_inject_preserves_original_order().
  _DummyStage: _DummyStage#
  TestInjectStage.test_inject_nonexistent_raises: TestInjectStage#test_inject_nonexistent_raises().
  TestRunnerInit.test_default_stages: TestRunnerInit#test_default_stages().
  TestRunnerInit.test_prompt_overrides_empty_by_default: TestRunnerInit#test_prompt_overrides_empty_by_default().
  _DummyStage.name: _DummyStage#name.
  _DummyStage.run: _DummyStage#run().
  TestInjectStage: TestInjectStage#
  TestRunnerInit: TestRunnerInit#
---
# Module: [`tests/test_runner.py`](../../../../../raw/code/bilevel-autoresearch/tests/test_runner.py)

## Classes
### `TestInjectStage`
- def: [`tests/test_runner.py:15`](../../../../../raw/code/bilevel-autoresearch/tests/test_runner.py#L15)
- signature: `class TestInjectStage:`
- members:
  - `test_inject_after_existing_stage(self)` — [`L16`](../../../../../raw/code/bilevel-autoresearch/tests/test_runner.py#L16)
  - `test_inject_after_first_stage(self)` — [`L25`](../../../../../raw/code/bilevel-autoresearch/tests/test_runner.py#L25)
  - `test_inject_after_last_stage(self)` — [`L32`](../../../../../raw/code/bilevel-autoresearch/tests/test_runner.py#L32)
  - `test_inject_nonexistent_raises(self)` — [`L38`](../../../../../raw/code/bilevel-autoresearch/tests/test_runner.py#L38)
  - `test_inject_preserves_original_order(self)` — [`L43`](../../../../../raw/code/bilevel-autoresearch/tests/test_runner.py#L43)
- uses (calls/refs, reference-scoped): [`stages`](../domains/article_opt/runner.md#InnerRunner.stages), [`inject_stage`](../domains/article_opt/runner.md#InnerRunner.inject_stage), [`InnerRunner`](../domains/article_opt/runner.md#InnerRunner)  (1 test-only)

### `TestRunnerInit`
- def: [`tests/test_runner.py:53`](../../../../../raw/code/bilevel-autoresearch/tests/test_runner.py#L53)
- signature: `class TestRunnerInit:`
- members:
  - `test_default_stages(self)` — [`L54`](../../../../../raw/code/bilevel-autoresearch/tests/test_runner.py#L54)
  - `test_prompt_overrides_empty_by_default(self)` — [`L65`](../../../../../raw/code/bilevel-autoresearch/tests/test_runner.py#L65)
- uses (calls/refs, reference-scoped): [`stages`](../domains/article_opt/runner.md#InnerRunner.stages), [`InnerRunner`](../domains/article_opt/runner.md#InnerRunner), [`prompt_overrides`](../domains/article_opt/runner.md#InnerRunner.prompt_overrides)

### `_DummyStage`  ·  implements/extends BaseStage
- def: [`tests/test_runner.py:8`](../../../../../raw/code/bilevel-autoresearch/tests/test_runner.py#L8)
- signature: `class _DummyStage(BaseStage):`
- members:
  - `run(self, context: dict)` — [`L11`](../../../../../raw/code/bilevel-autoresearch/tests/test_runner.py#L11)
  - `name` — [`L9`](../../../../../raw/code/bilevel-autoresearch/tests/test_runner.py#L9)
- uses (calls/refs, reference-scoped): [`BaseStage`](../domains/article_opt/pipeline/base.md#BaseStage)
- used by: [`BaseStage`](../domains/article_opt/pipeline/base.md#BaseStage), [`run`](../domains/article_opt/pipeline/base.md#BaseStage.run)  (5 test-only)


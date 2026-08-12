---
title: 'Module: OpenMLE-Gym/tests/test_graph_regression.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/tests/test_graph_regression.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.tests.test_graph_regression`/
symbols:
  GraphRegressionTests.test_full_graph_with_fixed_kaggle_and_llm_fixtures: GraphRegressionTests#test_full_graph_with_fixed_kaggle_and_llm_fixtures().
  GraphRegressionTests.fake_query: GraphRegressionTests#fake_query().
  HAS_GRAPH_DEPS: HAS_GRAPH_DEPS.
  METRIC_CODE: METRIC_CODE.
  REQUIRED_MODULES: REQUIRED_MODULES.
  PREPARE_CODE: PREPARE_CODE.
  GraphRegressionTests.fake_download: GraphRegressionTests#fake_download().
  GraphRegressionTests.fake_init: GraphRegressionTests#fake_init().
  GraphRegressionTests: GraphRegressionTests#
---
# Module: [`OpenMLE-Gym/tests/test_graph_regression.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_graph_regression.py)

## Classes
### `GraphRegressionTests`  ·  implements/extends TestCase
- def: [`OpenMLE-Gym/tests/test_graph_regression.py:47`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_graph_regression.py#L47)
- signature: `class GraphRegressionTests(unittest.TestCase):`
- members:
  - `fake_download(self, comp_id, target_dir)` — [`L55`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_graph_regression.py#L55)
  - `fake_init(self, *args, **kwargs)` — [`L62`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_graph_regression.py#L62)
  - `fake_query(self, prompts)` — [`L65`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_graph_regression.py#L65)
  - `test_full_graph_with_fixed_kaggle_and_llm_fixtures(self)` — [`L48`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_graph_regression.py#L48)
- uses (calls/refs, reference-scoped): [`Graph`](../builder_core/design.md#Graph), [`AgentState`](../builder_core/utils/state.md#AgentState), [`NodeExecutor`](../builder_core/utils/nodes.md#NodeExecutor), [`Task`](../builder_core/utils/task.md#Task), [`copy`](../builder_core/utils/task.md#Task.copy), [`describe`](../builder_core/utils/task.md#Task.describe), [`download`](../builder_core/utils/task.md#Task.download), [`errors`](../builder_core/utils/task.md#Task.errors), [`gen_prep`](../builder_core/utils/task.md#Task.gen_prep), [`metric`](../builder_core/utils/task.md#Task.metric), [`name`](../builder_core/utils/task.md#Task.name), [`perceive`](../builder_core/utils/task.md#Task.perceive), [`prepare`](../builder_core/utils/task.md#Task.prepare), [`prepares`](../builder_core/utils/task.md#Task.prepares), [`retry`](../builder_core/utils/task.md#Task.retry), [`success`](../builder_core/utils/task.md#Task.success), [`web_info`](../builder_core/utils/task.md#Task.web_info)  (2 test-only)

## Module values
- `HAS_GRAPH_DEPS` — [`L20`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_graph_regression.py#L20)
- `METRIC_CODE` — [`L39`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_graph_regression.py#L39)
- `PREPARE_CODE` — [`L23`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_graph_regression.py#L23)
- `REQUIRED_MODULES` — [`L13`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_graph_regression.py#L13)


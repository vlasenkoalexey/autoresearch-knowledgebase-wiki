---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.tests.test_final_node_selection`/
symbols:
  single_task_runner: single_task_runner.
  test_final_selection_uses_journal_best_metric_not_official_score: test_final_selection_uses_journal_best_metric_not_official_score().
  test_final_selection_falls_back_to_latest_non_root_when_journal_has_no_best_node: test_final_selection_falls_back_to_latest_non_root_when_journal_has_no_best_node().
  spec: spec.
  make_node: make_node().
  yaml_stub: yaml_stub.
  dotenv_stub: dotenv_stub.
  make_solver: make_solver().
  ComparableMetric.__lt__: ComparableMetric#__lt__().
  make_solver.Journal.get_best_node: make_solver().Journal#get_best_node().
  ComparableMetric.value: ComparableMetric#value.
  RUNNER_PATH: RUNNER_PATH.
  ComparableMetric: ComparableMetric#
  make_solver.Journal: make_solver().Journal#
  Journal.nodes: Journal#nodes.
  ComparableMetric.__init__: ComparableMetric#__init__().
  ComparableMetric.info: ComparableMetric#info.
  make_solver.Journal.__init__: make_solver().Journal#__init__().
  make_solver.Journal.is_root_node: make_solver().Journal#is_root_node().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py)

## Classes
### `ComparableMetric`
- def: [`OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py:30`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L30)
- signature: `class ComparableMetric:`
- members:
  - `info` — [`L33`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L33)
  - `value` — [`L32`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L32)
- protocol/private: `__init__`[`L31`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L31), `__lt__`[`L35`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L35)
- used by: (1 test-only callers)

### `Journal`
- def: [`OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py:67`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L67)
- signature: `class Journal:`
- members:
  - `get_best_node(self)` — [`L71`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L71)
  - `is_root_node(self, _node)` — [`L78`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L78)
  - `nodes` — [`L69`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L69)
- protocol/private: `__init__`[`L68`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L68)
- used by: (1 test-only callers)

## Functions
- `make_node(*, node_id: str, metric: float | None, official_score: float | None, status: str, is_buggy: bool = False, validation_score: float | None = None)` — [`L41`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L41)
- `make_solver(nodes, *, lower_is_better: bool = False)` — [`L66`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L66)
- `test_final_selection_falls_back_to_latest_non_root_when_journal_has_no_best_node()` — [`L112`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L112)
- `test_final_selection_uses_journal_best_metric_not_official_score()` — [`L84`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L84)

## Module values
- `RUNNER_PATH` — [`L18`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L18)
- `dotenv_stub` — [`L14`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L14)
- `single_task_runner` — [`L25`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L25)
- `spec` — [`L24`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L24)
- `yaml_stub` — [`L9`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_final_node_selection.py#L9)


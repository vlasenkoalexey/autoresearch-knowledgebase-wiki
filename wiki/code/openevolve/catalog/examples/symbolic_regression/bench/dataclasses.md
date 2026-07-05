---
title: 'Module: examples/symbolic_regression/bench/dataclasses.py'
type: catalog
provenance: extracted
module: examples/symbolic_regression/bench/dataclasses.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.symbolic_regression.bench.dataclasses`/
symbols:
  Problem.create_task: Problem#create_task().
  Problem.gt_equation: Problem#gt_equation.
  Problem.samples: Problem#samples.
  Problem: Problem#
  Problem.train_samples: Problem#train_samples().
  Equation: Equation#
  Problem.test_samples: Problem#test_samples().
  Problem.ood_test_samples: Problem#ood_test_samples().
  Equation.symbols: Equation#symbols.
  Equation.symbol_descs: Equation#symbol_descs.
  Equation.symbol_properties: Equation#symbol_properties.
  Problem.equation_idx: Problem#equation_idx.
  SearchResult.equation: SearchResult#equation.
  Equation.expression: Equation#expression.
  SEDTask: SEDTask#
  Problem.dataset_identifier: Problem#dataset_identifier.
  Equation.desc: Equation#desc.
  SEDTask.name: SEDTask#name.
  SEDTask.symbols: SEDTask#symbols.
  SEDTask.symbol_descs: SEDTask#symbol_descs.
  SEDTask.symbol_properties: SEDTask#symbol_properties.
  SEDTask.samples: SEDTask#samples.
  SEDTask.desc: SEDTask#desc.
  Equation.sympy_format: Equation#sympy_format.
  Equation.lambda_format: Equation#lambda_format.
  Equation.program_format: Equation#program_format.
  SearchResult: SearchResult#
  SearchResult.aux: SearchResult#aux.
---
# Module: [`examples/symbolic_regression/bench/dataclasses.py`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py)

## Classes
### `Equation`
- def: [`examples/symbolic_regression/bench/dataclasses.py:7`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L7)
- signature: `class Equation:`
- members:
  - `desc` — [`L12`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L12)
  - `expression` — [`L11`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L11)
  - `lambda_format` — [`L15`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L15)
  - `program_format` — [`L16`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L16)
  - `symbol_descs` — [`L9`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L9)
  - `symbol_properties` — [`L10`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L10)
  - `symbols` — [`L8`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L8)
  - `sympy_format` — [`L14`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L14)
- used by: (5 test-only callers)

### `Problem`
- def: [`examples/symbolic_regression/bench/dataclasses.py:36`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L36)
- signature: `class Problem:`
- members:
  - `create_task(self)` — [`L42`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L42)
  - `ood_test_samples(self)` — [`L61`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L61)
  - `test_samples(self)` — [`L57`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L57)
  - `train_samples(self)` — [`L53`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L53)
  - `dataset_identifier` — [`L37`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L37)
  - `equation_idx` — [`L38`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L38)
  - `gt_equation` — [`L39`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L39)
  - `samples` — [`L40`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L40)
- uses (calls/refs, reference-scoped): (16 test-only callers)
- used by: (6 test-only callers)

### `SEDTask`
- def: [`examples/symbolic_regression/bench/dataclasses.py:26`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L26)
- signature: `class SEDTask:`
- members:
  - `desc` — [`L32`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L32)
  - `name` — [`L27`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L27)
  - `samples` — [`L31`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L31)
  - `symbol_descs` — [`L29`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L29)
  - `symbol_properties` — [`L30`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L30)
  - `symbols` — [`L28`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L28)
- used by: (1 test-only callers)

### `SearchResult`
- def: [`examples/symbolic_regression/bench/dataclasses.py:20`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L20)
- signature: `class SearchResult:`
- members:
  - `aux` — [`L22`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L22)
  - `equation` — [`L21`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/dataclasses.py#L21)
- uses (calls/refs, reference-scoped): (1 test-only callers)


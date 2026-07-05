---
title: 'Module: examples/symbolic_regression/bench/datamodules.py'
type: catalog
provenance: extracted
module: examples/symbolic_regression/bench/datamodules.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.symbolic_regression.bench.datamodules`/
symbols:
  BaseSynthDataModule.problems: BaseSynthDataModule#problems.
  TransformedFeynmanDataModule.problems: TransformedFeynmanDataModule#problems.
  get_datamodule: get_datamodule().
  BaseSynthDataModule: BaseSynthDataModule#
  BaseSynthDataModule.setup: BaseSynthDataModule#setup().
  TransformedFeynmanDataModule.setup: TransformedFeynmanDataModule#setup().
  BaseSynthDataModule.name2id: BaseSynthDataModule#name2id.
  REPO_ID: REPO_ID.
  BaseSynthDataModule.__init__: BaseSynthDataModule#__init__().
  BaseSynthDataModule._dataset_identifier: BaseSynthDataModule#_dataset_identifier.
  MatSciDataModule: MatSciDataModule#
  ChemReactKineticsDataModule: ChemReactKineticsDataModule#
  BioPopGrowthDataModule: BioPopGrowthDataModule#
  PhysOscilDataModule: PhysOscilDataModule#
  TransformedFeynmanDataModule.name2id: TransformedFeynmanDataModule#name2id.
  SynProblem: SynProblem#
  SynProblem.train_samples: SynProblem#train_samples().
  SynProblem.test_samples: SynProblem#test_samples().
  SynProblem.ood_test_samples: SynProblem#ood_test_samples().
  BaseSynthDataModule.name: BaseSynthDataModule#name().
  MatSciDataModule.__init__: MatSciDataModule#__init__().
  ChemReactKineticsDataModule.__init__: ChemReactKineticsDataModule#__init__().
  BioPopGrowthDataModule.__init__: BioPopGrowthDataModule#__init__().
  PhysOscilDataModule.__init__: PhysOscilDataModule#__init__().
  _download: _download().
  TransformedFeynmanDataModule._dataset_dir: TransformedFeynmanDataModule#_dataset_dir.
  BaseSynthDataModule._dataset_dir: BaseSynthDataModule#_dataset_dir.
  TransformedFeynmanDataModule: TransformedFeynmanDataModule#
  TransformedFeynmanDataModule._dataset_identifier: TransformedFeynmanDataModule#_dataset_identifier.
  TransformedFeynmanDataModule.__init__: TransformedFeynmanDataModule#__init__().
  TransformedFeynmanDataModule.name: TransformedFeynmanDataModule#name().
  BaseSynthDataModule._short_dataset_identifier: BaseSynthDataModule#_short_dataset_identifier.
  BaseSynthDataModule._default_symbols: BaseSynthDataModule#_default_symbols.
  BaseSynthDataModule._default_symbol_descs: BaseSynthDataModule#_default_symbol_descs.
---
# Module: [`examples/symbolic_regression/bench/datamodules.py`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py)

## Classes
### `BaseSynthDataModule`
- def: [`examples/symbolic_regression/bench/datamodules.py:72`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L72)
- signature: `class BaseSynthDataModule:`
- members:
  - `name(self)` — [`L118`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L118)
  - `setup(self)` — [`L87`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L87)
  - `name2id` — [`L113`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L113)
  - `problems` — [`L91`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L91)
- protocol/private: `__init__`[`L73`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L73), `_dataset_dir`[`L81`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L81), `_dataset_identifier`[`L82`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L82), `_default_symbol_descs`[`L85`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L85), `_default_symbols`[`L84`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L84), `_short_dataset_identifier`[`L83`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L83)
- uses (calls/refs, reference-scoped): (16 test-only callers)
- used by: (9 test-only callers)

### `BioPopGrowthDataModule`  ·  implements/extends BaseSynthDataModule
- def: [`examples/symbolic_regression/bench/datamodules.py:142`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L142)
- signature: `class BioPopGrowthDataModule(BaseSynthDataModule):`
- protocol/private: `__init__`[`L143`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L143)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

### `ChemReactKineticsDataModule`  ·  implements/extends BaseSynthDataModule
- def: [`examples/symbolic_regression/bench/datamodules.py:127`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L127)
- signature: `class ChemReactKineticsDataModule(BaseSynthDataModule):`
- protocol/private: `__init__`[`L128`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L128)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

### `MatSciDataModule`  ·  implements/extends BaseSynthDataModule
- def: [`examples/symbolic_regression/bench/datamodules.py:122`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L122)
- signature: `class MatSciDataModule(BaseSynthDataModule):`
- protocol/private: `__init__`[`L123`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L123)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

### `PhysOscilDataModule`  ·  implements/extends BaseSynthDataModule
- def: [`examples/symbolic_regression/bench/datamodules.py:153`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L153)
- signature: `class PhysOscilDataModule(BaseSynthDataModule):`
- protocol/private: `__init__`[`L154`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L154)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

### `SynProblem`  ·  implements/extends Problem
- def: [`examples/symbolic_regression/bench/datamodules.py:58`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L58)
- signature: `class SynProblem(Problem):`
- members:
  - `ood_test_samples(self)` — [`L68`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L68)
  - `test_samples(self)` — [`L64`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L64)
  - `train_samples(self)` — [`L60`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L60)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (4 test-only callers)

### `TransformedFeynmanDataModule`
- def: [`examples/symbolic_regression/bench/datamodules.py:22`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L22)
- signature: `class TransformedFeynmanDataModule:`
- members:
  - `name(self)` — [`L54`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L54)
  - `setup(self)` — [`L27`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L27)
  - `name2id` — [`L51`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L51)
  - `problems` — [`L31`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L31)
- protocol/private: `__init__`[`L23`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L23), `_dataset_dir`[`L24`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L24), `_dataset_identifier`[`L25`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L25)
- uses (calls/refs, reference-scoped): (12 test-only callers)
- used by: (1 test-only callers)

## Functions
- `_download(repo_id)` — [`L18`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L18)
- `get_datamodule(name, root_folder)` — [`L169`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L169)

## Module values
- `REPO_ID` — [`L15`](../../../../../../../raw/code/openevolve/examples/symbolic_regression/bench/datamodules.py#L15)


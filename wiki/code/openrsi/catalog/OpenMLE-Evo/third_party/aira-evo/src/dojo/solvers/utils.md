---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/utils.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.solvers.utils`/
symbols:
  get_complextiy_level: get_complextiy_level().
  Complexity: Complexity#
  Complexity.LOW: Complexity#LOW.
  Complexity.MEDIUM: Complexity#MEDIUM.
  Complexity.HIGH: Complexity#HIGH.
  Complexity.__str__: Complexity#__str__().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/utils.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/utils.py)

## Classes
### `Complexity`  ·  implements/extends Enum
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/utils.py:11`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/utils.py#L11)
- signature: `class Complexity(Enum):`
- members:
  - `HIGH` — [`L14`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/utils.py#L14)
  - `LOW` — [`L12`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/utils.py#L12)
  - `MEDIUM` — [`L13`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/utils.py#L13)
- protocol/private: `__str__`[`L16`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/utils.py#L16)
- used by: [`improve_op`](../core/solvers/operators/improve.md#improve_op), [`get_complextiy_level`](utils.md#get_complextiy_level), [`draft_op`](../core/solvers/operators/draft.md#draft_op)

## Functions
- `get_complextiy_level(node: Node = None, num: int = None)` — [`L20`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/utils.py#L20) — Determine the complexity level based on the number of children.


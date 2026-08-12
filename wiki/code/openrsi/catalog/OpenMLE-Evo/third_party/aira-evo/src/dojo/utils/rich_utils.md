---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.utils.rich_utils`/
symbols:
  print_config_tree: print_config_tree().
  StringifyValue.__init__: StringifyValue#__init__().
  stringify_unsupported: stringify_unsupported().
  StringifyValue.__value: StringifyValue#__value.
  StringifyValue.value: StringifyValue#value().
  StringifyValue.__str__: StringifyValue#__str__().
  StringifyValue.__repr__: StringifyValue#__repr__().
  StringifyValue: StringifyValue#
  MAX_32_BIT_INT: MAX_32_BIT_INT.
  MIN_32_BIT_INT: MIN_32_BIT_INT.
  is_unsupported_float: is_unsupported_float().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py)

## Classes
### `StringifyValue`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py:45`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py#L45)
- doc: A wrapper class that processes and stores a value ensuring that it is
- signature: `class StringifyValue:`
- members:
  - `__init__(self, value: Any)` — [`L55`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py#L55) — Process the input value to ensure it is suitable for stringification.
  - `__repr__(self)` — [`L91`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py#L91) — Return the official string representation of the processed value.
  - `__str__(self)` — [`L82`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py#L82) — Return the string representation of the processed value.
  - `value(self)` — [`L73`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py#L73) — Retrieve the processed value.
- protocol/private: `__value`[`L70`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py#L70)
- uses (calls/refs, reference-scoped): [`MAX_32_BIT_INT`](rich_utils.md#MAX_32_BIT_INT), [`MIN_32_BIT_INT`](rich_utils.md#MIN_32_BIT_INT), [`is_unsupported_float`](rich_utils.md#is_unsupported_float)
- used by: [`stringify_unsupported`](rich_utils.md#stringify_unsupported)

## Functions
- `is_unsupported_float(value: Any)` — [`L30`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py#L30) — Determine if the given value is a float that is either infinite or NaN.
- `print_config_tree(cfg: RunConfig, print_order: Sequence[str] = [], resolve: bool = False, save_to_file: bool = False)` — [`L125`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py#L125) — Prints content of DictConfig using Rich library and its tree structure.
- `stringify_unsupported(value: Any)` — [`L101`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py#L101) — Recursively process a value, converting unsupported types to a StringifyValue instance.

## Module values
- `MAX_32_BIT_INT` — [`L26`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py#L26)
- `MIN_32_BIT_INT` — [`L27`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/rich_utils.py#L27)


---
title: 'Module: test/utils/test_misc.py'
type: catalog
provenance: extracted
module: test/utils/test_misc.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `test.utils.test_misc`/
symbols:
  A: A#
  A.__repr__: A#__repr__().
  MiscTest.test_singleton: MiscTest#test_singleton().
  A.__str__: A#__str__().
  A.__init__: A#__init__().
  A.kwargs: A#kwargs.
  MiscTest: MiscTest#
---
# Module: [`test/utils/test_misc.py`](../../../../../../raw/code/rd-agent/test/utils/test_misc.py)

## Classes
### `A`  ·  implements/extends SingletonBaseClass
- def: [`test/utils/test_misc.py:8`](../../../../../../raw/code/rd-agent/test/utils/test_misc.py#L8)
- signature: `class A(SingletonBaseClass):`
- members:
  - `kwargs` — [`L11`](../../../../../../raw/code/rd-agent/test/utils/test_misc.py#L11)
- protocol/private: `__init__`[`L9`](../../../../../../raw/code/rd-agent/test/utils/test_misc.py#L9), `__repr__`[`L16`](../../../../../../raw/code/rd-agent/test/utils/test_misc.py#L16), `__str__`[`L13`](../../../../../../raw/code/rd-agent/test/utils/test_misc.py#L13)
- uses (calls/refs, reference-scoped): [`SingletonBaseClass`](../../rdagent/core/utils.md#SingletonBaseClass)
- used by: [`SingletonBaseClass`](../../rdagent/core/utils.md#SingletonBaseClass)  (1 test-only)

### `MiscTest`  ·  implements/extends TestCase
- def: [`test/utils/test_misc.py:21`](../../../../../../raw/code/rd-agent/test/utils/test_misc.py#L21)
- signature: `class MiscTest(unittest.TestCase):`
- members:
  - `test_singleton(self)` — [`L22`](../../../../../../raw/code/rd-agent/test/utils/test_misc.py#L22)
- uses (calls/refs, reference-scoped): (1 test-only callers)


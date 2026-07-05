---
title: 'Module: utils/swe_log_parsers.py'
type: catalog
provenance: extracted
module: utils/swe_log_parsers.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `utils.swe_log_parsers`/
symbols:
  MAP_REPO_TO_PARSER: MAP_REPO_TO_PARSER.
  TestStatus: TestStatus#
  parse_log_pytest: parse_log_pytest().
  parse_log_django: parse_log_django().
  parse_log_sympy: parse_log_sympy().
  TestStatus.FAILED: TestStatus#FAILED.
  TestStatus.PASSED: TestStatus#PASSED.
  parse_log_seaborn: parse_log_seaborn().
  parse_log_pytest_options: parse_log_pytest_options().
  parse_log_pytest_v2: parse_log_pytest_v2().
  parse_log_matplotlib: parse_log_matplotlib().
  parse_log_astroid: parse_log_astroid.
  parse_log_flask: parse_log_flask.
  parse_log_marshmallow: parse_log_marshmallow.
  parse_log_pvlib: parse_log_pvlib.
  parse_log_pyvista: parse_log_pyvista.
  parse_log_sqlfluff: parse_log_sqlfluff.
  parse_log_xarray: parse_log_xarray.
  parse_log_pydicom: parse_log_pydicom.
  parse_log_requests: parse_log_requests.
  parse_log_pylint: parse_log_pylint.
  parse_log_astropy: parse_log_astropy.
  parse_log_scikit: parse_log_scikit.
  parse_log_sphinx: parse_log_sphinx.
  TestStatus.ERROR: TestStatus#ERROR.
  TestStatus.SKIPPED: TestStatus#SKIPPED.
  TestStatus.XFAIL: TestStatus#XFAIL.
---
# Module: [`utils/swe_log_parsers.py`](../../../../../raw/code/dgm/utils/swe_log_parsers.py)

## Classes
### `TestStatus`  ·  implements/extends Enum
- def: [`utils/swe_log_parsers.py:4`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L4) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- signature: `class TestStatus(Enum):`
- members:
  - `ERROR` — [`L8`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L8) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
  - `FAILED` — [`L5`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L5) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
  - `PASSED` — [`L6`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L6) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
  - `SKIPPED` — [`L7`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L7) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
  - `XFAIL` — [`L9`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L9)
- used by: [`parse_log_pytest`](swe_log_parsers.md#parse_log_pytest), [`parse_log_django`](swe_log_parsers.md#parse_log_django), [`parse_log_sympy`](swe_log_parsers.md#parse_log_sympy), [`parse_log_seaborn`](swe_log_parsers.md#parse_log_seaborn), [`parse_log_pytest_options`](swe_log_parsers.md#parse_log_pytest_options), [`parse_log_pytest_v2`](swe_log_parsers.md#parse_log_pytest_v2), [`parse_log_matplotlib`](swe_log_parsers.md#parse_log_matplotlib)

## Functions
- `parse_log_django(log: str)` — [`L64`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L64) — Parser for test logs generated with Django tester framework — documented in [coding_agent](../../concepts/coding_agent.md)
- `parse_log_matplotlib(log: str)` — [`L226`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L226) — Parser for test logs generated with PyTest framework — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_pytest(log: str)` — [`L11`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L11) — Parser for test logs generated with PyTest framework — documented in [coding_agent](../../concepts/coding_agent.md)
- `parse_log_pytest_options(log: str)` — [`L33`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L33) — Parser for test logs generated with PyTest framework with options — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_pytest_v2(log: str)` — [`L140`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L140) — Parser for test logs generated with PyTest framework (Later Version) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_seaborn(log: str)` — [`L167`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L167) — Parser for test logs generated with seaborn testing framework — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_sympy(log: str)` — [`L193`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L193) — Parser for test logs generated with Sympy framework — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)

## Module values
- `MAP_REPO_TO_PARSER` — [`L267`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L267) — documented in [coding_agent](../../concepts/coding_agent.md)
- `parse_log_astroid` — [`L250`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L250) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_astropy` — [`L262`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L262) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_flask` — [`L251`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L251) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_marshmallow` — [`L252`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L252) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_pvlib` — [`L253`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L253) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_pydicom` — [`L258`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L258) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_pylint` — [`L260`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L260) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_pyvista` — [`L254`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L254) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_requests` — [`L259`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L259) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_scikit` — [`L263`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L263) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_sphinx` — [`L264`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L264) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_sqlfluff` — [`L255`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L255) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)
- `parse_log_xarray` — [`L256`](../../../../../raw/code/dgm/utils/swe_log_parsers.py#L256) — documented in [utils-swe_log_parsers](../../concepts/utils-swe_log_parsers.md)


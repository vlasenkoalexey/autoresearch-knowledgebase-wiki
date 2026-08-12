---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.core.solvers.utils.search_utils`/
symbols:
  normalized: normalized().
  extract_code: extract_code().
  DataLogger.log: DataLogger#log().
  format_code: format_code().
  is_valid_python_script: is_valid_python_script().
  DataLogger.log_file_path: DataLogger#log_file_path.
  stable_softmax: stable_softmax().
  opt_messages_to_list: opt_messages_to_list().
  define_function_from_string: define_function_from_string().
  DataLogger: DataLogger#
  DataLogger.__init__: DataLogger#__init__().
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py)

## Classes
### `DataLogger`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py:159`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py#L159)
- signature: `class DataLogger:`
- members:
  - `log(self, data_sample)` — [`L163`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py#L163)
  - `log_file_path` — [`L161`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py#L161)
- protocol/private: `__init__`[`L160`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py#L160)

## Functions
- `define_function_from_string(function_string: str)` — [`L121`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py#L121) — Takes a string containing a function definition and returns the defined function.
- `extract_code(text)` — [`L69`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py#L69) — Extract Python code blocks from a given text.
- `format_code(code)` — [`L47`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py#L47) — Format Python code using the Black code formatter.
- `is_valid_python_script(script)` — [`L23`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py#L23) — Check if a given script is a valid Python script.
- `normalized(x: List[float], temp: float = 1)` — [`L177`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py#L177)
- `opt_messages_to_list(system_message: str | None, user_message: str | None, content_key: str)` — [`L109`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py#L109) — Helper function to turn optional system/user messages into a list.
- `stable_softmax(x, axis=-1, temp=1)` — [`L170`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_utils.py#L170)


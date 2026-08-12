---
title: 'Module: utils/json_utils.py'
type: catalog
provenance: extracted
module: utils/json_utils.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.json_utils`/
symbols:
  serialize_for_json: serialize_for_json().
  convert_protobuf_value: convert_protobuf_value().
  normalize_replan_edits: normalize_replan_edits().
  convert_protobuf_args: convert_protobuf_args().
  coerce_replan_edit_index: coerce_replan_edit_index().
  logger: logger.
  _is_protobuf: _is_protobuf().
---
# Module: [`utils/json_utils.py`](../../../../../raw/code/continual-harness/utils/json_utils.py)

## Functions
- `_is_protobuf(value: Any)` — [`L93`](../../../../../raw/code/continual-harness/utils/json_utils.py#L93) — Return True if *value* is a proto-plus / protobuf wrapper type.
- `coerce_replan_edit_index(idx: Any)` — [`L166`](../../../../../raw/code/continual-harness/utils/json_utils.py#L166) — Best-effort coercion of ``index`` to ``int`` (VLMs often emit string/float indices).
- `convert_protobuf_args(proto_args)` — [`L151`](../../../../../raw/code/continual-harness/utils/json_utils.py#L151) — Convert a protobuf argument mapping to a plain ``dict[str, Any]``.
- `convert_protobuf_value(value: Any)` — [`L102`](../../../../../raw/code/continual-harness/utils/json_utils.py#L102) — Recursively convert a protobuf value to a JSON-serialisable Python type.
- `normalize_replan_edits(edits: Any)` — [`L187`](../../../../../raw/code/continual-harness/utils/json_utils.py#L187) — Coerce ``edits`` into ``list[dict]`` for ``replan_objectives``.
- `serialize_for_json(obj)` — [`L18`](../../../../../raw/code/continual-harness/utils/json_utils.py#L18) — Recursively convert non-JSON-serializable objects to JSON-compatible types.

## Module values
- `logger` — [`L15`](../../../../../raw/code/continual-harness/utils/json_utils.py#L15)


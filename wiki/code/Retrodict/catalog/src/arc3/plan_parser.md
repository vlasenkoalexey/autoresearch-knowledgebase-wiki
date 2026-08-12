---
title: 'Module: src/arc3/plan_parser.py'
type: catalog
provenance: extracted
module: src/arc3/plan_parser.py
status: fresh
symbol_base: scip-python python Retrodict 0.0.0 `src.arc3.plan_parser`/
symbols:
  parse_actions: parse_actions().
  _validate_item: _validate_item().
  PlanParseError: PlanParseError#
  PlannedAction.name: PlannedAction#name.
  PlannedAction: PlannedAction#
  ParsedPlan: ParsedPlan#
  _decode_object: _decode_object().
  ParsedPlan.actions: ParsedPlan#actions.
  PlannedAction.x: PlannedAction#x.
  PlannedAction.y: PlannedAction#y.
  PlannedAction.expect: PlannedAction#expect.
  ParsedPlan.expect_levels: ParsedPlan#expect_levels.
  _validate_expect: _validate_expect().
  _with_truncation_hint: _with_truncation_hint().
  ACTIONS_MARKER: ACTIONS_MARKER.
  ParsedPlan.reasoning: ParsedPlan#reasoning.
  ParsedPlan.clamped: ParsedPlan#clamped.
  _CODE_FENCE: _CODE_FENCE.
---
# Module: [`src/arc3/plan_parser.py`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py)

## Classes
### `ParsedPlan`
- def: [`src/arc3/plan_parser.py:41`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L41) — documented in [arc3-plan_parser](../../../concepts/arc3-plan_parser.md)
- doc: A validated action plan.
- signature: `class ParsedPlan:`
- members:
  - `actions` — [`L44`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L44)
  - `clamped` — [`L46`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L46)
  - `expect_levels` — [`L47`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L47)
  - `reasoning` — [`L45`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L45)
- uses (calls/refs, reference-scoped): [`PlannedAction`](plan_parser.md#PlannedAction)
- used by: [`_accept`](runner.md#GameRunner._accept), [`_drain`](runner.md#GameRunner._drain), [`parse_actions`](plan_parser.md#parse_actions), [`_invoke`](runner.md#GameRunner._invoke)

### `PlanParseError`  ·  implements/extends Exception
- def: [`src/arc3/plan_parser.py:26`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L26) — documented in [arc3-plan_parser](../../../concepts/arc3-plan_parser.md)
- doc: The \[ACTIONS\] block is missing or invalid; the message is model-facing.
- signature: `class PlanParseError(Exception):`
- used by: [`parse_actions`](plan_parser.md#parse_actions), [`_invoke`](runner.md#GameRunner._invoke), [`_validate_item`](plan_parser.md#_validate_item), [`_decode_object`](plan_parser.md#_decode_object), [`_validate_expect`](plan_parser.md#_validate_expect)

### `PlannedAction`
- def: [`src/arc3/plan_parser.py:31`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L31) — documented in [arc3-plan_parser](../../../concepts/arc3-plan_parser.md)
- doc: One validated action from the agent's plan.
- signature: `class PlannedAction:`
- members:
  - `expect` — [`L37`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L37) — documented in [arc3-plan_parser](../../../concepts/arc3-plan_parser.md)
  - `name` — [`L34`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L34) — documented in [arc3-plan_parser](../../../concepts/arc3-plan_parser.md)
  - `x` — [`L35`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L35) — documented in [arc3-plan_parser](../../../concepts/arc3-plan_parser.md)
  - `y` — [`L36`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L36) — documented in [arc3-plan_parser](../../../concepts/arc3-plan_parser.md)
- used by: [`_step`](runner.md#GameRunner._step), [`_drain`](runner.md#GameRunner._drain), [`_check_expectations`](runner.md#GameRunner._check_expectations), [`_validate_item`](plan_parser.md#_validate_item), [`_render_action`](runner.md#_render_action), [`actions`](plan_parser.md#ParsedPlan.actions)

## Functions
- `_decode_object(payload: str, truncated: bool)` — [`L84`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L84) — Decode the first complete JSON object in the payload. — documented in [arc3-plan_parser](../../../concepts/arc3-plan_parser.md)
- `_validate_expect(value: object, index: int)` — [`L126`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L126)
- `_validate_item(item: object, index: int, available: set[str])` — [`L105`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L105) — documented in [arc3-plan_parser](../../../concepts/arc3-plan_parser.md)
- `_with_truncation_hint(message: str, truncated: bool)` — [`L145`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L145)
- `parse_actions(text: str, *, available: set[str], max_actions: int | None = None, truncated: bool = False)` — [`L50`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L50) — Parse the final [ACTIONS] block out of an agent reply. — documented in [arc3-plan_parser](../../../concepts/arc3-plan_parser.md)

## Module values
- `ACTIONS_MARKER` — [`L22`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L22)
- `_CODE_FENCE` — [`L23`](../../../../../../raw/code/Retrodict/src/arc3/plan_parser.py#L23)


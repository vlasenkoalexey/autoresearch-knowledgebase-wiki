---
title: 'Module: tests/test_milestones_part_b.py'
type: catalog
provenance: extracted
module: tests/test_milestones_part_b.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_milestones_part_b`/
symbols:
  _state: _state().
  test_full_part_b_sequence_through_dynamo_badge: test_full_part_b_sequence_through_dynamo_badge().
  _make_emulator: _make_emulator().
  test_route_116_requires_stone_badge: test_route_116_requires_stone_badge().
  test_non_linear_dewford_paths_and_slateport_or_logic: test_non_linear_dewford_paths_and_slateport_or_logic().
  test_route_110_requires_museum_event: test_route_110_requires_museum_event().
  _completed_before: _completed_before().
  test_order_and_comparison_are_canonical: test_order_and_comparison_are_canonical().
  _StubMilestoneTracker.mark_completed: _StubMilestoneTracker#mark_completed().
  _StubMilestoneTracker.is_completed: _StubMilestoneTracker#is_completed().
  PART_B_SEQUENCE: PART_B_SEQUENCE.
  _StubMilestoneTracker.completed: _StubMilestoneTracker#completed.
  _StubMilestoneTracker: _StubMilestoneTracker#
  _StubMilestoneTracker.marked: _StubMilestoneTracker#marked.
  _StubMilestoneTracker.__init__: _StubMilestoneTracker#__init__().
---
# Module: [`tests/test_milestones_part_b.py`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py)

## Classes
### `_StubMilestoneTracker`
- def: [`tests/test_milestones_part_b.py:24`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py#L24)
- signature: `class _StubMilestoneTracker:`
- members:
  - `is_completed(self, milestone_id)` — [`L29`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py#L29)
  - `mark_completed(self, milestone_id, timestamp=None, agent_step_count=None)` — [`L32`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py#L32)
  - `completed` — [`L26`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py#L26)
  - `marked` — [`L27`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py#L27)
- protocol/private: `__init__`[`L25`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py#L25)
- used by: (1 test-only callers)

## Functions
- `_completed_before(milestone_id)` — [`L44`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py#L44)
- `_make_emulator(completed=None)` — [`L38`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py#L38)
- `_state(location, badges=None)` — [`L49`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py#L49)
- `test_full_part_b_sequence_through_dynamo_badge()` — [`L103`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py#L103)
- `test_non_linear_dewford_paths_and_slateport_or_logic()` — [`L76`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py#L76)
- `test_order_and_comparison_are_canonical()` — [`L56`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py#L56)
- `test_route_110_requires_museum_event()` — [`L93`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py#L93)
- `test_route_116_requires_stone_badge()` — [`L67`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py#L67)

## Module values
- `PART_B_SEQUENCE` — [`L4`](../../../../../raw/code/continual-harness/tests/test_milestones_part_b.py#L4)


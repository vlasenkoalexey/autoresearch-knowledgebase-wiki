---
title: 'Module: tests/test_npc_reconciliation.py'
type: catalog
provenance: extracted
module: tests/test_npc_reconciliation.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_npc_reconciliation`/
symbols:
  test_porymap_result_contract_success: test_porymap_result_contract_success().
  test_porymap_result_contract_failure: test_porymap_result_contract_failure().
  test_reconciliation_local_id_priority: test_reconciliation_local_id_priority().
  test_reconciliation_coordinate_proximity_fallback: test_reconciliation_coordinate_proximity_fallback().
  test_reconciliation_static_reference_when_no_runtime: test_reconciliation_static_reference_when_no_runtime().
  test_pathfinding_blocks_runtime_objects_not_static_when_available: test_pathfinding_blocks_runtime_objects_not_static_when_available().
  OCEANIC_LOCATION: OCEANIC_LOCATION.
---
# Module: [`tests/test_npc_reconciliation.py`](../../../../../raw/code/continual-harness/tests/test_npc_reconciliation.py)

## Functions
- `test_pathfinding_blocks_runtime_objects_not_static_when_available()` — [`L68`](../../../../../raw/code/continual-harness/tests/test_npc_reconciliation.py#L68) — Pathfinding should prioritize runtime object_events for NPC blocking.
- `test_porymap_result_contract_failure()` — [`L20`](../../../../../raw/code/continual-harness/tests/test_npc_reconciliation.py#L20) — _format_porymap_info always returns a PorymapResult on failure.
- `test_porymap_result_contract_success()` — [`L11`](../../../../../raw/code/continual-harness/tests/test_npc_reconciliation.py#L11) — _format_porymap_info always returns a PorymapResult on success.
- `test_reconciliation_coordinate_proximity_fallback()` — [`L48`](../../../../../raw/code/continual-harness/tests/test_npc_reconciliation.py#L48) — Coordinate proximity + graphics_id should match nearby runtime NPCs.
- `test_reconciliation_local_id_priority()` — [`L28`](../../../../../raw/code/continual-harness/tests/test_npc_reconciliation.py#L28) — local_id matching should win even if coordinates are far away.
- `test_reconciliation_static_reference_when_no_runtime()` — [`L61`](../../../../../raw/code/continual-harness/tests/test_npc_reconciliation.py#L61) — No runtime NPC list should keep static porymap objects.

## Module values
- `OCEANIC_LOCATION` — [`L8`](../../../../../raw/code/continual-harness/tests/test_npc_reconciliation.py#L8)


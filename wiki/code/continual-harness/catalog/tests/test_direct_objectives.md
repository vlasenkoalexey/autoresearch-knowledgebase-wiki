---
title: 'Module: tests/test_direct_objectives.py'
type: catalog
provenance: extracted
module: tests/test_direct_objectives.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_direct_objectives`/TestDirectObjective
symbols:
  TestDirectObjectiveSerde.test_round_trip_full: Serde#test_round_trip_full().
  TestDirectObjective.test_direct_objective_creation: '#test_direct_objective_creation().'
  TestDirectObjective.test_direct_objective_defaults: '#test_direct_objective_defaults().'
  TestDirectObjectiveSerde.test_round_trip_minimal: Serde#test_round_trip_minimal().
  TestDirectObjectiveManagerSerde.test_serialize_restore_round_trip: ManagerSerde#test_serialize_restore_round_trip().
  TestDirectObjectiveSerde.test_to_dict_coords_are_list: Serde#test_to_dict_coords_are_list().
  TestDirectObjectiveManagerSerde.test_save_load_file_round_trip: ManagerSerde#test_save_load_file_round_trip().
  TestDirectObjectiveManagerSerde.test_current_objective_matches_after_restore: ManagerSerde#test_current_objective_matches_after_restore().
  TestDirectObjectiveManagerSerde.test_serialize_restore_preserves_completion: ManagerSerde#test_serialize_restore_preserves_completion().
  TestDirectObjectiveSerde.test_from_dict_coords_become_tuple: Serde#test_from_dict_coords_become_tuple().
  TestDirectObjectiveManagerSerde.populated_manager: ManagerSerde#populated_manager().
  TestDirectObjectiveManager.manager: Manager#manager().
  TestDirectObjectiveManager.test_get_first_objective_info_for_supported_sequences: Manager#test_get_first_objective_info_for_supported_sequences().
  TestDirectObjectiveIntegration.manager: Integration#manager().
  TestDirectObjective: '#'
  TestDirectObjectiveManager: Manager#
  TestDirectObjectiveManager.test_manager_initialization: Manager#test_manager_initialization().
  TestDirectObjectiveManager.test_load_categorized_full_game_sequence: Manager#test_load_categorized_full_game_sequence().
  TestDirectObjectiveManager.test_load_categorized_full_game_with_start_indexes: Manager#test_load_categorized_full_game_with_start_indexes().
  TestDirectObjectiveManager.test_load_autonomous_objective_creation_sequence: Manager#test_load_autonomous_objective_creation_sequence().
  TestDirectObjectiveManager.test_load_autonomous_sequence_mentions_replan_when_simplest_scaffold: Manager#test_load_autonomous_sequence_mentions_replan_when_simplest_scaffold().
  TestDirectObjectiveManager.test_get_categorized_objective_guidance: Manager#test_get_categorized_objective_guidance().
  TestDirectObjectiveManager.test_add_dynamic_objectives_legacy_mode: Manager#test_add_dynamic_objectives_legacy_mode().
  TestDirectObjectiveManager.test_add_objectives_to_category_updates_dynamics: Manager#test_add_objectives_to_category_updates_dynamics().
  TestDirectObjectiveManager.test_reset_sequence: Manager#test_reset_sequence().
  TestDirectObjectiveManager.test_save_completed_objectives_delegates_to_auto_save: Manager#test_save_completed_objectives_delegates_to_auto_save().
  TestDirectObjectiveSerde: Serde#
  TestDirectObjectiveManagerSerde: ManagerSerde#
  TestDirectObjectiveManagerSerde.test_json_schema_version: ManagerSerde#test_json_schema_version().
  TestDirectObjectiveIntegration: Integration#
  TestDirectObjectiveIntegration.test_categorized_progression_workflow: Integration#test_categorized_progression_workflow().
  TestDirectObjectiveIntegration.test_autonomous_sequence_can_seed_new_objectives: Integration#test_autonomous_sequence_can_seed_new_objectives().
---
# Module: [`tests/test_direct_objectives.py`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py)

## Classes
### `TestDirectObjective`
- def: [`tests/test_direct_objectives.py:19`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L19)
- signature: `class TestDirectObjective:`
- members:
  - `test_direct_objective_creation(self)` — [`L20`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L20)
  - `test_direct_objective_defaults(self)` — [`L43`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L43)
- uses (calls/refs, reference-scoped): [`id`](../agents/objectives/objective_types.md#DirectObjective.id), [`description`](../agents/objectives/objective_types.md#DirectObjective.description), [`DirectObjective`](../agents/objectives/objective_types.md#DirectObjective), [`action_type`](../agents/objectives/objective_types.md#DirectObjective.action_type), [`target_location`](../agents/objectives/objective_types.md#DirectObjective.target_location), [`completion_condition`](../agents/objectives/objective_types.md#DirectObjective.completion_condition), [`navigation_hint`](../agents/objectives/objective_types.md#DirectObjective.navigation_hint), [`priority`](../agents/objectives/objective_types.md#DirectObjective.priority), [`completed`](../agents/objectives/objective_types.md#DirectObjective.completed), [`target_coords`](../agents/objectives/objective_types.md#DirectObjective.target_coords)

### `TestDirectObjectiveIntegration`
- def: [`tests/test_direct_objectives.py:330`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L330)
- signature: `class TestDirectObjectiveIntegration:`
- members:
  - `manager(self)` — [`L332`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L332)
  - `test_autonomous_sequence_can_seed_new_objectives(self, manager)` — [`L349`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L349)
  - `test_categorized_progression_workflow(self, manager)` — [`L335`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L335)
- uses (calls/refs, reference-scoped): [`DirectObjectiveManager`](../agents/objectives/direct_objectives.md#DirectObjectiveManager)

### `TestDirectObjectiveManager`
- def: [`tests/test_direct_objectives.py:58`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L58)
- signature: `class TestDirectObjectiveManager:`
- members:
  - `manager(self)` — [`L60`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L60)
  - `test_add_dynamic_objectives_legacy_mode(self, manager)` — [`L129`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L129)
  - `test_add_objectives_to_category_updates_dynamics(self, manager)` — [`L150`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L150)
  - `test_get_categorized_objective_guidance(self, manager)` — [`L119`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L119)
  - `test_get_first_objective_info_for_supported_sequences(self)` — [`L109`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L109)
  - `test_load_autonomous_objective_creation_sequence(self, manager)` — [`L90`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L90)
  - `test_load_autonomous_sequence_mentions_replan_when_simplest_scaffold(self, manager, monkeypatch)` — [`L100`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L100)
  - `test_load_categorized_full_game_sequence(self, manager)` — [`L69`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L69)
  - `test_load_categorized_full_game_with_start_indexes(self, manager)` — [`L80`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L80)
  - `test_manager_initialization(self, manager)` — [`L63`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L63)
  - `test_reset_sequence(self, manager)` — [`L168`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L168)
  - `test_save_completed_objectives_delegates_to_auto_save(self, manager)` — [`L179`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L179) — save_completed_objectives is deprecated and should delegate to auto_save.
- uses (calls/refs, reference-scoped): [`DirectObjectiveManager`](../agents/objectives/direct_objectives.md#DirectObjectiveManager), [`get_first_objective_info`](../agents/objectives/direct_objectives.md#get_first_objective_info)

### `TestDirectObjectiveManagerSerde`
- def: [`tests/test_direct_objectives.py:263`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L263)
- doc: Tests for serialize_full_state / restore_from_state round-trip.
- signature: `class TestDirectObjectiveManagerSerde:`
- members:
  - `populated_manager(self)` — [`L267`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L267)
  - `test_current_objective_matches_after_restore(self, populated_manager)` — [`L311`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L311)
  - `test_json_schema_version(self, populated_manager)` — [`L323`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L323)
  - `test_save_load_file_round_trip(self, populated_manager)` — [`L298`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L298)
  - `test_serialize_restore_preserves_completion(self, populated_manager)` — [`L290`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L290)
  - `test_serialize_restore_round_trip(self, populated_manager)` — [`L276`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L276)
- uses (calls/refs, reference-scoped): [`id`](../agents/objectives/objective_types.md#DirectObjective.id), [`description`](../agents/objectives/objective_types.md#DirectObjective.description), [`story_sequence`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.story_sequence), [`add_objectives_to_category`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.add_objectives_to_category), [`load_categorized_full_game_sequence`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.load_categorized_full_game_sequence), [`restore_from_state`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.restore_from_state), [`_get_current_objective_for_category`](../agents/objectives/direct_objectives.md#DirectObjectiveManager._get_current_objective_for_category), [`completed`](../agents/objectives/objective_types.md#DirectObjective.completed), [`battling_sequence`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.battling_sequence), [`story_index`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.story_index), [`dynamics_sequence`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.dynamics_sequence), [`battling_index`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.battling_index), [`mode`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.mode), [`dynamics_index`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.dynamics_index), [`sequence_name`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.sequence_name), [`DirectObjectiveManager`](../agents/objectives/direct_objectives.md#DirectObjectiveManager), [`load_from_file`](../agents/objectives/direct_objectives.md#DirectObjectiveManager.load_from_file)

### `TestDirectObjectiveSerde`
- def: [`tests/test_direct_objectives.py:199`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L199)
- doc: Tests for DirectObjective.to_dict / from_dict round-trip.
- signature: `class TestDirectObjectiveSerde:`
- members:
  - `test_from_dict_coords_become_tuple(self)` — [`L256`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L256)
  - `test_round_trip_full(self)` — [`L202`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L202)
  - `test_round_trip_minimal(self)` — [`L238`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L238)
  - `test_to_dict_coords_are_list(self)` — [`L249`](../../../../../raw/code/continual-harness/tests/test_direct_objectives.py#L249)
- uses (calls/refs, reference-scoped): [`id`](../agents/objectives/objective_types.md#DirectObjective.id), [`description`](../agents/objectives/objective_types.md#DirectObjective.description), [`DirectObjective`](../agents/objectives/objective_types.md#DirectObjective), [`action_type`](../agents/objectives/objective_types.md#DirectObjective.action_type), [`target_location`](../agents/objectives/objective_types.md#DirectObjective.target_location), [`completion_condition`](../agents/objectives/objective_types.md#DirectObjective.completion_condition), [`navigation_hint`](../agents/objectives/objective_types.md#DirectObjective.navigation_hint), [`priority`](../agents/objectives/objective_types.md#DirectObjective.priority), [`category`](../agents/objectives/objective_types.md#DirectObjective.category), [`prerequisite_story_objective`](../agents/objectives/objective_types.md#DirectObjective.prerequisite_story_objective), [`recommended_battling_objectives`](../agents/objectives/objective_types.md#DirectObjective.recommended_battling_objectives), [`to_dict`](../agents/objectives/objective_types.md#DirectObjective.to_dict), [`completed`](../agents/objectives/objective_types.md#DirectObjective.completed), [`optional`](../agents/objectives/objective_types.md#DirectObjective.optional), [`target_coords`](../agents/objectives/objective_types.md#DirectObjective.target_coords), [`completed_at`](../agents/objectives/objective_types.md#DirectObjective.completed_at), [`from_dict`](../agents/objectives/objective_types.md#DirectObjective.from_dict)


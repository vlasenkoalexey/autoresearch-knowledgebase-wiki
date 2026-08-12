---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.tests.test_experience_memory`/
symbols:
  make_node: make_node().
  experience: experience.
  attach_card: attach_card().
  test_improve_experience_memory_includes_parent_card_and_board_stats: test_improve_experience_memory_includes_parent_card_and_board_stats().
  test_crossover_experience_memory_includes_two_cards_and_complementarity: test_crossover_experience_memory_includes_two_cards_and_complementarity().
  test_collect_operator_memory_nodes_uses_parent_ancestors_and_top_siblings: test_collect_operator_memory_nodes_uses_parent_ancestors_and_top_siblings().
  spec: spec.
  test_auto_card_extracts_method_family_delta_and_novelty: test_auto_card_extracts_method_family_delta_and_novelty().
  test_parent_utilities_combine_score_delta_and_novelty: test_parent_utilities_combine_score_delta_and_novelty().
  test_parent_utilities_use_self_validation_not_official_score: test_parent_utilities_use_self_validation_not_official_score().
  test_parent_utilities_can_switch_score_component_normalization: test_parent_utilities_can_switch_score_component_normalization().
  test_parent_utilities_can_switch_delta_component_normalization: test_parent_utilities_can_switch_delta_component_normalization().
  test_debug_experience_memory_includes_current_error_and_repeated_errors: test_debug_experience_memory_includes_current_error_and_repeated_errors().
  test_board_aggregates_family_stats_and_repeated_errors: test_board_aggregates_family_stats_and_repeated_errors().
  test_method_and_error_helpers_are_stable: test_method_and_error_helpers_are_stable().
  test_board_repeated_errors_ignores_successful_polluted_cards: test_board_repeated_errors_ignores_successful_polluted_cards().
  test_prompt_memory_master_switch_disables_targeted_memory: test_prompt_memory_master_switch_disables_targeted_memory().
  EXPERIENCE_PATH: EXPERIENCE_PATH.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py)

## Functions
- `attach_card(node, *, fitness=None, delta=None, family="lightgbm", rich_summary=None, runtime=12)` — [`L39`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L39)
- `make_node(code: str, metric: float | None, *, parents=None, is_buggy=False)` — [`L23`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L23)
- `test_auto_card_extracts_method_family_delta_and_novelty()` — [`L58`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L58)
- `test_board_aggregates_family_stats_and_repeated_errors()` — [`L92`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L92)
- `test_board_repeated_errors_ignores_successful_polluted_cards()` — [`L309`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L309)
- `test_collect_operator_memory_nodes_uses_parent_ancestors_and_top_siblings()` — [`L465`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L465)
- `test_crossover_experience_memory_includes_two_cards_and_complementarity()` — [`L377`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L377)
- `test_debug_experience_memory_includes_current_error_and_repeated_errors()` — [`L416`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L416)
- `test_improve_experience_memory_includes_parent_card_and_board_stats()` — [`L344`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L344)
- `test_method_and_error_helpers_are_stable()` — [`L300`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L300)
- `test_parent_utilities_can_switch_delta_component_normalization()` — [`L268`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L268)
- `test_parent_utilities_can_switch_score_component_normalization()` — [`L224`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L224)
- `test_parent_utilities_combine_score_delta_and_novelty()` — [`L151`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L151)
- `test_parent_utilities_use_self_validation_not_official_score()` — [`L178`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L178)
- `test_prompt_memory_master_switch_disables_targeted_memory()` — [`L502`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L502)

## Module values
- `EXPERIENCE_PATH` — [`L9`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L9)
- `experience` — [`L18`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L18)
- `spec` — [`L17`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_experience_memory.py#L17)


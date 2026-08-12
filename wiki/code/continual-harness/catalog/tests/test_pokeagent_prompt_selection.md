---
title: 'Module: tests/test_pokeagent_prompt_selection.py'
type: catalog
provenance: extracted
module: tests/test_pokeagent_prompt_selection.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_pokeagent_prompt_selection`/
symbols:
  _POKE_MODULE: _POKE_MODULE.
  test_auto_system_uses_pokeagent_with_optimization_and_run_manager: test_auto_system_uses_pokeagent_with_optimization_and_run_manager().
  test_auto_system_uses_pokeagent_without_optimization: test_auto_system_uses_pokeagent_without_optimization().
  test_optimization_requested_no_run_manager_raises: test_optimization_requested_no_run_manager_raises().
  test_explicit_system_path_still_requires_run_manager_for_optimization: test_explicit_system_path_still_requires_run_manager_for_optimization().
  test_simple_scaffold_uses_simple_prompt: test_simple_scaffold_uses_simple_prompt().
  test_simplest_scaffold_uses_simplest_prompt: test_simplest_scaffold_uses_simplest_prompt().
  test_continualharness_scaffold_uses_continualharness_prompt: test_continualharness_scaffold_uses_continualharness_prompt().
  test_tool_declarations_via_pokeagent: test_tool_declarations_via_pokeagent().
  test_simplest_prompt_excludes_stores_and_objectives: test_simplest_prompt_excludes_stores_and_objectives().
  test_simple_prompt_includes_all_sections: test_simple_prompt_includes_all_sections().
  _filename_arg: _filename_arg().
  test_tool_declarations_per_scaffold: test_tool_declarations_per_scaffold().
  EXPECTED_TOOLS_PER_SCAFFOLD: EXPECTED_TOOLS_PER_SCAFFOLD.
  test_run_scaffold_contract_uses_continualharness_not_legacy_name: test_run_scaffold_contract_uses_continualharness_not_legacy_name().
---
# Module: [`tests/test_pokeagent_prompt_selection.py`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py)

## Functions
- `_filename_arg(load_mock)` — [`L22`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py#L22) — Bound-method mock may record (filename,) or (self, filename).
- `test_auto_system_uses_pokeagent_with_optimization_and_run_manager()` — [`L41`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py#L41)
- `test_auto_system_uses_pokeagent_without_optimization()` — [`L28`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py#L28)
- `test_continualharness_scaffold_uses_continualharness_prompt()` — [`L118`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py#L118)
- `test_explicit_system_path_still_requires_run_manager_for_optimization()` — [`L73`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py#L73)
- `test_optimization_requested_no_run_manager_raises()` — [`L57`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py#L57) — Prompt optimization without run_data_manager is a configuration error.
- `test_run_scaffold_contract_uses_continualharness_not_legacy_name()` — [`L162`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py#L162)
- `test_simple_prompt_includes_all_sections()` — [`L230`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py#L230) — The simple scaffold prompt should still include all standard sections.
- `test_simple_scaffold_uses_simple_prompt()` — [`L92`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py#L92)
- `test_simplest_prompt_excludes_stores_and_objectives()` — [`L197`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py#L197) — The simplest scaffold prompt must omit OBJECTIVES, SKILL LIBRARY, and SUBAGENT REGISTRY.
- `test_simplest_scaffold_uses_simplest_prompt()` — [`L105`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py#L105)
- `test_tool_declarations_per_scaffold(scaffold)` — [`L169`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py#L169) — Each scaffold gets exactly the expected set of tools from the registry.
- `test_tool_declarations_via_pokeagent(scaffold)` — [`L180`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py#L180) — PokeAgent._create_tool_declarations delegates to the registry correctly.

## Module values
- `EXPECTED_TOOLS_PER_SCAFFOLD` — [`L135`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py#L135)
- `_POKE_MODULE` — [`L19`](../../../../../raw/code/continual-harness/tests/test_pokeagent_prompt_selection.py#L19)


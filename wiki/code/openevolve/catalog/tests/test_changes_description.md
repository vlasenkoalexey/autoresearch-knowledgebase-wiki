---
title: 'Module: tests/test_changes_description.py'
type: catalog
provenance: extracted
module: tests/test_changes_description.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_changes_description`/Test
symbols:
  TestChangesDescriptionFromDict.test_all_changes_description_options: ChangesDescriptionFromDict#test_all_changes_description_options().
  TestChangesDescriptionValidation.test_works_with_diff_based_evolution_enabled: ChangesDescriptionValidation#test_works_with_diff_based_evolution_enabled().
  TestChangesDescriptionValidation.test_disabled_without_diff_based_evolution_is_ok: ChangesDescriptionValidation#test_disabled_without_diff_based_evolution_is_ok().
  TestChangesDescriptionFromDict.test_custom_system_message: ChangesDescriptionFromDict#test_custom_system_message().
  TestChangesDescriptionFromDict.test_custom_initial_description: ChangesDescriptionFromDict#test_custom_initial_description().
  TestPromptConfigChangesDescription.test_prompt_config_defaults: PromptConfigChangesDescription#test_prompt_config_defaults().
  TestPromptConfigChangesDescription.test_prompt_config_custom_values: PromptConfigChangesDescription#test_prompt_config_custom_values().
  TestChangesDescriptionConfigDefaults.test_programs_as_changes_description_default_false: ChangesDescriptionConfigDefaults#test_programs_as_changes_description_default_false().
  TestChangesDescriptionConfigDefaults.test_system_message_changes_description_default_none: ChangesDescriptionConfigDefaults#test_system_message_changes_description_default_none().
  TestChangesDescriptionConfigDefaults.test_initial_changes_description_default_empty: ChangesDescriptionConfigDefaults#test_initial_changes_description_default_empty().
  TestChangesDescriptionValidation.test_requires_diff_based_evolution: ChangesDescriptionValidation#test_requires_diff_based_evolution().
  TestChangesDescriptionConfigDefaults: ChangesDescriptionConfigDefaults#
  TestChangesDescriptionValidation: ChangesDescriptionValidation#
  TestChangesDescriptionFromDict: ChangesDescriptionFromDict#
  TestPromptConfigChangesDescription: PromptConfigChangesDescription#
---
# Module: [`tests/test_changes_description.py`](../../../../../raw/code/openevolve/tests/test_changes_description.py)

## Classes
### `TestChangesDescriptionConfigDefaults`  ·  implements/extends TestCase
- def: [`tests/test_changes_description.py:11`](../../../../../raw/code/openevolve/tests/test_changes_description.py#L11)
- doc: Tests for changes description configuration defaults
- signature: `class TestChangesDescriptionConfigDefaults(unittest.TestCase):`
- members:
  - `test_initial_changes_description_default_empty(self)` — [`L24`](../../../../../raw/code/openevolve/tests/test_changes_description.py#L24) — Test that initial_changes_description defaults to empty string
  - `test_programs_as_changes_description_default_false(self)` — [`L14`](../../../../../raw/code/openevolve/tests/test_changes_description.py#L14) — Test that programs_as_changes_description defaults to False
  - `test_system_message_changes_description_default_none(self)` — [`L19`](../../../../../raw/code/openevolve/tests/test_changes_description.py#L19) — Test that system_message_changes_description defaults to None
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`prompt`](../openevolve/config.md#Config.prompt), [`programs_as_changes_description`](../openevolve/config.md#PromptConfig.programs_as_changes_description), [`initial_changes_description`](../openevolve/config.md#PromptConfig.initial_changes_description), [`system_message_changes_description`](../openevolve/config.md#PromptConfig.system_message_changes_description)

### `TestChangesDescriptionFromDict`  ·  implements/extends TestCase
- def: [`tests/test_changes_description.py:72`](../../../../../raw/code/openevolve/tests/test_changes_description.py#L72)
- doc: Tests for loading changes description config from dict
- signature: `class TestChangesDescriptionFromDict(unittest.TestCase):`
- members:
  - `test_all_changes_description_options(self)` — [`L107`](../../../../../raw/code/openevolve/tests/test_changes_description.py#L107) — Test setting all changes description options together
  - `test_custom_initial_description(self)` — [`L91`](../../../../../raw/code/openevolve/tests/test_changes_description.py#L91) — Test setting custom initial_changes_description
  - `test_custom_system_message(self)` — [`L75`](../../../../../raw/code/openevolve/tests/test_changes_description.py#L75) — Test setting custom system_message_changes_description
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`prompt`](../openevolve/config.md#Config.prompt), [`from_dict`](../openevolve/config.md#Config.from_dict), [`programs_as_changes_description`](../openevolve/config.md#PromptConfig.programs_as_changes_description), [`initial_changes_description`](../openevolve/config.md#PromptConfig.initial_changes_description), [`system_message_changes_description`](../openevolve/config.md#PromptConfig.system_message_changes_description)

### `TestChangesDescriptionValidation`  ·  implements/extends TestCase
- def: [`tests/test_changes_description.py:30`](../../../../../raw/code/openevolve/tests/test_changes_description.py#L30)
- doc: Tests for changes description validation rules
- signature: `class TestChangesDescriptionValidation(unittest.TestCase):`
- members:
  - `test_disabled_without_diff_based_evolution_is_ok(self)` — [`L59`](../../../../../raw/code/openevolve/tests/test_changes_description.py#L59) — Test that disabled changes description works without diff_based_evolution
  - `test_requires_diff_based_evolution(self)` — [`L33`](../../../../../raw/code/openevolve/tests/test_changes_description.py#L33) — Test that programs_as_changes_description requires diff_based_evolution
  - `test_works_with_diff_based_evolution_enabled(self)` — [`L46`](../../../../../raw/code/openevolve/tests/test_changes_description.py#L46) — Test that changes description works when diff_based_evolution=True
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`prompt`](../openevolve/config.md#Config.prompt), [`from_dict`](../openevolve/config.md#Config.from_dict), [`programs_as_changes_description`](../openevolve/config.md#PromptConfig.programs_as_changes_description), [`diff_based_evolution`](../openevolve/config.md#Config.diff_based_evolution)

### `TestPromptConfigChangesDescription`  ·  implements/extends TestCase
- def: [`tests/test_changes_description.py:130`](../../../../../raw/code/openevolve/tests/test_changes_description.py#L130)
- doc: Tests for PromptConfig changes description fields
- signature: `class TestPromptConfigChangesDescription(unittest.TestCase):`
- members:
  - `test_prompt_config_custom_values(self)` — [`L140`](../../../../../raw/code/openevolve/tests/test_changes_description.py#L140) — Test PromptConfig with custom changes description values
  - `test_prompt_config_defaults(self)` — [`L133`](../../../../../raw/code/openevolve/tests/test_changes_description.py#L133) — Test PromptConfig defaults for changes description
- uses (calls/refs, reference-scoped): [`programs_as_changes_description`](../openevolve/config.md#PromptConfig.programs_as_changes_description), [`PromptConfig`](../openevolve/config.md#PromptConfig), [`initial_changes_description`](../openevolve/config.md#PromptConfig.initial_changes_description), [`system_message_changes_description`](../openevolve/config.md#PromptConfig.system_message_changes_description)


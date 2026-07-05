---
title: 'Module: tests/test_early_stopping_config.py'
type: catalog
provenance: extracted
module: tests/test_early_stopping_config.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_early_stopping_config`/TestEarlyStopping
symbols:
  TestEarlyStoppingConfigFromDict.test_all_early_stopping_options: ConfigFromDict#test_all_early_stopping_options().
  TestEarlyStoppingConfigFromDict.test_custom_patience: ConfigFromDict#test_custom_patience().
  TestEarlyStoppingConfigFromDict.test_custom_convergence_threshold: ConfigFromDict#test_custom_convergence_threshold().
  TestEarlyStoppingConfigFromDict.test_custom_metric: ConfigFromDict#test_custom_metric().
  TestEarlyStoppingConfigFromDict.test_zero_patience_disables_early_stopping: ConfigFromDict#test_zero_patience_disables_early_stopping().
  TestEarlyStoppingConfigFromDict.test_negative_patience_allowed: ConfigFromDict#test_negative_patience_allowed().
  TestEarlyStoppingConfigDefaults.test_patience_default_is_none: ConfigDefaults#test_patience_default_is_none().
  TestEarlyStoppingConfigDefaults.test_convergence_threshold_default: ConfigDefaults#test_convergence_threshold_default().
  TestEarlyStoppingConfigDefaults.test_metric_default: ConfigDefaults#test_metric_default().
  TestEarlyStoppingWithYaml.test_config_to_dict_includes_early_stopping: WithYaml#test_config_to_dict_includes_early_stopping().
  TestEarlyStoppingConfigDefaults: ConfigDefaults#
  TestEarlyStoppingConfigFromDict: ConfigFromDict#
  TestEarlyStoppingWithYaml: WithYaml#
---
# Module: [`tests/test_early_stopping_config.py`](../../../../../raw/code/openevolve/tests/test_early_stopping_config.py)

## Classes
### `TestEarlyStoppingConfigDefaults`  ·  implements/extends TestCase
- def: [`tests/test_early_stopping_config.py:10`](../../../../../raw/code/openevolve/tests/test_early_stopping_config.py#L10)
- doc: Tests for early stopping configuration defaults
- signature: `class TestEarlyStoppingConfigDefaults(unittest.TestCase):`
- members:
  - `test_convergence_threshold_default(self)` — [`L18`](../../../../../raw/code/openevolve/tests/test_early_stopping_config.py#L18) — Test that convergence_threshold defaults to 0.001
  - `test_metric_default(self)` — [`L23`](../../../../../raw/code/openevolve/tests/test_early_stopping_config.py#L23) — Test that early_stopping_metric defaults to combined_score
  - `test_patience_default_is_none(self)` — [`L13`](../../../../../raw/code/openevolve/tests/test_early_stopping_config.py#L13) — Test that early_stopping_patience defaults to None (disabled)
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`early_stopping_patience`](../openevolve/config.md#Config.early_stopping_patience), [`early_stopping_metric`](../openevolve/config.md#Config.early_stopping_metric), [`convergence_threshold`](../openevolve/config.md#Config.convergence_threshold)

### `TestEarlyStoppingConfigFromDict`  ·  implements/extends TestCase
- def: [`tests/test_early_stopping_config.py:29`](../../../../../raw/code/openevolve/tests/test_early_stopping_config.py#L29)
- doc: Tests for loading early stopping config from dict
- signature: `class TestEarlyStoppingConfigFromDict(unittest.TestCase):`
- members:
  - `test_all_early_stopping_options(self)` — [`L59`](../../../../../raw/code/openevolve/tests/test_early_stopping_config.py#L59) — Test setting all early stopping options together
  - `test_custom_convergence_threshold(self)` — [`L41`](../../../../../raw/code/openevolve/tests/test_early_stopping_config.py#L41) — Test setting custom convergence_threshold
  - `test_custom_metric(self)` — [`L50`](../../../../../raw/code/openevolve/tests/test_early_stopping_config.py#L50) — Test setting custom early_stopping_metric
  - `test_custom_patience(self)` — [`L32`](../../../../../raw/code/openevolve/tests/test_early_stopping_config.py#L32) — Test setting custom early_stopping_patience
  - `test_negative_patience_allowed(self)` — [`L81`](../../../../../raw/code/openevolve/tests/test_early_stopping_config.py#L81) — Test that negative patience is allowed (but probably shouldn't be used)
  - `test_zero_patience_disables_early_stopping(self)` — [`L72`](../../../../../raw/code/openevolve/tests/test_early_stopping_config.py#L72) — Test that patience=0 effectively disables early stopping
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`from_dict`](../openevolve/config.md#Config.from_dict), [`early_stopping_patience`](../openevolve/config.md#Config.early_stopping_patience), [`early_stopping_metric`](../openevolve/config.md#Config.early_stopping_metric), [`convergence_threshold`](../openevolve/config.md#Config.convergence_threshold)

### `TestEarlyStoppingWithYaml`  ·  implements/extends TestCase
- def: [`tests/test_early_stopping_config.py:92`](../../../../../raw/code/openevolve/tests/test_early_stopping_config.py#L92)
- doc: Tests for early stopping config from YAML
- signature: `class TestEarlyStoppingWithYaml(unittest.TestCase):`
- members:
  - `test_config_to_dict_includes_early_stopping(self)` — [`L95`](../../../../../raw/code/openevolve/tests/test_early_stopping_config.py#L95) — Test that to_dict includes early stopping settings
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`to_dict`](../openevolve/config.md#Config.to_dict)


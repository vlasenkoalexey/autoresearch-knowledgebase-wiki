---
title: 'Module: rdagent/components/coder/data_science/share/ds_costeer.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/share/ds_costeer.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.share.ds_costeer`/DSCoSTEER#
symbols:
  DSCoSTEER: ''
  DSCoSTEER.get_develop_max_seconds: get_develop_max_seconds().
---
# Module: [`rdagent/components/coder/data_science/share/ds_costeer.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/ds_costeer.py)

## Classes
### `DSCoSTEER`  ·  implements/extends CoSTEER
- def: [`rdagent/components/coder/data_science/share/ds_costeer.py:4`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/ds_costeer.py#L4)
- signature: `class DSCoSTEER(CoSTEER):`
- members:
  - `get_develop_max_seconds(self)` — [`L5`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/ds_costeer.py#L5) — The coder uses the scenario's real debug timeout as the maximum seconds for development.
- uses (calls/refs, reference-scoped): [`CoSTEER`](../../CoSTEER/__init__.md#CoSTEER), [`scen`](../../../../core/developer.md#Developer.scen), [`DataLoaderCoSTEER`](../raw_data_loader/__init__.md#DataLoaderCoSTEER), [`EnsembleCoSTEER`](../ensemble/__init__.md#EnsembleCoSTEER), [`FeatureCoSTEER`](../feature/__init__.md#FeatureCoSTEER), [`ModelCoSTEER`](../model/__init__.md#ModelCoSTEER), [`WorkflowCoSTEER`](../workflow/__init__.md#WorkflowCoSTEER), [`settings`](../../CoSTEER/__init__.md#CoSTEER.settings), [`PipelineCoSTEER`](../pipeline/__init__.md#PipelineCoSTEER), [`max_seconds_multiplier`](../../CoSTEER/config.md#CoSTEERSettings.max_seconds_multiplier)
- used by: [`CoSTEER`](../../CoSTEER/__init__.md#CoSTEER), [`get_develop_max_seconds`](../../CoSTEER/__init__.md#CoSTEER.get_develop_max_seconds), [`DataLoaderCoSTEER`](../raw_data_loader/__init__.md#DataLoaderCoSTEER), [`EnsembleCoSTEER`](../ensemble/__init__.md#EnsembleCoSTEER), [`FeatureCoSTEER`](../feature/__init__.md#FeatureCoSTEER), [`ModelCoSTEER`](../model/__init__.md#ModelCoSTEER), [`WorkflowCoSTEER`](../workflow/__init__.md#WorkflowCoSTEER), [`PipelineCoSTEER`](../pipeline/__init__.md#PipelineCoSTEER)


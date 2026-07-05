---
title: 'Module: rdagent/scenarios/qlib/developer/utils.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/qlib/developer/utils.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.qlib.developer.utils`/
symbols:
  process_factor_data: process_factor_data().
  _build_execute_calls: _build_execute_calls().
  _build_base_feature_workspaces: _build_base_feature_workspaces().
  _process_message_and_df: _process_message_and_df().
  _normalize_factor_index: _normalize_factor_index().
  _resolve_index_level_values: _resolve_index_level_values().
  _format_index_info: _format_index_info().
---
# Module: [`rdagent/scenarios/qlib/developer/utils.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/utils.py)

## Functions
- `_build_base_feature_workspaces(exp: QlibFactorExperiment)` — [`L14`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/utils.py#L14)
- `_build_execute_calls(exp: QlibFactorExperiment, base_feature_workspaces: list[FactorFBWorkspace])` — [`L29`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/utils.py#L29)
- `_format_index_info(df: pd.DataFrame | None)` — [`L94`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/utils.py#L94)
- `_normalize_factor_index(df: pd.DataFrame)` — [`L68`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/utils.py#L68) — Normalize factor index to a 2-level MultiIndex: (datetime, instrument).
- `_process_message_and_df(source_name: str, message: str, df: pd.DataFrame | None, factor_dfs: list[pd.DataFrame], error_message: str)` — [`L100`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/utils.py#L100)
- `_resolve_index_level_values(df: pd.DataFrame, level_name: str)` — [`L44`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/utils.py#L44)
- `process_factor_data(exp_or_list: List[QlibFactorExperiment] | QlibFactorExperiment)` — [`L131`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/utils.py#L131) — Process and combine factor data from experiment implementations.


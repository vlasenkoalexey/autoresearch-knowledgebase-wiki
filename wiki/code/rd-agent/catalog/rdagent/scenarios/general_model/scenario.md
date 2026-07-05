---
title: 'Module: rdagent/scenarios/general_model/scenario.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/general_model/scenario.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.general_model.scenario`/GeneralModelScenario#
symbols:
  GeneralModelScenario.get_scenario_all_desc: get_scenario_all_desc().
  GeneralModelScenario: ''
  GeneralModelScenario._background: _background.
  GeneralModelScenario._output_format: _output_format.
  GeneralModelScenario._interface: _interface.
  GeneralModelScenario._simulator: _simulator.
  GeneralModelScenario._rich_style_description: _rich_style_description.
  GeneralModelScenario.background: background().
  GeneralModelScenario.output_format: output_format().
  GeneralModelScenario.interface: interface().
  GeneralModelScenario.simulator: simulator().
  GeneralModelScenario.rich_style_description: rich_style_description().
  GeneralModelScenario.__init__: __init__().
  GeneralModelScenario.source_data: source_data().
  GeneralModelScenario.get_runtime_environment: get_runtime_environment().
---
# Module: [`rdagent/scenarios/general_model/scenario.py`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py)

## Classes
### `GeneralModelScenario`  ·  implements/extends Scenario
- def: [`rdagent/scenarios/general_model/scenario.py:8`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py#L8)
- signature: `class GeneralModelScenario(Scenario):`
- members:
  - `background(self)` — [`L18`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py#L18)
  - `get_runtime_environment(self)` — [`L54`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py#L54)
  - `get_scenario_all_desc(self, task: Task | None = None, filtered_tag: str | None = None, simple_background: bool | None = None)` — [`L41`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py#L41)
  - `interface(self)` — [`L30`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py#L30)
  - `output_format(self)` — [`L26`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py#L26)
  - `rich_style_description(self)` — [`L38`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py#L38)
  - `simulator(self)` — [`L34`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py#L34)
  - `source_data(self)` — [`L22`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py#L22)
- protocol/private: `__init__`[`L9`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py#L9), `_background`[`L11`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py#L11), `_interface`[`L13`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py#L13), `_output_format`[`L12`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py#L12), `_rich_style_description`[`L15`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py#L15), `_simulator`[`L14`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/general_model/scenario.py#L14)
- uses (calls/refs, reference-scoped): [`T`](../../utils/agent/tpl.md#T), [`r`](../../utils/agent/tpl.md#RDAT.r), [`Scenario`](../../core/scenario.md#Scenario), [`Task`](../../core/experiment.md#Task)
- used by: [`Scenario`](../../core/scenario.md#Scenario), [`get_scenario_all_desc`](../../core/scenario.md#Scenario.get_scenario_all_desc), [`summary_window`](../../log/ui/app.md#summary_window), [`extract_models_and_implement`](../../app/general_model/general_model.md#extract_models_and_implement), [`research_window`](../../log/ui/app.md#research_window), [`d_c`](../../log/ui/app.md#d_c), [`get_runtime_environment`](../../core/scenario.md#Scenario.get_runtime_environment), [`background`](../../core/scenario.md#Scenario.background), [`rich_style_description`](../../core/scenario.md#Scenario.rich_style_description), [`source_data`](../../core/scenario.md#Scenario.source_data), [`toc`](../../log/ui/app.md#toc), [`css`](../../log/ui/app.md#css)


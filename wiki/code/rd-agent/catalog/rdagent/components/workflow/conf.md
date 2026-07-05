---
title: 'Module: rdagent/components/workflow/conf.py'
type: catalog
provenance: extracted
module: rdagent/components/workflow/conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.workflow.conf`/BasePropSetting#
symbols:
  BasePropSetting: ''
  BasePropSetting.scen: scen.
  BasePropSetting.hypothesis_gen: hypothesis_gen.
  BasePropSetting.summarizer: summarizer.
  BasePropSetting.hypothesis2experiment: hypothesis2experiment.
  BasePropSetting.knowledge_base: knowledge_base.
  BasePropSetting.coder: coder.
  BasePropSetting.runner: runner.
  BasePropSetting.knowledge_base_path: knowledge_base_path.
  BasePropSetting.interactor: interactor.
  BasePropSetting.evolving_n: evolving_n.
---
# Module: [`rdagent/components/workflow/conf.py`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/conf.py)

## Classes
### `BasePropSetting`  ·  implements/extends ExtendedBaseSettings
- def: [`rdagent/components/workflow/conf.py:4`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/conf.py#L4) — documented in [rdagent-core-conf](../../../../concepts/rdagent-core-conf.md)
- doc: The common part of the config for RD Loop to propose and development
- signature: `class BasePropSetting(ExtendedBaseSettings):`
- members:
  - `coder` — [`L16`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/conf.py#L16)
  - `evolving_n` — [`L20`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/conf.py#L20)
  - `hypothesis2experiment` — [`L15`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/conf.py#L15)
  - `hypothesis_gen` — [`L13`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/conf.py#L13)
  - `interactor` — [`L14`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/conf.py#L14)
  - `knowledge_base` — [`L11`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/conf.py#L11)
  - `knowledge_base_path` — [`L12`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/conf.py#L12)
  - `runner` — [`L17`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/conf.py#L17)
  - `scen` — [`L10`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/conf.py#L10)
  - `summarizer` — [`L18`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/conf.py#L18)
- uses (calls/refs, reference-scoped): [`ExtendedBaseSettings`](../../core/conf.md#ExtendedBaseSettings), [`FactorBasePropSetting`](../../app/qlib_rd_loop/conf.md#FactorBasePropSetting), [`ModelBasePropSetting`](../../app/qlib_rd_loop/conf.md#ModelBasePropSetting), [`QuantBasePropSetting`](../../app/qlib_rd_loop/conf.md#QuantBasePropSetting)
- used by: [`ExtendedBaseSettings`](../../core/conf.md#ExtendedBaseSettings), [`trace`](../../scenarios/data_science/loop.md#DataScienceRDLoop.trace), [`__init__`](rd_loop.md#RDLoop.__init__), [`__init__`](../../app/kaggle/loop.md#KaggleRDLoop.__init__), [`__init__`](../../scenarios/data_science/loop.md#DataScienceRDLoop.__init__), [`hypothesis2experiment`](../../app/kaggle/loop.md#KaggleRDLoop.hypothesis2experiment), [`hypothesis_gen`](../../app/kaggle/loop.md#KaggleRDLoop.hypothesis_gen), [`summarizer`](../../app/kaggle/loop.md#KaggleRDLoop.summarizer), [`__init__`](../../app/qlib_rd_loop/quant.md#QuantRDLoop.__init__), [`summarizer`](rd_loop.md#RDLoop.summarizer), [`coder`](rd_loop.md#RDLoop.coder), [`exp_gen`](../../scenarios/data_science/loop.md#DataScienceRDLoop.exp_gen), [`runner`](rd_loop.md#RDLoop.runner), [`hypothesis_gen`](rd_loop.md#RDLoop.hypothesis_gen), [`FactorBasePropSetting`](../../app/qlib_rd_loop/conf.md#FactorBasePropSetting), [`hypothesis2experiment`](rd_loop.md#RDLoop.hypothesis2experiment), [`interactor`](../../scenarios/data_science/loop.md#DataScienceRDLoop.interactor), [`ModelBasePropSetting`](../../app/qlib_rd_loop/conf.md#ModelBasePropSetting), [`QuantBasePropSetting`](../../app/qlib_rd_loop/conf.md#QuantBasePropSetting)


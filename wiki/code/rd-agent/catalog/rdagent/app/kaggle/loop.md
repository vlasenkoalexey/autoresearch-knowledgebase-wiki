---
title: 'Module: rdagent/app/kaggle/loop.py'
type: catalog
provenance: extracted
module: rdagent/app/kaggle/loop.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.kaggle.loop`/
symbols:
  KaggleRDLoop.running: KaggleRDLoop#running().
  main: main().
  KaggleRDLoop.coding: KaggleRDLoop#coding().
  KaggleRDLoop.__init__: KaggleRDLoop#__init__().
  KaggleRDLoop.hypothesis_gen: KaggleRDLoop#hypothesis_gen.
  KaggleRDLoop.hypothesis2experiment: KaggleRDLoop#hypothesis2experiment.
  KaggleRDLoop.summarizer: KaggleRDLoop#summarizer.
  KaggleRDLoop.feature_coder: KaggleRDLoop#feature_coder.
  KaggleRDLoop.model_feature_selection_coder: KaggleRDLoop#model_feature_selection_coder.
  KaggleRDLoop.model_coder: KaggleRDLoop#model_coder.
  KaggleRDLoop.feature_runner: KaggleRDLoop#feature_runner.
  KaggleRDLoop.model_runner: KaggleRDLoop#model_runner.
  KaggleRDLoop.trace: KaggleRDLoop#trace.
  KaggleRDLoop.skip_loop_error: KaggleRDLoop#skip_loop_error.
  KaggleRDLoop: KaggleRDLoop#
---
# Module: [`rdagent/app/kaggle/loop.py`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py)

## Classes
### `KaggleRDLoop`  ·  implements/extends RDLoop
- def: [`rdagent/app/kaggle/loop.py:29`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py#L29)
- signature: `class KaggleRDLoop(RDLoop):`
- members:
  - `coding(self, prev_out: dict[str, Any])` — [`L58`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py#L58)
  - `running(self, prev_out: dict[str, Any])` — [`L71`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py#L71)
  - `feature_coder` — [`L43`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py#L43)
  - `feature_runner` — [`L49`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py#L49)
  - `hypothesis2experiment` — [`L41`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py#L41)
  - `hypothesis_gen` — [`L39`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py#L39)
  - `model_coder` — [`L47`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py#L47)
  - `model_feature_selection_coder` — [`L45`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py#L45)
  - `model_runner` — [`L51`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py#L51)
  - `skip_loop_error` — [`L111`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py#L111)
  - `summarizer` — [`L53`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py#L53)
  - `trace` — [`L55`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py#L55)
- protocol/private: `__init__`[`L30`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py#L30)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`Scenario`](../../core/scenario.md#Scenario), [`log_object`](../../log/logger.md#RDAgentLog.log_object), [`import_class`](../../core/utils.md#import_class), [`CoderError`](../../core/exception.md#CoderError), [`error`](../../log/logger.md#RDAgentLog.error), [`Developer`](../../core/developer.md#Developer), [`KAGGLE_IMPLEMENT_SETTING`](conf.md#KAGGLE_IMPLEMENT_SETTING), [`develop`](../../core/developer.md#Developer.develop), [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`Experiment2Feedback`](../../core/proposal.md#Experiment2Feedback), [`BasePropSetting`](../../components/workflow/conf.md#BasePropSetting), [`competition`](conf.md#KaggleBasePropSetting.competition), [`FactorEmptyError`](../../core/exception.md#FactorEmptyError), [`ModelEmptyError`](../../core/exception.md#ModelEmptyError), [`Hypothesis2Experiment`](../../core/proposal.md#Hypothesis2Experiment), [`HypothesisGen`](../../core/proposal.md#HypothesisGen), [`KGTrace`](../../scenarios/kaggle/proposal/proposal.md#KGTrace), [`KG_ACTION_FEATURE_ENGINEERING`](../../scenarios/kaggle/experiment/scenario.md#KG_ACTION_FEATURE_ENGINEERING), [`KG_ACTION_FEATURE_PROCESSING`](../../scenarios/kaggle/experiment/scenario.md#KG_ACTION_FEATURE_PROCESSING), [`KG_ACTION_MODEL_FEATURE_SELECTION`](../../scenarios/kaggle/experiment/scenario.md#KG_ACTION_MODEL_FEATURE_SELECTION), [`__init__`](../../utils/workflow/loop.md#LoopBase.__init__), [`hypothesis_gen`](../../components/workflow/conf.md#BasePropSetting.hypothesis_gen), [`scen`](../../components/workflow/conf.md#BasePropSetting.scen), [`summarizer`](../../components/workflow/conf.md#BasePropSetting.summarizer), [`hypothesis2experiment`](../../components/workflow/conf.md#BasePropSetting.hypothesis2experiment), [`knowledge_base`](../../components/workflow/conf.md#BasePropSetting.knowledge_base), [`python_files_to_notebook`](../../scenarios/kaggle/experiment/utils.md#python_files_to_notebook), [`auto_submit`](conf.md#KaggleBasePropSetting.auto_submit), [`knowledge_base_path`](../../components/workflow/conf.md#BasePropSetting.knowledge_base_path)
- used by: [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`main`](loop.md#main), [`coding`](../../components/workflow/rd_loop.md#RDLoop.coding), [`running`](../../components/workflow/rd_loop.md#RDLoop.running)

## Functions
- `main(path=None, step_n=None, competition=None)` — [`L114`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/loop.py#L114) — Auto R&D Evolving loop for models in a kaggle{} scenario. — documented in [rdagent-utils-workflow-loop](../../../../concepts/rdagent-utils-workflow-loop.md)


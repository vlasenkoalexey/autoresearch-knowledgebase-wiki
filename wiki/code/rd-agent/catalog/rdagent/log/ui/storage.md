---
title: 'Module: rdagent/log/ui/storage.py'
type: catalog
provenance: extracted
module: rdagent/log/ui/storage.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.log.ui.storage`/WebStorage#
symbols:
  WebStorage._obj_to_json: _obj_to_json().
  WebStorage.log: log().
  WebStorage.iter_msg: iter_msg().
  WebStorage: ''
  WebStorage.msgs: msgs.
  WebStorage.url: url.
  WebStorage.__str__: __str__().
  WebStorage.truncate: truncate().
  WebStorage.path: path.
  WebStorage.__init__: __init__().
---
# Module: [`rdagent/log/ui/storage.py`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/storage.py)

## Classes
### `WebStorage`  ·  implements/extends Storage
- def: [`rdagent/log/ui/storage.py:13`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/storage.py#L13) — documented in [rdagent-log-base](../../../../concepts/rdagent-log-base.md)
- doc: The storage for web app.
- signature: `class WebStorage(Storage):`
- members:
  - `__init__(self, port: int, path: str)` — [`L19`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/storage.py#L19) — Initializes the storage object with the specified port and identifier.
  - `iter_msg(self, **kwargs: Any)` — [`L57`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/storage.py#L57) — documented in [rdagent-log-base](../../../../concepts/rdagent-log-base.md)
  - `log(self, obj: object, tag: str, timestamp: datetime | None = None, **kwargs: Any)` — [`L33`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/storage.py#L33)
  - `truncate(self, time: datetime)` — [`L54`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/storage.py#L54)
  - `msgs` — [`L28`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/storage.py#L28)
  - `path` — [`L27`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/storage.py#L27)
  - `url` — [`L26`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/storage.py#L26)
- protocol/private: `__str__`[`L30`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/storage.py#L30), `_obj_to_json`[`L66`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/storage.py#L66)
- uses (calls/refs, reference-scoped): [`FBWorkspace`](../../core/experiment.md#FBWorkspace), [`file_dict`](../../core/experiment.md#FBWorkspace.file_dict), [`Experiment`](../../core/experiment.md#Experiment), [`DSExperiment`](../../scenarios/data_science/experiment/experiment.md#DSExperiment), [`content`](../base.md#Message.content), [`CoSTEERSingleFeedback`](../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`Hypothesis`](../../core/proposal.md#Hypothesis), [`tag`](../base.md#Message.tag), [`final_decision`](../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.final_decision), [`hypothesis`](../../core/experiment.md#Experiment.hypothesis), [`Message`](../base.md#Message), [`FactorTask`](../../components/coder/factor_coder/factor.md#FactorTask), [`result`](../../core/experiment.md#Experiment.result), [`ModelTask`](../../components/coder/model_coder/model.md#ModelTask), [`ExperimentFeedback`](../../core/proposal.md#ExperimentFeedback), [`HypothesisFeedback`](../../core/proposal.md#HypothesisFeedback), [`return_checking`](../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.return_checking), [`name`](../../core/experiment.md#AbsTask.name), [`UI_SETTING`](conf.md#UI_SETTING), [`DSHypothesis`](../../scenarios/data_science/proposal/exp_gen/base.md#DSHypothesis), [`target_task`](../../core/experiment.md#Workspace.target_task), [`hypothesis`](../../core/proposal.md#Hypothesis.hypothesis), [`code`](../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.code), [`execution`](../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.execution), [`decision`](../../core/proposal.md#ExperimentFeedback.decision), [`model_type`](../../components/coder/model_coder/model.md#ModelTask.model_type), [`Storage`](../base.md#Storage), [`report_figure`](qlib_report_figure.md#report_figure), [`description`](../../core/experiment.md#Task.description), [`extract_loopid_func_name`](../utils/__init__.md#extract_loopid_func_name), [`reason`](../../core/proposal.md#Hypothesis.reason), [`timestamp`](../base.md#Message.timestamp), [`component`](../../scenarios/data_science/proposal/exp_gen/base.md#DSHypothesis.component), [`factor_name`](../../components/coder/factor_coder/factor.md#FactorTask.factor_name), [`variables`](../../components/coder/factor_coder/factor.md#FactorTask.variables), [`pending_tasks_list`](../../scenarios/data_science/experiment/experiment.md#DSExperiment.pending_tasks_list), [`factor_description`](../../components/coder/factor_coder/factor.md#FactorTask.factor_description), [`extract_evoid`](../utils/__init__.md#extract_evoid), [`factor_formulation`](../../components/coder/factor_coder/factor.md#FactorTask.factor_formulation), [`level`](../base.md#Message.level)  (+14 more)
- used by: [`read_trace`](../server/app.md#read_trace), [`read_trace`](../server/debug_app.md#upload_file.read_trace), [`Storage`](../base.md#Storage), [`iter_msg`](../base.md#Storage.iter_msg), [`log`](../base.md#Storage.log), [`truncate`](../base.md#Storage.truncate)


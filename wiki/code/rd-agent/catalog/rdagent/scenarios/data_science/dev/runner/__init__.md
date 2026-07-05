---
title: 'Module: rdagent/scenarios/data_science/dev/runner/__init__.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/dev/runner/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.dev.runner`/DS
symbols:
  DSRunnerMultiProcessEvolvingStrategy.implement_one_task: RunnerMultiProcessEvolvingStrategy#implement_one_task().
  DSCoSTEERRunner.develop: CoSTEERRunner#develop().
  DSCoSTEERRunner.__init__: CoSTEERRunner#__init__().
  DSRunnerCoSTEERSettings: RunnerCoSTEERSettings#
  DSCoSTEERRunner.get_develop_max_seconds: CoSTEERRunner#get_develop_max_seconds().
  DSCoSTEERRunner.should_use_new_evo: CoSTEERRunner#should_use_new_evo().
  DSCoSTEERRunner: CoSTEERRunner#
  DSRunnerMultiProcessEvolvingStrategy: RunnerMultiProcessEvolvingStrategy#
  DSCoSTEERRunner.compare_scores: CoSTEERRunner#compare_scores().
  DSRunnerMultiProcessEvolvingStrategy.assign_code_list_to_evo: RunnerMultiProcessEvolvingStrategy#assign_code_list_to_evo().
  DSRunnerCoSTEERSettings.max_seconds_multiplier: RunnerCoSTEERSettings#max_seconds_multiplier.
  DSRunnerCoSTEERSettings.dump_stdout_type: RunnerCoSTEERSettings#dump_stdout_type.
  DSRunnerCoSTEERSettings.Config: RunnerCoSTEERSettings#Config#
  DSRunnerCoSTEERSettings.Config.env_prefix: RunnerCoSTEERSettings#Config#env_prefix.
  DSRunnerCoSTEERSettings.env_type: RunnerCoSTEERSettings#env_type.
  DSRunnerCoSTEERSettings.diff_mode: RunnerCoSTEERSettings#diff_mode.
---
# Module: [`rdagent/scenarios/data_science/dev/runner/__init__.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py)

## Classes
### `Config`
- def: [`rdagent/scenarios/data_science/dev/runner/__init__.py:32`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L32)
- signature: `class Config:`
- members:
  - `env_prefix` — [`L33`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L33)

### `DSCoSTEERRunner`  ·  implements/extends CoSTEER
- def: [`rdagent/scenarios/data_science/dev/runner/__init__.py:135`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L135)
- signature: `class DSCoSTEERRunner(CoSTEER):`
- members:
  - `compare_scores(s1, s2)` — [`L187`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L187)
  - `develop(self, exp)` — [`L196`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L196)
  - `get_develop_max_seconds(self)` — [`L169`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L169) — The coder uses the scenario's real debug timeout as the maximum seconds for development.
  - `should_use_new_evo(self, base_fb: CoSTEERMultiFeedback | None, new_fb: CoSTEERMultiFeedback)` — [`L175`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L175)
- protocol/private: `__init__`[`L136`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L136)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`experiment_workspace`](../../../../core/experiment.md#Experiment.experiment_workspace), [`Scenario`](../../../../core/scenario.md#Scenario), [`sub_tasks`](../../../../core/experiment.md#Experiment.sub_tasks), [`error`](../../../../log/logger.md#RDAgentLog.error), [`CoSTEERTask`](../../../../components/coder/CoSTEER/task.md#CoSTEERTask), [`result`](../../../../core/experiment.md#Experiment.result), [`CoSTEER`](../../../../components/coder/CoSTEER/__init__.md#CoSTEER), [`develop`](../../../../components/coder/CoSTEER/__init__.md#CoSTEER.develop), [`CoSTEERMultiFeedback`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEERMultiFeedback), [`md5_hash`](../../../../utils/__init__.md#md5_hash), [`CoSTEERMultiEvaluator`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEERMultiEvaluator), [`__init__`](../../../../components/coder/CoSTEER/__init__.md#CoSTEER.__init__), [`DSRunnerCoSTEERSettings`](__init__.md#DSRunnerCoSTEERSettings), [`scen`](../../../../core/developer.md#Developer.scen), [`is_acceptable`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEERMultiFeedback.is_acceptable), [`running_time`](../../../../core/experiment.md#RunningInfo.running_time), [`ModelDumpEvaluator`](../../../../components/coder/data_science/share/eval.md#ModelDumpEvaluator), [`running_info`](../../../../core/experiment.md#Experiment.running_info), [`RunnerError`](../../../../core/exception.md#RunnerError), [`settings`](../../../../components/coder/CoSTEER/__init__.md#CoSTEER.settings), [`DSRunnerEvaluator`](eval.md#DSRunnerEvaluator), [`enable_model_dump`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.enable_model_dump), [`DSRunnerMultiProcessEvolvingStrategy`](__init__.md#DSRunnerMultiProcessEvolvingStrategy), [`max_seconds_multiplier`](../../../../components/coder/CoSTEER/config.md#CoSTEERSettings.max_seconds_multiplier), [`if_using_mle_data`](../../../../app/kaggle/conf.md#KaggleBasePropSetting.if_using_mle_data), [`runner_max_loop`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.runner_max_loop)
- used by: [`CoSTEER`](../../../../components/coder/CoSTEER/__init__.md#CoSTEER), [`develop`](../../../../components/coder/CoSTEER/__init__.md#CoSTEER.develop), [`pipeline_coder`](../../loop.md#DataScienceRDLoop.pipeline_coder), [`get_develop_max_seconds`](../../../../components/coder/CoSTEER/__init__.md#CoSTEER.get_develop_max_seconds), [`should_use_new_evo`](../../../../components/coder/CoSTEER/__init__.md#CoSTEER.should_use_new_evo)

### `DSRunnerCoSTEERSettings`  ·  implements/extends CoSTEERSettings
- def: [`rdagent/scenarios/data_science/dev/runner/__init__.py:29`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L29)
- doc: Data Science CoSTEER settings
- signature: `class DSRunnerCoSTEERSettings(CoSTEERSettings):`
- members:
  - `diff_mode` — [`L37`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L37)
  - `dump_stdout_type` — [`L38`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L38)
  - `env_type` — [`L36`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L36)
  - `max_seconds_multiplier` — [`L35`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L35)
- uses (calls/refs, reference-scoped): [`CoSTEERSettings`](../../../../components/coder/CoSTEER/config.md#CoSTEERSettings)
- used by: [`evaluate`](eval.md#DSRunnerEvaluator.evaluate), [`CoSTEERSettings`](../../../../components/coder/CoSTEER/config.md#CoSTEERSettings), [`__init__`](__init__.md#DSCoSTEERRunner.__init__)  (1 test-only)

### `DSRunnerMultiProcessEvolvingStrategy`  ·  implements/extends MultiProcessEvolvingStrategy
- def: [`rdagent/scenarios/data_science/dev/runner/__init__.py:42`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L42)
- signature: `class DSRunnerMultiProcessEvolvingStrategy(MultiProcessEvolvingStrategy):`
- members:
  - `assign_code_list_to_evo(self, code_list: list[dict[str, str]], evo)` — [`L116`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L116) — Assign the code list to the evolving item.
  - `implement_one_task(self, target_task: CoSTEERTask, queried_knowledge: CoSTEERQueriedKnowledge | None = None, workspace: FBWorkspace | None = None, prev_task_feedback: CoSTEERSingleFeedback | None = None)` — [`L44`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/__init__.py#L44) — documented in [rdagent-oai-llm_utils](../../../../../../concepts/rdagent-oai-llm_utils.md)
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`APIBackend`](../../../../oai/llm_utils.md#APIBackend), [`FBWorkspace`](../../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../../core/experiment.md#FBWorkspace.file_dict), [`workspace_path`](../../../../core/experiment.md#FBWorkspace.workspace_path), [`CoSTEERSingleFeedback`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`MultiProcessEvolvingStrategy`](../../../../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`get_task_information`](../../../../core/experiment.md#Task.get_task_information), [`CoSTEERTask`](../../../../components/coder/CoSTEER/task.md#CoSTEERTask), [`build_chat_completion`](../../../../oai/backend/base.md#ChatSession.build_chat_completion), [`CoSTEERQueriedKnowledge`](../../../../components/coder/CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge), [`wait_retry`](../../../../utils/workflow/misc.md#wait_retry), [`all_codes`](../../../../core/experiment.md#FBWorkspace.all_codes), [`build_chat_session`](../../../../oai/backend/base.md#APIBackend.build_chat_session), [`PythonBatchEditOut`](../../../../utils/agent/ret.md#PythonBatchEditOut), [`get_spec`](../../../../utils/agent/ret.md#PythonBatchEditOut.get_spec), [`get_spec`](../../../../utils/agent/ret.md#PythonBatchPatchOut.get_spec), [`PythonBatchPatchOut`](../../../../utils/agent/ret.md#PythonBatchPatchOut), [`KEY_CHANGE_SUMMARY`](../../../../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.KEY_CHANGE_SUMMARY), [`settings`](../../../../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.settings), [`extract_output`](../../../../utils/agent/ret.md#PythonBatchPatchOut.extract_output), [`change_summary`](../../../../core/experiment.md#FBWorkspace.change_summary), [`extract_output`](../../../../utils/agent/ret.md#PythonBatchEditOut.extract_output), [`runner_enable_code_change_summary`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.runner_enable_code_change_summary)
- used by: [`MultiProcessEvolvingStrategy`](../../../../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`implement_one_task`](../../../../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.implement_one_task), [`assign_code_list_to_evo`](../../../../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.assign_code_list_to_evo), [`__init__`](__init__.md#DSCoSTEERRunner.__init__)


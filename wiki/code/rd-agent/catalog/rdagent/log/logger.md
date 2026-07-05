---
title: 'Module: rdagent/log/logger.py'
type: catalog
provenance: extracted
module: rdagent/log/logger.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.log.logger`/RDAgentLog#
symbols:
  RDAgentLog.info: info().
  RDAgentLog.warning: warning().
  RDAgentLog.log_object: log_object().
  RDAgentLog.error: error().
  RDAgentLog._log: _log().
  RDAgentLog.refresh_storages_from_settings: refresh_storages_from_settings().
  RDAgentLog: ''
  RDAgentLog.storage: storage.
  RDAgentLog.tag: tag().
  RDAgentLog.set_storages_path: set_storages_path().
  RDAgentLog.other_storages: other_storages.
  RDAgentLog._configure_console_sinks: _configure_console_sinks().
  RDAgentLog._tag: _tag().
  RDAgentLog.truncate_storages: truncate_storages().
  RDAgentLog._tag_ctx: _tag_ctx.
  RDAgentLog.get_pids: get_pids().
  RDAgentLog.rebind_console_to_current_streams: rebind_console_to_current_streams().
  RDAgentLog.__init__: __init__().
  RDAgentLog._raw_log_key: _raw_log_key.
  RDAgentLog.main_pid: main_pid.
---
# Module: [`rdagent/log/logger.py`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py)

## Classes
### `RDAgentLog`  ·  implements/extends SingletonBaseClass
- def: [`rdagent/log/logger.py:20`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L20) — documented in [rdagent-app-CI-run](../../../concepts/rdagent-app-CI-run.md)
- doc: The files are organized based on the tag & PID
- signature: `class RDAgentLog(SingletonBaseClass):`
- members:
  - `error(self, msg: str, *, tag: str = "", raw: bool = False)` — [`L152`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L152) — documented in [rdagent-log-logger](../../../concepts/rdagent-log-logger.md)
  - `get_pids(self)` — [`L117`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L117) — Returns a string of pids from the current process to the main process.
  - `info(self, msg: str, *, tag: str = "", raw: bool = False)` — [`L146`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L146) — documented in [rdagent-log-logger](../../../concepts/rdagent-log-logger.md)
  - `log_object(self, obj: object, *, tag: str = "")` — [`L132`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L132) — documented in [rdagent-app-CI-run](../../../concepts/rdagent-app-CI-run.md)
  - `rebind_console_to_current_streams(self)` — [`L82`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L82) — Rebind loguru sinks to the current stdio objects.
  - `refresh_storages_from_settings(self)` — [`L76`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L76) — documented in [rdagent-app-CI-run](../../../concepts/rdagent-app-CI-run.md)
  - `set_storages_path(self, path: str | Path)` — [`L106`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L106)
  - `tag(self, tag: str)` — [`L92`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L92) — documented in [rdagent-app-CI-run](../../../concepts/rdagent-app-CI-run.md)
  - `truncate_storages(self, time: datetime)` — [`L113`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L113)
  - `warning(self, msg: str, *, tag: str = "", raw: bool = False)` — [`L149`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L149) — documented in [rdagent-log-logger](../../../concepts/rdagent-log-logger.md)
  - `main_pid` — [`L74`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L74)
  - `other_storages` — [`L71`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L71) — documented in [rdagent-app-CI-run](../../../concepts/rdagent-app-CI-run.md)
  - `storage` — [`L70`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L70) — documented in [rdagent-app-CI-run](../../../concepts/rdagent-app-CI-run.md)
- protocol/private: `__init__`[`L66`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L66), `_configure_console_sinks`[`L48`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L48), `_log`[`L138`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L138), `_raw_log_key`[`L45`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L45), `_tag`[`L59`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L59), `_tag_ctx`[`L44`](../../../../../../raw/code/rd-agent/rdagent/log/logger.py#L44)
- uses (calls/refs, reference-scoped): [`import_class`](../core/utils.md#import_class), [`SingletonBaseClass`](../core/utils.md#SingletonBaseClass), [`FileStorage`](storage.md#FileStorage), [`Storage`](base.md#Storage), [`LOG_SETTINGS`](conf.md#LOG_SETTINGS), [`path`](storage.md#FileStorage.path), [`log`](base.md#Storage.log), [`truncate`](base.md#Storage.truncate), [`get_caller_info`](utils/__init__.md#get_caller_info), [`trace_path`](conf.md#LogSettings.trace_path), [`storages`](conf.md#LogSettings.storages), [`format_console`](conf.md#LogSettings.format_console)
- used by: [`rdagent_logger`](__init__.md#rdagent_logger.rdagent_logger), [`r`](../utils/agent/tpl.md#RDAT.r), [`evaluate`](../scenarios/data_science/dev/runner/eval.md#DSRunnerEvaluator.evaluate), [`evaluate`](../components/coder/data_science/pipeline/eval.md#PipelineCoSTEEREvaluator.evaluate), [`record`](../scenarios/data_science/loop.md#DataScienceRDLoop.record), [`async_gen`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.async_gen), [`gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.gen), [`build_messages_and_create_chat_completion`](../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`evaluate`](../scenarios/finetune/train/eval.md#FTRunnerEvaluator.evaluate), [`develop`](../scenarios/qlib/developer/factor_runner.md#QlibFactorRunner.develop), [`develop`](../scenarios/qlib/developer/model_runner.md#QlibModelRunner.develop), [`hypothesis_gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_gen), [`evolve_agent`](../components/coder/CoSTEER/__init__.md#CoSTEER.evolve_agent), [`evaluate`](../components/coder/finetune/eval.md#FTCoderEvaluator.evaluate), [`evaluate`](../components/coder/data_science/workflow/eval.md#WorkflowGeneralCaseSpecEvaluator.evaluate), [`_gen_hypothesis`](../scenarios/finetune/proposal/proposal.md#LLMFinetuneExpGen._gen_hypothesis), [`_create_chat_completion_inner_function`](../oai/backend/deprec.md#DeprecBackend._create_chat_completion_inner_function), [`implement_data`](../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy.implement_data), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV2.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2Hypothesis.gen), [`task_gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.task_gen), [`_run_step`](../utils/workflow/loop.md#LoopBase._run_step), [`generate_feedback`](../scenarios/kaggle/developer/feedback.md#KGExperiment2Feedback.generate_feedback), [`multistep_evolve`](../core/evolving_agent.md#RAGEvoAgent.multistep_evolve), [`_create_chat_completion_auto_continue`](../oai/backend/base.md#APIBackend._create_chat_completion_auto_continue), [`run`](../utils/env.md#Env.run), [`run`](../scenarios/rl/autorl_bench/run.md#run), [`direct_exp_gen`](../app/qlib_rd_loop/factor_from_report.md#FactorReportLoop.direct_exp_gen), [`evaluate`](../components/coder/finetune/eval.md#FTDataEvaluator.evaluate), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV3.gen), [`_generate_llamafactory_config_with_llm`](../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy._generate_llamafactory_config_with_llm), [`_generate_llm_feedback`](../components/coder/finetune/eval.md#FTDataEvaluator._generate_llm_feedback), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMerge.gen), [`run`](../utils/workflow/loop.md#LoopBase.run), [`_run`](server/app.md#RDAgentTask._run), [`_generate_llm_feedback`](../scenarios/finetune/train/eval.md#FTRunnerEvaluator._generate_llm_feedback), [`generate_feedback`](../scenarios/qlib/developer/feedback.md#QlibFactorExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/qlib/developer/feedback.md#QlibModelExperiment2Feedback.generate_feedback), [`_try_create_chat_completion_or_embedding`](../oai/backend/base.md#APIBackend._try_create_chat_completion_or_embedding), [`_run_micro_batch_test`](../components/coder/finetune/unified_validator.md#LLMConfigValidator._run_micro_batch_test)  (+208 more; 13 test-only)


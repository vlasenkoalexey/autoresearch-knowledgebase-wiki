---
title: 'Module: rdagent/utils/agent/tpl.py'
type: catalog
provenance: extracted
module: rdagent/utils/agent/tpl.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.utils.agent.tpl`/
symbols:
  T: T.
  RDAT.r: RDAT#r().
  load_content: load_content().
  RDAT.uri: RDAT#uri.
  PROJ_PATH: PROJ_PATH.
  RDAT.template: RDAT#template.
  get_caller_dir: get_caller_dir().
  DIRNAME: DIRNAME.
  RDAT: RDAT#
  RDAT.__init__: RDAT#__init__().
---
# Module: [`rdagent/utils/agent/tpl.py`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/tpl.py)

## Classes
### `RDAT`
- def: [`rdagent/utils/agent/tpl.py:85`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/tpl.py#L85)
- doc: RD-Agent's Template
- signature: `class RDAT:`
- members:
  - `__init__(self, uri: str, ftype: str = "yaml")` — [`L91`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/tpl.py#L91) — here are some uri usages
  - `r(self, **context: Any)` — [`L122`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/tpl.py#L122) — Render the template with the given context. — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
  - `template` — [`L120`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/tpl.py#L120)
  - `uri` — [`L112`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/tpl.py#L112) — documented in [rdagent-utils-agent-tpl](../../../../concepts/rdagent-utils-agent-tpl.md)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`log_object`](../../log/logger.md#RDAgentLog.log_object), [`load_content`](tpl.md#load_content), [`PROJ_PATH`](tpl.md#PROJ_PATH), [`get_caller_dir`](tpl.md#get_caller_dir)
- used by: [`T`](tpl.md#T), [`evaluate`](../../scenarios/data_science/dev/runner/eval.md#DSRunnerEvaluator.evaluate), [`evaluate`](../../components/coder/data_science/pipeline/eval.md#PipelineCoSTEEREvaluator.evaluate), [`gen`](../../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.gen), [`hypothesis_gen`](../../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_gen), [`evaluate`](../../components/coder/finetune/eval.md#FTCoderEvaluator.evaluate), [`evaluate`](../../components/coder/data_science/workflow/eval.md#WorkflowGeneralCaseSpecEvaluator.evaluate), [`_gen_hypothesis`](../../scenarios/finetune/proposal/proposal.md#LLMFinetuneExpGen._gen_hypothesis), [`implement_data`](../../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy.implement_data), [`hypothesis_select_with_llm`](../../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_select_with_llm), [`gen`](../../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2Hypothesis.gen), [`task_gen`](../../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.task_gen), [`evaluate`](../../components/coder/data_science/model/eval.md#ModelGeneralCaseSpecEvaluator.evaluate), [`evaluate`](../../components/coder/data_science/raw_data_loader/eval.md#DataLoaderCoSTEEREvaluator.evaluate), [`gen`](../../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV1ExpGen.gen), [`generate_feedback`](../../scenarios/data_science/dev/feedback.md#DSExperiment2Feedback.generate_feedback), [`generate_feedback`](../../scenarios/finetune/dev/feedback.md#FTExperiment2Feedback.generate_feedback), [`generate_feedback`](../../scenarios/kaggle/developer/feedback.md#KGExperiment2Feedback.generate_feedback), [`gen`](../../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftExpGen.gen), [`evaluate`](../../components/coder/data_science/share/eval.md#ModelDumpEvaluator.evaluate), [`evaluate`](../../components/coder/data_science/ensemble/eval.md#EnsembleCoSTEEREvaluator.evaluate), [`evaluate`](../../components/coder/data_science/feature/eval.md#FeatureCoSTEEREvaluator.evaluate), [`implement_one_task`](../../scenarios/data_science/dev/runner/__init__.md#DSRunnerMultiProcessEvolvingStrategy.implement_one_task), [`_generate_and_run_script`](../../scenarios/data_science/proposal/exp_gen/select/submit.md#ValidationSelector._generate_and_run_script), [`implement_one_task`](../../components/coder/data_science/pipeline/__init__.md#PipelineMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../../components/coder/data_science/raw_data_loader/__init__.md#DataLoaderMultiProcessEvolvingStrategy.implement_one_task), [`_generate_llamafactory_config_with_llm`](../../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy._generate_llamafactory_config_with_llm), [`_generate_llm_feedback`](../../components/coder/finetune/eval.md#FTDataEvaluator._generate_llm_feedback), [`implement_one_task`](../../components/coder/data_science/model/__init__.md#ModelMultiProcessEvolvingStrategy.implement_one_task), [`_generate_llm_feedback`](../../scenarios/finetune/train/eval.md#FTRunnerEvaluator._generate_llm_feedback), [`generate_feedback`](../../scenarios/qlib/developer/feedback.md#QlibFactorExperiment2Feedback.generate_feedback), [`generate_feedback`](../../scenarios/qlib/developer/feedback.md#QlibModelExperiment2Feedback.generate_feedback), [`get_scenario_all_desc`](../../scenarios/data_science/scen/__init__.md#DataScienceScen.get_scenario_all_desc), [`implement_one_task`](../../components/coder/data_science/ensemble/__init__.md#EnsembleMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../../components/coder/factor_coder/evolving_strategy.md#FactorMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../../components/coder/data_science/feature/__init__.md#FeatureMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../../components/coder/data_science/workflow/__init__.md#WorkflowMultiProcessEvolvingStrategy.implement_one_task), [`_prepare_validation_scripts`](../../scenarios/data_science/proposal/exp_gen/select/submit.md#ValidationSelector._prepare_validation_scripts), [`process_experiment`](../../scenarios/data_science/proposal/exp_gen/select/submit.md#process_experiment), [`gen`](../../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftV2ExpGen.gen)  (+115 more; 6 test-only)

## Functions
- `get_caller_dir(upshift: int = 0)` — [`L21`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/tpl.py#L21)
- `load_content(uri: str, caller_dir: Path | None = None, ftype: str = "yaml")` — [`L33`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/tpl.py#L33) — Please refer to RDAT.__init__ file — documented in [rdagent-utils-agent-tpl](../../../../concepts/rdagent-utils-agent-tpl.md)

## Module values
- `DIRNAME` — [`L17`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/tpl.py#L17)
- `PROJ_PATH` — [`L18`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/tpl.py#L18)
- `T` — [`L148`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/tpl.py#L148) — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)


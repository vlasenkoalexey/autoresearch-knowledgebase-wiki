---
title: 'Module: rdagent/app/kaggle/conf.py'
type: catalog
provenance: extracted
module: rdagent/app/kaggle/conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.kaggle.conf`/K
symbols:
  KAGGLE_IMPLEMENT_SETTING: AGGLE_IMPLEMENT_SETTING.
  KaggleBasePropSetting.local_data_path: aggleBasePropSetting#local_data_path.
  KaggleBasePropSetting.competition: aggleBasePropSetting#competition.
  KaggleBasePropSetting: aggleBasePropSetting#
  KaggleBasePropSetting.if_using_mle_data: aggleBasePropSetting#if_using_mle_data.
  KaggleBasePropSetting.domain_knowledge_path: aggleBasePropSetting#domain_knowledge_path.
  KaggleBasePropSetting.rag_path: aggleBasePropSetting#rag_path.
  KaggleBasePropSetting.if_using_graph_rag: aggleBasePropSetting#if_using_graph_rag.
  KaggleBasePropSetting.template_path: aggleBasePropSetting#template_path.
  KaggleBasePropSetting.auto_submit: aggleBasePropSetting#auto_submit.
  KaggleBasePropSetting.knowledge_base: aggleBasePropSetting#knowledge_base.
  KaggleBasePropSetting.if_action_choosing_based_on_UCB: aggleBasePropSetting#if_action_choosing_based_on_UCB.
  KaggleBasePropSetting.if_using_vector_rag: aggleBasePropSetting#if_using_vector_rag.
  KaggleBasePropSetting.mini_case: aggleBasePropSetting#mini_case.
  KaggleBasePropSetting.time_ratio_limit_to_enable_hyperparameter_tuning: aggleBasePropSetting#time_ratio_limit_to_enable_hyperparameter_tuning.
  KaggleBasePropSetting.res_time_ratio_limit_to_enable_hyperparameter_tuning: aggleBasePropSetting#res_time_ratio_limit_to_enable_hyperparameter_tuning.
  KaggleBasePropSetting.only_first_loop_enable_hyperparameter_tuning: aggleBasePropSetting#only_first_loop_enable_hyperparameter_tuning.
  KaggleBasePropSetting.only_enable_tuning_in_merge: aggleBasePropSetting#only_enable_tuning_in_merge.
  KaggleBasePropSetting.model_config: aggleBasePropSetting#model_config.
  KaggleBasePropSetting.scen: aggleBasePropSetting#scen.
  KaggleBasePropSetting.hypothesis_gen: aggleBasePropSetting#hypothesis_gen.
  KaggleBasePropSetting.hypothesis2experiment: aggleBasePropSetting#hypothesis2experiment.
  KaggleBasePropSetting.feature_coder: aggleBasePropSetting#feature_coder.
  KaggleBasePropSetting.model_feature_selection_coder: aggleBasePropSetting#model_feature_selection_coder.
  KaggleBasePropSetting.model_coder: aggleBasePropSetting#model_coder.
  KaggleBasePropSetting.feature_runner: aggleBasePropSetting#feature_runner.
  KaggleBasePropSetting.model_runner: aggleBasePropSetting#model_runner.
  KaggleBasePropSetting.summarizer: aggleBasePropSetting#summarizer.
  KaggleBasePropSetting.evolving_n: aggleBasePropSetting#evolving_n.
  KaggleBasePropSetting.knowledge_base_path: aggleBasePropSetting#knowledge_base_path.
---
# Module: [`rdagent/app/kaggle/conf.py`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py)

## Classes
### `KaggleBasePropSetting`  ·  implements/extends ExtendedBaseSettings
- def: [`rdagent/app/kaggle/conf.py:6`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L6)
- signature: `class KaggleBasePropSetting(ExtendedBaseSettings):`
- members:
  - `auto_submit` — [`L51`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L51) — ---
  - `competition` — [`L40`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L40) — --- — documented in [rdagent-components-coder-factor_coder-factor](../../../../concepts/rdagent-components-coder-factor_coder-factor.md)
  - `domain_knowledge_path` — [`L60`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L60) — ---
  - `evolving_n` — [`L37`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L37) — ---
  - `feature_coder` — [`L19`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L19) — ---
  - `feature_runner` — [`L28`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L28) — ---
  - `hypothesis2experiment` — [`L16`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L16) — ---
  - `hypothesis_gen` — [`L13`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L13) — ---
  - `if_action_choosing_based_on_UCB` — [`L57`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L57) — ---
  - `if_using_graph_rag` — [`L72`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L72) — ---
  - `if_using_mle_data` — [`L50`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L50)
  - `if_using_vector_rag` — [`L69`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L69) — ---
  - `knowledge_base` — [`L55`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L55) — ---
  - `knowledge_base_path` — [`L63`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L63) — ---
  - `local_data_path` — [`L46`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L46) — --- — documented in [rdagent-components-coder-factor_coder-factor](../../../../concepts/rdagent-components-coder-factor_coder-factor.md)
  - `mini_case` — [`L75`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L75) — ---
  - `model_coder` — [`L25`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L25) — ---
  - `model_config` — [`L7`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L7)
  - `model_feature_selection_coder` — [`L22`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L22) — ---
  - `model_runner` — [`L31`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L31) — ---
  - `only_enable_tuning_in_merge` — [`L92`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L92) — ---
  - `only_first_loop_enable_hyperparameter_tuning` — [`L89`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L89) — ---
  - `rag_path` — [`L66`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L66) — ---
  - `res_time_ratio_limit_to_enable_hyperparameter_tuning` — [`L83`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L83) — ---
  - `scen` — [`L10`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L10) — ---
  - `summarizer` — [`L34`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L34) — ---
  - `template_path` — [`L43`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L43) — ---
  - `time_ratio_limit_to_enable_hyperparameter_tuning` — [`L78`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L78) — ---
- uses (calls/refs, reference-scoped): [`ExtendedBaseSettings`](../../core/conf.md#ExtendedBaseSettings), [`DataScienceBasePropSetting`](../data_science/conf.md#DataScienceBasePropSetting)
- used by: [`evaluate`](../../scenarios/data_science/dev/runner/eval.md#DSRunnerEvaluator.evaluate), [`ExtendedBaseSettings`](../../core/conf.md#ExtendedBaseSettings), [`evaluate`](../../components/coder/data_science/share/eval.md#ModelDumpEvaluator.evaluate), [`execute`](../../components/coder/factor_coder/factor.md#FactorFBWorkspace.execute), [`_generate_and_run_script`](../../scenarios/data_science/proposal/exp_gen/select/submit.md#ValidationSelector._generate_and_run_script), [`evaluate_one_trace`](../../scenarios/data_science/proposal/exp_gen/select/submit.md#evaluate_one_trace), [`_prepare_validation_scripts`](../../scenarios/data_science/proposal/exp_gen/select/submit.md#ValidationSelector._prepare_validation_scripts), [`KAGGLE_IMPLEMENT_SETTING`](conf.md#KAGGLE_IMPLEMENT_SETTING), [`develop`](../../scenarios/data_science/dev/runner/__init__.md#DSCoSTEERRunner.develop), [`dump_and_wait_for_user_input`](../../scenarios/data_science/interactor/__init__.md#FBDSInteractor.dump_and_wait_for_user_input), [`main`](../data_science/loop.md#main), [`running`](loop.md#KaggleRDLoop.running), [`execute`](../../scenarios/kaggle/experiment/workspace.md#KGFBWorkspace.execute), [`background`](../../scenarios/kaggle/experiment/scenario.md#KGScenario.background), [`load`](../../scenarios/data_science/loop.md#DataScienceRDLoop.load), [`generate_preprocess_data`](../../scenarios/kaggle/experiment/workspace.md#KGFBWorkspace.generate_preprocess_data), [`main`](loop.md#main), [`__init__`](../../scenarios/kaggle/experiment/kaggle_experiment.md#KGFactorExperiment.__init__), [`__init__`](../../scenarios/kaggle/experiment/kaggle_experiment.md#KGModelExperiment.__init__), [`develop`](../../components/coder/data_science/raw_data_loader/__init__.md#DataLoaderCoSTEER.develop), [`if_using_vector_rag`](../../scenarios/kaggle/experiment/scenario.md#KGScenario.if_using_vector_rag), [`run`](../utils/ws.md#run), [`_get_description`](../../scenarios/data_science/scen/__init__.md#DataScienceScen._get_description), [`source_data`](../../scenarios/kaggle/experiment/scenario.md#KGScenario.source_data), [`__init__`](../../scenarios/data_science/scen/__init__.md#DataScienceScen.__init__), [`_get_data_folder_description`](../../scenarios/data_science/scen/__init__.md#DataScienceScen._get_data_folder_description), [`update_settings`](../finetune/data_science/conf.md#update_settings), [`main`](../finetune/data_science/loop.md#main), [`_get_data_folder_description`](../finetune/data_science/scen.md#DSFinetuneScen._get_data_folder_description), [`_get_description`](../../scenarios/data_science/scen/__init__.md#KaggleScen._get_description), [`path`](../../scenarios/kaggle/knowledge_management/graph.md#KGKnowledgeGraph.path), [`competition_descriptions`](../../scenarios/kaggle/experiment/scenario.md#KGScenario.competition_descriptions), [`mini_case`](../../scenarios/kaggle/experiment/scenario.md#KGScenario.mini_case), [`if_using_graph_rag`](../../scenarios/kaggle/experiment/scenario.md#KGScenario.if_using_graph_rag), [`if_action_choosing_based_on_UCB`](../../scenarios/kaggle/experiment/scenario.md#KGScenario.if_action_choosing_based_on_UCB), [`DataScienceBasePropSetting`](../data_science/conf.md#DataScienceBasePropSetting)  (7 test-only)

## Module values
- `KAGGLE_IMPLEMENT_SETTING` — [`L96`](../../../../../../../raw/code/rd-agent/rdagent/app/kaggle/conf.py#L96) — documented in [rdagent-components-coder-factor_coder-factor](../../../../concepts/rdagent-components-coder-factor_coder-factor.md)


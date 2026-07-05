---
title: 'Module: rdagent/scenarios/kaggle/experiment/scenario.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/scenario.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.scenario`/KG
symbols:
  KGScenario._analysis_competition_description: Scenario#_analysis_competition_description().
  KGScenario.background: Scenario#background().
  KGScenario.if_using_vector_rag: Scenario#if_using_vector_rag.
  KGScenario.get_competition_full_desc: Scenario#get_competition_full_desc().
  KGScenario.source_data: Scenario#source_data().
  KG_ACTION_LIST: _ACTION_LIST.
  KGScenario.simulator: Scenario#simulator().
  KGScenario: Scenario#
  KGScenario.get_scenario_all_desc: Scenario#get_scenario_all_desc().
  KGScenario.interface: Scenario#interface().
  KGScenario.common_description: Scenario#common_description().
  KGScenario.competition_descriptions: Scenario#competition_descriptions.
  KGScenario.mini_case: Scenario#mini_case.
  KGScenario.output_format: Scenario#output_format().
  KG_ACTION_FEATURE_PROCESSING: _ACTION_FEATURE_PROCESSING.
  KG_ACTION_FEATURE_ENGINEERING: _ACTION_FEATURE_ENGINEERING.
  KGScenario.reward_estimates: Scenario#reward_estimates.
  KGScenario.if_using_graph_rag: Scenario#if_using_graph_rag.
  KGScenario.evaluation_metric_direction: Scenario#evaluation_metric_direction.
  KGScenario.output: Scenario#output().
  KG_ACTION_MODEL_FEATURE_SELECTION: _ACTION_MODEL_FEATURE_SELECTION.
  KGScenario.submission_specifications: Scenario#submission_specifications.
  KGScenario.vector_base: Scenario#vector_base.
  KGScenario.if_action_choosing_based_on_UCB: Scenario#if_action_choosing_based_on_UCB.
  KGScenario.leaderboard: Scenario#leaderboard.
  KGScenario.competition: Scenario#competition.
  KG_ACTION_MODEL_TUNING: _ACTION_MODEL_TUNING.
  KGScenario.competition_type: Scenario#competition_type.
  KGScenario.competition_description: Scenario#competition_description.
  KGScenario.target_description: Scenario#target_description.
  KGScenario.competition_features: Scenario#competition_features.
  KGScenario.model_output_channel: Scenario#model_output_channel.
  KGScenario.evaluation_desc: Scenario#evaluation_desc.
  KGScenario.action_counts: Scenario#action_counts.
  KGScenario.rich_style_description: Scenario#rich_style_description().
  KGScenario.input_shape: Scenario#input_shape.
  KGScenario.__init__: Scenario#__init__().
  KGScenario.confidence_parameter: Scenario#confidence_parameter.
  KGScenario.initial_performance: Scenario#initial_performance.
---
# Module: [`rdagent/scenarios/kaggle/experiment/scenario.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py)

## Classes
### `KGScenario`  ·  implements/extends Scenario
- def: [`rdagent/scenarios/kaggle/experiment/scenario.py:36`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L36)
- signature: `class KGScenario(Scenario):`
- members:
  - `background(self)` — [`L114`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L114)
  - `common_description()` — [`L245`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L245)
  - `get_competition_full_desc(self)` — [`L101`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L101)
  - `get_scenario_all_desc(self, task: Task | None = None, filtered_tag: str | None = None, simple_background: bool | None = None)` — [`L242`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L242)
  - `interface(self, tag=None)` — [`L182`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L182)
  - `output(tag: str | None)` — [`L262`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L262)
  - `output_format(self, tag=None)` — [`L167`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L167)
  - `rich_style_description(self)` — [`L215`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L215)
  - `simulator(self, tag=None)` — [`L197`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L197)
  - `source_data(self)` — [`L134`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L134)
  - `action_counts` — [`L64`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L64)
  - `competition` — [`L39`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L39)
  - `competition_description` — [`L44`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L44)
  - `competition_descriptions` — [`L40`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L40)
  - `competition_features` — [`L46`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L46)
  - `competition_type` — [`L43`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L43)
  - `confidence_parameter` — [`L70`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L70)
  - `evaluation_desc` — [`L49`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L49)
  - `evaluation_metric_direction` — [`L51`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L51)
  - `if_action_choosing_based_on_UCB` — [`L55`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L55)
  - `if_using_graph_rag` — [`L56`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L56)
  - `if_using_vector_rag` — [`L57`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L57)
  - `initial_performance` — [`L71`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L71)
  - `input_shape` — [`L41`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L41)
  - `leaderboard` — [`L50`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L50)
  - `mini_case` — [`L53`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L53)
  - `model_output_channel` — [`L48`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L48)
  - `reward_estimates` — [`L65`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L65)
  - `submission_specifications` — [`L47`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L47)
  - `target_description` — [`L45`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L45)
  - `vector_base` — [`L52`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L52)
- protocol/private: `__init__`[`L37`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L37), `_analysis_competition_description`[`L73`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L73)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`Scenario`](../../../core/scenario.md#Scenario), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`Task`](../../../core/experiment.md#Task), [`KAGGLE_IMPLEMENT_SETTING`](../../../app/kaggle/conf.md#KAGGLE_IMPLEMENT_SETTING), [`local_data_path`](../../../app/kaggle/conf.md#KaggleBasePropSetting.local_data_path), [`generate_preprocess_data`](workspace.md#KGFBWorkspace.generate_preprocess_data), [`KGFactorExperiment`](kaggle_experiment.md#KGFactorExperiment), [`competition`](../../../app/kaggle/conf.md#KaggleBasePropSetting.competition), [`KG_ACTION_LIST`](scenario.md#KG_ACTION_LIST), [`crawl_descriptions`](../kaggle_crawler.md#crawl_descriptions), [`dump`](../../../core/knowledge_base.md#KnowledgeBase.dump), [`leaderboard_scores`](../kaggle_crawler.md#leaderboard_scores), [`path`](../../../core/knowledge_base.md#KnowledgeBase.path), [`KaggleExperienceBase`](../knowledge_management/vector_base.md#KaggleExperienceBase), [`if_using_graph_rag`](../../../app/kaggle/conf.md#KaggleBasePropSetting.if_using_graph_rag), [`rag_path`](../../../app/kaggle/conf.md#KaggleBasePropSetting.rag_path), [`if_action_choosing_based_on_UCB`](../../../app/kaggle/conf.md#KaggleBasePropSetting.if_action_choosing_based_on_UCB), [`if_using_vector_rag`](../../../app/kaggle/conf.md#KaggleBasePropSetting.if_using_vector_rag), [`mini_case`](../../../app/kaggle/conf.md#KaggleBasePropSetting.mini_case)
- used by: [`Scenario`](../../../core/scenario.md#Scenario), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`feedback_window`](../../../log/ui/app.md#feedback_window), [`generate_RAG_content`](../proposal/proposal.md#generate_RAG_content), [`load_from_documents`](../knowledge_management/graph.md#KGKnowledgeGraph.load_from_documents), [`SIMILAR_SCENARIOS`](../../../log/ui/app.md#SIMILAR_SCENARIOS), [`analyze_one_document`](../knowledge_management/graph.md#KGKnowledgeGraph.analyze_one_document), [`background`](../../../core/scenario.md#Scenario.background), [`rich_style_description`](../../../core/scenario.md#Scenario.rich_style_description), [`source_data`](../../../core/scenario.md#Scenario.source_data), [`KGTrace`](../proposal/proposal.md#KGTrace), [`__init__`](../knowledge_management/graph.md#KGKnowledgeGraph.__init__), [`add_document`](../knowledge_management/graph.md#KGKnowledgeGraph.add_document)

## Module values
- `KG_ACTION_FEATURE_ENGINEERING` — [`L25`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L25)
- `KG_ACTION_FEATURE_PROCESSING` — [`L24`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L24)
- `KG_ACTION_LIST` — [`L28`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L28)
- `KG_ACTION_MODEL_FEATURE_SELECTION` — [`L26`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L26)
- `KG_ACTION_MODEL_TUNING` — [`L27`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/scenario.py#L27)


---
title: 'Module: rdagent/scenarios/data_science/proposal/exp_gen/proposal.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/proposal/exp_gen/proposal.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.proposal.exp_gen.proposal`/
symbols:
  DSProposalV2ExpGen.gen: DSProposalV2ExpGen#gen().
  DSProposalV2ExpGen.hypothesis_gen: DSProposalV2ExpGen#hypothesis_gen().
  DSProposalV2ExpGen.hypothesis_select_with_llm: DSProposalV2ExpGen#hypothesis_select_with_llm().
  DSProposalV2ExpGen.task_gen: DSProposalV2ExpGen#task_gen().
  DSProposalV1ExpGen.gen: DSProposalV1ExpGen#gen().
  DSProposalV2ExpGen.hypothesis_rewrite: DSProposalV2ExpGen#hypothesis_rewrite().
  DSProposalV2ExpGen.identify_scenario_problem: DSProposalV2ExpGen#identify_scenario_problem().
  DSProposalV2ExpGen.identify_feedback_problem: DSProposalV2ExpGen#identify_feedback_problem().
  DSProposalV2ExpGen.supports_response_schema: DSProposalV2ExpGen#supports_response_schema.
  DSProposalV2ExpGen.hypothesis_critique: DSProposalV2ExpGen#hypothesis_critique().
  DSProposalV2ExpGen._prob_dis_torch: DSProposalV2ExpGen#_prob_dis_torch().
  _COMPONENT_META._COMPONENT_META: _COMPONENT_META._COMPONENT_META.
  draft_exp_in_decomposition: draft_exp_in_decomposition().
  DSProposalV2ExpGen.scen_prob_multiplier: DSProposalV2ExpGen#scen_prob_multiplier.
  DSProposalV1ExpGen._f: DSProposalV1ExpGen#_f().
  DSProposalV2ExpGen.select_hypothesis: DSProposalV2ExpGen#select_hypothesis().
  DSProposalV2ExpGen._llm_select_extra_hypo: DSProposalV2ExpGen#_llm_select_extra_hypo().
  get_component: get_component().
  DSProposalV2ExpGen: DSProposalV2ExpGen#
  DSProposalV2ExpGen.hypothesis_rank: DSProposalV2ExpGen#hypothesis_rank().
  HypothesisDetail.evaluation: HypothesisDetail#evaluation.
  DSProposalV2ExpGen._get_current_exp_score_list: DSProposalV2ExpGen#_get_current_exp_score_list().
  HypothesisEvaluationReasoningScore: HypothesisEvaluationReasoningScore#
  HypothesisEvaluationReasoningScore.score: HypothesisEvaluationReasoningScore#score.
  DSProposalV2ExpGen._get_path: DSProposalV2ExpGen#_get_path().
  DSProposalV2ExpGen.get_all_hypotheses: DSProposalV2ExpGen#get_all_hypotheses().
  ScenarioChallenges: ScenarioChallenges#
  TraceChallenges: TraceChallenges#
  HypothesisComponent: HypothesisComponent#
  HypothesisList: HypothesisList#
  ScenarioChallenges.challenges: ScenarioChallenges#challenges.
  TraceChallenges.challenges: TraceChallenges#challenges.
  HypothesisEvaluation.alignment: HypothesisEvaluation#alignment.
  HypothesisEvaluation.impact: HypothesisEvaluation#impact.
  HypothesisEvaluation.novelty: HypothesisEvaluation#novelty.
  HypothesisEvaluation.feasibility: HypothesisEvaluation#feasibility.
  HypothesisEvaluation.risk_reward_balance: HypothesisEvaluation#risk_reward_balance.
  HypothesisDetail.component: HypothesisDetail#component.
  HypothesisList.hypotheses: HypothesisList#hypotheses.
  DSProposalV2ExpGen.identify_problem: DSProposalV2ExpGen#identify_problem().
  TraceAnalysisDetail: TraceAnalysisDetail#
  CodingSketch: CodingSketch#
  ScenarioChallengeDetail.category: ScenarioChallengeDetail#category.
  ScenarioChallenges.analysis: ScenarioChallenges#analysis.
  TraceAnalysis.feedback: TraceAnalysis#feedback.
  TraceAnalysis.implementation_review: TraceAnalysis#implementation_review.
  TraceAnalysis.trace_history: TraceAnalysis#trace_history.
  TraceChallenges.analysis: TraceChallenges#analysis.
  HypothesisSimple.component: HypothesisSimple#component.
  DSProposalV1ExpGen: DSProposalV1ExpGen#
  DSProposalV2ExpGen.__init__: DSProposalV2ExpGen#__init__().
  ScenarioChallengeCategory: ScenarioChallengeCategory#
  ScenarioChallengeDetail: ScenarioChallengeDetail#
  ScenarioChallengeDetail.reasoning: ScenarioChallengeDetail#reasoning.
  ScenarioChallengeDetail.statement: ScenarioChallengeDetail#statement.
  ScenarioChallengeDetail.caption: ScenarioChallengeDetail#caption.
  ScenarioAnalysis: ScenarioAnalysis#
  TraceAnalysis: TraceAnalysis#
  TraceChallengeDetail: TraceChallengeDetail#
  TraceChallengeDetail.reasoning: TraceChallengeDetail#reasoning.
  TraceChallengeDetail.statement: TraceChallengeDetail#statement.
  TraceChallengeDetail.caption: TraceChallengeDetail#caption.
  HypothesisEvaluation: HypothesisEvaluation#
  HypothesisDetail: HypothesisDetail#
  HypothesisDetail.caption: HypothesisDetail#caption.
  HypothesisDetail.challenge: HypothesisDetail#challenge.
  HypothesisDetail.hypothesis: HypothesisDetail#hypothesis.
  HypothesisSimple: HypothesisSimple#
  DSProposalV1ExpGen._append_retry: DSProposalV1ExpGen#_append_retry().
  DSProposalV2ExpGen.compute_top_scores: DSProposalV2ExpGen#compute_top_scores().
  DSProposalV2ExpGen._cosine_similarity_matrix_torch: DSProposalV2ExpGen#_cosine_similarity_matrix_torch().
  ScenarioChallengeCategory.DATASET_DRIVEN: ScenarioChallengeCategory#DATASET_DRIVEN.
  ScenarioChallengeCategory.DOMAIN_INFORMED: ScenarioChallengeCategory#DOMAIN_INFORMED.
  ScenarioChallengeDetail.metric_impact: ScenarioChallengeDetail#metric_impact.
  ScenarioAnalysis.sota_alignment_analysis: ScenarioAnalysis#sota_alignment_analysis.
  ScenarioAnalysis.gap_identification: ScenarioAnalysis#gap_identification.
  ScenarioAnalysis.domain_implementation_coherence_check: ScenarioAnalysis#domain_implementation_coherence_check.
  ScenarioAnalysis.scenario_first_focus: ScenarioAnalysis#scenario_first_focus.
  TraceAnalysisDetail.category: TraceAnalysisDetail#category.
  TraceAnalysisDetail.statement: TraceAnalysisDetail#statement.
  TraceChallengeDetail.category: TraceChallengeDetail#category.
  TraceChallengeDetail.metric_impact: TraceChallengeDetail#metric_impact.
  HypothesisComponent.DataLoadSpec: HypothesisComponent#DataLoadSpec.
  HypothesisComponent.FeatureEng: HypothesisComponent#FeatureEng.
  HypothesisComponent.Model: HypothesisComponent#Model.
  HypothesisComponent.Ensemble: HypothesisComponent#Ensemble.
  HypothesisComponent.Workflow: HypothesisComponent#Workflow.
  HypothesisEvaluationReasoningScore.reasoning: HypothesisEvaluationReasoningScore#reasoning.
  HypothesisDetail.metric_impact: HypothesisDetail#metric_impact.
  HypothesisSimple.hypothesis: HypothesisSimple#hypothesis.
  HypothesisList.deduplicated_challenges: HypothesisList#deduplicated_challenges.
  CodingSketch.current_state: CodingSketch#current_state.
  CodingSketch.modifications: CodingSketch#modifications.
  CodingSketch.structure: CodingSketch#structure.
  CodingSketch.sketch: CodingSketch#sketch.
  CodingSketch.packages: CodingSketch#packages.
---
# Module: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py)

## Classes
### `CodingSketch`  ·  implements/extends BaseModel
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:276`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L276)
- signature: `class CodingSketch(BaseModel):`
- members:
  - `current_state` — [`L277`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L277)
  - `modifications` — [`L280`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L280)
  - `packages` — [`L299`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L299)
  - `sketch` — [`L293`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L293)
  - `structure` — [`L287`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L287)
- used by: [`task_gen`](proposal.md#DSProposalV2ExpGen.task_gen), [`llm_log_win`](../../../../log/ui/ds_trace.md#llm_log_win)

### `DSProposalV1ExpGen`  ·  implements/extends ExpGen
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:317`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L317)
- signature: `class DSProposalV1ExpGen(ExpGen):`
- members:
  - `gen(self, trace: DSTrace, plan: DSExperimentPlan | None = None)` — [`L318`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L318)
- protocol/private: `_append_retry`[`L429`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L429), `_f`[`L436`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L436)
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`APIBackend`](../../../../oai/llm_utils.md#APIBackend), [`file_dict`](../../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../../core/experiment.md#Experiment.experiment_workspace), [`DSExperiment`](../../experiment/experiment.md#DSExperiment), [`build_messages_and_create_chat_completion`](../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`DSTrace`](base.md#DSTrace), [`ExpGen`](../../../../core/proposal.md#ExpGen), [`get_scenario_all_desc`](../../scen/__init__.md#DataScienceScen.get_scenario_all_desc), [`scen`](../../../../core/proposal.md#Trace.scen), [`DSHypothesis`](base.md#DSHypothesis), [`experiment_and_feedback_list_after_init`](base.md#DSTrace.experiment_and_feedback_list_after_init), [`wait_retry`](../../../../utils/workflow/misc.md#wait_retry), [`DSExperimentPlan`](planner/__init__.md#DSExperimentPlan), [`scen`](../../../../core/proposal.md#ExpGen.scen), [`WorkflowTask`](../../../../components/coder/data_science/workflow/exp.md#WorkflowTask), [`draft_exp_in_decomposition`](proposal.md#draft_exp_in_decomposition), [`inject_code_from_file_dict`](../../../../core/experiment.md#FBWorkspace.inject_code_from_file_dict), [`sota_experiment`](base.md#DSTrace.sota_experiment), [`get_component`](proposal.md#get_component), [`pending_tasks_list`](../../experiment/experiment.md#DSExperiment.pending_tasks_list), [`spec_enabled`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.spec_enabled), [`generate_diff_from_dict`](../../../../utils/repo/diff.md#generate_diff_from_dict), [`template`](../../../../utils/agent/tpl.md#RDAT.template), [`last_exp`](base.md#DSTrace.last_exp), [`enable_notebook_conversion`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.enable_notebook_conversion)
- used by: [`ExpGen`](../../../../core/proposal.md#ExpGen), [`gen`](../../../../core/proposal.md#ExpGen.gen)

### `DSProposalV2ExpGen`  ·  implements/extends ExpGen
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:492`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L492)
- signature: `class DSProposalV2ExpGen(ExpGen):`
- members:
  - `_llm_select_extra_hypo(self, trace: DSTrace)` — [`L1028`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L1028) — Retrieve a list of additional hypotheses along with their ensemble scores
  - `compute_top_scores(self, hypothesis_dict: dict)` — [`L859`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L859) — Compute weighted total scores for each hypothesis and return the top five.
  - `gen(self, trace: DSTrace, plan: DSExperimentPlan | None = None)` — [`L1300`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L1300) — documented in [rdagent-app-data_science-conf](../../../../../../concepts/rdagent-app-data_science-conf.md)
  - `get_all_hypotheses(self, problem_dict: dict, hypothesis_dict: dict)` — [`L1283`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L1283)
  - `hypothesis_critique(self, hypothesis_dict: Dict, problems_dict: Dict, scenario_desc: str, sota_exp_desc: str, exp_feedback_list_desc: str)` — [`L705`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L705) — Critique the generated hypotheses, identifying flaws and suggesting improvements.
  - `hypothesis_gen(self, component_desc: str, scenario_desc: str, exp_feedback_list_desc: str, sota_exp_desc: str, problems: dict, pipeline: bool, enable_idea_pool: bool, is_new_tree: bool, inject_diverse: bool = False, exp_gen_plan: Optional[Dict] = None, sibling_exp: List[DSExperiment] | None = None, former_user_instructions: UserInstructions | None = None)` — [`L609`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L609) — documented in [rdagent-log-logger](../../../../../../concepts/rdagent-log-logger.md)
  - `hypothesis_rank(self, hypothesis_dict: dict, problem_dict: dict, selected_idx: Optional[int] = None)` — [`L1158`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L1158) — Wrapper method that computes the top five hypotheses by weighted scoring and then selects one
  - `hypothesis_rewrite(self, hypothesis_dict: Dict, critiques_dict: Dict, scenario_desc: str, sota_exp_desc: str, exp_feedback_list_desc: str, sibling_exp: List[DSExperiment] | None = None, former_user_instructions: UserInstructions | None = None)` — [`L774`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L774) — Generate improved hypotheses based on critique feedback for each original hypothesis. — documented in [rdagent-log-logger](../../../../../../concepts/rdagent-log-logger.md)
  - `hypothesis_select_with_llm(self, scenario_desc: str, exp_feedback_list_desc: str, sota_exp_desc: str, hypothesis_candidates: dict, trace: DSTrace)` — [`L1055`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L1055) — documented in [rdagent-log-timer](../../../../../../concepts/rdagent-log-timer.md)
  - `identify_feedback_problem(self, scenario_desc: str, exp_feedback_list_desc: str, sota_exp_desc: str, inject_diverse: bool = False, sibling_exp: List[DSExperiment] | None = None)` — [`L532`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L532)
  - `identify_problem(self, current_sub_trace, scenario_desc, sota_exp_desc, exp_feedback_list_desc, inject_diverse, exp_gen_plan, sibling_exp: List[DSExperiment] | None = None)` — [`L569`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L569)
  - `identify_scenario_problem(self, scenario_desc: str, sota_exp_desc: str, exp_gen_plan: Dict, sibling_exp: List[DSExperiment] | None = None)` — [`L497`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L497)
  - `select_hypothesis(self, scores_sorted: pd.Series, hypothesis_dict: dict, problem_dict: dict)` — [`L893`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L893) — From the top five hypotheses (by weighted score), select one based on additional weighting rules
  - `task_gen(self, component_desc: str, scenario_desc: str, sota_exp_desc: str, sota_exp: DSExperiment, hypotheses: list[DSHypothesis], hypotheses_candidates: list[DSHypothesis], pipeline: bool, failed_exp_feedback_list_desc: str, fb_to_sota_exp: ExperimentFeedback | None = None, sibling_exp: List[DSExperiment] | None = None, former_user_instructions: UserInstructions = None)` — [`L1184`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L1184) — documented in [rdagent-log](../../../../../../concepts/rdagent-log.md)
  - `scen_prob_multiplier` — [`L582`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L582)
  - `supports_response_schema` — [`L495`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L495)
- protocol/private: `__init__`[`L493`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L493), `_cosine_similarity_matrix_torch`[`L924`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L924), `_get_current_exp_score_list`[`L995`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L995), `_get_path`[`L987`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L987), `_prob_dis_torch`[`L932`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L932)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../../log/logger.md#RDAgentLog.info), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`APIBackend`](../../../../oai/llm_utils.md#APIBackend), [`file_dict`](../../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../../core/experiment.md#Experiment.experiment_workspace), [`warning`](../../../../log/logger.md#RDAgentLog.warning), [`DSExperiment`](../../experiment/experiment.md#DSExperiment), [`build_messages_and_create_chat_completion`](../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`gen`](merge.md#ExpGen2Hypothesis.gen), [`DSTrace`](base.md#DSTrace), [`ExpGen`](../../../../core/proposal.md#ExpGen), [`hypothesis`](../../../../core/experiment.md#Experiment.hypothesis), [`error`](../../../../log/logger.md#RDAgentLog.error), [`get_scenario_all_desc`](../../../../core/scenario.md#Scenario.get_scenario_all_desc), [`result`](../../../../core/experiment.md#Experiment.result), [`RD_Agent_TIMER_wrapper`](../../../../log/timer.md#RD_Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper), [`ExperimentFeedback`](../../../../core/proposal.md#ExperimentFeedback), [`scen`](../../../../core/proposal.md#Trace.scen), [`hist`](base.md#DSTrace.hist), [`DSHypothesis`](base.md#DSHypothesis), [`knowledge_base`](../../../../core/proposal.md#Trace.knowledge_base), [`hypothesis`](../../../../core/proposal.md#Hypothesis.hypothesis), [`md5_hash`](../../../../utils/__init__.md#md5_hash), [`experiment_and_feedback_list_after_init`](base.md#DSTrace.experiment_and_feedback_list_after_init), [`remain_time`](../../../../log/timer.md#RDAgentTimer.remain_time), [`sota_experiment_fb`](base.md#DSTrace.sota_experiment_fb), [`timer`](../../../../log/timer.md#RDAgentTimerWrapper.timer), [`wait_retry`](../../../../utils/workflow/misc.md#wait_retry), [`DSExperimentPlan`](planner/__init__.md#DSExperimentPlan), [`scen`](../../../../core/proposal.md#ExpGen.scen), [`retrieve_search_list`](base.md#DSTrace.retrieve_search_list), [`started`](../../../../log/timer.md#RDAgentTimer.started), [`PipelineTask`](../../../../components/coder/data_science/pipeline/exp.md#PipelineTask), [`WorkflowTask`](../../../../components/coder/data_science/workflow/exp.md#WorkflowTask), [`all_duration`](../../../../log/timer.md#RDAgentTimer.all_duration), [`get_parent_exps`](../../../../core/proposal.md#Trace.get_parent_exps), [`get_sibling_exps`](base.md#DSTrace.get_sibling_exps)  (+67 more)
- used by: [`gen`](merge.md#ExpGen2Hypothesis.gen), [`ExpGen`](../../../../core/proposal.md#ExpGen), [`gen`](../../../../core/proposal.md#ExpGen.gen), [`default_exp_gen`](../../loop.md#DataScienceRDLoop.default_exp_gen), [`ExpGen2Hypothesis`](merge.md#ExpGen2Hypothesis)

### `HypothesisComponent`  ·  implements/extends Enum, str
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:210`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L210)
- signature: `class HypothesisComponent(str, Enum):`
- members:
  - `DataLoadSpec` — [`L211`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L211)
  - `Ensemble` — [`L214`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L214)
  - `FeatureEng` — [`L212`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L212)
  - `Model` — [`L213`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L213)
  - `Workflow` — [`L215`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L215)
- used by: [`hypothesis_select_with_llm`](proposal.md#DSProposalV2ExpGen.hypothesis_select_with_llm), [`component`](proposal.md#HypothesisDetail.component), [`component`](proposal.md#HypothesisSimple.component)

### `HypothesisDetail`  ·  implements/extends BaseModel
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:243`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L243)
- signature: `class HypothesisDetail(BaseModel):`
- members:
  - `caption` — [`L244`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L244)
  - `challenge` — [`L245`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L245)
  - `component` — [`L256`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L256)
  - `evaluation` — [`L257`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L257)
  - `hypothesis` — [`L248`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L248)
  - `metric_impact` — [`L251`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L251)
- uses (calls/refs, reference-scoped): [`HypothesisComponent`](proposal.md#HypothesisComponent), [`HypothesisEvaluation`](proposal.md#HypothesisEvaluation)
- used by: [`hypothesis_gen`](proposal.md#DSProposalV2ExpGen.hypothesis_gen), [`hypotheses`](proposal.md#HypothesisList.hypotheses)

### `HypothesisEvaluation`  ·  implements/extends BaseModel
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:225`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L225)
- signature: `class HypothesisEvaluation(BaseModel):`
- members:
  - `alignment` — [`L226`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L226)
  - `feasibility` — [`L235`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L235)
  - `impact` — [`L229`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L229)
  - `novelty` — [`L232`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L232)
  - `risk_reward_balance` — [`L238`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L238)
- uses (calls/refs, reference-scoped): [`HypothesisEvaluationReasoningScore`](proposal.md#HypothesisEvaluationReasoningScore)
- used by: [`hypothesis_gen`](proposal.md#DSProposalV2ExpGen.hypothesis_gen), [`evaluation`](proposal.md#HypothesisDetail.evaluation)

### `HypothesisEvaluationReasoningScore`  ·  implements/extends BaseModel
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:218`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L218)
- signature: `class HypothesisEvaluationReasoningScore(BaseModel):`
- members:
  - `reasoning` — [`L219`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L219)
  - `score` — [`L222`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L222)
- used by: [`hypothesis_gen`](proposal.md#DSProposalV2ExpGen.hypothesis_gen), [`alignment`](proposal.md#HypothesisEvaluation.alignment), [`feasibility`](proposal.md#HypothesisEvaluation.feasibility), [`impact`](proposal.md#HypothesisEvaluation.impact), [`novelty`](proposal.md#HypothesisEvaluation.novelty), [`risk_reward_balance`](proposal.md#HypothesisEvaluation.risk_reward_balance)

### `HypothesisList`  ·  implements/extends BaseModel
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:267`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L267)
- signature: `class HypothesisList(BaseModel):`
- members:
  - `deduplicated_challenges` — [`L268`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L268)
  - `hypotheses` — [`L271`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L271)
- uses (calls/refs, reference-scoped): [`HypothesisDetail`](proposal.md#HypothesisDetail)
- used by: [`hypothesis_gen`](proposal.md#DSProposalV2ExpGen.hypothesis_gen), [`llm_log_win`](../../../../log/ui/ds_trace.md#llm_log_win)

### `HypothesisSimple`  ·  implements/extends BaseModel
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:260`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L260)
- signature: `class HypothesisSimple(BaseModel):`
- members:
  - `component` — [`L264`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L264)
  - `hypothesis` — [`L261`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L261)
- uses (calls/refs, reference-scoped): [`HypothesisComponent`](proposal.md#HypothesisComponent)
- used by: [`hypothesis_select_with_llm`](proposal.md#DSProposalV2ExpGen.hypothesis_select_with_llm)

### `ScenarioAnalysis`  ·  implements/extends BaseModel
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:121`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L121)
- signature: `class ScenarioAnalysis(BaseModel):`
- members:
  - `domain_implementation_coherence_check` — [`L126`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L126)
  - `gap_identification` — [`L123`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L123)
  - `scenario_first_focus` — [`L129`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L129)
  - `sota_alignment_analysis` — [`L122`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L122)
- used by: [`analysis`](proposal.md#ScenarioChallenges.analysis)

### `ScenarioChallengeCategory`  ·  implements/extends Enum, str
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:98`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L98)
- signature: `class ScenarioChallengeCategory(str, Enum):`
- members:
  - `DATASET_DRIVEN` — [`L99`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L99)
  - `DOMAIN_INFORMED` — [`L100`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L100)
- used by: [`category`](proposal.md#ScenarioChallengeDetail.category)

### `ScenarioChallengeDetail`  ·  implements/extends BaseModel
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:103`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L103)
- signature: `class ScenarioChallengeDetail(BaseModel):`
- members:
  - `caption` — [`L118`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L118)
  - `category` — [`L111`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L111)
  - `metric_impact` — [`L115`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L115)
  - `reasoning` — [`L104`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L104)
  - `statement` — [`L112`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L112)
- uses (calls/refs, reference-scoped): [`ScenarioChallengeCategory`](proposal.md#ScenarioChallengeCategory)
- used by: [`identify_scenario_problem`](proposal.md#DSProposalV2ExpGen.identify_scenario_problem), [`challenges`](proposal.md#ScenarioChallenges.challenges)

### `ScenarioChallenges`  ·  implements/extends BaseModel
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:134`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L134)
- signature: `class ScenarioChallenges(BaseModel):`
- members:
  - `analysis` — [`L136`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L136)
  - `challenges` — [`L139`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L139)
- uses (calls/refs, reference-scoped): [`ScenarioAnalysis`](proposal.md#ScenarioAnalysis), [`ScenarioChallengeDetail`](proposal.md#ScenarioChallengeDetail)
- used by: [`llm_log_win`](../../../../log/ui/ds_trace.md#llm_log_win), [`identify_scenario_problem`](proposal.md#DSProposalV2ExpGen.identify_scenario_problem)

### `TraceAnalysis`  ·  implements/extends BaseModel
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:155`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L155)
- signature: `class TraceAnalysis(BaseModel):`
- members:
  - `feedback` — [`L157`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L157)
  - `implementation_review` — [`L160`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L160)
  - `trace_history` — [`L163`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L163)
- uses (calls/refs, reference-scoped): [`TraceAnalysisDetail`](proposal.md#TraceAnalysisDetail)
- used by: [`analysis`](proposal.md#TraceChallenges.analysis)

### `TraceAnalysisDetail`  ·  implements/extends BaseModel
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:145`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L145)
- signature: `class TraceAnalysisDetail(BaseModel):`
- members:
  - `category` — [`L147`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L147)
  - `statement` — [`L150`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L150)
- used by: [`feedback`](proposal.md#TraceAnalysis.feedback), [`implementation_review`](proposal.md#TraceAnalysis.implementation_review), [`trace_history`](proposal.md#TraceAnalysis.trace_history)

### `TraceChallengeDetail`  ·  implements/extends BaseModel
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:168`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L168)
- signature: `class TraceChallengeDetail(BaseModel):`
- members:
  - `caption` — [`L192`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L192)
  - `category` — [`L174`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L174)
  - `metric_impact` — [`L186`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L186)
  - `reasoning` — [`L169`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L169)
  - `statement` — [`L180`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L180)
- used by: [`identify_feedback_problem`](proposal.md#DSProposalV2ExpGen.identify_feedback_problem), [`challenges`](proposal.md#TraceChallenges.challenges)

### `TraceChallenges`  ·  implements/extends BaseModel
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/proposal.py:195`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L195)
- signature: `class TraceChallenges(BaseModel):`
- members:
  - `analysis` — [`L196`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L196)
  - `challenges` — [`L202`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L202)
- uses (calls/refs, reference-scoped): [`TraceAnalysis`](proposal.md#TraceAnalysis), [`TraceChallengeDetail`](proposal.md#TraceChallengeDetail)
- used by: [`llm_log_win`](../../../../log/ui/ds_trace.md#llm_log_win), [`identify_feedback_problem`](proposal.md#DSProposalV2ExpGen.identify_feedback_problem)

## Functions
- `draft_exp_in_decomposition(scen: Scenario, trace: DSTrace)` — [`L306`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L306)
- `get_component(name: str)` — [`L85`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L85)

## Module values
- `_COMPONENT_META` — [`L45`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/proposal.py#L45)


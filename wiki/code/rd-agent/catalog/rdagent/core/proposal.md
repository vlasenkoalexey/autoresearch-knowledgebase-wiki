---
title: 'Module: rdagent/core/proposal.py'
type: catalog
provenance: extracted
module: rdagent/core/proposal.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.core.proposal`/
symbols:
  Trace.hist: Trace#hist.
  Trace: Trace#
  Hypothesis: Hypothesis#
  ExpGen: ExpGen#
  ExpGen.gen: ExpGen#gen().
  ExperimentFeedback: ExperimentFeedback#
  Trace.scen: Trace#scen.
  HypothesisFeedback: HypothesisFeedback#
  Experiment2Feedback: Experiment2Feedback#
  Trace.knowledge_base: Trace#knowledge_base.
  Experiment2Feedback.generate_feedback: Experiment2Feedback#generate_feedback().
  Hypothesis.hypothesis: Hypothesis#hypothesis.
  Trace.NEW_ROOT: Trace#NEW_ROOT.
  ExpGen.async_gen: ExpGen#async_gen().
  ExpGen.scen: ExpGen#scen.
  Trace.sync_dag_parent_and_hist: Trace#sync_dag_parent_and_hist().
  ExperimentFeedback.decision: ExperimentFeedback#decision.
  Experiment2Feedback.scen: Experiment2Feedback#scen.
  Trace.get_sota_experiment: Trace#get_sota_experiment().
  HypothesisGen.scen: HypothesisGen#scen.
  Trace.get_parent_exps: Trace#get_parent_exps().
  Trace.set_current_selection: Trace#set_current_selection().
  Trace.dag_parent: Trace#dag_parent.
  HypothesisFeedback.__str__: HypothesisFeedback#__str__().
  CheckpointSelector: CheckpointSelector#
  SOTAexpSelector: SOTAexpSelector#
  SOTAexpSelector.get_sota_exp_to_submit: SOTAexpSelector#get_sota_exp_to_submit().
  Hypothesis2Experiment: Hypothesis2Experiment#
  Trace.get_sota_hypothesis_and_experiment: Trace#get_sota_hypothesis_and_experiment().
  Trace.is_selection_new_tree: Trace#is_selection_new_tree().
  Trace.get_parents: Trace#get_parents().
  Hypothesis2Experiment.convert: Hypothesis2Experiment#convert().
  CheckpointSelector.get_selection: CheckpointSelector#get_selection().
  Hypothesis.reason: Hypothesis#reason.
  Trace.exp2idx: Trace#exp2idx().
  Trace.get_children: Trace#get_children().
  HypothesisGen.gen: HypothesisGen#gen().
  Trace.current_selection: Trace#current_selection.
  Trace.get_current_selection: Trace#get_current_selection().
  ExpGen.__init__: ExpGen#__init__().
  HypothesisGen: HypothesisGen#
  Trace.NodeType: Trace#NodeType.
  Trace.__init__: Trace#__init__().
  ExpPlanner: ExpPlanner#
  ExpPlanner.plan: ExpPlanner#plan().
  ExperimentFeedback.reason: ExperimentFeedback#reason.
  ExperimentFeedback.__str__: ExperimentFeedback#__str__().
  Trace.idx2loop_id: Trace#idx2loop_id.
  ASpecificScen: ASpecificScen.
  ASpecificKB: ASpecificKB.
  Experiment2Feedback.__init__: Experiment2Feedback#__init__().
  Hypothesis.concise_reason: Hypothesis#concise_reason.
  Hypothesis.__str__: Hypothesis#__str__().
  ExperimentFeedback.exception: ExperimentFeedback#exception.
  HypothesisFeedback.observations: HypothesisFeedback#observations.
  HypothesisFeedback.hypothesis_evaluation: HypothesisFeedback#hypothesis_evaluation.
  HypothesisFeedback.new_hypothesis: HypothesisFeedback#new_hypothesis.
  Trace.idx2exp: Trace#idx2exp().
  Trace.is_parent: Trace#is_parent().
  Hypothesis.__init__: Hypothesis#__init__().
  Hypothesis.concise_justification: Hypothesis#concise_justification.
  ExperimentFeedback.from_exception: ExperimentFeedback#from_exception().
  ExpGen.reset: ExpGen#reset().
  HypothesisGen.__init__: HypothesisGen#__init__().
  Hypothesis.concise_observation: Hypothesis#concise_observation.
  Hypothesis.concise_knowledge: Hypothesis#concise_knowledge.
  ExperimentFeedback.eda_improvement: ExperimentFeedback#eda_improvement.
  ExperimentFeedback.__bool__: ExperimentFeedback#__bool__().
  HypothesisFeedback.__init__: HypothesisFeedback#__init__().
  ExpPlanner.__init__: ExpPlanner#__init__().
  HypothesisFeedback.acceptable: HypothesisFeedback#acceptable.
  ExperimentFeedback.__init__: ExperimentFeedback#__init__().
  ExperimentFeedback.code_change_summary: ExperimentFeedback#code_change_summary.
  Trace.SEL_LATEST_SOTA: Trace#SEL_LATEST_SOTA.
  ExpPlanner.scen: ExpPlanner#scen.
---
# Module: [`rdagent/core/proposal.py`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py)

## Classes
### `CheckpointSelector`
- def: [`rdagent/core/proposal.py:321`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L321)
- doc: In the trace, we may start from any check point (we'll represent it as a variable `from_checkpoint_idx`)
- signature: `class CheckpointSelector:`
- members:
  - `get_selection(self, trace: Trace)` — [`L327`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L327) — checkpoint_idx represents the place where we want to create a new node.
- uses (calls/refs, reference-scoped): [`Trace`](proposal.md#Trace), [`get_selection`](../scenarios/data_science/proposal/exp_gen/select/expand.md#LimitTimeCKPSelector.get_selection), [`get_selection`](../scenarios/data_science/proposal/exp_gen/select/expand.md#BackJumpCKPSelector.get_selection), [`get_selection`](../scenarios/data_science/proposal/exp_gen/select/expand.md#SOTAJumpCKPSelector.get_selection), [`BackJumpCKPSelector`](../scenarios/data_science/proposal/exp_gen/select/expand.md#BackJumpCKPSelector), [`LatestCKPSelector`](../scenarios/data_science/proposal/exp_gen/select/expand.md#LatestCKPSelector), [`LimitTimeCKPSelector`](../scenarios/data_science/proposal/exp_gen/select/expand.md#LimitTimeCKPSelector), [`SOTAJumpCKPSelector`](../scenarios/data_science/proposal/exp_gen/select/expand.md#SOTAJumpCKPSelector), [`get_selection`](../scenarios/data_science/proposal/exp_gen/select/expand.md#LatestCKPSelector.get_selection)
- used by: [`BackJumpCKPSelector`](../scenarios/data_science/proposal/exp_gen/select/expand.md#BackJumpCKPSelector), [`LatestCKPSelector`](../scenarios/data_science/proposal/exp_gen/select/expand.md#LatestCKPSelector), [`LimitTimeCKPSelector`](../scenarios/data_science/proposal/exp_gen/select/expand.md#LimitTimeCKPSelector), [`SOTAJumpCKPSelector`](../scenarios/data_science/proposal/exp_gen/select/expand.md#SOTAJumpCKPSelector)

### `ExpGen`  ·  implements/extends ABC
- def: [`rdagent/core/proposal.py:372`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L372) — documented in [rdagent-core-proposal](../../../concepts/rdagent-core-proposal.md)
- signature: `class ExpGen(ABC):`
- members:
  - `async_gen(self, trace: Trace, loop: LoopBase)` — [`L394`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L394) — generate the experiment and decide whether to stop yield generation and give up control to other routines. — documented in [rdagent-core-conf](../../../concepts/rdagent-core-conf.md)
  - `gen(self, trace: Trace)` — [`L378`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L378) — Generate the experiment based on the trace. — documented in [rdagent-core-proposal](../../../concepts/rdagent-core-proposal.md)
  - `reset(self)` — [`L405`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L405) — Reset the proposal to the initial state.
  - `scen` — [`L375`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L375)
- protocol/private: `__init__`[`L374`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L374)
- uses (calls/refs, reference-scoped): [`Scenario`](scenario.md#Scenario), [`Experiment`](experiment.md#Experiment), [`async_gen`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.async_gen), [`gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.gen), [`Trace`](proposal.md#Trace), [`RD_AGENT_SETTINGS`](conf.md#RD_AGENT_SETTINGS), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV2.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV1ExpGen.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftExpGen.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV3.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMerge.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftV2ExpGen.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#MergeExpGen.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#MergeExpGen_MultiTrace.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/naive.md#NaiveExpGen.gen), [`gen`](../scenarios/rl/proposal/proposal.md#RLPostTrainingExpGen.gen), [`gen`](../scenarios/finetune/proposal/proposal.md#LLMFinetuneExpGen.gen), [`LoopBase`](../utils/workflow/loop.md#LoopBase), [`loop_idx`](../utils/workflow/loop.md#LoopBase.loop_idx), [`get_max_parallel`](conf.md#RDAgentSettings.get_max_parallel), [`DSProposalV2ExpGen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen), [`get_unfinished_loop_cnt`](../utils/workflow/loop.md#LoopBase.get_unfinished_loop_cnt), [`gen`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.gen), [`DSDraftExpGen`](../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftExpGen), [`reset`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.reset), [`DSDraftV2ExpGen`](../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftV2ExpGen), [`MergeExpGen`](../scenarios/data_science/proposal/exp_gen/merge.md#MergeExpGen), [`MergeExpGen_MultiTrace`](../scenarios/data_science/proposal/exp_gen/merge.md#MergeExpGen_MultiTrace), [`DSProposalV1ExpGen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV1ExpGen), [`ExpGen2TraceAndMerge`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMerge), [`ExpGen2TraceAndMergeV2`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV2), [`ExpGen2TraceAndMergeV3`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV3), [`LLMFinetuneExpGen`](../scenarios/finetune/proposal/proposal.md#LLMFinetuneExpGen), [`NaiveExpGen`](../scenarios/data_science/proposal/exp_gen/naive.md#NaiveExpGen), [`ParallelMultiTraceExpGen`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen), [`RLPostTrainingExpGen`](../scenarios/rl/proposal/proposal.md#RLPostTrainingExpGen)
- used by: [`record`](../scenarios/data_science/loop.md#DataScienceRDLoop.record), [`async_gen`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.async_gen), [`gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.gen), [`_gen_hypothesis`](../scenarios/finetune/proposal/proposal.md#LLMFinetuneExpGen._gen_hypothesis), [`hypothesis_select_with_llm`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_select_with_llm), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV2.gen), [`task_gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.task_gen), [`gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV1ExpGen.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV3.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMerge.gen), [`task_gen`](../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftV2ExpGen.task_gen), [`main`](../app/data_science/loop.md#main), [`direct_exp_gen`](../scenarios/data_science/loop.md#DataScienceRDLoop.direct_exp_gen), [`exp_gen`](../scenarios/data_science/loop.md#DataScienceRDLoop.exp_gen), [`knowledge_gen`](../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftV2ExpGen.knowledge_gen), [`planner`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.planner), [`exp_gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV2.exp_gen), [`DSProposalV2ExpGen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen), [`exp_gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMerge.exp_gen), [`exp_gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV3.exp_gen), [`exp_gen`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.exp_gen), [`default_exp_gen`](../scenarios/data_science/loop.md#DataScienceRDLoop.default_exp_gen), [`draft_exp_gen`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.draft_exp_gen), [`merge_exp_gen`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.merge_exp_gen), [`merge_exp_gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMerge.merge_exp_gen), [`merge_exp_gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV2.merge_exp_gen), [`merge_exp_gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV3.merge_exp_gen), [`DSDraftExpGen`](../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftExpGen), [`__init__`](../scenarios/finetune/proposal/proposal.md#LLMFinetuneExpGen.__init__), [`__init__`](../scenarios/rl/proposal/proposal.md#RLPostTrainingExpGen.__init__), [`DSDraftV2ExpGen`](../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftV2ExpGen), [`MergeExpGen`](../scenarios/data_science/proposal/exp_gen/merge.md#MergeExpGen), [`MergeExpGen_MultiTrace`](../scenarios/data_science/proposal/exp_gen/merge.md#MergeExpGen_MultiTrace), [`DSProposalV1ExpGen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV1ExpGen), [`ExpGen2TraceAndMerge`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMerge), [`ExpGen2TraceAndMergeV2`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV2), [`ExpGen2TraceAndMergeV3`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV3), [`LLMFinetuneExpGen`](../scenarios/finetune/proposal/proposal.md#LLMFinetuneExpGen), [`NaiveExpGen`](../scenarios/data_science/proposal/exp_gen/naive.md#NaiveExpGen), [`ParallelMultiTraceExpGen`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen)  (+7 more)

### `ExpPlanner`  ·  implements/extends ABC, Generic
- def: [`rdagent/core/proposal.py:355`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L355)
- doc: An abstract class for planning the experiment.
- signature: `class ExpPlanner(ABC, Generic[ASpecificPlan]):`
- members:
  - `plan(self, trace: Trace)` — [`L365`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L365) — Generate a plan for the experiment based on the trace.
  - `scen` — [`L362`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L362)
- protocol/private: `__init__`[`L361`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L361)
- uses (calls/refs, reference-scoped): [`Scenario`](scenario.md#Scenario), [`Trace`](proposal.md#Trace), [`plan`](../scenarios/data_science/proposal/exp_gen/planner/__init__.md#DSExpPlannerHandCraft.plan), [`ASpecificPlan`](experiment.md#ASpecificPlan), [`DSExpPlannerHandCraft`](../scenarios/data_science/proposal/exp_gen/planner/__init__.md#DSExpPlannerHandCraft)
- used by: [`DSExpPlannerHandCraft`](../scenarios/data_science/proposal/exp_gen/planner/__init__.md#DSExpPlannerHandCraft)

### `Experiment2Feedback`  ·  implements/extends ABC
- def: [`rdagent/core/proposal.py:451`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L451)
- doc: "Generated feedbacks on the hypothesis from **Executed** Implementations of different tasks
- signature: `class Experiment2Feedback(ABC):`
- members:
  - `generate_feedback(self, exp: Experiment, trace: Trace, exception: Exception | None = None)` — [`L459`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L459) — The `exp` should be executed and the results should be included, as well as the comparison
  - `scen` — [`L456`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L456)
- protocol/private: `__init__`[`L455`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L455)
- uses (calls/refs, reference-scoped): [`Scenario`](scenario.md#Scenario), [`Experiment`](experiment.md#Experiment), [`Trace`](proposal.md#Trace), [`generate_feedback`](../scenarios/data_science/dev/feedback.md#DSExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/finetune/dev/feedback.md#FTExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/kaggle/developer/feedback.md#KGExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/qlib/developer/feedback.md#QlibFactorExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/qlib/developer/feedback.md#QlibModelExperiment2Feedback.generate_feedback), [`ExperimentFeedback`](proposal.md#ExperimentFeedback), [`generate_feedback`](../scenarios/rl/dev/feedback.md#RLExperiment2Feedback.generate_feedback), [`DSExperiment2Feedback`](../scenarios/data_science/dev/feedback.md#DSExperiment2Feedback), [`FTExperiment2Feedback`](../scenarios/finetune/dev/feedback.md#FTExperiment2Feedback), [`KGExperiment2Feedback`](../scenarios/kaggle/developer/feedback.md#KGExperiment2Feedback), [`QlibFactorExperiment2Feedback`](../scenarios/qlib/developer/feedback.md#QlibFactorExperiment2Feedback), [`QlibModelExperiment2Feedback`](../scenarios/qlib/developer/feedback.md#QlibModelExperiment2Feedback), [`RLExperiment2Feedback`](../scenarios/rl/dev/feedback.md#RLExperiment2Feedback)
- used by: [`generate_feedback`](../scenarios/data_science/dev/feedback.md#DSExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/finetune/dev/feedback.md#FTExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/kaggle/developer/feedback.md#KGExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/qlib/developer/feedback.md#QlibFactorExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/qlib/developer/feedback.md#QlibModelExperiment2Feedback.generate_feedback), [`feedback`](../scenarios/data_science/loop.md#DataScienceRDLoop.feedback), [`feedback`](../components/workflow/rd_loop.md#RDLoop.feedback), [`feedback`](../app/qlib_rd_loop/quant.md#QuantRDLoop.feedback), [`summarizer`](../app/kaggle/loop.md#KaggleRDLoop.summarizer), [`feedback`](../scenarios/finetune/loop.md#LLMFinetuneRDLoop.feedback), [`feedback`](../scenarios/rl/loop.md#RLPostTrainingRDLoop.feedback), [`factor_summarizer`](../app/qlib_rd_loop/quant.md#QuantRDLoop.factor_summarizer), [`model_summarizer`](../app/qlib_rd_loop/quant.md#QuantRDLoop.model_summarizer), [`summarizer`](../components/workflow/rd_loop.md#RDLoop.summarizer), [`__init__`](../scenarios/data_science/dev/feedback.md#DSExperiment2Feedback.__init__), [`__init__`](../scenarios/finetune/dev/feedback.md#FTExperiment2Feedback.__init__), [`__init__`](../scenarios/rl/dev/feedback.md#RLExperiment2Feedback.__init__), [`process_results`](../scenarios/kaggle/developer/feedback.md#KGExperiment2Feedback.process_results), [`DSExperiment2Feedback`](../scenarios/data_science/dev/feedback.md#DSExperiment2Feedback), [`FTExperiment2Feedback`](../scenarios/finetune/dev/feedback.md#FTExperiment2Feedback), [`KGExperiment2Feedback`](../scenarios/kaggle/developer/feedback.md#KGExperiment2Feedback), [`QlibFactorExperiment2Feedback`](../scenarios/qlib/developer/feedback.md#QlibFactorExperiment2Feedback), [`QlibModelExperiment2Feedback`](../scenarios/qlib/developer/feedback.md#QlibModelExperiment2Feedback), [`RLExperiment2Feedback`](../scenarios/rl/dev/feedback.md#RLExperiment2Feedback)

### `ExperimentFeedback`  ·  implements/extends Feedback
- def: [`rdagent/core/proposal.py:58`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L58) — documented in [rdagent-app-CI-run](../../../concepts/rdagent-app-CI-run.md)
- signature: `class ExperimentFeedback(Feedback):`
- members:
  - `from_exception(cls, e: Exception)` — [`L89`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L89) — A convenient method to create Feedback from an exception.
  - `code_change_summary` — [`L76`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L76)
  - `decision` — [`L68`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L68)
  - `eda_improvement` — [`L69`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L69)
  - `exception` — [`L73`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L73)
  - `reason` — [`L70`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L70)
- protocol/private: `__bool__`[`L78`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L78), `__init__`[`L59`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L59), `__str__`[`L81`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L81)
- uses (calls/refs, reference-scoped): [`HypothesisFeedback`](proposal.md#HypothesisFeedback), [`Feedback`](evaluation.md#Feedback)
- used by: [`record`](../scenarios/data_science/loop.md#DataScienceRDLoop.record), [`_obj_to_json`](../log/ui/storage.md#WebStorage._obj_to_json), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2Hypothesis.gen), [`task_gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.task_gen), [`generate_feedback`](../scenarios/data_science/dev/feedback.md#DSExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/finetune/dev/feedback.md#FTExperiment2Feedback.generate_feedback), [`gen`](../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftExpGen.gen), [`summarize_folder`](../log/mle_summary.md#summarize_folder), [`HypothesisFeedback`](proposal.md#HypothesisFeedback), [`feedback_window`](../log/ui/app.md#feedback_window), [`Feedback`](evaluation.md#Feedback), [`feedback`](../scenarios/data_science/loop.md#DataScienceRDLoop.feedback), [`hist`](../scenarios/data_science/proposal/exp_gen/base.md#DSTrace.hist), [`generate_feedback`](proposal.md#Experiment2Feedback.generate_feedback), [`experiment_and_feedback_list_after_init`](../scenarios/data_science/proposal/exp_gen/base.md#DSTrace.experiment_and_feedback_list_after_init), [`get_msgs_until`](../log/ui/app.md#get_msgs_until), [`sota_experiment_fb`](../scenarios/data_science/proposal/exp_gen/base.md#DSTrace.sota_experiment_fb), [`prepare_context`](../scenarios/qlib/proposal/model_proposal.md#QlibModelHypothesis2Experiment.prepare_context), [`consume_msg`](../log/ui/web.md#HypothesisFeedbackWindow.consume_msg), [`sync_dag_parent_and_hist`](../scenarios/data_science/proposal/exp_gen/base.md#DSTrace.sync_dag_parent_and_hist), [`_build_trace_summary`](../scenarios/rl/proposal/proposal.md#RLPostTrainingExpGen._build_trace_summary), [`get_sota_experiment`](proposal.md#Trace.get_sota_experiment), [`retrieve_search_list`](../scenarios/data_science/proposal/exp_gen/base.md#DSTrace.retrieve_search_list), [`targets`](../scenarios/qlib/proposal/quant_proposal.md#QlibQuantHypothesisGen.targets), [`has_component`](../scenarios/data_science/proposal/exp_gen/base.md#DSTrace.has_component), [`__str__`](proposal.md#HypothesisFeedback.__str__), [`get_sort_key`](../scenarios/data_science/proposal/exp_gen/select/submit.md#BestValidSelector.get_sort_key), [`get_sota_hypothesis_and_experiment`](proposal.md#Trace.get_sota_hypothesis_and_experiment), [`calculate_potential`](../scenarios/data_science/proposal/exp_gen/trace_scheduler.md#SOTABasedScheduler.calculate_potential), [`prepare_context`](../scenarios/qlib/proposal/model_proposal.md#QlibModelHypothesisGen.prepare_context), [`last_runnable_exp_fb`](../scenarios/data_science/proposal/exp_gen/base.md#DSTrace.last_runnable_exp_fb), [`get_sort_key_without_decision`](../scenarios/data_science/proposal/exp_gen/select/submit.md#BestValidSelector.get_sort_key_without_decision), [`last_exp_fb`](../scenarios/data_science/proposal/exp_gen/base.md#DSTrace.last_exp_fb), [`NodeType`](proposal.md#Trace.NodeType), [`last_successful_exp`](../scenarios/data_science/proposal/exp_gen/base.md#DSTrace.last_successful_exp), [`hist`](../scenarios/finetune/proposal/trace.md#FTTrace.hist), [`__init__`](proposal.md#HypothesisFeedback.__init__)

### `Hypothesis`
- def: [`rdagent/core/proposal.py:24`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L24) — documented in [rdagent-core-proposal](../../../concepts/rdagent-core-proposal.md)
- doc: TODO: We may have better name for it.
- signature: `class Hypothesis:`
- members:
  - `concise_justification` — [`L45`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L45)
  - `concise_knowledge` — [`L46`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L46)
  - `concise_observation` — [`L44`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L44)
  - `concise_reason` — [`L43`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L43)
  - `hypothesis` — [`L41`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L41)
  - `reason` — [`L42`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L42)
- protocol/private: `__init__`[`L32`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L32), `__str__`[`L48`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L48)
- uses (calls/refs, reference-scoped): [`DSHypothesis`](../scenarios/data_science/proposal/exp_gen/base.md#DSHypothesis), [`FTHypothesis`](../scenarios/finetune/proposal/proposal.md#FTHypothesis), [`KGHypothesis`](../scenarios/kaggle/proposal/proposal.md#KGHypothesis), [`QlibQuantHypothesis`](../scenarios/qlib/proposal/quant_proposal.md#QlibQuantHypothesis)
- used by: [`_obj_to_json`](../log/ui/storage.md#WebStorage._obj_to_json), [`consume_msg`](../log/ui/web.md#SimpleTraceWindow.consume_msg), [`generate_feedback`](../scenarios/data_science/dev/feedback.md#DSExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/kaggle/developer/feedback.md#KGExperiment2Feedback.generate_feedback), [`hypothesis`](experiment.md#Experiment.hypothesis), [`generate_feedback`](../scenarios/qlib/developer/feedback.md#QlibFactorExperiment2Feedback.generate_feedback), [`evaluate_one_trace`](../scenarios/data_science/proposal/exp_gen/select/submit.md#evaluate_one_trace), [`interact`](../scenarios/data_science/interactor/__init__.md#DSInteractor.interact), [`process_factor_data`](../scenarios/qlib/developer/utils.md#process_factor_data), [`consume_msg`](../log/ui/web.md#TraceWindow.consume_msg), [`dump_and_wait_for_user_input`](../scenarios/data_science/interactor/__init__.md#FBDSInteractor.dump_and_wait_for_user_input), [`DSHypothesis`](../scenarios/data_science/proposal/exp_gen/base.md#DSHypothesis), [`convert_model_experiment`](../scenarios/kaggle/proposal/proposal.md#KGHypothesis2Experiment.convert_model_experiment), [`convert`](../components/proposal/__init__.md#LLMHypothesis2Experiment.convert), [`gen`](../components/proposal/__init__.md#LLMHypothesisGen.gen), [`prepare_context`](../scenarios/qlib/proposal/model_proposal.md#QlibModelHypothesis2Experiment.prepare_context), [`convert_response`](../scenarios/kaggle/proposal/proposal.md#KGHypothesis2Experiment.convert_response), [`convert_response`](../scenarios/qlib/proposal/factor_proposal.md#QlibFactorHypothesis2Experiment.convert_response), [`current_action`](../scenarios/kaggle/proposal/proposal.md#KGHypothesis2Experiment.current_action), [`prepare_context`](../scenarios/qlib/proposal/factor_proposal.md#QlibFactorHypothesis2Experiment.prepare_context), [`research_window`](../log/ui/app.md#research_window), [`gen`](../scenarios/rl/proposal/proposal.md#RLPostTrainingExpGen.gen), [`prepare_context`](../scenarios/kaggle/proposal/proposal.md#KGHypothesis2Experiment.prepare_context), [`_build_trace_summary`](../scenarios/rl/proposal/proposal.md#RLPostTrainingExpGen._build_trace_summary), [`__init__`](experiment.md#Experiment.__init__), [`__str__`](../scenarios/kaggle/proposal/proposal.md#KGHypothesis.__str__), [`convert_response`](../scenarios/qlib/proposal/model_proposal.md#QlibModelHypothesis2Experiment.convert_response), [`consume_msg`](../log/ui/web.md#HypothesisWindow.consume_msg), [`_exp_gen`](../components/workflow/rd_loop.md#RDLoop._exp_gen), [`_prob_dis_torch`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen._prob_dis_torch), [`convert_feature_experiment`](../scenarios/kaggle/proposal/proposal.md#KGHypothesis2Experiment.convert_feature_experiment), [`convert_response`](../components/proposal/__init__.md#LLMHypothesis2Experiment.convert_response), [`__str__`](../scenarios/data_science/proposal/exp_gen/base.md#DSHypothesis.__str__), [`_init_task_gen`](../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftExpGen._init_task_gen), [`_interact_hypo`](../components/workflow/rd_loop.md#RDLoop._interact_hypo), [`convert_response`](../components/proposal/__init__.md#LLMHypothesisGen.convert_response), [`generate_hypothesis`](../app/qlib_rd_loop/factor_from_report.md#generate_hypothesis), [`get_sota_hypothesis_and_experiment`](proposal.md#Trace.get_sota_hypothesis_and_experiment), [`prepare_context`](../components/proposal/__init__.md#LLMHypothesis2Experiment.prepare_context), [`convert`](proposal.md#Hypothesis2Experiment.convert)  (+21 more; 3 test-only)

### `Hypothesis2Experiment`  ·  implements/extends ABC, Generic
- def: [`rdagent/core/proposal.py:437`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L437)
- doc: \[Abstract description =&gt; concrete description\] =&gt; Code implementation Card
- signature: `class Hypothesis2Experiment(ABC, Generic[ASpecificExp]):`
- members:
  - `convert(self, hypothesis: Hypothesis, trace: Trace)` — [`L443`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L443) — Connect the idea proposal to implementation
- uses (calls/refs, reference-scoped): [`Trace`](proposal.md#Trace), [`Hypothesis`](proposal.md#Hypothesis), [`convert`](../components/proposal/__init__.md#LLMHypothesis2Experiment.convert), [`ASpecificExp`](experiment.md#ASpecificExp), [`LLMHypothesis2Experiment`](../components/proposal/__init__.md#LLMHypothesis2Experiment)
- used by: [`direct_exp_gen`](../app/qlib_rd_loop/quant.md#QuantRDLoop.direct_exp_gen), [`_exp_gen`](../components/workflow/rd_loop.md#RDLoop._exp_gen), [`hypothesis2experiment`](../app/kaggle/loop.md#KaggleRDLoop.hypothesis2experiment), [`LLMHypothesis2Experiment`](../components/proposal/__init__.md#LLMHypothesis2Experiment), [`factor_hypothesis2experiment`](../app/qlib_rd_loop/quant.md#QuantRDLoop.factor_hypothesis2experiment), [`model_hypothesis2experiment`](../app/qlib_rd_loop/quant.md#QuantRDLoop.model_hypothesis2experiment), [`hypothesis2experiment`](../components/workflow/rd_loop.md#RDLoop.hypothesis2experiment)

### `HypothesisFeedback`  ·  implements/extends ExperimentFeedback
- def: [`rdagent/core/proposal.py:96`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L96) — documented in [rdagent-app-CI-run](../../../concepts/rdagent-app-CI-run.md)
- signature: `class HypothesisFeedback(ExperimentFeedback):`
- members:
  - `acceptable` — [`L120`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L120)
  - `hypothesis_evaluation` — [`L118`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L118)
  - `new_hypothesis` — [`L119`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L119)
  - `observations` — [`L117`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L117)
- protocol/private: `__init__`[`L97`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L97), `__str__`[`L122`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L122)
- uses (calls/refs, reference-scoped): [`ExperimentFeedback`](proposal.md#ExperimentFeedback), [`__str__`](proposal.md#ExperimentFeedback.__str__), [`eda_improvement`](proposal.md#ExperimentFeedback.eda_improvement), [`__init__`](proposal.md#ExperimentFeedback.__init__)
- used by: [`_obj_to_json`](../log/ui/storage.md#WebStorage._obj_to_json), [`consume_msg`](../log/ui/web.md#SimpleTraceWindow.consume_msg), [`generate_feedback`](../scenarios/data_science/dev/feedback.md#DSExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/finetune/dev/feedback.md#FTExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/kaggle/developer/feedback.md#KGExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/qlib/developer/feedback.md#QlibFactorExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/qlib/developer/feedback.md#QlibModelExperiment2Feedback.generate_feedback), [`ExperimentFeedback`](proposal.md#ExperimentFeedback), [`feedback_window`](../log/ui/app.md#feedback_window), [`consume_msg`](../log/ui/web.md#FeedbackWindow.consume_msg), [`feedback`](../components/workflow/rd_loop.md#RDLoop.feedback), [`get_msgs_until`](../log/ui/app.md#get_msgs_until), [`consume_msg`](../log/ui/web.md#HypothesisFeedbackWindow.consume_msg), [`feedback`](../app/qlib_rd_loop/quant.md#QuantRDLoop.feedback), [`_gen_error_feedback`](../scenarios/rl/dev/feedback.md#RLExperiment2Feedback._gen_error_feedback), [`_gen_feedback_with_llm`](../scenarios/rl/dev/feedback.md#RLExperiment2Feedback._gen_feedback_with_llm), [`_interact_feedback`](../components/workflow/rd_loop.md#RDLoop._interact_feedback), [`generate_feedback`](../scenarios/rl/dev/feedback.md#RLExperiment2Feedback.generate_feedback)

### `HypothesisGen`  ·  implements/extends ABC
- def: [`rdagent/core/proposal.py:414`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L414)
- signature: `class HypothesisGen(ABC):`
- members:
  - `gen(self, trace: Trace, plan: ExperimentPlan | None = None)` — [`L420`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L420) — Motivation of the variable `scenario_desc`:
  - `scen` — [`L417`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L417)
- protocol/private: `__init__`[`L416`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L416)
- uses (calls/refs, reference-scoped): [`Scenario`](scenario.md#Scenario), [`Trace`](proposal.md#Trace), [`Hypothesis`](proposal.md#Hypothesis), [`gen`](../components/proposal/__init__.md#LLMHypothesisGen.gen), [`ExperimentPlan`](experiment.md#ExperimentPlan), [`LLMHypothesisGen`](../components/proposal/__init__.md#LLMHypothesisGen)
- used by: [`gen`](../components/proposal/__init__.md#LLMHypothesisGen.gen), [`prepare_context`](../scenarios/kaggle/proposal/proposal.md#KGHypothesisGen.prepare_context), [`_propose`](../components/workflow/rd_loop.md#RDLoop._propose), [`hypothesis_gen`](../app/kaggle/loop.md#KaggleRDLoop.hypothesis_gen), [`hypothesis_gen`](../app/qlib_rd_loop/quant.md#QuantRDLoop.hypothesis_gen), [`LLMHypothesisGen`](../components/proposal/__init__.md#LLMHypothesisGen), [`hypothesis_gen`](../components/workflow/rd_loop.md#RDLoop.hypothesis_gen), [`__init__`](../components/proposal/__init__.md#LLMHypothesisGen.__init__), [`update_reward_estimates`](../scenarios/kaggle/proposal/proposal.md#KGHypothesisGen.update_reward_estimates), [`execute_next_action`](../scenarios/kaggle/proposal/proposal.md#KGHypothesisGen.execute_next_action)

### `SOTAexpSelector`
- def: [`rdagent/core/proposal.py:343`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L343)
- doc: Select the SOTA experiment from the trace to submit
- signature: `class SOTAexpSelector:`
- members:
  - `get_sota_exp_to_submit(self, trace: Trace)` — [`L349`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L349) — Select the SOTA experiment from the trace to submit
- uses (calls/refs, reference-scoped): [`Experiment`](experiment.md#Experiment), [`Trace`](proposal.md#Trace), [`get_sota_exp_to_submit`](../scenarios/data_science/proposal/exp_gen/select/submit.md#AutoSOTAexpSelector.get_sota_exp_to_submit), [`get_sota_exp_to_submit`](../scenarios/data_science/proposal/exp_gen/select/submit.md#ValidationSelector.get_sota_exp_to_submit), [`get_sota_exp_to_submit`](../scenarios/data_science/proposal/exp_gen/select/submit.md#BestValidSelector.get_sota_exp_to_submit), [`BestValidSelector`](../scenarios/data_science/proposal/exp_gen/select/submit.md#BestValidSelector), [`get_sota_exp_to_submit`](../scenarios/data_science/proposal/exp_gen/select/submit.md#GlobalSOTASelector.get_sota_exp_to_submit), [`AutoSOTAexpSelector`](../scenarios/data_science/proposal/exp_gen/select/submit.md#AutoSOTAexpSelector), [`GlobalSOTASelector`](../scenarios/data_science/proposal/exp_gen/select/submit.md#GlobalSOTASelector), [`ValidationSelector`](../scenarios/data_science/proposal/exp_gen/select/submit.md#ValidationSelector)
- used by: [`BestValidSelector`](../scenarios/data_science/proposal/exp_gen/select/submit.md#BestValidSelector), [`AutoSOTAexpSelector`](../scenarios/data_science/proposal/exp_gen/select/submit.md#AutoSOTAexpSelector), [`GlobalSOTASelector`](../scenarios/data_science/proposal/exp_gen/select/submit.md#GlobalSOTASelector), [`ValidationSelector`](../scenarios/data_science/proposal/exp_gen/select/submit.md#ValidationSelector)

### `Trace`  ·  implements/extends Generic
- def: [`rdagent/core/proposal.py:141`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L141) — documented in [rdagent-core-proposal](../../../concepts/rdagent-core-proposal.md)
- signature: `class Trace(Generic[ASpecificScen, ASpecificKB]):`
- members:
  - `exp2idx(self, exp: Experiment | list[Experiment])` — [`L219`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L219)
  - `get_children(self, parent_idx: int | None = None)` — [`L286`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L286) — Get all children nodes for a given parent index.
  - `get_current_selection(self)` — [`L197`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L197)
  - `get_parent_exps(self, selection: tuple[int, ...] | None = None)` — [`L203`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L203) — Collect all ancestors of the given selection.
  - `get_parents(self, child_idx: int)` — [`L241`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L241)
  - `get_sota_experiment(self, node_id: int | None = None)` — [`L298`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L298) — Get the SOTA experiment from the trace by traversing ancestors backwards from node_id. — documented in [rdagent-core-proposal](../../../concepts/rdagent-core-proposal.md)
  - `get_sota_hypothesis_and_experiment(self)` — [`L178`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L178) — Access the last experiment result, sub-task, and the corresponding hypothesis.
  - `idx2exp(self, idx: int | list[int])` — [`L231`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L231)
  - `is_parent(self, parent_idx: int, child_idx: int)` — [`L237`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L237)
  - `is_selection_new_tree(self, selection: tuple[int, ...] | None = None)` — [`L187`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L187) — Check if the current trace is a new tree.
  - `set_current_selection(self, selection: tuple[int, ...])` — [`L200`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L200)
  - `sync_dag_parent_and_hist(self, exp_and_fb: NodeType, cur_loop_id: int)` — [`L256`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L256) — Adding corresponding parent index to the dag_parent when the hist is going to be changed. — documented in [rdagent-core-proposal](../../../concepts/rdagent-core-proposal.md)
  - `NEW_ROOT` — [`L143`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L143)
  - `NodeType` — [`L142`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L142)
  - `SEL_LATEST_SOTA` — [`L144`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L144)
  - `current_selection` — [`L176`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L176)
  - `dag_parent` — [`L153`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L153)
  - `hist` — [`L150`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L150) — documented in [rdagent-core-proposal](../../../concepts/rdagent-core-proposal.md)
  - `idx2loop_id` — [`L165`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L165)
  - `knowledge_base` — [`L173`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L173)
  - `scen` — [`L147`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L147)
- protocol/private: `__init__`[`L146`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L146)
- uses (calls/refs, reference-scoped): [`Experiment`](experiment.md#Experiment), [`Hypothesis`](proposal.md#Hypothesis), [`DSTrace`](../scenarios/data_science/proposal/exp_gen/base.md#DSTrace), [`hypothesis`](experiment.md#Experiment.hypothesis), [`ExperimentFeedback`](proposal.md#ExperimentFeedback), [`sync_dag_parent_and_hist`](../scenarios/data_science/proposal/exp_gen/base.md#DSTrace.sync_dag_parent_and_hist), [`decision`](proposal.md#ExperimentFeedback.decision), [`FTTrace`](../scenarios/finetune/proposal/trace.md#FTTrace), [`KGTrace`](../scenarios/kaggle/proposal/proposal.md#KGTrace), [`ASpecificKB`](proposal.md#ASpecificKB), [`ASpecificScen`](proposal.md#ASpecificScen), [`QuantTrace`](../scenarios/qlib/proposal/quant_proposal.md#QuantTrace)
- used by: [`record`](../scenarios/data_science/loop.md#DataScienceRDLoop.record), [`async_gen`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.async_gen), [`gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.gen), [`_gen_hypothesis`](../scenarios/finetune/proposal/proposal.md#LLMFinetuneExpGen._gen_hypothesis), [`hypothesis_select_with_llm`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_select_with_llm), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV2.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2Hypothesis.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV1ExpGen.gen), [`generate_feedback`](../scenarios/data_science/dev/feedback.md#DSExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/kaggle/developer/feedback.md#KGExperiment2Feedback.generate_feedback), [`gen`](../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftExpGen.gen), [`DSTrace`](../scenarios/data_science/proposal/exp_gen/base.md#DSTrace), [`direct_exp_gen`](../app/qlib_rd_loop/factor_from_report.md#FactorReportLoop.direct_exp_gen), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV3.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMerge.gen), [`generate_feedback`](../scenarios/qlib/developer/feedback.md#QlibFactorExperiment2Feedback.generate_feedback), [`generate_feedback`](../scenarios/qlib/developer/feedback.md#QlibModelExperiment2Feedback.generate_feedback), [`evaluate_one_trace`](../scenarios/data_science/proposal/exp_gen/select/submit.md#evaluate_one_trace), [`gen`](proposal.md#ExpGen.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftV2ExpGen.gen), [`interact`](../scenarios/data_science/interactor/__init__.md#DSInteractor.interact), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#MergeExpGen.gen), [`consume_msg`](../log/ui/web.md#TraceObjWindow.consume_msg), [`gen`](../scenarios/data_science/proposal/exp_gen/naive.md#NaiveExpGen.gen), [`feedback`](../scenarios/data_science/loop.md#DataScienceRDLoop.feedback), [`get_sota_exp_to_submit`](../scenarios/data_science/proposal/exp_gen/select/submit.md#AutoSOTAexpSelector.get_sota_exp_to_submit), [`generate_RAG_content`](../scenarios/kaggle/proposal/proposal.md#generate_RAG_content), [`select`](../scenarios/data_science/proposal/exp_gen/trace_scheduler.md#MCTSScheduler.select), [`convert_model_experiment`](../scenarios/kaggle/proposal/proposal.md#KGHypothesis2Experiment.convert_model_experiment), [`generate_feedback`](proposal.md#Experiment2Feedback.generate_feedback), [`get_sota_exp_to_submit`](../scenarios/data_science/proposal/exp_gen/select/submit.md#ValidationSelector.get_sota_exp_to_submit), [`observe_feedback`](../scenarios/data_science/proposal/exp_gen/trace_scheduler.md#MCTSScheduler.observe_feedback), [`convert`](../components/proposal/__init__.md#LLMHypothesis2Experiment.convert), [`gen`](../components/proposal/__init__.md#LLMHypothesisGen.gen), [`prepare_context`](../scenarios/qlib/proposal/model_proposal.md#QlibModelHypothesis2Experiment.prepare_context), [`convert_response`](../scenarios/kaggle/proposal/proposal.md#KGHypothesis2Experiment.convert_response), [`convert_response`](../scenarios/qlib/proposal/factor_proposal.md#QlibFactorHypothesis2Experiment.convert_response), [`prepare_context`](../scenarios/qlib/proposal/quant_proposal.md#QlibQuantHypothesisGen.prepare_context), [`collect_sota_candidates`](../scenarios/data_science/proposal/exp_gen/select/submit.md#BestValidSelector.collect_sota_candidates), [`current_action`](../scenarios/kaggle/proposal/proposal.md#KGHypothesis2Experiment.current_action)  (+64 more; 2 test-only)

## Module values
- `ASpecificKB` — [`L138`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L138)
- `ASpecificScen` — [`L137`](../../../../../../raw/code/rd-agent/rdagent/core/proposal.py#L137)


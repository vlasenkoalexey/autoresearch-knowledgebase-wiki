---
title: 'Module: rdagent/scenarios/data_science/proposal/exp_gen/base.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/proposal/exp_gen/base.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.proposal.exp_gen.base`/DS
symbols:
  DSTrace: Trace#
  DSTrace.hist: Trace#hist.
  DSHypothesis: Hypothesis#
  DSTrace.experiment_and_feedback_list_after_init: Trace#experiment_and_feedback_list_after_init().
  DSTrace.sota_experiment_fb: Trace#sota_experiment_fb().
  DSTrace.sync_dag_parent_and_hist: Trace#sync_dag_parent_and_hist().
  DSTrace.retrieve_search_list: Trace#retrieve_search_list().
  DSTrace.get_leaves: Trace#get_leaves().
  DSTrace.get_sibling_exps: Trace#get_sibling_exps().
  DSTrace.has_component: Trace#has_component().
  DSHypothesis.__str__: Hypothesis#__str__().
  DSTrace.sota_experiment: Trace#sota_experiment().
  DSTrace.should_inject_diversity: Trace#should_inject_diversity().
  DSTrace.next_incomplete_component: Trace#next_incomplete_component().
  DSTrace.sota_exp_to_submit: Trace#sota_exp_to_submit.
  DSHypothesis.component: Hypothesis#component.
  DSTrace.last_runnable_exp_fb: Trace#last_runnable_exp_fb().
  DSTrace.sub_trace_count: Trace#sub_trace_count().
  DSTrace.last_exp_fb: Trace#last_exp_fb().
  DSTrace.last_successful_exp: Trace#last_successful_exp().
  DSTrace.__init__: Trace#__init__().
  DSTrace.last_exp: Trace#last_exp().
  DSTrace.uncommitted_experiments: Trace#uncommitted_experiments.
  DSTrace.register_uncommitted_exp: Trace#register_uncommitted_exp().
  DSTrace.set_sota_exp_to_submit: Trace#set_sota_exp_to_submit().
  DSHypothesis.__init__: Hypothesis#__init__().
  DSTrace.deregister_uncommitted_exp: Trace#deregister_uncommitted_exp().
  DSHypothesis.problem_name: Hypothesis#problem_name.
  DSHypothesis.problem_desc: Hypothesis#problem_desc.
  DSHypothesis.appendix: Hypothesis#appendix.
  DSTrace.COMPLETE_ORDER: Trace#COMPLETE_ORDER.
  DSHypothesis.problem_label: Hypothesis#problem_label.
---
# Module: [`rdagent/scenarios/data_science/proposal/exp_gen/base.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py)

## Classes
### `DSHypothesis`  ·  implements/extends Hypothesis
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/base.py:13`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L13) — documented in [rdagent-log-ui-web](../../../../../../concepts/rdagent-log-ui-web.md)
- signature: `class DSHypothesis(Hypothesis):`
- members:
  - `appendix` — [`L35`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L35)
  - `component` — [`L31`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L31)
  - `problem_desc` — [`L33`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L33)
  - `problem_label` — [`L34`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L34)
  - `problem_name` — [`L32`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L32)
- protocol/private: `__init__`[`L14`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L14), `__str__`[`L37`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L37)
- uses (calls/refs, reference-scoped): [`Hypothesis`](../../../../core/proposal.md#Hypothesis), [`hypothesis`](../../../../core/proposal.md#Hypothesis.hypothesis), [`reason`](../../../../core/proposal.md#Hypothesis.reason), [`COMPONENT`](../../experiment/experiment.md#COMPONENT), [`__init__`](../../../../core/proposal.md#Hypothesis.__init__)
- used by: [`_obj_to_json`](../../../../log/ui/storage.md#WebStorage._obj_to_json), [`gen`](proposal.md#DSProposalV2ExpGen.gen), [`Hypothesis`](../../../../core/proposal.md#Hypothesis), [`task_gen`](proposal.md#DSProposalV2ExpGen.task_gen), [`gen`](draft/draft.md#DSDraftExpGen.gen), [`gen`](merge.md#MergeExpGen.gen), [`gen`](merge.md#MergeExpGen_MultiTrace.gen), [`task_gen`](draft/draft.md#DSDraftV2ExpGen.task_gen), [`gen`](naive.md#NaiveExpGen.gen), [`dump_and_wait_for_user_input`](../../interactor/__init__.md#FBDSInteractor.dump_and_wait_for_user_input), [`_prob_dis_torch`](proposal.md#DSProposalV2ExpGen._prob_dis_torch), [`has_component`](base.md#DSTrace.has_component), [`_f`](proposal.md#DSProposalV1ExpGen._f), [`hypothesis_gen`](draft/draft.md#DSDraftV2ExpGen.hypothesis_gen), [`dump_and_wait_for_user_input`](../../interactor/__init__.md#DSInteractor.dump_and_wait_for_user_input), [`hypothesis_rank`](proposal.md#DSProposalV2ExpGen.hypothesis_rank), [`get_all_hypotheses`](proposal.md#DSProposalV2ExpGen.get_all_hypotheses)

### `DSTrace`  ·  implements/extends Trace
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/base.py:55`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L55) — documented in [rdagent-core-proposal](../../../../../../concepts/rdagent-core-proposal.md)
- signature: `class DSTrace(Trace[DataScienceScen, KnowledgeBase]):`
- members:
  - `deregister_uncommitted_exp(self, loop_id: int)` — [`L84`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L84)
  - `experiment_and_feedback_list_after_init(self, return_type: Literal["sota", "failed", "all"], search_type: Literal["all", "ancestors"] = "ancestors", selection: tuple[int, ...] | None = None, max_retrieve_num: int | None = None)` — [`L221`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L221) — Retrieve a list of experiments and feedbacks based on the return_type. — documented in [rdagent-scenarios-data_science-proposal-exp_gen-base](../../../../../../concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
  - `get_leaves(self)` — [`L95`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L95) — Get the indices of nodes (in hist) that have no children—i.e., "leaves" of current DAG. — documented in [rdagent-scenarios-data_science-proposal-exp_gen-base](../../../../../../concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
  - `get_sibling_exps(self, current_selection: tuple[int, ...] | None = None)` — [`L114`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L114) — Get the sibling experiments of the current selection.
  - `has_component(self, component: COMPONENT, search_list: list[tuple[DSExperiment, ExperimentFeedback]] = [])` — [`L212`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L212) — documented in [rdagent-scenarios-data_science-proposal-exp_gen-base](../../../../../../concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
  - `last_exp(self, search_type: Literal["all", "ancestors"] = "ancestors")` — [`L312`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L312) — Access the last experiment
  - `last_exp_fb(self, search_type: Literal["all", "ancestors"] = "ancestors", selection: tuple[int, ...] | None = None)` — [`L323`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L323) — Access the last experiment and feedback
  - `last_runnable_exp_fb(self, search_type: Literal["all", "ancestors"] = "ancestors")` — [`L336`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L336) — Access the last runnable experiment (no exception, usually not all task failed) and feedback
  - `last_successful_exp(self, search_type: Literal["all", "ancestors"] = "ancestors", selection: tuple[int, ...] | None = None)` — [`L297`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L297) — Access the last successful experiment even part of the components are not completed.
  - `next_incomplete_component(self, search_type: Literal["all", "ancestors"] = "ancestors")` — [`L194`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L194) — NOTE:
  - `register_uncommitted_exp(self, exp: DSExperiment, loop_id: int)` — [`L81`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L81)
  - `retrieve_search_list(self, search_type: Literal["all", "ancestors"] = "ancestors", selection: tuple[int, ...] | None = None)` — [`L165`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L165) — Retrieve the search list based on the selection and search_type. — documented in [rdagent-scenarios-data_science-proposal-exp_gen-base](../../../../../../concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
  - `set_sota_exp_to_submit(self, exp: DSExperiment)` — [`L88`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L88)
  - `should_inject_diversity(self, current_selection: tuple[int, ...] | None = None)` — [`L66`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L66) — Check if diversity context should be injected based on the current selection.
  - `sota_experiment(self, search_type: Literal["all", "ancestors"] = "ancestors", selection: tuple[int, ...] | None = None)` — [`L287`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L287)
  - `sota_experiment_fb(self, search_type: Literal["all", "ancestors"] = "ancestors", selection: tuple[int, ...] | None = None)` — [`L267`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L267) — Returns
  - `sub_trace_count(self)` — [`L92`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L92)
  - `sync_dag_parent_and_hist(self, exp_and_fb: tuple[Experiment, ExperimentFeedback], cur_loop_id: int)` — [`L139`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L139) — Adding corresponding parent index to the dag_parent when the hist is going to be changed. — documented in [rdagent-scenarios-data_science-proposal-exp_gen-base](../../../../../../concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
  - `COMPLETE_ORDER` — [`L79`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L79)
  - `hist` — [`L60`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L60) — documented in [rdagent-scenarios-data_science-proposal-exp_gen-base](../../../../../../concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
  - `sota_exp_to_submit` — [`L62`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L62)
  - `uncommitted_experiments` — [`L64`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L64)
- protocol/private: `__init__`[`L56`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/base.py#L56)
- uses (calls/refs, reference-scoped): [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`Experiment`](../../../../core/experiment.md#Experiment), [`DSExperiment`](../../experiment/experiment.md#DSExperiment), [`Trace`](../../../../core/proposal.md#Trace), [`import_class`](../../../../core/utils.md#import_class), [`hypothesis`](../../../../core/experiment.md#Experiment.hypothesis), [`ExperimentFeedback`](../../../../core/proposal.md#ExperimentFeedback), [`DSHypothesis`](base.md#DSHypothesis), [`NEW_ROOT`](../../../../core/proposal.md#Trace.NEW_ROOT), [`KnowledgeBase`](../../../../core/knowledge_base.md#KnowledgeBase), [`DataScienceScen`](../../scen/__init__.md#DataScienceScen), [`decision`](../../../../core/proposal.md#ExperimentFeedback.decision), [`get_parent_exps`](../../../../core/proposal.md#Trace.get_parent_exps), [`dag_parent`](../../../../core/proposal.md#Trace.dag_parent), [`coder_on_whole_pipeline`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.coder_on_whole_pipeline), [`component`](base.md#DSHypothesis.component), [`local_selection`](../../../../core/experiment.md#Experiment.local_selection), [`current_selection`](../../../../core/proposal.md#Trace.current_selection), [`get_current_selection`](../../../../core/proposal.md#Trace.get_current_selection), [`__init__`](../../../../core/proposal.md#Trace.__init__), [`COMPONENT`](../../experiment/experiment.md#COMPONENT), [`idx2loop_id`](../../../../core/proposal.md#Trace.idx2loop_id), [`exception`](../../../../core/proposal.md#ExperimentFeedback.exception), [`enable_cross_trace_diversity`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.enable_cross_trace_diversity), [`diversity_injection_strategy`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.diversity_injection_strategy)
- used by: [`record`](../../loop.md#DataScienceRDLoop.record), [`async_gen`](router/__init__.md#ParallelMultiTraceExpGen.async_gen), [`gen`](proposal.md#DSProposalV2ExpGen.gen), [`Trace`](../../../../core/proposal.md#Trace), [`hypothesis_select_with_llm`](proposal.md#DSProposalV2ExpGen.hypothesis_select_with_llm), [`gen`](merge.md#ExpGen2TraceAndMergeV2.gen), [`gen`](merge.md#ExpGen2Hypothesis.gen), [`gen`](proposal.md#DSProposalV1ExpGen.gen), [`generate_feedback`](../../dev/feedback.md#DSExperiment2Feedback.generate_feedback), [`gen`](draft/draft.md#DSDraftExpGen.gen), [`gen`](merge.md#ExpGen2TraceAndMergeV3.gen), [`trace`](../../loop.md#DataScienceRDLoop.trace), [`gen`](merge.md#ExpGen2TraceAndMerge.gen), [`gen`](draft/draft.md#DSDraftV2ExpGen.gen), [`interact`](../../interactor/__init__.md#DSInteractor.interact), [`gen`](merge.md#MergeExpGen.gen), [`gen`](merge.md#MergeExpGen_MultiTrace.gen), [`gen`](naive.md#NaiveExpGen.gen), [`feedback`](../../loop.md#DataScienceRDLoop.feedback), [`select`](trace_scheduler.md#MCTSScheduler.select), [`observe_feedback`](trace_scheduler.md#MCTSScheduler.observe_feedback), [`plan`](planner/__init__.md#DSExpPlannerHandCraft.plan), [`select`](trace_scheduler.md#ProbabilisticScheduler.select), [`sync_dag_parent_and_hist`](../../../../core/proposal.md#Trace.sync_dag_parent_and_hist), [`next`](trace_scheduler.md#BaseScheduler.next), [`get_exp_index`](merge.md#ExpGen2Hypothesis.get_exp_index), [`select`](trace_scheduler.md#RoundRobinScheduler.select), [`draft_exp_in_decomposition`](proposal.md#draft_exp_in_decomposition), [`calculate_potential`](trace_scheduler.md#SOTABasedScheduler.calculate_potential), [`process_uncommitted_nodes`](trace_scheduler.md#MCTSScheduler.process_uncommitted_nodes), [`calculate_potential`](trace_scheduler.md#ProbabilisticScheduler.calculate_potential), [`_llm_select_extra_hypo`](proposal.md#DSProposalV2ExpGen._llm_select_extra_hypo), [`should_inject`](diversity_strategy.md#DiversityContextStrategy.should_inject), [`select`](trace_scheduler.md#BaseScheduler.select), [`calculate_potential`](trace_scheduler.md#TraceLengthScheduler.calculate_potential), [`gen`](router/__init__.md#ParallelMultiTraceExpGen.gen), [`should_inject`](diversity_strategy.md#InjectUntilSOTAGainedStrategy.should_inject), [`next`](trace_scheduler.md#TraceScheduler.next), [`process_uncommitted_nodes`](trace_scheduler.md#BaseScheduler.process_uncommitted_nodes), [`should_inject`](diversity_strategy.md#InjectAtRootStrategy.should_inject)  (+2 more)


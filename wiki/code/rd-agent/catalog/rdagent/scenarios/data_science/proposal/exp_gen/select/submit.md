---
title: 'Module: rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.proposal.exp_gen.select.submit`/
symbols:
  ValidationSelector._generate_and_run_script: ValidationSelector#_generate_and_run_script().
  evaluate_one_trace: evaluate_one_trace().
  ValidationSelector._prepare_validation_scripts: ValidationSelector#_prepare_validation_scripts().
  process_experiment: process_experiment().
  AutoSOTAexpSelector.get_sota_exp_to_submit: AutoSOTAexpSelector#get_sota_exp_to_submit().
  ValidationSelector.get_sota_exp_to_submit: ValidationSelector#get_sota_exp_to_submit().
  BestValidSelector.collect_sota_candidates: BestValidSelector#collect_sota_candidates().
  select_on_existing_trace: select_on_existing_trace().
  BestValidSelector.get_sort_key: BestValidSelector#get_sort_key().
  check_hit: check_hit().
  try_get_loop_id: try_get_loop_id().
  AutoSOTAexpSelector.collect_sota_candidates: AutoSOTAexpSelector#collect_sota_candidates().
  BestValidSelector.get_sota_exp_to_submit: BestValidSelector#get_sota_exp_to_submit().
  BestValidSelector.get_sort_key_without_decision: BestValidSelector#get_sort_key_without_decision().
  ValidationSelector.hypothesis_loop_id: ValidationSelector#hypothesis_loop_id.
  BestValidSelector: BestValidSelector#
  ValidationSelector.hypothesis_exp: ValidationSelector#hypothesis_exp.
  GlobalSOTASelector.get_sota_exp_to_submit: GlobalSOTASelector#get_sota_exp_to_submit().
  ValidationSelector.candidate: ValidationSelector#candidate.
  GlobalSOTASelector: GlobalSOTASelector#
  AutoSOTAexpSelector: AutoSOTAexpSelector#
  ValidationSelector: ValidationSelector#
  MAX_API_RETRIES: MAX_API_RETRIES.
  ValidationSelector.competition: ValidationSelector#competition.
  ValidationSelector.sample_code_path: ValidationSelector#sample_code_path.
  ValidationSelector.sample_rate: ValidationSelector#sample_rate.
  ValidationSelector.__init__: ValidationSelector#__init__().
  BestValidSelector.num_candidates: BestValidSelector#num_candidates.
  ValidationSelector.print_code: ValidationSelector#print_code().
  _parsing_score: _parsing_score().
  DEFAULT_NUM_WORKERS: DEFAULT_NUM_WORKERS.
  MAX_SOTA_CANDIDATES: MAX_SOTA_CANDIDATES.
  BestValidSelector.use_decision: BestValidSelector#use_decision.
  BestValidSelector.each_trace: BestValidSelector#each_trace.
  ValidationSelector.direction_sign: ValidationSelector#direction_sign.
  extract_tar: extract_tar().
  GlobalSOTASelector.__init__: GlobalSOTASelector#__init__().
  AutoSOTAexpSelector.__init__: AutoSOTAexpSelector#__init__().
  BestValidSelector.__init__: BestValidSelector#__init__().
  ValidationSelector.only_sample: ValidationSelector#only_sample.
---
# Module: [`rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py)

## Classes
### `AutoSOTAexpSelector`  ·  implements/extends SOTAexpSelector
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py:58`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L58)
- doc: Uses an LLM to select the best SOTA experiment from a list of candidates.
- signature: `class AutoSOTAexpSelector(SOTAexpSelector):`
- members:
  - `collect_sota_candidates(self, trace: Trace)` — [`L130`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L130) — Helper to gather SOTA experiments from trace leaves.
  - `get_sota_exp_to_submit(self, trace: Trace, **kwargs)` — [`L68`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L68) — Retrieves SOTA experiments, then uses an LLM to choose the most promising one. — documented in [rdagent-oai-backend-base](../../../../../../../concepts/rdagent-oai-backend-base.md)
- protocol/private: `__init__`[`L64`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L64)
- uses (calls/refs, reference-scoped): [`T`](../../../../../utils/agent/tpl.md#T), [`r`](../../../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../../../app/data_science/conf.md#DS_RD_SETTING), [`APIBackend`](../../../../../oai/llm_utils.md#APIBackend), [`LLM_SETTINGS`](../../../../../oai/llm_conf.md#LLM_SETTINGS), [`DSExperiment`](../../../experiment/experiment.md#DSExperiment), [`Trace`](../../../../../core/proposal.md#Trace), [`build_messages_and_create_chat_completion`](../../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`scen`](../../../../../core/proposal.md#Trace.scen), [`wait_retry`](../../../../../utils/workflow/misc.md#wait_retry), [`build_messages_and_calculate_token`](../../../../../oai/backend/base.md#APIBackend.build_messages_and_calculate_token), [`SOTAexpSelector`](../../../../../core/proposal.md#SOTAexpSelector), [`max_sota_retrieved_num`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.max_sota_retrieved_num), [`MAX_API_RETRIES`](submit.md#MAX_API_RETRIES), [`chat_token_limit`](../../../../../oai/llm_conf.md#LLMSettings.chat_token_limit)
- used by: [`evaluate_one_trace`](submit.md#evaluate_one_trace), [`SOTAexpSelector`](../../../../../core/proposal.md#SOTAexpSelector), [`get_sota_exp_to_submit`](../../../../../core/proposal.md#SOTAexpSelector.get_sota_exp_to_submit)

### `BestValidSelector`  ·  implements/extends SOTAexpSelector
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py:158`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L158)
- doc: Selects the top N experiments based on their performance score.
- signature: `class BestValidSelector(SOTAexpSelector):`
- members:
  - `__init__(self, num_candidates: int = 1, use_decision: bool = True, each_trace: bool = False)` — [`L164`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L164) — Args:
  - `collect_sota_candidates(self, trace: Trace)` — [`L187`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L187) — Helper to gather SOTA experiments from trace leaves.
  - `get_sort_key(exp_fb: Tuple[DSExperiment, ExperimentFeedback])` — [`L194`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L194)
  - `get_sort_key_without_decision(exp_fb: Tuple[DSExperiment, ExperimentFeedback])` — [`L209`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L209)
  - `get_sota_exp_to_submit(self, trace: Trace, **kwargs)` — [`L178`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L178) — Sorts all valid experiments by score and returns the top N.
  - `each_trace` — [`L176`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L176)
  - `num_candidates` — [`L174`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L174)
  - `use_decision` — [`L175`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L175)
- uses (calls/refs, reference-scoped): [`hist`](../../../../../core/proposal.md#Trace.hist), [`DSExperiment`](../../../experiment/experiment.md#DSExperiment), [`Trace`](../../../../../core/proposal.md#Trace), [`result`](../../../../../core/experiment.md#Experiment.result), [`ExperimentFeedback`](../../../../../core/proposal.md#ExperimentFeedback), [`scen`](../../../../../core/proposal.md#Trace.scen), [`decision`](../../../../../core/proposal.md#ExperimentFeedback.decision), [`SOTAexpSelector`](../../../../../core/proposal.md#SOTAexpSelector), [`get_parents`](../../../../../core/proposal.md#Trace.get_parents)
- used by: [`evaluate_one_trace`](submit.md#evaluate_one_trace), [`get_sota_exp_stat`](../../../../../log/ui/utils.md#get_sota_exp_stat), [`SOTAexpSelector`](../../../../../core/proposal.md#SOTAexpSelector), [`get_sota_exp_to_submit`](../../../../../core/proposal.md#SOTAexpSelector.get_sota_exp_to_submit)

### `GlobalSOTASelector`  ·  implements/extends SOTAexpSelector
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py:43`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L43)
- doc: Selects the single best State-Of-The-Art (SOTA) experiment from the entire trace history.
- signature: `class GlobalSOTASelector(SOTAexpSelector):`
- members:
  - `get_sota_exp_to_submit(self, trace: Trace, **kwargs)` — [`L51`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L51) — Returns the single best experiment from all historical runs.
- protocol/private: `__init__`[`L48`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L48)
- uses (calls/refs, reference-scoped): [`DSExperiment`](../../../experiment/experiment.md#DSExperiment), [`Trace`](../../../../../core/proposal.md#Trace), [`SOTAexpSelector`](../../../../../core/proposal.md#SOTAexpSelector)
- used by: [`evaluate_one_trace`](submit.md#evaluate_one_trace), [`SOTAexpSelector`](../../../../../core/proposal.md#SOTAexpSelector), [`get_sota_exp_to_submit`](../../../../../core/proposal.md#SOTAexpSelector.get_sota_exp_to_submit)

### `ValidationSelector`  ·  implements/extends SOTAexpSelector
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py:263`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L263)
- doc: A meta-selector that re-validates candidates from a base selector.
- signature: `class ValidationSelector(SOTAexpSelector):`
- members:
  - `_generate_and_run_script(self, script_type: str, prompt_template_key: str, reference_exp: DSExperiment, competition: str, mock_folder: str, prompt_kwargs: dict)` — [`L429`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L429) — A helper to generate, run, and validate a script (data.py or grade.py).
  - `_prepare_validation_scripts(self, reference_exp: DSExperiment, competition: str, mock_folder: str)` — [`L353`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L353) — Generates and verifies data.py and grade.py using an LLM. — documented in [rdagent-app-data_science-conf](../../../../../../../concepts/rdagent-app-data_science-conf.md)
  - `get_sota_exp_to_submit(self, trace: Trace)` — [`L289`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L289) — Helper to gather SOTA experiments from trace leaves.
  - `print_code(self, data_py_code: str, grade_py_code: str)` — [`L345`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L345)
  - `candidate` — [`L280`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L280)
  - `competition` — [`L282`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L282)
  - `direction_sign` — [`L281`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L281)
  - `hypothesis_exp` — [`L287`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L287)
  - `hypothesis_loop_id` — [`L286`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L286)
  - `only_sample` — [`L283`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L283)
  - `sample_code_path` — [`L284`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L284)
  - `sample_rate` — [`L285`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L285)
- protocol/private: `__init__`[`L271`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L271)
- uses (calls/refs, reference-scoped): [`T`](../../../../../utils/agent/tpl.md#T), [`r`](../../../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../../../app/data_science/conf.md#DS_RD_SETTING), [`APIBackend`](../../../../../oai/llm_utils.md#APIBackend), [`FBWorkspace`](../../../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../../../core/experiment.md#Experiment.experiment_workspace), [`DSExperiment`](../../../experiment/experiment.md#DSExperiment), [`workspace_path`](../../../../../core/experiment.md#FBWorkspace.workspace_path), [`Trace`](../../../../../core/proposal.md#Trace), [`build_messages_and_create_chat_completion`](../../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`get_ds_env`](../../../../../components/coder/data_science/conf.md#get_ds_env), [`inject_files`](../../../../../core/experiment.md#FBWorkspace.inject_files), [`hypothesis`](../../../../../core/experiment.md#Experiment.hypothesis), [`exit_code`](../../../../../utils/env.md#EnvResult.exit_code), [`stdout`](../../../../../utils/env.md#EnvResult.stdout), [`process_experiment`](submit.md#process_experiment), [`run`](../../../../../core/experiment.md#FBWorkspace.run), [`multiprocessing_wrapper`](../../../../../core/utils.md#multiprocessing_wrapper), [`hypothesis`](../../../../../core/proposal.md#Hypothesis.hypothesis), [`local_data_path`](../../../../../app/kaggle/conf.md#KaggleBasePropSetting.local_data_path), [`PythonAgentOut`](../../../../../utils/agent/ret.md#PythonAgentOut), [`SOTAexpSelector`](../../../../../core/proposal.md#SOTAexpSelector), [`inject_code_from_file_dict`](../../../../../core/experiment.md#FBWorkspace.inject_code_from_file_dict), [`extract_output`](../../../../../utils/agent/ret.md#PythonAgentOut.extract_output), [`full_timeout`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.full_timeout), [`shrink_text`](../../../../../utils/fmt.md#shrink_text), [`MAX_API_RETRIES`](submit.md#MAX_API_RETRIES), [`_parsing_score`](submit.md#_parsing_score), [`DEFAULT_NUM_WORKERS`](submit.md#DEFAULT_NUM_WORKERS)
- used by: [`evaluate_one_trace`](submit.md#evaluate_one_trace), [`SOTAexpSelector`](../../../../../core/proposal.md#SOTAexpSelector), [`get_sota_exp_to_submit`](../../../../../core/proposal.md#SOTAexpSelector.get_sota_exp_to_submit)

## Functions
- `_parsing_score(grade_stdout: str)` — [`L575`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L575)
- `check_hit(selected_exp: DSExperiment, trace: Trace, sota_result: Dict[str, Any])` — [`L602`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L602) — Checks if any of the selected experiments are considered medal-winning.
- `evaluate_one_trace(selector_name: str, trace: Trace, debug: bool, only_sample: bool, sample_code_path: str, sota_result: dict[str, Any] = {}, experiment: str = "validation", log_path: Path | None = None, sample_rate: float = 0.8)` — [`L639`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L639) — Loads a single trace, uses the specified selector to pick an experiment, — documented in [rdagent-app-data_science-conf](../../../../../../../concepts/rdagent-app-data_science-conf.md)
- `extract_tar(tar_path: str, to_dir: str = "log")` — [`L629`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L629)
- `process_experiment(exp: DSExperiment, competition: str, folder: str, grade_py_code: str, loop_id: str)` — [`L521`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L521) — Worker function to process a single experiment in an isolated directory. — documented in [rdagent-app-data_science-conf](../../../../../../../concepts/rdagent-app-data_science-conf.md)
- `select_on_existing_trace(selector_name: str, trace_root: str = "", experiment: str | None = None, competition: str | None = None, debug: bool = False, only_sample: bool = False, sample_code_path: str = "", sample_rate: float = 0.8)` — [`L744`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L744) — Offline evaluation of a SOTA experiment selector on existing traces.
- `try_get_loop_id(trace: Trace, exp: DSExperiment)` — [`L622`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L622)

## Module values
- `DEFAULT_NUM_WORKERS` — [`L34`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L34)
- `MAX_API_RETRIES` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L33)
- `MAX_SOTA_CANDIDATES` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/select/submit.py#L35)


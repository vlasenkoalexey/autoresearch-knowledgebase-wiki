---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.analysis_utils.meta_data_wrangling`/
symbols:
  _load_experiment_data: _load_experiment_data().
  format_experiment_data: format_experiment_data().
  metaexp2ids: metaexp2ids().
  get_submitit_logs2exp_mapping: get_submitit_logs2exp_mapping().
  prepare_meta_exp_slurm_dataframe: prepare_meta_exp_slurm_dataframe().
  analyze_slurm_meta_exp: analyze_slurm_meta_exp().
  collect_all_meta_experiments_in_one_df: collect_all_meta_experiments_in_one_df().
  filter_dataframe_based_on_data_validity: filter_dataframe_based_on_data_validity().
  get_competition_id_from_cmd: get_competition_id_from_cmd().
  link_jobs_to_experiments: link_jobs_to_experiments().
  process_all_meta_experiments: process_all_meta_experiments().
  get_metric: get_metric().
  get_seed_from_cmd: get_seed_from_cmd().
  truncate_dataframe_based_on_elapsed: truncate_dataframe_based_on_elapsed().
  _get_job_data: _get_job_data().
  get_exp_name_from_cmd: get_exp_name_from_cmd().
  gather_all_meta_experiment_data: gather_all_meta_experiment_data().
  filter_dataframe_to_have_limited_nodes: filter_dataframe_to_have_limited_nodes().
  get_statistics: get_statistics().
  _is_sequence_like: _is_sequence_like().
  render_output_paths: render_output_paths().
  get_slurm_data: get_slurm_data().
  analyze_failures: analyze_failures().
  analyze_all_slurm_meta_exps: analyze_all_slurm_meta_exps().
  process_experiment_folder_journal_log: process_experiment_folder_journal_log().
  _truncate_to_max: _truncate_to_max().
  _slice_to_len: _slice_to_len().
  get_expected_return_node: get_expected_return_node().
  get_selection_mask: get_selection_mask().
  get_rank_and_percentile: get_rank_and_percentile().
  filter_dataframe_based_on_node_to_node_elapsed: filter_dataframe_based_on_node_to_node_elapsed().
  add_node_elapsed_from_first: add_node_elapsed_from_first().
  render_output_paths.has_valid_pattern: render_output_paths().has_valid_pattern().
  is_lower_better: is_lower_better().
  run_bash_command: run_bash_command().
  get_submitit_stdout_stderr_paths: get_submitit_stdout_stderr_paths().
  try_get_clean_err_messsage: try_get_clean_err_messsage().
  print_failure_summary: print_failure_summary().
  print_detailed_failures: print_detailed_failures().
  load_method_name: load_method_name().
  build_dataframe_one_row_per_experiment: build_dataframe_one_row_per_experiment().
  filter_dataframe_based_on_node_to_node_elapsed.get_timestamp_diff: filter_dataframe_based_on_node_to_node_elapsed().get_timestamp_diff().
  _sentinel: _sentinel().
  add_node_elapsed_from_first._row_elapsed: add_node_elapsed_from_first()._row_elapsed().
  truncate_dataframe_based_on_elapsed._new_len: truncate_dataframe_based_on_elapsed()._new_len().
  get_valid_submission: get_valid_submission().
  extract_path: extract_path().
  load_competition_id: load_competition_id().
  load_seed: load_seed().
  filter_dataframe_based_on_slurm: filter_dataframe_based_on_slurm().
  filter_dataframe_based_on_slurm_elapsed: filter_dataframe_based_on_slurm_elapsed().
  parse_into_aggregate_dict: parse_into_aggregate_dict().
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py)

## Functions
- `_get_job_data(job_ids: List[str])` — [`L111`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L111) — Get job data from Slurm for specified job IDs.
- `_is_sequence_like(x: Any)` — [`L1292`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1292) — True for list / np.ndarray / pd.Series; False otherwise.
- `_load_experiment_data(meta_path: Path, experiment_folder: Path, path_to_method_name: Dict[str, str])` — [`L746`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L746) — Loads data for a single experiment folder in parallel:
- `_new_len(elapsed_seq: Sequence[Any])` — [`L1488`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1488) — Return the number of nodes to keep so that every retained
- `_row_elapsed(row)` — [`L1390`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1390)
- `_sentinel(lower_is_better: bool)` — [`L1164`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1164) — Returns a numeric sentinel:  +1e12   if lower scores are better,
- `_slice_to_len(seq: Any, new_len: int)` — [`L1417`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1417) — Return *seq* sliced to ``new_len`` while preserving its type.
- `_truncate_to_max(seq: Any, max_len: int)` — [`L1297`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1297) — Return `seq` truncated to the first `max_len` elements if needed.
- `add_node_elapsed_from_first(df: pd.DataFrame, *, output_col: str = "seconds_from_first_node", unit: str = "seconds")` — [`L1357`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1357) — For every row, compute how much time has elapsed between each node’s
- `analyze_all_slurm_meta_exps(meta_experiment_paths: List[Union[str, Path]])` — [`L647`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L647) — Analyze multiple meta-experiments based on slurm.
- `analyze_failures(df_clean: pd.DataFrame, mexp_dir: Union[str, Path], std_err_k: int = 300, std_out_k: int = 50)` — [`L497`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L497) — Analyze failures in the meta-experiment.
- `analyze_slurm_meta_exp(metaexp_dir: Union[str, Path], show_failures: bool = True, show_std_err: bool = True, show_std_out: bool = False)` — [`L612`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L612) — Analyze a meta-experiment.
- `build_dataframe_one_row_per_experiment(all_experiments: List[dict], all_keys: set, max_steps: int)` — [`L918`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L918) — Given:
- `collect_all_meta_experiments_in_one_df(meta_experiment_paths: List[Union[str, Path]], path_to_method_name: dict, max_steps_cap: int = 500, regenerate_trees: bool = False, seconds_cutoff: float = None, max_processes: int | None = None)` — [`L981`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L981) — Performs Phase A: Processing meta experiments to generate trees.
- `extract_path(file_path: Path)` — [`L223`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L223) — Extract output directory path from a log file.
- `filter_dataframe_based_on_data_validity(df: pd.DataFrame, min_length: int = 5)` — [`L1173`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1173) — Ensures that every (competition, method, seed) group contains at least one valid node.
- `filter_dataframe_based_on_node_to_node_elapsed(df: pd.DataFrame, elapsed_time: str = "0-23:00:00", *, length_cutoff: int | None = None, show_filtered_times: bool = True, max_examples: int = 5)` — [`L1042`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1042) — Drops rows whose first node to last node duration < `elapsed_time`.
- `filter_dataframe_based_on_slurm(df: pd.DataFrame)` — [`L1018`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1018)
- `filter_dataframe_based_on_slurm_elapsed(df: pd.DataFrame, elapsed_time: str = "0-23:00:00", *, length_cutoff: int | None = None, show_filtered_times: bool = True, max_examples: int = 5)` — [`L1100`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1100) — • Drops rows where 'method' is NaN.
- `filter_dataframe_to_have_limited_nodes(df: pd.DataFrame, max_num_nodes: int)` — [`L1310`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1310) — Truncates every *sequence‑like* column so that each row contains
- `format_experiment_data(experiments_df: pd.DataFrame, max_num_seeds: int = 20, select_using_test: bool = False, node_selector_function: Optional[Callable] = None)` — [`L1709`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1709) — Take in the dataframe containing experiment data per row and convert it into competition reports.
- `gather_all_meta_experiment_data(meta_experiment_paths: List[Union[str, Path]], path_to_method_name: dict, max_steps_cap: int = 500, max_processes: int | None = None)` — [`L843`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L843) — Phase B: Iterates through each meta experiment folder and each experiment inside,
- `get_competition_id_from_cmd(cmd: RunConfig)` — [`L292`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L292) — Extract competition ID from a command string.
- `get_exp_name_from_cmd(cmd: RunConfig)` — [`L275`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L275) — Extract experiment name from a command string.
- `get_expected_return_node(row, lower_is_better: bool, use_validation_score: bool = True)` — [`L1558`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1558) — Process the validation metric data to see what node the search would have returned.
- `get_metric(row, metric_key, valid_submission, expected_return_node, lower_is_better)` — [`L1589`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1589)
- `get_rank_and_percentile(score: float, leaderboard: pd.DataFrame, lower_is_better: bool)` — [`L1617`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1617) — Calculates the percentile rank of `score` as if it were an additional submission in the leaderboard.
- `get_seed_from_cmd(cmd: RunConfig)` — [`L309`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L309) — Extract seed from a command string.
- `get_selection_mask(row)` — [`L1533`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1533) — Get the mask of nodes that could be selected.
- `get_slurm_data(job_ids: Union[str, List[str]], k: int = 10)` — [`L199`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L199) — Get comprehensive job data from Slurm for the specified job IDs.
- `get_statistics(x, label)` — [`L1693`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1693)
- `get_submitit_logs2exp_mapping(mexp_dir: Union[str, Path])` — [`L257`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L257) — Map submitit job IDs to experiment directories.
- `get_submitit_stdout_stderr_paths(mexp_dir: Union[str, Path], job_id: str)` — [`L326`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L326) — Get paths to stdout and stderr files for a job.
- `get_timestamp_diff(row)` — [`L1061`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1061)
- `get_valid_submission(row, node_idx)` — [`L1553`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1553) — Simply check if a node has a valid submission csv.
- `has_valid_pattern(pat)` — [`L90`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L90)
- `is_lower_better(competition)` — [`L1682`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1682)
- `link_jobs_to_experiments(mexp_dir: Union[str, Path])` — [`L354`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L354) — Link Slurm jobs to experiment directories and extract relevant information.
- `load_competition_id(config_file: Union[str, Path])` — [`L719`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L719) — Reads the .hydra/config.yaml file and returns the competition_id
- `load_method_name(meta_experiment_path: Path, path_to_method_name: Dict[str, str])` — [`L738`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L738) — Returns the method name for a given meta_experiment_path
- `load_seed(config_file: Union[str, Path])` — [`L729`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L729) — Reads the .hydra/config.yaml file and returns the seed of the experiment.
- `metaexp2ids(metaexp_path: Path)` — [`L40`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L40) — Extract job IDs from a meta-experiment directory.
- `parse_into_aggregate_dict(report_df, metric, algorithms=None)` — [`L1859`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1859)
- `prepare_meta_exp_slurm_dataframe(metaexp_dir: Union[str, Path])` — [`L426`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L426) — Prepare a DataFrame with meta-experiment data.
- `print_detailed_failures(df_with_logs: pd.DataFrame, show_std_err: bool = True, show_std_out: bool = False)` — [`L565`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L565) — Print detailed information about failed jobs.
- `print_failure_summary(df_with_logs: pd.DataFrame)` — [`L554`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L554) — Print a summary of failures in the meta-experiment.
- `process_all_meta_experiments(meta_experiment_paths: List[Path], regenerate_trees: bool, max_processes: int | None = None, seconds_cutoff: float = None)` — [`L797`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L797) — Phase A:
- `process_experiment_folder_journal_log(experiment_path: Path, regenerate_tree: bool, seconds_cutoff: float = None)` — [`L699`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L699) — Processes a single experiment folder:
- `render_output_paths(job: Dict[str, Any])` — [`L79`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L79) — Render the output paths for stdout and stderr based on job data.
- `run_bash_command(command: str)` — [`L59`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L59) — Run a bash command and return the output.
- `truncate_dataframe_based_on_elapsed(df: pd.DataFrame, max_elapsed: str | int | float | pd.Timedelta, *, elapsed_col: str = "seconds_from_first_node")` — [`L1428`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L1428) — Remove every node that lies *after* ``max_elapsed`` from the first node.
- `try_get_clean_err_messsage(err_file: Path, k: int)` — [`L391`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_data_wrangling.py#L391) — Extract a clean error message from stderr logs.


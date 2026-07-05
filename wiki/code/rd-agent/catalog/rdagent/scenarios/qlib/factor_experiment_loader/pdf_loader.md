---
title: 'Module: rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.qlib.factor_experiment_loader.pdf_loader`/
symbols:
  FactorExperimentLoaderFromPDFfiles.load: FactorExperimentLoaderFromPDFfiles#load().
  __deduplicate_factor_dict: __deduplicate_factor_dict().
  classify_report_from_dict: classify_report_from_dict().
  extract_factors_from_report_dict: extract_factors_from_report_dict().
  __check_factor_duplication_simulate_json_mode: __check_factor_duplication_simulate_json_mode().
  __extract_factors_name_and_desc_from_content: __extract_factors_name_and_desc_from_content().
  __extract_factors_formulation_from_content: __extract_factors_formulation_from_content().
  __check_factor_dict_relevance: __check_factor_dict_relevance().
  __check_factor_dict_viability_simulate_json_mode: __check_factor_dict_viability_simulate_json_mode().
  check_factor_viability: check_factor_viability().
  check_factor_relevance: check_factor_relevance().
  deduplicate_factors_by_llm: deduplicate_factors_by_llm().
  __extract_factor_and_formulation_from_one_report: __extract_factor_and_formulation_from_one_report().
  FactorExperimentLoaderFromPDFfiles: FactorExperimentLoaderFromPDFfiles#
  __kmeans_embeddings: __kmeans_embeddings().
  __kmeans_embeddings.find_closest_cluster_cosine_similarity: __kmeans_embeddings().find_closest_cluster_cosine_similarity().
  merge_file_to_factor_dict_to_factor_dict: merge_file_to_factor_dict_to_factor_dict().
---
# Module: [`rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py)

## Classes
### `FactorExperimentLoaderFromPDFfiles`  ·  implements/extends FactorExperimentLoader
- def: [`rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py:567`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L567)
- signature: `class FactorExperimentLoaderFromPDFfiles(FactorExperimentLoader):`
- members:
  - `load(self, file_or_folder_path: str)` — [`L568`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L568)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`log_object`](../../../log/logger.md#RDAgentLog.log_object), [`QlibFactorExperiment`](../experiment/factor_experiment.md#QlibFactorExperiment), [`FactorExperimentLoader`](../../../components/loader/experiment_loader.md#FactorExperimentLoader), [`classify_report_from_dict`](pdf_loader.md#classify_report_from_dict), [`extract_factors_from_report_dict`](pdf_loader.md#extract_factors_from_report_dict), [`check_factor_viability`](pdf_loader.md#check_factor_viability), [`load_and_process_pdfs_by_langchain`](../../../components/document_reader/document_reader.md#load_and_process_pdfs_by_langchain), [`tag`](../../../log/logger.md#RDAgentLog.tag), [`load`](json_loader.md#FactorExperimentLoaderFromDict.load), [`FactorExperimentLoaderFromDict`](json_loader.md#FactorExperimentLoaderFromDict), [`merge_file_to_factor_dict_to_factor_dict`](pdf_loader.md#merge_file_to_factor_dict_to_factor_dict)
- used by: [`extract_hypothesis_and_exp_from_reports`](../../../app/qlib_rd_loop/factor_from_report.md#extract_hypothesis_and_exp_from_reports), [`FactorExperimentLoader`](../../../components/loader/experiment_loader.md#FactorExperimentLoader), [`load`](../../../core/experiment.md#Loader.load)

## Functions
- `__check_factor_dict_relevance(factor_df_string: str)` — [`L270`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L270)
- `__check_factor_dict_viability_simulate_json_mode(factor_df_string: str)` — [`L313`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L313)
- `__check_factor_duplication_simulate_json_mode(factor_df: pd.DataFrame)` — [`L356`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L356)
- `__deduplicate_factor_dict(factor_dict: dict[str, dict[str, str]])` — [`L453`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L453)
- `__extract_factor_and_formulation_from_one_report(content: str)` — [`L182`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L182)
- `__extract_factors_formulation_from_content(content: str, factor_dict: dict[str, str])` — [`L141`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L141)
- `__extract_factors_name_and_desc_from_content(content: str)` — [`L115`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L115)
- `__kmeans_embeddings(embeddings: np.ndarray, k: int = 20)` — [`L397`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L397)
- `check_factor_relevance(factor_dict: dict[str, dict[str, str]])` — [`L281`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L281)
- `check_factor_viability(factor_dict: dict[str, dict[str, str]])` — [`L324`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L324)
- `classify_report_from_dict(report_dict: Mapping[str, str], vote_time: int = 1, substrings: tuple[str] = ())` — [`L29`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L29) — Parameters:
- `deduplicate_factors_by_llm(factor_dict: dict[str, dict[str, str]], factor_viability_dict: dict[str, dict[str, str]] | None = None)` — [`L513`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L513)
- `extract_factors_from_report_dict(report_dict: dict[str, str], useful_no_dict: dict[str, dict[str, str]], n_proc: int = 11)` — [`L219`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L219)
- `find_closest_cluster_cosine_similarity(data: np.ndarray, centroids: np.ndarray)` — [`L411`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L411)
- `merge_file_to_factor_dict_to_factor_dict(file_to_factor_dict: dict[str, dict])` — [`L249`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/factor_experiment_loader/pdf_loader.py#L249)


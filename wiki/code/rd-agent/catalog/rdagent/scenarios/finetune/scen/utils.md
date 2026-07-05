---
title: 'Module: rdagent/scenarios/finetune/scen/utils.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/scen/utils.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.scen.utils`/
symbols:
  FinetuneDatasetDescriptor.describe_dataset_folder: FinetuneDatasetDescriptor#describe_dataset_folder().
  FinetuneDatasetDescriptor.analyze_dataset: FinetuneDatasetDescriptor#analyze_dataset().
  FinetuneDatasetDescriptor._generate_stats: FinetuneDatasetDescriptor#_generate_stats().
  FinetuneDatasetDescriptor._extract_samples_for_template: FinetuneDatasetDescriptor#_extract_samples_for_template().
  FinetuneDatasetDescriptor.describe_model: FinetuneDatasetDescriptor#describe_model().
  generate_dataset_info_config: generate_dataset_info_config().
  FinetuneDatasetDescriptor.describe_data_file: FinetuneDatasetDescriptor#describe_data_file().
  FinetuneDatasetDescriptor._generate_file_tree: FinetuneDatasetDescriptor#_generate_file_tree().
  FinetuneDatasetDescriptor._read_dataset_readme: FinetuneDatasetDescriptor#_read_dataset_readme().
  FinetuneDatasetDescriptor.describe_file_json: FinetuneDatasetDescriptor#describe_file_json().
  FinetuneDatasetDescriptor.describe_file_jsonl: FinetuneDatasetDescriptor#describe_file_jsonl().
  FinetuneDatasetDescriptor.describe_file_csv: FinetuneDatasetDescriptor#describe_file_csv().
  FinetuneDatasetDescriptor.describe_file_parquet: FinetuneDatasetDescriptor#describe_file_parquet().
  _truncate_long_values: _truncate_long_values().
  _compute_column_stats: _compute_column_stats().
  FinetuneFileDescription: FinetuneFileDescription#
  _read_single_dataset_readme: _read_single_dataset_readme().
  _load_dataset_for_stats: _load_dataset_for_stats().
  FinetuneDatasetDescriptor._count_samples_in_file: FinetuneDatasetDescriptor#_count_samples_in_file().
  check_all_dataset_in_info: check_all_dataset_in_info().
  FinetuneDatasetDescriptor: FinetuneDatasetDescriptor#
  FinetuneDatasetDescriptor._walk: FinetuneDatasetDescriptor#_walk().
  FinetuneDatasetDescriptor.hash_dataset_path: FinetuneDatasetDescriptor#hash_dataset_path().
  FinetuneDatasetDescription: FinetuneDatasetDescription#
  FinetuneDatasetDescriptor.get_dataset_stats: FinetuneDatasetDescriptor#get_dataset_stats().
  _TOKENIZER_MODEL: _TOKENIZER_MODEL.
  _find_data_files: _find_data_files().
  FinetuneDatasetDescriptor._discover_subtasks: FinetuneDatasetDescriptor#_discover_subtasks().
  FinetuneDatasetDescription.__str__: FinetuneDatasetDescription#__str__().
  FinetuneFileDescription.__str__: FinetuneFileDescription#__str__().
---
# Module: [`rdagent/scenarios/finetune/scen/utils.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py)

## Classes
### `FinetuneDatasetDescription`  ·  implements/extends dict
- def: [`rdagent/scenarios/finetune/scen/utils.py:187`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L187)
- doc: Specialized dataset description for finetune scenarios.
- signature: `class FinetuneDatasetDescription(dict):`
- members:
  - `__str__(self)` — [`L190`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L190) — Generate human-readable description for LLM prompts.
- used by: [`describe_dataset_folder`](utils.md#FinetuneDatasetDescriptor.describe_dataset_folder)

### `FinetuneDatasetDescriptor`
- def: [`rdagent/scenarios/finetune/scen/utils.py:230`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L230)
- doc: Specialized dataset descriptor for finetune scenarios that provides separated file tree and data samples.
- signature: `class FinetuneDatasetDescriptor:`
- members:
  - `_count_samples_in_file(self, data_file: Path)` — [`L242`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L242) — Count total samples in a single data file.
  - `_discover_subtasks(self, dataset_dir: Path)` — [`L677`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L677) — Discover subtasks by scanning directory structure.
  - `_extract_samples_for_template(self, data_files: list[Path], max_samples: int = 2)` — [`L467`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L467) — Extract samples from first data file for template usage.
  - `_generate_file_tree(self, dataset_path: Path)` — [`L233`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L233) — Generate file tree for the dataset directory.
  - `_generate_stats(self, dataset_path: Path, include_column_stats: bool = False)` — [`L275`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L275) — Calculate dataset statistics: sample count, file size, and optionally column token stats.
  - `_read_dataset_readme(self, dataset_path: Path, max_chars: int = 5000)` — [`L445`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L445) — Read README description from dataset directory.
  - `analyze_dataset(self, dataset_dir: Path)` — [`L712`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L712) — Analyze a dataset directory and generate dataset_info.json entry.
  - `describe_data_file(self, data_file: Path)` — [`L652`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L652) — Describe data file based on suffix, dispatching to specific format handlers.
  - `describe_dataset_folder(self, dataset_path: Path, dataset_name: str | None = None, include_dataset_readme: bool = False)` — [`L348`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L348) — Generate complete dataset folder description. — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)
  - `describe_file_csv(self, data_file: Path, max_samples: int = 3)` — [`L616`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L616)
  - `describe_file_json(self, data_file: Path, max_samples: int = 3)` — [`L579`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L579)
  - `describe_file_jsonl(self, data_file: Path, max_samples: int = 3)` — [`L594`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L594)
  - `describe_file_parquet(self, data_file: Path, max_samples: int = 3)` — [`L634`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L634)
  - `describe_model(self, base_model_name: str = None, ft_file_path: str = None)` — [`L502`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L502) — Extract model information from config and metadata.
  - `get_dataset_stats(self, dataset_path: Path)` — [`L425`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L425) — Calculate dataset statistics (public interface for compatibility).
  - `hash_dataset_path(self, dataset_path: Path, dataset_name: str | None = None, include_dataset_readme: bool = False)` — [`L334`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L334) — Generate hash key for dataset description caching.
- protocol/private: `_walk`[`L429`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L429)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../log/logger.md#RDAgentLog.info), [`warning`](../../../log/logger.md#RDAgentLog.warning), [`FT_RD_SETTING`](../../../app/finetune/llm/conf.md#FT_RD_SETTING), [`cache_with_pickle`](../../../core/utils.md#cache_with_pickle), [`md5_hash`](../../../utils/__init__.md#md5_hash), [`generate_tree`](../../data_science/scen/utils.md#FileTreeGenerator.generate_tree), [`file_path`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.file_path), [`_compute_column_stats`](utils.md#_compute_column_stats), [`_truncate_long_values`](utils.md#_truncate_long_values), [`FinetuneFileDescription`](utils.md#FinetuneFileDescription), [`base_model`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.base_model), [`FileTreeGenerator`](../../data_science/scen/utils.md#FileTreeGenerator), [`_load_dataset_for_stats`](utils.md#_load_dataset_for_stats), [`FinetuneDatasetDescription`](utils.md#FinetuneDatasetDescription), [`_TOKENIZER_MODEL`](utils.md#_TOKENIZER_MODEL), [`_find_data_files`](utils.md#_find_data_files), [`data_sample_count`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.data_sample_count)
- used by: [`implement_data`](../../../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy.implement_data), [`generate_dataset_info_config`](utils.md#generate_dataset_info_config), [`model_info`](scenario.md#LLMFinetuneScen.model_info)

### `FinetuneFileDescription`  ·  implements/extends dict
- def: [`rdagent/scenarios/finetune/scen/utils.py:216`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L216)
- doc: Specialized file description for finetune scenarios.
- signature: `class FinetuneFileDescription(dict):`
- members:
  - `__str__(self)` — [`L219`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L219) — Generate human-readable file description.
- used by: [`describe_data_file`](utils.md#FinetuneDatasetDescriptor.describe_data_file), [`describe_file_csv`](utils.md#FinetuneDatasetDescriptor.describe_file_csv), [`describe_file_json`](utils.md#FinetuneDatasetDescriptor.describe_file_json), [`describe_file_jsonl`](utils.md#FinetuneDatasetDescriptor.describe_file_jsonl), [`describe_file_parquet`](utils.md#FinetuneDatasetDescriptor.describe_file_parquet)

## Functions
- `_compute_column_stats(data: list[dict])` — [`L67`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L67) — Compute token statistics for each string column in the dataset.
- `_find_data_files(dataset_path: Path, max_files: int = 50)` — [`L21`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L21) — Find data files in dataset directory using recursive glob.
- `_load_dataset_for_stats(data_files: list[Path], max_samples: int = 50000)` — [`L138`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L138) — Load dataset samples from data files for statistics computation.
- `_read_single_dataset_readme(dataset_path: Path, max_chars: int = 2000)` — [`L774`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L774) — Read README file from a single dataset directory or its parent directories.
- `_truncate_long_values(obj, max_length: int = 3000)` — [`L40`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L40) — Recursively truncate long string values in nested data structures.
- `check_all_dataset_in_info(ft_file_path, existing_config, max_depth: int = 3)` — [`L830`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L830) — Scan datasets directory and return top-level dataset names not yet in existing_config.
- `generate_dataset_info_config(target_dataset_list: list, ft_file_path: str, existing_config: dict)` — [`L863`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L863) — Generate dataset_info.json configuration with auto-discovered subtasks.

## Module values
- `_TOKENIZER_MODEL` — [`L18`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/utils.py#L18)


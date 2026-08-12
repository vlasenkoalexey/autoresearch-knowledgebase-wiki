---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.eval_config`/
symbols:
  EvalDatasetConfig.cache_key: EvalDatasetConfig#cache_key().
  build_eval_dataset_configs: build_eval_dataset_configs().
  _apply_dataset_field_overrides: _apply_dataset_field_overrides().
  EvalDatasetConfig: EvalDatasetConfig#
  EvalDatasetConfig.inject_metadata: EvalDatasetConfig#inject_metadata().
  _MISSING: _MISSING.
  EvalDatasetConfig.__post_init__: EvalDatasetConfig#__post_init__().
  _pick_from_mapping: _pick_from_mapping().
  EvalDatasetConfig.name: EvalDatasetConfig#name.
  _first_not_missing: _first_not_missing().
  EvalDatasetConfig.path: EvalDatasetConfig#path.
  EvalDatasetConfig.metadata_overrides: EvalDatasetConfig#metadata_overrides.
  EvalDatasetConfig.rm_type: EvalDatasetConfig#rm_type.
  EvalDatasetConfig.input_key: EvalDatasetConfig#input_key.
  EvalDatasetConfig.label_key: EvalDatasetConfig#label_key.
  EvalDatasetConfig.tool_key: EvalDatasetConfig#tool_key.
  EvalDatasetConfig.metadata_key: EvalDatasetConfig#metadata_key.
  ensure_dataset_list: ensure_dataset_list().
  pick_from_args: pick_from_args().
  _ensure_metadata_overrides: _ensure_metadata_overrides().
  EvalDatasetConfig.n_samples_per_eval_prompt: EvalDatasetConfig#n_samples_per_eval_prompt.
  EvalDatasetConfig.temperature: EvalDatasetConfig#temperature.
  EvalDatasetConfig.top_p: EvalDatasetConfig#top_p.
  EvalDatasetConfig.top_k: EvalDatasetConfig#top_k.
  EvalDatasetConfig.max_response_len: EvalDatasetConfig#max_response_len.
  DATASET_RUNTIME_SPECS.DATASET_RUNTIME_SPECS: DATASET_RUNTIME_SPECS.DATASET_RUNTIME_SPECS.
  DATASET_SAMPLE_SPECS.DATASET_SAMPLE_SPECS: DATASET_SAMPLE_SPECS.DATASET_SAMPLE_SPECS.
  EvalDatasetConfig.stop: EvalDatasetConfig#stop.
  EvalDatasetConfig.stop_token_ids: EvalDatasetConfig#stop_token_ids.
  EvalDatasetConfig.min_new_tokens: EvalDatasetConfig#min_new_tokens.
  EvalDatasetConfig.custom_generate_function_path: EvalDatasetConfig#custom_generate_function_path.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py)

## Classes
### `EvalDatasetConfig`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py:95`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L95)
- doc: Configuration for a single evaluation dataset.
- signature: `class EvalDatasetConfig:`
- members:
  - `cache_key(self)` — [`L127`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L127) — Return a tuple uniquely identifying dataset config for caching.
  - `inject_metadata(self, sample_metadata: Any)` — [`L138`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L138) — Return updated metadata merging overrides.
  - `custom_generate_function_path` — [`L119`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L119)
  - `input_key` — [`L103`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L103)
  - `label_key` — [`L104`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L104)
  - `max_response_len` — [`L113`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L113)
  - `metadata_key` — [`L106`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L106)
  - `metadata_overrides` — [`L121`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L121)
  - `min_new_tokens` — [`L116`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L116)
  - `n_samples_per_eval_prompt` — [`L108`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L108)
  - `name` — [`L98`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L98)
  - `path` — [`L99`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L99)
  - `rm_type` — [`L100`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L100)
  - `stop` — [`L114`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L114)
  - `stop_token_ids` — [`L115`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L115)
  - `temperature` — [`L110`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L110)
  - `tool_key` — [`L105`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L105)
  - `top_k` — [`L112`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L112)
  - `top_p` — [`L111`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L111)
- protocol/private: `__post_init__`[`L123`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L123)
- uses (calls/refs, reference-scoped): [`_ensure_metadata_overrides`](eval_config.md#_ensure_metadata_overrides)
- used by: [`eval_rollout_single_dataset`](../rollout/sglang_rollout.md#eval_rollout_single_dataset), [`_resolve_eval_datasets`](arguments.md#_resolve_eval_datasets), [`build_eval_dataset_configs`](eval_config.md#build_eval_dataset_configs), [`with_opd_teacher`](../ray/train_actor.md#TrainRayActor.with_opd_teacher)

## Functions
- `_apply_dataset_field_overrides(args: Any, dataset_cfg: dict[str, Any], defaults: dict[str, Any], spec_names: dict[str, Any])` — [`L182`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L182)
- `_ensure_metadata_overrides(value: Any)` — [`L86`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L86)
- `_first_not_missing(*values: Any)` — [`L62`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L62)
- `_pick_from_mapping(data: dict[str, Any], key_names: tuple[str, ...] | None)` — [`L69`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L69)
- `build_eval_dataset_configs(args: Any, raw_config: Iterable[dict[str, Any]], defaults: dict[str, Any])` — [`L195`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L195)
- `ensure_dataset_list(config: Any)` — [`L154`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L154) — Normalize OmegaConf containers into a list of dicts.
- `pick_from_args(args: Any, attrs: tuple[str, ...])` — [`L78`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L78)

## Module values
- `DATASET_RUNTIME_SPECS` — [`L10`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L10)
- `DATASET_SAMPLE_SPECS` — [`L38`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L38)
- `_MISSING` — [`L7`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/eval_config.py#L7)


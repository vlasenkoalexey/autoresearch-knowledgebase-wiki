---
title: 'Module: OpenMLE-Evo/scripts/evaluate_airaevo.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/scripts/evaluate_airaevo.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.scripts.evaluate_airaevo`/
symbols:
  main: main().
  _maybe_patch_eval_data_with_validation_guidance: _maybe_patch_eval_data_with_validation_guidance().
  _maybe_patch_eval_data_with_task_skill_guidance: _maybe_patch_eval_data_with_task_skill_guidance().
  logger: logger.
  REPO_ROOT: REPO_ROOT.
  _inject_task_skill_into_prompt_value: _inject_task_skill_into_prompt_value().
  _to_plain: _to_plain().
  _resolve_repo_path: _resolve_repo_path().
  TTS_SEARCH_DIR: TTS_SEARCH_DIR.
  _first_model_payload: _first_model_payload().
  _generation_kwargs_from_litellm_params: _generation_kwargs_from_litellm_params().
  _metadata_task_name: _metadata_task_name().
  _write_yaml: _write_yaml().
---
# Module: [`OpenMLE-Evo/scripts/evaluate_airaevo.py`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_airaevo.py)

## Functions
- `_first_model_payload(cfg: DictConfig)` — [`L38`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_airaevo.py#L38)
- `_generation_kwargs_from_litellm_params(litellm_params: dict[str, Any])` — [`L45`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_airaevo.py#L45)
- `_inject_task_skill_into_prompt_value(prompt_value: Any, *, task_name: str, injector: TaskSkillGuidanceInjector)` — [`L164`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_airaevo.py#L164)
- `_maybe_patch_eval_data_with_task_skill_guidance(cfg: DictConfig, *, eval_data_path: Path, hydra_dir: Path)` — [`L204`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_airaevo.py#L204)
- `_maybe_patch_eval_data_with_validation_guidance(cfg: DictConfig, *, hydra_dir: Path)` — [`L97`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_airaevo.py#L97)
- `_metadata_task_name(metadata: Any)` — [`L148`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_airaevo.py#L148)
- `_resolve_repo_path(path_value: str | None)` — [`L88`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_airaevo.py#L88)
- `_to_plain(value: Any)` — [`L32`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_airaevo.py#L32)
- `_write_yaml(path: Path, payload: dict[str, Any])` — [`L81`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_airaevo.py#L81)
- `main(cfg: DictConfig)` — [`L295`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_airaevo.py#L295)

## Module values
- `REPO_ROOT` — [`L16`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_airaevo.py#L16)
- `TTS_SEARCH_DIR` — [`L19`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_airaevo.py#L19)
- `logger` — [`L20`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_airaevo.py#L20)


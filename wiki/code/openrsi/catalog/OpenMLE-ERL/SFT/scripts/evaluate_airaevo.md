---
title: 'Module: OpenMLE-ERL/SFT/scripts/evaluate_airaevo.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/scripts/evaluate_airaevo.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.scripts.evaluate_airaevo`/
symbols:
  main: main().
  REPO_ROOT: REPO_ROOT.
  _to_plain: _to_plain().
  _task_list_from_eval_data: _task_list_from_eval_data().
  logger: logger.
  TTS_SEARCH_DIR: TTS_SEARCH_DIR.
  _first_model_payload: _first_model_payload().
  _generation_kwargs_from_litellm_params: _generation_kwargs_from_litellm_params().
  _write_yaml: _write_yaml().
  _configure_airaevo_api_key_env: _configure_airaevo_api_key_env().
  _sanitize_task_name: _sanitize_task_name().
---
# Module: [`OpenMLE-ERL/SFT/scripts/evaluate_airaevo.py`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/evaluate_airaevo.py)

## Functions
- `_configure_airaevo_api_key_env(litellm_params: dict[str, Any])` — [`L74`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/evaluate_airaevo.py#L74) — Bridge Hydra LiteLLM keys to the AIRA Evo backend env convention.
- `_first_model_payload(cfg: DictConfig)` — [`L31`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/evaluate_airaevo.py#L31)
- `_generation_kwargs_from_litellm_params(litellm_params: dict[str, Any])` — [`L38`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/evaluate_airaevo.py#L38)
- `_sanitize_task_name(task_name: str)` — [`L82`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/evaluate_airaevo.py#L82)
- `_task_list_from_eval_data(cfg: DictConfig)` — [`L86`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/evaluate_airaevo.py#L86)
- `_to_plain(value: Any)` — [`L25`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/evaluate_airaevo.py#L25)
- `_write_yaml(path: Path, payload: dict[str, Any])` — [`L104`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/evaluate_airaevo.py#L104)
- `main(cfg: DictConfig)` — [`L116`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/evaluate_airaevo.py#L116)

## Module values
- `REPO_ROOT` — [`L16`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/evaluate_airaevo.py#L16)
- `TTS_SEARCH_DIR` — [`L19`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/evaluate_airaevo.py#L19)
- `logger` — [`L20`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/evaluate_airaevo.py#L20)


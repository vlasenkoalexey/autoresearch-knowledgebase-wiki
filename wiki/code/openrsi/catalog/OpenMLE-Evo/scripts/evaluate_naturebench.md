---
title: 'Module: OpenMLE-Evo/scripts/evaluate_naturebench.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/scripts/evaluate_naturebench.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.scripts.evaluate_naturebench`/
symbols:
  _data_value: _data_value().
  main: main().
  _build_payloads: _build_payloads().
  REPO_ROOT: REPO_ROOT.
  logger: logger.
  _to_plain: _to_plain().
  _first_model_payload: _first_model_payload().
  TTS_SEARCH_DIR: TTS_SEARCH_DIR.
  _generation_kwargs_from_litellm_params: _generation_kwargs_from_litellm_params().
  _subprocess_env: _subprocess_env().
  _write_yaml: _write_yaml().
---
# Module: [`OpenMLE-Evo/scripts/evaluate_naturebench.py`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_naturebench.py)

## Functions
- `_build_payloads(cfg: DictConfig, *, output_dir: Path, task_root: Path)` — [`L95`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_naturebench.py#L95)
- `_data_value(cfg: DictConfig, key: str, default: Any = None)` — [`L91`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_naturebench.py#L91)
- `_first_model_payload(cfg: DictConfig)` — [`L31`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_naturebench.py#L31)
- `_generation_kwargs_from_litellm_params(litellm_params: dict[str, Any])` — [`L38`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_naturebench.py#L38)
- `_subprocess_env(*extra_paths: Path)` — [`L81`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_naturebench.py#L81)
- `_to_plain(value: Any)` — [`L25`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_naturebench.py#L25)
- `_write_yaml(path: Path, payload: dict[str, Any])` — [`L74`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_naturebench.py#L74)
- `main(cfg: DictConfig)` — [`L221`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_naturebench.py#L221)

## Module values
- `REPO_ROOT` — [`L15`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_naturebench.py#L15)
- `TTS_SEARCH_DIR` — [`L18`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_naturebench.py#L18)
- `logger` — [`L19`](../../../../../../raw/code/openrsi/OpenMLE-Evo/scripts/evaluate_naturebench.py#L19)


---
title: 'Module: OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.evaluate_pass_k`/
symbols:
  run_pass_k_evaluation: run_pass_k_evaluation().
  logger: logger.
  main: main().
  run_pass_k_evaluation.monitor_progress: run_pass_k_evaluation().monitor_progress().
  main.run_sharded_evals: main().run_sharded_evals().
  _merge_dirs: _merge_dirs().
  _migrate_task_dirs: _migrate_task_dirs().
  TTS_SEARCH_DIR: TTS_SEARCH_DIR.
  _parse_minimax_api_keys: _parse_minimax_api_keys().
  REPO_ROOT: REPO_ROOT.
  _build_router_with_key: _build_router_with_key().
  _is_minimax_config: _is_minimax_config().
  _split_tasks_evenly: _split_tasks_evenly().
---
# Module: [`OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py)

## Functions
- `_build_router_with_key(cfg: DictConfig, api_key: str)` — [`L129`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py#L129) — Build a LiteLLM router for one API key.
- `_is_minimax_config(cfg: DictConfig)` — [`L73`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py#L73) — Check if config uses MiniMax provider.
- `_merge_dirs(src: Path, dst: Path)` — [`L144`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py#L144) — Merge src directory into dst without overwriting existing files.
- `_migrate_task_dirs(output_dir: Path, task_subdir: str = "tasks")` — [`L158`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py#L158) — Move task folders under output_dir into task_subdir.
- `_parse_minimax_api_keys(cfg: DictConfig | None = None)` — [`L82`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py#L82) — Parse MiniMax API keys only if config uses MiniMax.
- `_split_tasks_evenly(tasks: list[dict[str, Any]], n_shards: int)` — [`L111`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py#L111) — Split task records across shards.
- `main(cfg: DictConfig)` — [`L697`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py#L697) — CLI entry for pass@k generation/evaluation.
- `monitor_progress()` — [`L516`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py#L516) — Monitor and log progress every 30 seconds with separate gen/eval tracking.
- `run_pass_k_evaluation(cfg: DictConfig, router: Router, tasks: list[dict[str, Any]], output_dir: Path)` — [`L178`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py#L178) — Run pass@k evaluation for all tasks.
- `run_sharded_evals()` — [`L824`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py#L824) — Run one pass@k evaluation coroutine per API-key shard.

## Module values
- `REPO_ROOT` — [`L65`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py#L65)
- `TTS_SEARCH_DIR` — [`L66`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py#L66)
- `logger` — [`L67`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/evaluate_pass_k.py#L67)


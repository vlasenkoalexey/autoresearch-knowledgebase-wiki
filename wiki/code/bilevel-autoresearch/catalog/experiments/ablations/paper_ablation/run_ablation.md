---
title: 'Module: experiments/ablations/paper_ablation/run_ablation.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run_ablation.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run_ablation`/
symbols:
  run_group_d: run_group_d().
  run_group_c: run_group_c().
  run_group_a: run_group_a().
  logger: logger.
  run_group_b: run_group_b().
  _v: _v.
  main: main().
  _make_search_config: _make_search_config().
  _line: _line.
  _make_llm_client: _make_llm_client().
  PROJECT_ROOT: PROJECT_ROOT.
  _save_report: _save_report().
  _env_path: _env_path.
  RESULTS_DIR: RESULTS_DIR.
  _build_run_dir: _build_run_dir().
  _snapshot_runner: _snapshot_runner().
  _load_runner_module: _load_runner_module().
  _get_train_py: _get_train_py().
  _setup_run_logging: _setup_run_logging().
  _teardown_run_logging: _teardown_run_logging().
  parse_args: parse_args().
  LEVEL2_CYCLE_INTERVAL: LEVEL2_CYCLE_INTERVAL.
  _print_group_summary: _print_group_summary().
  ABLATION_DIR: ABLATION_DIR.
  FORBIDDEN_PARAMS: FORBIDDEN_PARAMS.
  TIME_BUDGET: TIME_BUDGET.
  LEVEL2_BATCH_SIZE: LEVEL2_BATCH_SIZE.
  _k: _k.
---
# Module: [`experiments/ablations/paper_ablation/run_ablation.py`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py)

## Functions
- `_build_run_dir(group: str, repeat: int)` — [`L120`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L120) — Return the directory for a single run, creating it if necessary.
- `_get_train_py(autoresearch_dir: Path)` — [`L109`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L109) — Return path to the baseline train.py, raising if not found.
- `_load_runner_module(runner_py: Path)` — [`L855`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L855) — Dynamically import a runner.py from an arbitrary path.
- `_make_llm_client(provider: str, model: str)` — [`L86`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L86) — Create an LLM client, resolving API key from env.
- `_make_search_config(iterations: int, time_budget: int)` — [`L100`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L100) — Build SearchConfig with DEPTH and ASPECT_RATIO removed from editable_params.
- `_print_group_summary(group: str, results: list[dict])` — [`L161`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L161) — Print a formatted summary table for a group after all repeats.
- `_save_report(run_dir: Path, report: dict)` — [`L147`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L147) — Save a structured report.json to the run directory.
- `_setup_run_logging(run_dir: Path)` — [`L127`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L127) — Attach a file handler for the run's experiment.log.
- `_snapshot_runner(run_dir: Path, runner_py: Path)` — [`L154`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L154) — Copy the runner.py used for this run to the results directory.
- `_teardown_run_logging(fh: logging.FileHandler)` — [`L141`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L141) — Remove and close the per-run file handler.
- `main()` — [`L957`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L957)
- `parse_args()` — [`L903`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L903)
- `run_group_a(repeat: int, iterations: int, time_budget: int, provider: str, model: str, autoresearch_dir: Path)` — [`L192`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L192) — Run one repeat of Group A: inner loop only. — documented in [domains-train_opt-runner](../../../../concepts/domains-train_opt-runner.md)
- `run_group_b(repeat: int, iterations: int, outer_cycles: int, time_budget: int, provider: str, model: str, autoresearch_dir: Path)` — [`L277`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L277) — Run one repeat of Group B: inner + outer loop.
- `run_group_c(repeat: int, iterations: int, outer_cycles: int, time_budget: int, provider: str, model: str, autoresearch_dir: Path)` — [`L362`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L362) — Run one repeat of Group C: inner + outer + Level-2 mechanism researcher. — documented in [domains-train_opt-mechanism_research](../../../../concepts/domains-train_opt-mechanism_research.md)
- `run_group_d(repeat: int, iterations: int, time_budget: int, provider: str, model: str, autoresearch_dir: Path)` — [`L607`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L607) — Run one repeat of Group D: inner loop only + Level-2 mechanism researcher. — documented in [domains-train_opt-mechanism_research](../../../../concepts/domains-train_opt-mechanism_research.md)

## Module values
- `ABLATION_DIR` — [`L56`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L56)
- `FORBIDDEN_PARAMS` — [`L61`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L61)
- `LEVEL2_BATCH_SIZE` — [`L605`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L605)
- `LEVEL2_CYCLE_INTERVAL` — [`L68`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L68)
- `PROJECT_ROOT` — [`L35`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L35)
- `RESULTS_DIR` — [`L57`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L57)
- `TIME_BUDGET` — [`L64`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L64)
- `_env_path` — [`L38`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L38)
- `_k` — [`L43`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L43)
- `_line` — [`L40`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L40)
- `_v` — [`L43`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L43)
- `logger` — [`L79`](../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run_ablation.py#L79)


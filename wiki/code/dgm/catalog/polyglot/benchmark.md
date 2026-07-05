---
title: 'Module: polyglot/benchmark.py'
type: catalog
provenance: extracted
module: polyglot/benchmark.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `polyglot.benchmark`/
symbols:
  main: main().
  summarize_results: summarize_results().
  summarize_results.show: summarize_results().show().
  BENCHMARK_DNAME: BENCHMARK_DNAME.
  run_test_real: run_test_real().
  run_test: run_test().
  find_latest_benchmark_dir: find_latest_benchmark_dir().
  show_stats: show_stats().
  resolve_dirname: resolve_dirname().
  show_diffs: show_diffs().
  run_unit_tests: run_unit_tests().
  app: app.
  load_results: load_results().
  EXERCISES_DIR_DEFAULT: EXERCISES_DIR_DEFAULT.
  main.get_exercise_dirs: main().get_exercise_dirs().
  get_versions: get_versions().
  get_replayed_content: get_replayed_content().
  cleanup_test_output: cleanup_test_output().
---
# Module: [`polyglot/benchmark.py`](../../../../../raw/code/dgm/polyglot/benchmark.py)

## Functions
- `cleanup_test_output(output, testdir)` — [`L1009`](../../../../../raw/code/dgm/polyglot/benchmark.py#L1009)
- `find_latest_benchmark_dir()` — [`L43`](../../../../../raw/code/dgm/polyglot/benchmark.py#L43)
- `get_exercise_dirs(base_dir, languages=None)` — [`L252`](../../../../../raw/code/dgm/polyglot/benchmark.py#L252) — Get all exercise directories for specified languages (or all if none specified)
- `get_replayed_content(replay_dname, test_dname)` — [`L619`](../../../../../raw/code/dgm/polyglot/benchmark.py#L619)
- `get_versions(commit_hashes)` — [`L602`](../../../../../raw/code/dgm/polyglot/benchmark.py#L602)
- `load_results(dirname, stats_languages=None)` — [`L434`](../../../../../raw/code/dgm/polyglot/benchmark.py#L434)
- `main(dirnames: Optional[List[str]] = typer.Argument(None, help="Directory names"), graphs: bool = typer.Option(False, "--graphs", help="Generate graphs"), model: str = typer.Option("gpt-3.5-turbo", "--model", "-m", help="Model name"), sleep: float = typer.Option(0, "--sleep", help="Sleep seconds between tests when single threaded"), languages: str = typer.Option(None, "--languages", "-l", help="Only run tests for specific languages (comma separated)"), edit_format: str = typer.Option(None, "--edit-format", "-e", help="Edit format"), editor_model: str = typer.Option(None, "--editor-model", help="Editor model name"), editor_edit_format: str = typer.Option(None, "--editor-edit-format", help="Editor edit format"), replay: str = typer.Option(None, "--replay", help="Replay previous .aider.chat.history.md responses from previous benchmark run"), keywords: str = typer.Option(None, "--keywords", "-k", help="Only run tests that contain keywords (comma sep)"), clean: bool = typer.Option(False, "--clean", "-c", help="Discard the existing testdir and make a clean copy"), cont: bool = typer.Option(False, "--cont", help="Continue the (single) matching testdir"), make_new: bool = typer.Option(False, "--new", "-n", help="Make a new dated testdir"), no_unit_tests: bool = typer.Option(False, "--no-unit-tests", help="Do not run unit tests"), no_aider: bool = typer.Option(False, "--no-aider", help="Do not run aider"), verbose: bool = typer.Option(False, "--verbose", "-v", help="Verbose output"), stats_only: bool = typer.Option(False, "--stats", "-s", help="Do not run tests, just collect stats on completed tests"), stats_languages: str = typer.Option(None, "--stats-languages", help="Only include stats for specific languages (comma separated)"), diffs_only: bool = typer.Option(False, "--diffs", help="Just diff the provided stats dirs"), tries: int = typer.Option(2, "--tries", "-r", help="Number of tries for running tests"), threads: int = typer.Option(1, "--threads", "-t", help="Number of threads to run in parallel"), num_tests: int = typer.Option(-1, "--num-tests", "-n", help="Number of tests to run"), num_ctx: Optional[int] = typer.Option(None, "--num-ctx", help="Override model context window size"), read_model_settings: str = typer.Option(None, "--read-model-settings", help="Load aider model settings from YAML file"), exercises_dir: str = typer.Option(EXERCISES_DIR_DEFAULT, "--exercises-dir", help="Directory with exercise files"))` — [`L162`](../../../../../raw/code/dgm/polyglot/benchmark.py#L162)
- `resolve_dirname(dirname, use_single_prior, make_new)` — [`L136`](../../../../../raw/code/dgm/polyglot/benchmark.py#L136)
- `run_test(original_dname, testdir, *args, **kwargs)` — [`L636`](../../../../../raw/code/dgm/polyglot/benchmark.py#L636)
- `run_test_real(original_dname, testdir, model_name, edit_format, tries, no_unit_tests, no_aider, verbose, commit_hash, replay, editor_model, editor_edit_format, num_ctx=None, sleep=0, read_model_settings=None)` — [`L650`](../../../../../raw/code/dgm/polyglot/benchmark.py#L650)
- `run_unit_tests(original_dname, testdir, history_fname, test_files)` — [`L939`](../../../../../raw/code/dgm/polyglot/benchmark.py#L939)
- `show(stat, red="red")` — [`L529`](../../../../../raw/code/dgm/polyglot/benchmark.py#L529)
- `show_diffs(dirnames)` — [`L397`](../../../../../raw/code/dgm/polyglot/benchmark.py#L397)
- `show_stats(dirnames, graphs, stats_languages=None)` — [`L91`](../../../../../raw/code/dgm/polyglot/benchmark.py#L91)
- `summarize_results(dirname, stats_languages=None)` — [`L455`](../../../../../raw/code/dgm/polyglot/benchmark.py#L455)

## Module values
- `BENCHMARK_DNAME` — [`L33`](../../../../../raw/code/dgm/polyglot/benchmark.py#L33)
- `EXERCISES_DIR_DEFAULT` — [`L35`](../../../../../raw/code/dgm/polyglot/benchmark.py#L35)
- `app` — [`L37`](../../../../../raw/code/dgm/polyglot/benchmark.py#L37)


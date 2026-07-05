---
title: 'Module: rdagent/app/benchmark/factor/analysis.py'
type: catalog
provenance: extracted
module: rdagent/app/benchmark/factor/analysis.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.benchmark.factor.analysis`/
symbols:
  main: main().
  BenchmarkAnalyzer.process_results: BenchmarkAnalyzer#process_results().
  BenchmarkAnalyzer.reformat_index: BenchmarkAnalyzer#reformat_index().
  BenchmarkAnalyzer.analyze_data: BenchmarkAnalyzer#analyze_data().
  BenchmarkAnalyzer.index_map: BenchmarkAnalyzer#index_map.
  BenchmarkAnalyzer.load_index_map: BenchmarkAnalyzer#load_index_map().
  Plotter: Plotter#
  BenchmarkAnalyzer: BenchmarkAnalyzer#
  BenchmarkAnalyzer.settings: BenchmarkAnalyzer#settings.
  BenchmarkAnalyzer.only_correct_format: BenchmarkAnalyzer#only_correct_format.
  BenchmarkAnalyzer.load_data: BenchmarkAnalyzer#load_data().
  BenchmarkAnalyzer.result_all_key_order: BenchmarkAnalyzer#result_all_key_order().
  Plotter.change_fs: Plotter#change_fs().
  Plotter.plot_data: Plotter#plot_data().
  BenchmarkAnalyzer.__init__: BenchmarkAnalyzer#__init__().
---
# Module: [`rdagent/app/benchmark/factor/analysis.py`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py)

## Classes
### `BenchmarkAnalyzer`
- def: [`rdagent/app/benchmark/factor/analysis.py:15`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py#L15)
- signature: `class BenchmarkAnalyzer:`
- members:
  - `analyze_data(self, sum_df)` — [`L96`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py#L96)
  - `load_data(self, file_path)` — [`L29`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py#L29)
  - `load_index_map(self)` — [`L21`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py#L21)
  - `process_results(self, results)` — [`L39`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py#L39)
  - `reformat_index(self, display_df)` — [`L48`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py#L48) — reform the results from
  - `result_all_key_order(self, x)` — [`L81`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py#L81)
  - `index_map` — [`L18`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py#L18)
  - `only_correct_format` — [`L19`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py#L19)
  - `settings` — [`L17`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py#L17)
- protocol/private: `__init__`[`L16`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py#L16)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (1 test-only callers)

### `Plotter`
- def: [`rdagent/app/benchmark/factor/analysis.py:178`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py#L178)
- signature: `class Plotter:`
- members:
  - `change_fs(font_size)` — [`L180`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py#L180)
  - `plot_data(data, file_name, title)` — [`L190`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py#L190)
- used by: (1 test-only callers)

## Functions
- `main(path="git_ignore_folder/eval_results/res_promptV220240724-060037.pkl", round=1, title="Comparison of Different Methods", only_correct_format=False)` — [`L204`](../../../../../../../../raw/code/rd-agent/rdagent/app/benchmark/factor/analysis.py#L204)


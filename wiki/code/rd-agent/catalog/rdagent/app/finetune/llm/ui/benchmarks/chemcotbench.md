---
title: 'Module: rdagent/app/finetune/llm/ui/benchmarks/chemcotbench.py'
type: catalog
provenance: extracted
module: rdagent/app/finetune/llm/ui/benchmarks/chemcotbench.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.finetune.llm.ui.benchmarks.chemcotbench`/ChemCotBenchProcessor#
symbols:
  ChemCotBenchProcessor.get_core_metric: get_core_metric().
  ChemCotBenchProcessor: ''
  ChemCotBenchProcessor.METRIC_GROUPS: METRIC_GROUPS.
  ChemCotBenchProcessor.CORE_METRICS: CORE_METRICS.
  ChemCotBenchProcessor.match: match().
---
# Module: [`rdagent/app/finetune/llm/ui/benchmarks/chemcotbench.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/chemcotbench.py)

## Classes
### `ChemCotBenchProcessor`  ·  implements/extends BenchmarkProcessor
- def: [`rdagent/app/finetune/llm/ui/benchmarks/chemcotbench.py:6`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/chemcotbench.py#L6)
- doc: ChemCotBench: Chemistry reasoning with various subtasks.
- signature: `class ChemCotBenchProcessor(BenchmarkProcessor):`
- members:
  - `get_core_metric(cls, accuracy_summary: dict)` — [`L47`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/chemcotbench.py#L47)
  - `match(cls, benchmark_name: str)` — [`L43`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/chemcotbench.py#L43)
  - `CORE_METRICS` — [`L13`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/chemcotbench.py#L13)
  - `METRIC_GROUPS` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/chemcotbench.py#L35)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (4 test-only callers)


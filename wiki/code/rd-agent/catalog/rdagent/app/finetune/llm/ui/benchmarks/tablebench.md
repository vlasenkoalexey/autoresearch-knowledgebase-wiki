---
title: 'Module: rdagent/app/finetune/llm/ui/benchmarks/tablebench.py'
type: catalog
provenance: extracted
module: rdagent/app/finetune/llm/ui/benchmarks/tablebench.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.finetune.llm.ui.benchmarks.tablebench`/TableBenchProcessor#
symbols:
  TableBenchProcessor.HIGHER_IS_BETTER: HIGHER_IS_BETTER.
  TableBenchProcessor.get_core_metric: get_core_metric().
  TableBenchProcessor: ''
  TableBenchProcessor.CORE_METRICS: CORE_METRICS.
  TableBenchProcessor.match: match().
---
# Module: [`rdagent/app/finetune/llm/ui/benchmarks/tablebench.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/tablebench.py)

## Classes
### `TableBenchProcessor`  ·  implements/extends BenchmarkProcessor
- def: [`rdagent/app/finetune/llm/ui/benchmarks/tablebench.py:6`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/tablebench.py#L6)
- doc: TableBench: Table QA with different subtasks.
- signature: `class TableBenchProcessor(BenchmarkProcessor):`
- members:
  - `get_core_metric(cls, accuracy_summary: dict)` — [`L28`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/tablebench.py#L28)
  - `match(cls, benchmark_name: str)` — [`L24`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/tablebench.py#L24)
  - `CORE_METRICS` — [`L9`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/tablebench.py#L9)
  - `HIGHER_IS_BETTER` — [`L17`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/tablebench.py#L17)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (4 test-only callers)


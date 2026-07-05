---
title: 'Module: rdagent/app/finetune/llm/ui/benchmarks/base.py'
type: catalog
provenance: extracted
module: rdagent/app/finetune/llm/ui/benchmarks/base.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.finetune.llm.ui.benchmarks.base`/BenchmarkProcessor#
symbols:
  BenchmarkProcessor: ''
  BenchmarkProcessor.match: match().
  BenchmarkProcessor.get_core_metric: get_core_metric().
  BenchmarkProcessor.is_higher_better: is_higher_better().
  BenchmarkProcessor.HIGHER_IS_BETTER: HIGHER_IS_BETTER.
---
# Module: [`rdagent/app/finetune/llm/ui/benchmarks/base.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/base.py)

## Classes
### `BenchmarkProcessor`  ·  implements/extends ABC
- def: [`rdagent/app/finetune/llm/ui/benchmarks/base.py:6`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/base.py#L6)
- doc: Base class for benchmark core metric extraction.
- signature: `class BenchmarkProcessor(ABC):`
- members:
  - `get_core_metric(cls, accuracy_summary: dict)` — [`L34`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/base.py#L34) — Extract core metric name, value, and direction from accuracy_summary.
  - `is_higher_better(cls, metric_name: str)` — [`L49`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/base.py#L49) — Check if higher values are better for this metric.
  - `match(cls, benchmark_name: str)` — [`L28`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/base.py#L28) — Check if this processor handles the given benchmark.
  - `HIGHER_IS_BETTER` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/base.py#L11)
- uses (calls/refs, reference-scoped): (15 test-only callers)
- used by: (10 test-only callers)


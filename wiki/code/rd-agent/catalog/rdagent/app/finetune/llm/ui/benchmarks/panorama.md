---
title: 'Module: rdagent/app/finetune/llm/ui/benchmarks/panorama.py'
type: catalog
provenance: extracted
module: rdagent/app/finetune/llm/ui/benchmarks/panorama.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.finetune.llm.ui.benchmarks.panorama`/PanoramaProcessor#
symbols:
  PanoramaProcessor.get_core_metric: get_core_metric().
  PanoramaProcessor: ''
  PanoramaProcessor.CORE_METRICS: CORE_METRICS.
  PanoramaProcessor.match: match().
---
# Module: [`rdagent/app/finetune/llm/ui/benchmarks/panorama.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/panorama.py)

## Classes
### `PanoramaProcessor`  ·  implements/extends BenchmarkProcessor
- def: [`rdagent/app/finetune/llm/ui/benchmarks/panorama.py:6`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/panorama.py#L6)
- doc: Panorama: Different sub-datasets use different metrics.
- signature: `class PanoramaProcessor(BenchmarkProcessor):`
- members:
  - `get_core_metric(cls, accuracy_summary: dict)` — [`L20`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/panorama.py#L20)
  - `match(cls, benchmark_name: str)` — [`L16`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/panorama.py#L16)
  - `CORE_METRICS` — [`L9`](../../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/benchmarks/panorama.py#L9)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (4 test-only callers)


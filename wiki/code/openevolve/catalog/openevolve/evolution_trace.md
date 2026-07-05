---
title: 'Module: openevolve/evolution_trace.py'
type: catalog
provenance: extracted
module: openevolve/evolution_trace.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.evolution_trace`/
symbols:
  EvolutionTracer.log_trace: EvolutionTracer#log_trace().
  extract_evolution_trace_from_checkpoint: extract_evolution_trace_from_checkpoint().
  EvolutionTracer.close: EvolutionTracer#close().
  EvolutionTracer.stats: EvolutionTracer#stats.
  EvolutionTracer.flush: EvolutionTracer#flush().
  logger: logger.
  EvolutionTracer.output_path: EvolutionTracer#output_path.
  EvolutionTracer: EvolutionTracer#
  EvolutionTrace: EvolutionTrace#
  EvolutionTracer.buffer: EvolutionTracer#buffer.
  EvolutionTracer._update_stats: EvolutionTracer#_update_stats().
  EvolutionTrace.iteration: EvolutionTrace#iteration.
  EvolutionTrace.parent_metrics: EvolutionTrace#parent_metrics.
  EvolutionTrace.child_metrics: EvolutionTrace#child_metrics.
  EvolutionTrace.calculate_improvement: EvolutionTrace#calculate_improvement().
  EvolutionTracer.json_traces: EvolutionTracer#json_traces.
  extract_full_lineage_traces: extract_full_lineage_traces().
  EvolutionTrace.parent_id: EvolutionTrace#parent_id.
  EvolutionTrace.child_id: EvolutionTrace#child_id.
  EvolutionTracer.format: EvolutionTracer#format.
  EvolutionTrace.improvement_delta: EvolutionTrace#improvement_delta.
  EvolutionTracer.get_statistics: EvolutionTracer#get_statistics().
  EvolutionTrace.timestamp: EvolutionTrace#timestamp.
  EvolutionTrace.parent_code: EvolutionTrace#parent_code.
  EvolutionTrace.child_code: EvolutionTrace#child_code.
  EvolutionTracer.enabled: EvolutionTracer#enabled.
  EvolutionTrace.island_id: EvolutionTrace#island_id.
  EvolutionTrace.generation: EvolutionTrace#generation.
  EvolutionTracer.include_code: EvolutionTracer#include_code.
  EvolutionTracer.include_prompts: EvolutionTracer#include_prompts.
  EvolutionTracer.__exit__: EvolutionTracer#__exit__().
  EvolutionTrace.parent_changes_description: EvolutionTrace#parent_changes_description.
  EvolutionTrace.child_changes_description: EvolutionTrace#child_changes_description.
  EvolutionTrace.prompt: EvolutionTrace#prompt.
  EvolutionTrace.llm_response: EvolutionTrace#llm_response.
  EvolutionTrace.metadata: EvolutionTrace#metadata.
  EvolutionTracer.compress: EvolutionTracer#compress.
  EvolutionTrace.artifacts: EvolutionTrace#artifacts.
  EvolutionTrace.to_dict: EvolutionTrace#to_dict().
  EvolutionTracer.include_changes_description: EvolutionTracer#include_changes_description.
  EvolutionTracer.buffer_size: EvolutionTracer#buffer_size.
  EvolutionTrace.code_diff: EvolutionTrace#code_diff.
  EvolutionTracer.__init__: EvolutionTracer#__init__().
  EvolutionTracer.__enter__: EvolutionTracer#__enter__().
---
# Module: [`openevolve/evolution_trace.py`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py)

## Classes
### `EvolutionTrace`
- def: [`openevolve/evolution_trace.py:25`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L25) — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
- doc: Represents a single evolution trace entry
- signature: `class EvolutionTrace:`
- members:
  - `calculate_improvement(self)` — [`L51`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L51) — Calculate improvement deltas between parent and child metrics — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `to_dict(self)` — [`L47`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L47) — Convert trace to dictionary format
  - `artifacts` — [`L44`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L44)
  - `child_changes_description` — [`L37`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L37)
  - `child_code` — [`L35`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L35)
  - `child_id` — [`L31`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L31)
  - `child_metrics` — [`L33`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L33)
  - `code_diff` — [`L38`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L38)
  - `generation` — [`L43`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L43)
  - `improvement_delta` — [`L41`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L41)
  - `island_id` — [`L42`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L42)
  - `iteration` — [`L28`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L28)
  - `llm_response` — [`L40`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L40)
  - `metadata` — [`L45`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L45)
  - `parent_changes_description` — [`L36`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L36)
  - `parent_code` — [`L34`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L34)
  - `parent_id` — [`L30`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L30)
  - `parent_metrics` — [`L32`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L32)
  - `prompt` — [`L39`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L39)
  - `timestamp` — [`L29`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L29)
- used by: [`log_trace`](evolution_trace.md#EvolutionTracer.log_trace), [`extract_evolution_trace_from_checkpoint`](evolution_trace.md#extract_evolution_trace_from_checkpoint), [`_update_stats`](evolution_trace.md#EvolutionTracer._update_stats), [`buffer`](evolution_trace.md#EvolutionTracer.buffer)  (7 test-only)

### `EvolutionTracer`
- def: [`openevolve/evolution_trace.py:63`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L63)
- doc: Manages evolution trace logging with support for multiple formats
- signature: `class EvolutionTracer:`
- members:
  - `__enter__(self)` — [`L311`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L311) — Context manager entry
  - `__exit__(self, exc_type, exc_val, exc_tb)` — [`L315`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L315) — Context manager exit — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `__init__(self, output_path: Optional[str] = None, format: str = "jsonl", include_code: bool = False, include_prompts: bool = True, enabled: bool = True, buffer_size: int = 10, compress: bool = False, include_changes_description: bool = True)` — [`L66`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L66) — Initialize the evolution tracer
  - `_update_stats(self, trace: EvolutionTrace)` — [`L210`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L210) — Update running statistics — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `close(self)` — [`L271`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L271) — Close the tracer and flush remaining data — documented in [openevolve-controller](../../concepts/openevolve-controller.md)
  - `flush(self)` — [`L235`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L235) — Write buffered traces to file — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `get_statistics(self)` — [`L260`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L260) — Get current tracing statistics — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `log_trace(self, iteration: int, parent_program: Any, child_program: Any, prompt: Optional[Dict[str, str]] = None, llm_response: Optional[str] = None, artifacts: Optional[Dict[str, Any]] = None, island_id: Optional[int] = None, metadata: Optional[Dict[str, Any]] = None)` — [`L133`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L133) — Log an evolution trace entry — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `buffer` — [`L125`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L125) — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `buffer_size` — [`L96`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L96)
  - `compress` — [`L95`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L95)
  - `enabled` — [`L90`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L90)
  - `format` — [`L91`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L91)
  - `include_changes_description` — [`L94`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L94)
  - `include_code` — [`L92`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L92)
  - `include_prompts` — [`L93`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L93)
  - `json_traces` — [`L129`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L129) — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `output_path` — [`L113`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L113)
  - `stats` — [`L99`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L99) — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
- uses (calls/refs, reference-scoped): [`logger`](evolution_trace.md#logger), [`export_traces`](utils/trace_export_utils.md#export_traces), [`EvolutionTrace`](evolution_trace.md#EvolutionTrace), [`calculate_improvement`](evolution_trace.md#EvolutionTrace.calculate_improvement), [`child_metrics`](evolution_trace.md#EvolutionTrace.child_metrics), [`iteration`](evolution_trace.md#EvolutionTrace.iteration), [`parent_metrics`](evolution_trace.md#EvolutionTrace.parent_metrics), [`child_id`](evolution_trace.md#EvolutionTrace.child_id), [`parent_id`](evolution_trace.md#EvolutionTrace.parent_id), [`export_traces_json`](utils/trace_export_utils.md#export_traces_json), [`improvement_delta`](evolution_trace.md#EvolutionTrace.improvement_delta), [`parent_code`](evolution_trace.md#EvolutionTrace.parent_code), [`timestamp`](evolution_trace.md#EvolutionTrace.timestamp), [`child_code`](evolution_trace.md#EvolutionTrace.child_code), [`generation`](evolution_trace.md#EvolutionTrace.generation), [`island_id`](evolution_trace.md#EvolutionTrace.island_id), [`append_trace_jsonl`](utils/trace_export_utils.md#append_trace_jsonl), [`child_changes_description`](evolution_trace.md#EvolutionTrace.child_changes_description), [`llm_response`](evolution_trace.md#EvolutionTrace.llm_response), [`metadata`](evolution_trace.md#EvolutionTrace.metadata), [`parent_changes_description`](evolution_trace.md#EvolutionTrace.parent_changes_description), [`prompt`](evolution_trace.md#EvolutionTrace.prompt), [`artifacts`](evolution_trace.md#EvolutionTrace.artifacts)
- used by: [`run`](controller.md#OpenEvolve.run), [`evolution_tracer`](controller.md#OpenEvolve.evolution_tracer)  (7 test-only)

## Functions
- `extract_evolution_trace_from_checkpoint(checkpoint_dir: Union[str, Path], output_path: Optional[str] = None, format: str = "jsonl", include_code: bool = True, include_prompts: bool = True, include_changes_description: bool = True)` — [`L320`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L320) — Extract evolution traces from an existing checkpoint directory — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
- `extract_full_lineage_traces(checkpoint_dir: Union[str, Path], output_path: Optional[str] = None, format: str = "json")` — [`L439`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L439) — Extract complete evolution traces with full lineage chains and prompts/actions

## Module values
- `logger` — [`L21`](../../../../../raw/code/openevolve/openevolve/evolution_trace.py#L21)


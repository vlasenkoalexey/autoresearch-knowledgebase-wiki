---
title: 'Module: OpenMLE-ERL/RL/airaevo_experience.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/RL/airaevo_experience.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.RL.airaevo_experience`/
symbols:
  build_experience_card: build_experience_card().
  compute_parent_utilities: compute_parent_utilities().
  build_operator_experience_memory: build_operator_experience_memory().
  program_selection_score: program_selection_score().
  is_success_program: is_success_program().
  error_signature: error_signature().
  _card: _card().
  _append_section: _append_section().
  _recent_ancestors: _recent_ancestors().
  _memory_node_lines: _memory_node_lines().
  detect_method_family.add: detect_method_family().add().
  parent_ids: parent_ids().
  _metadata: _metadata().
  _program_id: _program_id().
  _format_value: _format_value().
  compact_text: compact_text().
  is_debug_candidate: is_debug_candidate().
  finite_float: finite_float().
  _sort_programs.key: _sort_programs().key().
  _children_of: _children_of().
  build_strategy_board: build_strategy_board().
  _status_text: _status_text().
  _index: _index().
  status_is_failure: status_is_failure().
  _sort_programs: _sort_programs().
  detect_method_family: detect_method_family().
  _rich_summary_lines: _rich_summary_lines().
  _positive_delta: _positive_delta().
  _family_count_before: _family_count_before().
  parse_json_object: parse_json_object().
  FAILED_STATUSES: FAILED_STATUSES.
  DEFAULT_PARENT_UTILITY_WEIGHTS: DEFAULT_PARENT_UTILITY_WEIGHTS.
  extract_imports: extract_imports().
  _normalize_values: _normalize_values().
  _normalize_positive: _normalize_positive().
  softmax: softmax().
  SUCCESS_STATUSES: SUCCESS_STATUSES.
---
# Module: [`OpenMLE-ERL/RL/airaevo_experience.py`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py)

## Functions
- `_append_section(lines: list[str], title: str, prefix: str, programs: list[Any], all_programs: list[Any])` — [`L518`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L518) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `_card(program: Any, all_programs: list[Any])` — [`L304`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L304) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `_children_of(parent: Any, all_programs: list[Any])` — [`L445`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L445) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `_family_count_before(method_family: str, previous_cards: list[dict[str, Any]], node_id: str | None = None)` — [`L225`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L225) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `_format_value(value: Any)` — [`L476`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L476)
- `_index(programs: Iterable[Any])` — [`L192`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L192)
- `_memory_node_lines(prefix: str, program: Any, all_programs: list[Any])` — [`L501`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L501) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `_metadata(program: Any)` — [`L49`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L49) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `_normalize_positive(values: list[float | None])` — [`L331`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L331) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `_normalize_values(values: list[float | None], lower_is_better: bool)` — [`L312`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L312) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `_positive_delta(child_score: float | None, parent_score: float | None, lower_is_better: bool)` — [`L201`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L201) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `_program_id(program: Any)` — [`L184`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L184) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `_recent_ancestors(program: Any, all_programs: list[Any], max_items: int)` — [`L424`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L424) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `_rich_summary_lines(prefix: str, card: dict[str, Any])` — [`L485`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L485)
- `_sort_programs(programs: Iterable[Any], lower_is_better: bool = False)` — [`L414`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L414)
- `_status_text(program: Any)` — [`L73`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L73) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `add(name: str)` — [`L136`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L136)
- `build_experience_card(program: Any, *, all_programs: Iterable[Any] | None = None, lower_is_better: bool = False)` — [`L235`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L235) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `build_operator_experience_memory(operator: str, parent_programs: list[Any], *, all_programs: Iterable[Any], current_program: Any | None = None, lower_is_better: bool = False, max_related_cards: int = 3, ancestor_k: int | None = None, sibling_k: int | None = None)` — [`L527`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L527) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `build_strategy_board(programs: list[Any], lower_is_better: bool = False)` — [`L452`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L452) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `compact_text(value: Any, max_chars: int = 240)` — [`L42`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L42)
- `compute_parent_utilities(candidates: list[Any], *, all_programs: Iterable[Any], lower_is_better: bool = False, temperature: float = 1, weights: dict[str, float] | None = None)` — [`L352`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L352) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `detect_method_family(code: str, imports: Iterable[str] | None = None)` — [`L131`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L131) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `error_signature(program: Any)` — [`L207`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L207) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `extract_imports(code: str)` — [`L115`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L115) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `finite_float(value: Any)` — [`L32`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L32)
- `is_debug_candidate(program: Any)` — [`L110`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L110)
- `is_success_program(program: Any)` — [`L97`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L97) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `key(program: Any)` — [`L415`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L415)
- `parent_ids(program: Any)` — [`L165`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L165) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `parse_json_object(text: str)` — [`L639`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L639)
- `program_selection_score(program: Any)` — [`L54`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L54) — Return the test-reward fitness signal used by RL AIRA-Evo selection. — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `softmax(values: list[float], temperature: float = 1)` — [`L339`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L339) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `status_is_failure(status: str)` — [`L88`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L88) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)

## Module values
- `DEFAULT_PARENT_UTILITY_WEIGHTS` — [`L29`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L29) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `FAILED_STATUSES` — [`L16`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L16)
- `SUCCESS_STATUSES` — [`L28`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/airaevo_experience.py#L28)


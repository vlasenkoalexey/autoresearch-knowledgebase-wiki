---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.solvers.evo.experience`/
symbols:
  compute_parent_utilities: compute_parent_utilities().
  collect_operator_memory_nodes: collect_operator_memory_nodes().
  build_operator_experience_memory: build_operator_experience_memory().
  _config_get: _config_get().
  build_experience_card: build_experience_card().
  _card_for_node: _card_for_node().
  _build_improve_experience_memory: _build_improve_experience_memory().
  _build_debug_experience_memory: _build_debug_experience_memory().
  prompt_memory_operator_k: prompt_memory_operator_k().
  _format_value: _format_value().
  _build_crossover_experience_memory: _build_crossover_experience_memory().
  _status_indicates_success: _status_indicates_success().
  _append_memory_node_section: _append_memory_node_section().
  _official_score_value: _official_score_value().
  _node_id: _node_id().
  _horizontal_siblings: _horizontal_siblings().
  prompt_memory_enabled: prompt_memory_enabled().
  _normalize_values: _normalize_values().
  prompt_memory_max_related_cards: prompt_memory_max_related_cards().
  prompt_memory_sibling_rank_weights: prompt_memory_sibling_rank_weights().
  _finite_float: _finite_float().
  detect_method_family.add: detect_method_family().add().
  _metric_value: _metric_value().
  _has_official_score: _has_official_score().
  _component_normalization_config: _component_normalization_config().
  _normalize_positive_deltas: _normalize_positive_deltas().
  build_strategy_board: build_strategy_board().
  _dedupe_nodes: _dedupe_nodes().
  prompt_memory_use_base_memory: prompt_memory_use_base_memory().
  _memory_node_lines: _memory_node_lines().
  _official_status: _official_status().
  _card_indicates_failure: _card_indicates_failure().
  _rank_nodes_by_utility: _rank_nodes_by_utility().
  append_experience_memory: append_experience_memory().
  _status_is_failure: _status_is_failure().
  detect_method_family: detect_method_family().
  _family_stats_line: _family_stats_line().
  detect_error_signature: detect_error_signature().
  _collect_attached_cards: _collect_attached_cards().
  _journal_nodes: _journal_nodes().
  _recent_ancestors: _recent_ancestors().
  _rich_summary_lines: _rich_summary_lines().
  _current_error_signature: _current_error_signature().
  _normalization_mode: _normalization_mode().
  _metric_info: _metric_info().
  _hybrid_minmax_weight: _hybrid_minmax_weight().
  _compact_text: _compact_text().
  extract_imports: extract_imports().
  _format_repeated_errors: _format_repeated_errors().
  _normalize_rank_values: _normalize_rank_values().
  _positive_delta: _positive_delta().
  _coerce_status_code: _coerce_status_code().
  _normalized_status: _normalized_status().
  _family_count_before: _family_count_before().
  _node_card: _node_card().
  DEFAULT_PARENT_UTILITY_WEIGHTS: DEFAULT_PARENT_UTILITY_WEIGHTS.
  DEFAULT_PARENT_COMPONENT_NORMALIZATION: DEFAULT_PARENT_COMPONENT_NORMALIZATION.
  FAILED_STATUSES: FAILED_STATUSES.
  SUCCESS_STATUSES: SUCCESS_STATUSES.
  _normalize_minmax_values: _normalize_minmax_values().
  _parent_steps: _parent_steps().
  _format_list: _format_list().
  softmax: softmax().
  load_experience_cards: load_experience_cards().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py)

## Functions
- `_append_memory_node_section(lines: list[str], title: str, prefix: str, nodes: list[Any], cards: list[dict[str, Any]])` — [`L858`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L858)
- `_build_crossover_experience_memory(parent_nodes: list[Any], cards: list[dict[str, Any]], board: dict[str, Any], sections: dict[str, list[Any]])` — [`L945`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L945)
- `_build_debug_experience_memory(parent_nodes: list[Any], cards: list[dict[str, Any]], board: dict[str, Any], current_node: Any | None, max_related_cards: int, sections: dict[str, list[Any]])` — [`L991`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L991)
- `_build_improve_experience_memory(parent_nodes: list[Any], cards: list[dict[str, Any]], board: dict[str, Any], sections: dict[str, list[Any]])` — [`L911`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L911)
- `_card_for_node(node: Any, cards: list[dict[str, Any]])` — [`L796`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L796)
- `_card_indicates_failure(card: dict[str, Any])` — [`L358`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L358)
- `_coerce_status_code(status_code: Any)` — [`L334`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L334)
- `_collect_attached_cards(journal: Any | None, nodes: Iterable[Any] | None = None)` — [`L591`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L591)
- `_compact_text(value: Any, max_chars: int = 240)` — [`L235`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L235)
- `_component_normalization_config(config: dict[str, Any] | None)` — [`L149`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L149)
- `_config_get(config: Any, key: str, default: Any = None)` — [`L1090`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L1090)
- `_current_error_signature(current_node: Any | None)` — [`L894`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L894)
- `_dedupe_nodes(nodes: Iterable[Any])` — [`L610`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L610)
- `_family_count_before(method_family: str, previous_cards: list[dict[str, Any]], node_id: str | None = None)` — [`L369`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L369)
- `_family_stats_line(label: str, family: str, board: dict[str, Any])` — [`L874`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L874)
- `_finite_float(value: Any)` — [`L36`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L36)
- `_format_list(values: Iterable[Any], *, empty: str = "none")` — [`L251`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L251)
- `_format_repeated_errors(repeated_errors: dict[str, Any])` — [`L886`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L886)
- `_format_value(value: Any)` — [`L242`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L242)
- `_has_official_score(node: Any)` — [`L73`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L73)
- `_horizontal_siblings(node: Any, journal: Any | None, *, lower_is_better: bool, cards: list[dict[str, Any]], max_siblings: int, sibling_rank_weights: dict[str, float] | None = None)` — [`L663`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L663)
- `_hybrid_minmax_weight(value: Any, default: float = 0.5)` — [`L141`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L141)
- `_journal_nodes(journal: Any | None, extra_nodes: Iterable[Any] | None = None)` — [`L622`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L622)
- `_memory_node_lines(prefix: str, card: dict[str, Any])` — [`L841`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L841)
- `_metric_info(node: Any)` — [`L51`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L51)
- `_metric_value(node: Any)` — [`L46`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L46)
- `_node_card(node: Any)` — [`L584`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L584)
- `_node_id(node: Any)` — [`L606`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L606)
- `_normalization_mode(value: Any, default: str = "minmax")` — [`L130`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L130)
- `_normalize_minmax_values(values: list[float | None], lower_is_better: bool)` — [`L82`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L82)
- `_normalize_positive_deltas(positive_deltas: list[float], *, mode: str = "minmax", hybrid_minmax_weight: float = 0.5)` — [`L181`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L181)
- `_normalize_rank_values(values: list[float | None], lower_is_better: bool)` — [`L102`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L102)
- `_normalize_values(values: list[float | None], lower_is_better: bool, *, mode: str = "minmax", hybrid_minmax_weight: float = 0.5)` — [`L158`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L158)
- `_normalized_status(status: str | None)` — [`L343`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L343)
- `_official_score_value(node: Any)` — [`L62`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L62)
- `_official_status(node: Any)` — [`L58`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L58)
- `_parent_steps(node: Any)` — [`L218`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L218)
- `_positive_delta(child_score: float | None, parent_score: float | None, lower_is_better: bool)` — [`L211`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L211)
- `_rank_nodes_by_utility(nodes: list[Any], *, lower_is_better: bool, cards: list[dict[str, Any]], weights: dict[str, float] | None = None)` — [`L626`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L626)
- `_recent_ancestors(node: Any, max_depth: int)` — [`L645`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L645)
- `_rich_summary_lines(prefix: str, card: dict[str, Any])` — [`L819`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L819)
- `_status_indicates_success(status: str | None, status_code: Any)` — [`L347`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L347)
- `_status_is_failure(status: str)` — [`L231`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L231)
- `add(name: str)` — [`L277`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L277)
- `append_experience_memory(memory: str | None, experience_memory: str)` — [`L1080`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L1080)
- `build_experience_card(*, node: Any, step_index: int, generation_id: int, lower_is_better: bool, previous_cards: list[dict[str, Any]], step_stat: dict[str, Any], usage: dict[str, Any] | None = None, clear_run_log: str = "", raw_run_log: str = "")` — [`L379`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L379)
- `build_operator_experience_memory(operator: str, parent_nodes: list[Any], *, journal: Any | None, lower_is_better: bool, current_node: Any | None = None, max_related_cards: int = 3, ancestor_k: int | None = None, sibling_k: int | None = None, sibling_rank_weights: dict[str, float] | None = None)` — [`L1035`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L1035)
- `build_strategy_board(cards: list[dict[str, Any]], lower_is_better: bool)` — [`L450`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L450)
- `collect_operator_memory_nodes(operator: str, parent_nodes: list[Any], *, journal: Any | None, lower_is_better: bool, current_node: Any | None = None, ancestor_k: int | None = None, sibling_k: int | None = None, sibling_rank_weights: dict[str, float] | None = None, max_related_cards: int = 8)` — [`L704`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L704) — Select the small targeted memory set used by one operator call.
- `compute_parent_utilities(nodes: list[Any], *, lower_is_better: bool, previous_cards: list[dict[str, Any]] | None = None, weights: dict[str, float] | None = None, component_normalization: dict[str, Any] | None = None, temperature: float = 1)` — [`L1152`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L1152)
- `detect_error_signature(status: str | None, status_code: int | None, raw_run_log: str, clear_run_log: str)` — [`L305`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L305)
- `detect_method_family(code: str, imports: Iterable[str] | None = None)` — [`L272`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L272)
- `extract_imports(code: str)` — [`L256`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L256)
- `load_experience_cards(output_dir: Path)` — [`L1266`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L1266)
- `prompt_memory_enabled(cfg: Any)` — [`L1098`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L1098)
- `prompt_memory_max_related_cards(cfg: Any, operator: str | None = None)` — [`L1106`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L1106)
- `prompt_memory_operator_k(cfg: Any, operator: str, key: str, default: int)` — [`L1129`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L1129)
- `prompt_memory_sibling_rank_weights(cfg: Any)` — [`L1139`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L1139)
- `prompt_memory_use_base_memory(cfg: Any)` — [`L1123`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L1123)
- `softmax(values: list[float], temperature: float = 1)` — [`L1253`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L1253)

## Module values
- `DEFAULT_PARENT_COMPONENT_NORMALIZATION` — [`L16`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L16)
- `DEFAULT_PARENT_UTILITY_WEIGHTS` — [`L10`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L10)
- `FAILED_STATUSES` — [`L22`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L22)
- `SUCCESS_STATUSES` — [`L33`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/experience.py#L33)


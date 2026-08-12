---
title: 'Module: OpenMLE-Gym/openmle_gym/local_evaluator.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/openmle_gym/local_evaluator.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.openmle_gym.local_evaluator`/
symbols:
  evaluate_tasks: evaluate_tasks().
  evaluate_tasks.evaluate_one: evaluate_tasks().evaluate_one().
  analyze_task_structure: analyze_task_structure().
  _evaluate_with_ai: _evaluate_with_ai().
  _evaluate_with_openai: _evaluate_with_openai().
  _finding: _finding().
  _evaluate_task: _evaluate_task().
  _chunked_map: _chunked_map().
  evaluate_tasks.evaluate_one_safe: evaluate_tasks().evaluate_one_safe().
  _inspect_csv: _inspect_csv().
  _validate_ai_quality: _validate_ai_quality().
  _failed_task_result: _failed_task_result().
  _deterministic_validation: _deterministic_validation().
  _chunked_map.process_chunk: _chunked_map().process_chunk().
  R: R.
  evaluation_has_task_failures: evaluation_has_task_failures().
  _build_raw_usage_evidence: _build_raw_usage_evidence().
  T: T.
  _directory_size: _directory_size().
  _is_identifier_column: _is_identifier_column().
  _extract_json_response: _extract_json_response().
  _message_text: _message_text().
  _preview_cell: _preview_cell().
  _hard_gate_quality: _hard_gate_quality().
  _get_anthropic_client: _get_anthropic_client().
  QUALITY_DIMENSIONS: QUALITY_DIMENSIONS.
  _read_overview_rows: _read_overview_rows().
---
# Module: [`OpenMLE-Gym/openmle_gym/local_evaluator.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py)

## Functions
- `_build_raw_usage_evidence(result: dict[str, Any])` — [`L279`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L279)
- `_chunked_map(items: list[T], worker_count: int, func: Callable[[T], R])` — [`L853`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L853) — Run work in deterministic chunks and return results in input order.
- `_deterministic_validation(result: dict[str, Any])` — [`L342`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L342)
- `_directory_size(path: Path)` — [`L89`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L89)
- `_evaluate_task(root_dir: str, task: str, overview: dict[str, str], local_only: bool, skip_llm: bool, metric_execution_mode: str = "process", metric_timeout: float = 120)` — [`L887`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L887)
- `_evaluate_with_ai(task_info: dict[str, Any])` — [`L745`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L745)
- `_evaluate_with_openai(prompt: str)` — [`L624`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L624)
- `_extract_json_response(text: str)` — [`L572`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L572)
- `_failed_task_result(task: str, task_path: Path, reason: str)` — [`L934`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L934)
- `_finding(finding_id: str, message: str, *, evidence_source: str, evidence: str)` — [`L253`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L253)
- `_get_anthropic_client()` — [`L598`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L598)
- `_hard_gate_quality(validation: dict[str, Any])` — [`L553`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L553)
- `_inspect_csv(path: Path, max_preview_rows: int = 10, *, profile_first_column: bool = True)` — [`L40`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L40)
- `_is_identifier_column(name: str)` — [`L270`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L270)
- `_message_text(content: Any)` — [`L581`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L581)
- `_preview_cell(value: str, max_chars: int = 300)` — [`L33`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L33)
- `_read_overview_rows(path: Path)` — [`L844`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L844)
- `_validate_ai_quality(value: Any)` — [`L663`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L663)
- `analyze_task_structure(task_dir: str | Path, metric_execution_mode: str = "process", metric_timeout: float = 120)` — [`L102`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L102)
- `evaluate_one(item: tuple[int, str, Path, str | None, bool])` — [`L1051`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L1051) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)
- `evaluate_one_safe(item: tuple[int, str, Path, str | None, bool])` — [`L1112`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L1112)
- `evaluate_tasks(root_dir: str | Path, task_list: str | Path, output_dir: str | Path, local_only: bool = False, skip_llm: bool = False, overview_csv: str | Path | None = None, workers: int = 1, execution_mode: str = "process", task_timeout: float = 600)` — [`L1000`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L1000)
- `evaluation_has_task_failures(paths: dict[str, Path])` — [`L987`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L987)
- `process_chunk(chunk: list[tuple[int, T]])` — [`L873`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L873)

## Module values
- `QUALITY_DIMENSIONS` — [`L654`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L654)
- `R` — [`L30`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L30)
- `T` — [`L29`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/local_evaluator.py#L29)


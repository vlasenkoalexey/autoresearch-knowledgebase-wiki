---
title: 'Module: polyglot/run_evaluation.py'
type: catalog
provenance: extracted
module: polyglot/run_evaluation.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `polyglot.run_evaluation`/
symbols:
  run_instance: run_instance().
  main: main().
  parser: parser.
  args: args.
  EvaluationError.__str__: EvaluationError#__str__().
  run_instances: run_instances().
  make_run_report: make_run_report().
  EvaluationError: EvaluationError#
  EvaluationError.super_str: EvaluationError#super_str.
  EvaluationError.instance_id: EvaluationError#instance_id.
  EvaluationError.log_file: EvaluationError#log_file.
  get_dataset_from_preds: get_dataset_from_preds().
  get_gold_predictions: get_gold_predictions().
  EvaluationError.__init__: EvaluationError#__init__().
  EvaluationError.logger: EvaluationError#logger.
---
# Module: [`polyglot/run_evaluation.py`](../../../../../raw/code/dgm/polyglot/run_evaluation.py)

## Classes
### `EvaluationError`  ·  implements/extends Exception
- def: [`polyglot/run_evaluation.py:41`](../../../../../raw/code/dgm/polyglot/run_evaluation.py#L41)
- signature: `class EvaluationError(Exception):`
- members:
  - `instance_id` — [`L45`](../../../../../raw/code/dgm/polyglot/run_evaluation.py#L45)
  - `log_file` — [`L46`](../../../../../raw/code/dgm/polyglot/run_evaluation.py#L46)
  - `logger` — [`L47`](../../../../../raw/code/dgm/polyglot/run_evaluation.py#L47)
  - `super_str` — [`L44`](../../../../../raw/code/dgm/polyglot/run_evaluation.py#L44)
- protocol/private: `__init__`[`L42`](../../../../../raw/code/dgm/polyglot/run_evaluation.py#L42), `__str__`[`L49`](../../../../../raw/code/dgm/polyglot/run_evaluation.py#L49)
- used by: [`run_instance`](run_evaluation.md#run_instance)

## Functions
- `get_dataset_from_preds(dataset_name: str, split: str, instance_ids: list, predictions: dict, run_id: str, exclude_completed: bool = True)` — [`L291`](../../../../../raw/code/dgm/polyglot/run_evaluation.py#L291) — Return only instances that have predictions and are in the dataset.
- `get_gold_predictions(dataset_name: str, split: str)` — [`L473`](../../../../../raw/code/dgm/polyglot/run_evaluation.py#L473) — Get gold predictions for the given dataset and split.
- `main(dataset_name: str, split: str, instance_ids: list, predictions_path: str, max_workers: int, force_rebuild: bool, cache_level: str, clean: bool, open_file_limit: int, run_id: str, timeout: int)` — [`L487`](../../../../../raw/code/dgm/polyglot/run_evaluation.py#L487) — Run evaluation harness for the given dataset and predictions. — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `make_run_report(predictions: dict, full_dataset: list, client: docker.DockerClient, run_id: str)` — [`L355`](../../../../../raw/code/dgm/polyglot/run_evaluation.py#L355) — Make a final evaluation and run report of the instances that have been run.
- `run_instance(test_spec: TestSpec, pred: dict, rm_image: bool, force_rebuild: bool, client: docker.DockerClient, run_id: str, timeout: int | None = None)` — [`L56`](../../../../../raw/code/dgm/polyglot/run_evaluation.py#L56) — Run a single instance with the given prediction. — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `run_instances(predictions: dict, instances: list, cache_level: str, clean: bool, force_rebuild: bool, max_workers: int, run_id: str, timeout: int)` — [`L221`](../../../../../raw/code/dgm/polyglot/run_evaluation.py#L221) — Run all instances for the given predictions in parallel.

## Module values
- `args` — [`L567`](../../../../../raw/code/dgm/polyglot/run_evaluation.py#L567)
- `parser` — [`L541`](../../../../../raw/code/dgm/polyglot/run_evaluation.py#L541)


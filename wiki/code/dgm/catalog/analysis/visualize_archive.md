---
title: 'Module: analysis/visualize_archive.py'
type: catalog
provenance: extracted
module: analysis/visualize_archive.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `analysis.visualize_archive`/
symbols:
  build_graph: build_graph().
  main: main().
  to_eval_quantity_enum: to_eval_quantity_enum().
  get_performance_score: get_performance_score().
  create_plotly_figure: create_plotly_figure().
  visualize_experiment_run: visualize_experiment_run().
  visualize_experiment_run_halluc: visualize_experiment_run_halluc().
  EvalQuantity: EvalQuantity#
  analyse_experiment_run: analyse_experiment_run().
  analyse_experiment_run_halluc: analyse_experiment_run_halluc().
  get_evalswe_command: get_evalswe_command().
  get_evalquantity: get_evalquantity().
  EvalQuantity.SMALL: EvalQuantity#SMALL.
  get_parent_commit: get_parent_commit().
  get_hallucination_score: get_hallucination_score().
  EvalQuantity.MED: EvalQuantity#MED.
  EvalQuantity.BIG: EvalQuantity#BIG.
---
# Module: [`analysis/visualize_archive.py`](../../../../../raw/code/dgm/analysis/visualize_archive.py)

## Classes
### `EvalQuantity`
- def: [`analysis/visualize_archive.py:11`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L11) — documented in [analysis-visualize_archive](../../concepts/analysis-visualize_archive.md)
- signature: `class EvalQuantity:`
- members:
  - `BIG` — [`L14`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L14)
  - `MED` — [`L13`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L13)
  - `SMALL` — [`L12`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L12)
- used by: [`to_eval_quantity_enum`](visualize_archive.md#to_eval_quantity_enum), [`create_plotly_figure`](visualize_archive.md#create_plotly_figure)

## Functions
- `analyse_experiment_run(dgm_dir, archives, metadata_name="metadata.json")` — [`L373`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L373) — Analyse the experiment run (using accuracy_score) and print some statistics. — documented in [analysis-visualize_archive](../../concepts/analysis-visualize_archive.md)
- `analyse_experiment_run_halluc(dgm_dir, archives, metadata_name="metadata.json")` — [`L436`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L436) — Analyse the experiment run (using solved_halluc_score + percent_toolutilized if solved=1) — documented in [analysis-visualize_archive](../../concepts/analysis-visualize_archive.md)
- `build_graph(dgm_dir, archives, score_func, metadata_name="metadata.json")` — [`L92`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L92) — Generic helper to build a DiGraph with node attributes from the archives. — documented in [analysis-visualize_archive](../../concepts/analysis-visualize_archive.md)
- `create_plotly_figure(graph, pos, html_path, colorbar_title="Score")` — [`L166`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L166) — Given a graph and node positions (pos), — documented in [analysis-visualize_archive](../../concepts/analysis-visualize_archive.md)
- `get_evalquantity(dgm_dir, node_id, metadata_name="metadata.json", halluc=False)` — [`L31`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L31) — Retrieve the eval_quantity from the metadata of a node. — documented in [analysis-visualize_archive](../../concepts/analysis-visualize_archive.md)
- `get_evalswe_command(dgm_dir, node_id)` — [`L356`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L356) — Generate the command to evaluate a node on the SWE-bench dataset. — documented in [analysis-visualize_archive](../../concepts/analysis-visualize_archive.md)
- `get_hallucination_score(dgm_dir, node_id, metadata_name="metadata.json")` — [`L70`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L70) — Retrieve the 'solved_halluc_score' and, if it's 1, add the 'percent_toolutilized' from — documented in [analysis-visualize_archive](../../concepts/analysis-visualize_archive.md)
- `get_parent_commit(dgm_dir, child_node_id, metadata_name="metadata.json")` — [`L44`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L44) — Retrieve the parent commit from the metadata of a child node. — documented in [analysis-visualize_archive](../../concepts/analysis-visualize_archive.md)
- `get_performance_score(dgm_dir, node_id, metadata_name="metadata.json")` — [`L56`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L56) — Retrieve the accuracy_score from the metadata of a node. — documented in [analysis-visualize_archive](../../concepts/analysis-visualize_archive.md)
- `main()` — [`L503`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L503) — documented in [analysis-visualize_archive](../../concepts/analysis-visualize_archive.md)
- `to_eval_quantity_enum(eval_quantity, halluc=False)` — [`L16`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L16) — documented in [analysis-visualize_archive](../../concepts/analysis-visualize_archive.md)
- `visualize_experiment_run(dgm_dir, archives, metadata_name="metadata.json")` — [`L324`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L324) — Visualize the experiment run as a directed tree-like graph (using accuracy_score). — documented in [analysis-visualize_archive](../../concepts/analysis-visualize_archive.md)
- `visualize_experiment_run_halluc(dgm_dir, archives, metadata_name="metadata.json")` — [`L339`](../../../../../raw/code/dgm/analysis/visualize_archive.py#L339) — Visualize the experiment run as a directed tree-like graph (using the — documented in [analysis-visualize_archive](../../concepts/analysis-visualize_archive.md)


---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.core.solvers.utils.metric`/
symbols:
  MetricValue.value: MetricValue#value.
  MetricValue: MetricValue#
  MetricValue.info: MetricValue#info.
  MetricValue.maximize: MetricValue#maximize.
  WorstMetricValue: WorstMetricValue#
  MetricValue.__str__: MetricValue#__str__().
  MetricValue.__gt__: MetricValue#__gt__().
  MetricValue.get_value: MetricValue#get_value().
  MetricValue.value_npsafe: MetricValue#value_npsafe().
  MetricValue.__post_init__: MetricValue#__post_init__().
  MetricValue.__eq__: MetricValue#__eq__().
  MetricValue.is_worst: MetricValue#is_worst().
  MetricValue.add_value: MetricValue#add_value().
  WorstMetricValue.__repr__: WorstMetricValue#__repr__().
  WorstMetricValue.__str__: WorstMetricValue#__str__().
  MetricValue.__repr__: MetricValue#__repr__().
  WorstMetricValue.value: WorstMetricValue#value.
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py)

## Classes
### `MetricValue`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py:23`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L23)
- doc: Represents the value of a metric to be optimized, which can be compared to other metric values.
- signature: `class MetricValue(DataClassJsonMixin):`
- members:
  - `__gt__(self, other)` — [`L38`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L38) — True if self is a _better_ (not necessarily larger) metric value than other
  - `add_value(self, add_value: float)` — [`L84`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L84)
  - `get_value(self)` — [`L78`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L78)
  - `is_worst(self)` — [`L69`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L69) — True if the metric value is the worst possible value.
  - `value_npsafe(self)` — [`L74`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L74)
  - `info` — [`L31`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L31)
  - `maximize` — [`L30`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L30)
  - `value` — [`L29`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L29)
- protocol/private: `__eq__`[`L53`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L53), `__post_init__`[`L33`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L33), `__repr__`[`L56`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L56), `__str__`[`L59`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L59)
- uses (calls/refs, reference-scoped): [`WorstMetricValue`](metric.md#WorstMetricValue)
- used by: [`test_export_and_reconstruct_search_data`](search_exporter.md#test_export_and_reconstruct_search_data), [`metric`](journal.md#Node.metric), [`from_export_data`](journal.md#Journal.from_export_data), [`get_node_data`](journal.md#Journal.get_node_data), [`parse_eval_result`](../../../solvers/evo/evo.md#Evolutionary.parse_eval_result), [`parse_eval_result`](../../../solvers/mcts/mcts.md#MCTS.parse_eval_result), [`parse_eval_result`](../../../solvers/greedy/greedy.md#Greedy.parse_eval_result), [`_expand_leaf_and_backprop`](../../../solvers/mcts/mcts.md#MCTS._expand_leaf_and_backprop), [`add_nodes_to_islands`](../../../solvers/evo/evo.md#SolutionsDatabase.add_nodes_to_islands), [`debug_cycle`](../../../solvers/mcts/mcts.md#MCTS.debug_cycle), [`create_root_node`](../../../solvers/greedy/greedy.md#Greedy.create_root_node), [`cfg_to_tree_struct`](tree_export.md#cfg_to_tree_struct), [`create_root_node`](../../../solvers/evo/evo.md#Evolutionary.create_root_node), [`calculate_tree_statistics`](../../../analysis_utils/meta_tree_analysis.md#calculate_tree_statistics), [`debug_cycle`](../../../solvers/evo/evo.md#Evolutionary.debug_cycle), [`_build_solution_database_from_journal`](../../../solvers/evo/evo.md#Evolutionary._build_solution_database_from_journal), [`create_root_node`](../../../solvers/mcts/mcts.md#MCTS.create_root_node), [`register_node_in_island`](../../../solvers/evo/evo.md#Island.register_node_in_island), [`generate_summary`](journal.md#Journal.generate_summary), [`only_keep_best`](../../../solvers/evo/evo.md#Island.only_keep_best), [`get_best_node`](journal.md#Journal.get_best_node), [`get_node_summary`](../operators/memory.md#get_node_summary), [`seed_islands_with_nodes`](../../../solvers/evo/evo.md#SolutionsDatabase.seed_islands_with_nodes), [`WorstMetricValue`](metric.md#WorstMetricValue), [`fitness_scores`](../../../solvers/evo/evo.md#Island.fitness_scores), [`get_metric_history`](journal.md#Journal.get_metric_history), [`__repr__`](metric.md#WorstMetricValue.__repr__), [`__str__`](metric.md#WorstMetricValue.__str__)

### `WorstMetricValue`  ·  implements/extends MetricValue
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py:91`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L91)
- doc: Represents an invalid metric value, e.g. when the agent creates a buggy solution.
- signature: `class WorstMetricValue(MetricValue):`
- members:
  - `value` — [`L97`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L97)
- protocol/private: `__repr__`[`L99`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L99), `__str__`[`L102`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/metric.py#L102)
- uses (calls/refs, reference-scoped): [`MetricValue`](metric.md#MetricValue), [`__str__`](metric.md#MetricValue.__str__), [`__repr__`](metric.md#MetricValue.__repr__)
- used by: [`from_export_data`](journal.md#Journal.from_export_data), [`get_node_data`](journal.md#Journal.get_node_data), [`parse_eval_result`](../../../solvers/evo/evo.md#Evolutionary.parse_eval_result), [`parse_eval_result`](../../../solvers/mcts/mcts.md#MCTS.parse_eval_result), [`parse_eval_result`](../../../solvers/greedy/greedy.md#Greedy.parse_eval_result), [`create_root_node`](../../../solvers/greedy/greedy.md#Greedy.create_root_node), [`create_root_node`](../../../solvers/evo/evo.md#Evolutionary.create_root_node), [`create_root_node`](../../../solvers/mcts/mcts.md#MCTS.create_root_node), [`is_root_node`](journal.md#Journal.is_root_node), [`MetricValue`](metric.md#MetricValue)


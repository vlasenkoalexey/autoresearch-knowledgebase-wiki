---
title: 'Module: ai_scientist/treesearch/utils/metric.py'
type: catalog
provenance: extracted
module: ai_scientist/treesearch/utils/metric.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.treesearch.utils.metric`/
symbols:
  MetricValue.value: MetricValue#value.
  MetricValue_old.value: MetricValue_old#value.
  MetricValue: MetricValue#
  MetricValue.__str__: MetricValue#__str__().
  WorstMetricValue: WorstMetricValue#
  MetricValue.maximize: MetricValue#maximize.
  MetricValue_old.__str__: MetricValue_old#__str__().
  MetricValue.__gt__: MetricValue#__gt__().
  MetricValue.name: MetricValue#name.
  MetricValue_old.value_npsafe: MetricValue_old#value_npsafe().
  MetricValue._should_maximize: MetricValue#_should_maximize().
  MetricValue_old.__gt__: MetricValue_old#__gt__().
  MetricValue.__eq__: MetricValue#__eq__().
  MetricValue_old.maximize: MetricValue_old#maximize.
  MetricValue.value_npsafe: MetricValue#value_npsafe().
  MetricValue.get_mean_value: MetricValue#get_mean_value().
  MetricValue.description: MetricValue#description.
  MetricValue_old.__post_init__: MetricValue_old#__post_init__().
  MetricValue_old.__eq__: MetricValue_old#__eq__().
  MetricValue_old.is_worst: MetricValue_old#is_worst().
  MetricValue_old.get_dataset_value: MetricValue_old#get_dataset_value().
  MetricValue_old.get_mean_value: MetricValue_old#get_mean_value().
  MetricValue.__post_init__: MetricValue#__post_init__().
  WorstMetricValue.__repr__: WorstMetricValue#__repr__().
  WorstMetricValue.__str__: WorstMetricValue#__str__().
  MetricValue_old.name: MetricValue_old#name.
  MetricValue.__repr__: MetricValue#__repr__().
  MetricValue_old: MetricValue_old#
  MetricValue_old.description: MetricValue_old#description.
  MetricValue_old.__repr__: MetricValue_old#__repr__().
  WorstMetricValue.value: WorstMetricValue#value.
---
# Module: [`ai_scientist/treesearch/utils/metric.py`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py)

## Classes
### `MetricValue`
- def: [`ai_scientist/treesearch/utils/metric.py:114`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L114) — documented in [ai_scientist-treesearch-journal](../../../../concepts/ai_scientist-treesearch-journal.md)
- doc: Represents one or more metric values to be optimized, which can be compared to other metric values.
- signature: `class MetricValue(DataClassJsonMixin):`
- members:
  - `__eq__(self, other: Any)` — [`L237`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L237) — Compare equality of metric values — documented in [ai_scientist-treesearch-utils-metric](../../../../concepts/ai_scientist-treesearch-utils-metric.md)
  - `__repr__(self)` — [`L259`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L259) — Return string representation
  - `_should_maximize(self)` — [`L191`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L191) — Determine if we should maximize based on the metric format — documented in [ai_scientist-treesearch-utils-metric](../../../../concepts/ai_scientist-treesearch-utils-metric.md)
  - `get_mean_value(self)` — [`L302`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L302) — Get the mean value across all metrics and datasets — documented in [ai_scientist-treesearch-utils-metric](../../../../concepts/ai_scientist-treesearch-utils-metric.md)
  - `value_npsafe(self)` — [`L264`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L264) — Return a NaN-safe version of the value — documented in [ai_scientist-treesearch-utils-metric](../../../../concepts/ai_scientist-treesearch-utils-metric.md)
  - `description` — [`L142`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L142)
  - `maximize` — [`L140`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L140) — documented in [ai_scientist-treesearch-journal](../../../../concepts/ai_scientist-treesearch-journal.md)
  - `name` — [`L141`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L141)
  - `value` — [`L139`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L139) — documented in [ai_scientist-treesearch-agent_manager](../../../../concepts/ai_scientist-treesearch-agent_manager.md)
- protocol/private: `__gt__`[`L171`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L171), `__post_init__`[`L144`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L144), `__str__`[`L206`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L206)
- uses (calls/refs, reference-scoped): [`WorstMetricValue`](metric.md#WorstMetricValue)
- used by: [`_process_node_wrapper`](../parallel_agent.md#ParallelAgent._process_node_wrapper), [`to_dict`](../journal.md#Node.to_dict), [`cfg_to_tree_struct`](tree_export.md#cfg_to_tree_struct), [`metric`](../journal.md#Node.metric), [`from_dict`](../journal.md#Node.from_dict), [`_gather_stage_metrics`](../agent_manager.md#AgentManager._gather_stage_metrics), [`_analyze_progress`](../agent_manager.md#AgentManager._analyze_progress), [`append_rec`](../perform_experiments_bfts_with_agentmanager.md#journal_to_rich_tree.append_rec), [`generate_summary_old`](../journal.md#Journal.generate_summary_old), [`WorstMetricValue`](metric.md#WorstMetricValue), [`get_metric_history`](../journal.md#Journal.get_metric_history), [`__repr__`](metric.md#WorstMetricValue.__repr__), [`__str__`](metric.md#WorstMetricValue.__str__)

### `MetricValue_old`
- def: [`ai_scientist/treesearch/utils/metric.py:11`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L11)
- doc: Represents the value of a metric to be optimized, which can be compared to other metric values.
- signature: `class MetricValue_old(DataClassJsonMixin):`
- members:
  - `__gt__(self, other)` — [`L34`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L34) — True if self is a _better_ (not necessarily larger) metric value than other — documented in [ai_scientist-treesearch-utils-metric](../../../../concepts/ai_scientist-treesearch-utils-metric.md)
  - `get_dataset_value(self, dataset_name: str)` — [`L97`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L97) — Get the metric value for a specific dataset — documented in [ai_scientist-treesearch-utils-metric](../../../../concepts/ai_scientist-treesearch-utils-metric.md)
  - `get_mean_value(self)` — [`L103`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L103) — Get the mean value across all datasets (or single value if not multi-dataset)
  - `is_worst(self)` — [`L83`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L83) — True if the metric value is the worst possible value. — documented in [ai_scientist-treesearch-utils-metric](../../../../concepts/ai_scientist-treesearch-utils-metric.md)
  - `value_npsafe(self)` — [`L88`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L88)
  - `description` — [`L22`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L22)
  - `maximize` — [`L18`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L18)
  - `name` — [`L19`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L19)
  - `value` — [`L17`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L17)
- protocol/private: `__eq__`[`L61`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L61), `__post_init__`[`L26`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L26), `__repr__`[`L64`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L64), `__str__`[`L67`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L67)

### `WorstMetricValue`  ·  implements/extends MetricValue
- def: [`ai_scientist/treesearch/utils/metric.py:328`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L328) — documented in [ai_scientist-treesearch-log_summarization](../../../../concepts/ai_scientist-treesearch-log_summarization.md)
- doc: Represents an invalid metric value, e.g. when the agent creates a buggy solution.
- signature: `class WorstMetricValue(MetricValue):`
- members:
  - `value` — [`L334`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L334)
- protocol/private: `__repr__`[`L336`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L336), `__str__`[`L339`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/metric.py#L339)
- uses (calls/refs, reference-scoped): [`MetricValue`](metric.md#MetricValue), [`__str__`](metric.md#MetricValue.__str__), [`__repr__`](metric.md#MetricValue.__repr__)
- used by: [`_process_node_wrapper`](../parallel_agent.md#ParallelAgent._process_node_wrapper), [`from_dict`](../journal.md#Node.from_dict), [`MetricValue`](metric.md#MetricValue)


---
title: 'Module: domains/train_opt/mechanisms/gene_regulatory_network.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/gene_regulatory_network.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.gene_regulatory_network`/
symbols:
  GeneRegulatoryNetwork.build_rules: GeneRegulatoryNetwork#build_rules().
  GeneRegulatoryNetwork._rules: GeneRegulatoryNetwork#_rules.
  GeneRegulatoryNetwork.record_config: GeneRegulatoryNetwork#record_config().
  GeneRegulatoryNetwork._rank_correlation: GeneRegulatoryNetwork#_rank_correlation().
  GeneRegulatoryNetwork.get_grn_text: GeneRegulatoryNetwork#get_grn_text().
  GeneRegulatoryNetwork: GeneRegulatoryNetwork#
  GeneRegulatoryNetwork._min_elites: GeneRegulatoryNetwork#_min_elites.
  GeneRegulatoryNetwork._ranks: GeneRegulatoryNetwork#_ranks().
  logger: logger.
  GeneRegulatoryNetwork._observations: GeneRegulatoryNetwork#_observations.
  GeneRegulatoryNetwork.__init__: GeneRegulatoryNetwork#__init__().
---
# Module: [`domains/train_opt/mechanisms/gene_regulatory_network.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/gene_regulatory_network.py)

## Classes
### `GeneRegulatoryNetwork`
- def: [`domains/train_opt/mechanisms/gene_regulatory_network.py:25`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/gene_regulatory_network.py#L25)
- doc: Models learned parameter dependency rules (compensatory changes).
- signature: `class GeneRegulatoryNetwork:`
- members:
  - `_rank_correlation(x: list[float], y: list[float])` — [`L150`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/gene_regulatory_network.py#L150) — Compute Spearman rank correlation (stdlib-only implementation).
  - `build_rules(self, elite_configs: list[tuple[float, dict]])` — [`L50`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/gene_regulatory_network.py#L50) — Build regulatory rules from elite config patterns. — documented in [domains-train_opt-runner](../../../../concepts/domains-train_opt-runner.md)
  - `get_grn_text(self, proposed_changes: dict | None = None)` — [`L189`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/gene_regulatory_network.py#L189) — Generate regulatory network recommendations for the proposal prompt.
  - `record_config(self, config: dict, val_bpb: float, was_improvement: bool)` — [`L45`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/gene_regulatory_network.py#L45) — Record a full config snapshot with its outcome.
- protocol/private: `__init__`[`L37`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/gene_regulatory_network.py#L37), `_min_elites`[`L38`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/gene_regulatory_network.py#L38), `_observations`[`L40`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/gene_regulatory_network.py#L40), `_ranks`[`L160`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/gene_regulatory_network.py#L160), `_rules`[`L43`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/gene_regulatory_network.py#L43)
- uses (calls/refs, reference-scoped): [`logger`](gene_regulatory_network.md#logger)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`run_baseline`](../runner.md#TrainRunner.run_baseline), [`grn`](../runner.md#TrainRunner.grn)

## Module values
- `logger` — [`L22`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/gene_regulatory_network.py#L22)


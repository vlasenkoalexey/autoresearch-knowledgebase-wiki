---
title: 'Module: rdagent/scenarios/qlib/proposal/bandit.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/qlib/proposal/bandit.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.qlib.proposal.bandit`/
symbols:
  extract_metrics_from_experiment: extract_metrics_from_experiment().
  Metrics.as_vector: Metrics#as_vector().
  EnvController.record: EnvController#record().
  EnvController.decide: EnvController#decide().
  LinearThompsonTwoArm.sample_reward: LinearThompsonTwoArm#sample_reward().
  LinearThompsonTwoArm.update: LinearThompsonTwoArm#update().
  EnvController.reward: EnvController#reward().
  Metrics: Metrics#
  EnvController.bandit: EnvController#bandit.
  LinearThompsonTwoArm.mean: LinearThompsonTwoArm#mean.
  LinearThompsonTwoArm.next_arm: LinearThompsonTwoArm#next_arm().
  LinearThompsonTwoArm.precision: LinearThompsonTwoArm#precision.
  Metrics.ic: Metrics#ic.
  Metrics.icir: Metrics#icir.
  Metrics.rank_ic: Metrics#rank_ic.
  Metrics.rank_icir: Metrics#rank_icir.
  Metrics.arr: Metrics#arr.
  Metrics.ir: Metrics#ir.
  Metrics.mdd: Metrics#mdd.
  Metrics.sharpe: Metrics#sharpe.
  LinearThompsonTwoArm.dim: LinearThompsonTwoArm#dim.
  LinearThompsonTwoArm.noise_var: LinearThompsonTwoArm#noise_var.
  EnvController: EnvController#
  LinearThompsonTwoArm: LinearThompsonTwoArm#
  EnvController.weights: EnvController#weights.
  LinearThompsonTwoArm.__init__: LinearThompsonTwoArm#__init__().
  EnvController.__init__: EnvController#__init__().
---
# Module: [`rdagent/scenarios/qlib/proposal/bandit.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py)

## Classes
### `EnvController`
- def: [`rdagent/scenarios/qlib/proposal/bandit.py:95`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L95)
- signature: `class EnvController:`
- members:
  - `decide(self, m: Metrics)` — [`L103`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L103)
  - `record(self, m: Metrics, arm: str)` — [`L107`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L107)
  - `reward(self, m: Metrics)` — [`L100`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L100)
  - `bandit` — [`L98`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L98)
  - `weights` — [`L97`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L97)
- protocol/private: `__init__`[`L96`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L96)
- uses (calls/refs, reference-scoped): [`as_vector`](bandit.md#Metrics.as_vector), [`update`](bandit.md#LinearThompsonTwoArm.update), [`Metrics`](bandit.md#Metrics), [`next_arm`](bandit.md#LinearThompsonTwoArm.next_arm), [`LinearThompsonTwoArm`](bandit.md#LinearThompsonTwoArm)
- used by: [`controller`](quant_proposal.md#QuantTrace.controller)

### `LinearThompsonTwoArm`
- def: [`rdagent/scenarios/qlib/proposal/bandit.py:55`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L55)
- signature: `class LinearThompsonTwoArm:`
- members:
  - `next_arm(self, x: np.ndarray)` — [`L90`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L90)
  - `sample_reward(self, arm: str, x: np.ndarray)` — [`L69`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L69)
  - `update(self, arm: str, x: np.ndarray, r: float)` — [`L84`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L84)
  - `dim` — [`L57`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L57)
  - `mean` — [`L60`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L60)
  - `noise_var` — [`L58`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L58)
  - `precision` — [`L64`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L64)
- protocol/private: `__init__`[`L56`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L56)
- used by: [`record`](bandit.md#EnvController.record), [`decide`](bandit.md#EnvController.decide), [`bandit`](bandit.md#EnvController.bandit)

### `Metrics`
- def: [`rdagent/scenarios/qlib/proposal/bandit.py:11`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L11)
- signature: `class Metrics:`
- members:
  - `as_vector(self)` — [`L21`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L21)
  - `arr` — [`L16`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L16)
  - `ic` — [`L12`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L12)
  - `icir` — [`L13`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L13)
  - `ir` — [`L17`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L17)
  - `mdd` — [`L18`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L18)
  - `rank_ic` — [`L14`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L14)
  - `rank_icir` — [`L15`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L15)
  - `sharpe` — [`L19`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L19)
- used by: [`extract_metrics_from_experiment`](bandit.md#extract_metrics_from_experiment), [`record`](bandit.md#EnvController.record), [`decide`](bandit.md#EnvController.decide), [`reward`](bandit.md#EnvController.reward)

## Functions
- `extract_metrics_from_experiment(experiment)` — [`L36`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/bandit.py#L36) — Extract metrics from experiment feedback


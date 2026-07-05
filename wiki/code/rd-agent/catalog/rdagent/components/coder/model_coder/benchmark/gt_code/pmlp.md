---
title: 'Module: rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.model_coder.benchmark.gt_code.pmlp`/
symbols:
  PMLP.forward: PMLP#forward().
  PMLP.lins: PMLP#lins.
  output: output.
  PMLP.__repr__: PMLP#__repr__().
  PMLP.reset_parameters: PMLP#reset_parameters().
  model: model.
  PMLP.norm: PMLP#norm.
  PMLP.bias: PMLP#bias.
  PMLP.num_layers: PMLP#num_layers.
  node_features: node_features.
  PMLP.conv: PMLP#conv.
  model_cls: model_cls.
  PMLP: PMLP#
  PMLP.in_channels: PMLP#in_channels.
  PMLP.out_channels: PMLP#out_channels.
  PMLP.dropout: PMLP#dropout.
  edge_index: edge_index.
  PMLP.__init__: PMLP#__init__().
  PMLP.hidden_channels: PMLP#hidden_channels.
---
# Module: [`rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py)

## Classes
### `PMLP`
- def: [`rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py:10`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L10)
- doc: The P(ropagational)MLP model from the `"Graph Neural Networks are
- signature: `class PMLP(torch.nn.Module):`
- members:
  - `forward(self, x: torch.Tensor, edge_index: Optional[Tensor] = None)` — [`L75`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L75)
  - `reset_parameters(self)` — [`L68`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L68) — Resets all learnable parameters of the module.
  - `bias` — [`L47`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L47)
  - `conv` — [`L64`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L64)
  - `dropout` — [`L46`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L46)
  - `hidden_channels` — [`L43`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L43)
  - `in_channels` — [`L42`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L42)
  - `lins` — [`L49`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L49)
  - `norm` — [`L56`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L56)
  - `num_layers` — [`L45`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L45)
  - `out_channels` — [`L44`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L44)
- protocol/private: `__init__`[`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L30), `__repr__`[`L98`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L98)
- used by: (2 test-only callers)

## Module values
- `edge_index` — [`L106`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L106)
- `model` — [`L109`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L109)
- `model_cls` — [`L102`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L102)
- `node_features` — [`L105`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L105)
- `output` — [`L115`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/pmlp.py#L115)


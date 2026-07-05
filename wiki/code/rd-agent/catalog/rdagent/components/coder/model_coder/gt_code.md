---
title: 'Module: rdagent/components/coder/model_coder/gt_code.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/model_coder/gt_code.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.model_coder.gt_code`/
symbols:
  AntiSymmetricConv.forward: AntiSymmetricConv#forward().
  AntiSymmetricConv.__repr__: AntiSymmetricConv#__repr__().
  output: output.
  AntiSymmetricConv.reset_parameters: AntiSymmetricConv#reset_parameters().
  model: model.
  AntiSymmetricConv.bias: AntiSymmetricConv#bias.
  AntiSymmetricConv.W: AntiSymmetricConv#W.
  AntiSymmetricConv.phi: AntiSymmetricConv#phi.
  AntiSymmetricConv.num_iters: AntiSymmetricConv#num_iters.
  AntiSymmetricConv.gamma: AntiSymmetricConv#gamma.
  AntiSymmetricConv.epsilon: AntiSymmetricConv#epsilon.
  AntiSymmetricConv.act: AntiSymmetricConv#act.
  node_features: node_features.
  AntiSymmetricConv: AntiSymmetricConv#
  AntiSymmetricConv.in_channels: AntiSymmetricConv#in_channels.
  edge_index: edge_index.
  AntiSymmetricConv.__init__: AntiSymmetricConv#__init__().
---
# Module: [`rdagent/components/coder/model_coder/gt_code.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py)

## Classes
### `AntiSymmetricConv`
- def: [`rdagent/components/coder/model_coder/gt_code.py:18`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L18)
- doc: The anti-symmetric graph convolutional operator from the
- signature: `class AntiSymmetricConv(torch.nn.Module):`
- members:
  - `forward(self, x: Tensor, edge_index: Adj, *args, **kwargs)` — [`L98`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L98) — Runs the forward pass of the module.
  - `reset_parameters(self)` — [`L92`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L92) — Resets all learnable parameters of the module.
  - `W` — [`L81`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L81)
  - `act` — [`L76`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L76)
  - `bias` — [`L86`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L86)
  - `epsilon` — [`L75`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L75)
  - `gamma` — [`L74`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L74)
  - `in_channels` — [`L72`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L72)
  - `num_iters` — [`L73`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L73)
  - `phi` — [`L83`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L83)
- protocol/private: `__init__`[`L59`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L59), `__repr__`[`L116`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L116)
- used by: [`model`](gt_code.md#model)

## Module values
- `edge_index` — [`L129`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L129)
- `model` — [`L132`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L132)
- `node_features` — [`L128`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L128)
- `output` — [`L133`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/gt_code.py#L133)


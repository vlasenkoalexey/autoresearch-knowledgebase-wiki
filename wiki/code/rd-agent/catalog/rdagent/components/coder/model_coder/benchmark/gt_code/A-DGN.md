---
title: 'Module: rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.model_coder.benchmark.gt_code.A-DGN`/
symbols:
  AntiSymmetricConv.forward: AntiSymmetricConv#forward().
  AntiSymmetricConv.__repr__: AntiSymmetricConv#__repr__().
  output: output.
  AntiSymmetricConv.reset_parameters: AntiSymmetricConv#reset_parameters().
  model: model.
  AntiSymmetricConv.bias: AntiSymmetricConv#bias.
  AntiSymmetricConv.W: AntiSymmetricConv#W.
  AntiSymmetricConv.phi: AntiSymmetricConv#phi.
  model_cls: model_cls.
  AntiSymmetricConv: AntiSymmetricConv#
  AntiSymmetricConv.num_iters: AntiSymmetricConv#num_iters.
  AntiSymmetricConv.gamma: AntiSymmetricConv#gamma.
  AntiSymmetricConv.epsilon: AntiSymmetricConv#epsilon.
  AntiSymmetricConv.act: AntiSymmetricConv#act.
  node_features: node_features.
  AntiSymmetricConv.in_channels: AntiSymmetricConv#in_channels.
  edge_index: edge_index.
  AntiSymmetricConv.__init__: AntiSymmetricConv#__init__().
---
# Module: [`rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py)

## Classes
### `AntiSymmetricConv`
- def: [`rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py:13`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L13)
- doc: The anti-symmetric graph convolutional operator from the
- signature: `class AntiSymmetricConv(torch.nn.Module):`
- members:
  - `forward(self, x: Tensor, edge_index: Adj, *args, **kwargs)` — [`L93`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L93) — Runs the forward pass of the module.
  - `reset_parameters(self)` — [`L87`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L87) — Resets all learnable parameters of the module.
  - `W` — [`L76`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L76)
  - `act` — [`L71`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L71)
  - `bias` — [`L81`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L81)
  - `epsilon` — [`L70`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L70)
  - `gamma` — [`L69`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L69)
  - `in_channels` — [`L67`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L67)
  - `num_iters` — [`L68`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L68)
  - `phi` — [`L78`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L78)
- protocol/private: `__init__`[`L54`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L54), `__repr__`[`L111`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L111)
- used by: (2 test-only callers)

## Module values
- `edge_index` — [`L127`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L127)
- `model` — [`L130`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L130)
- `model_cls` — [`L122`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L122)
- `node_features` — [`L126`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L126)
- `output` — [`L131`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/A-DGN.py#L131)


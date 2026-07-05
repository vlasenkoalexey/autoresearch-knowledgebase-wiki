---
title: 'Module: rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.model_coder.benchmark.gt_code.dirgnn`/
symbols:
  DirGNNConv.forward: DirGNNConv#forward().
  output: output.
  DirGNNConv.conv_out: DirGNNConv#conv_out.
  DirGNNConv.lin: DirGNNConv#lin.
  DirGNNConv.reset_parameters: DirGNNConv#reset_parameters().
  DirGNNConv.conv_in: DirGNNConv#conv_in.
  DirGNNConv.__repr__: DirGNNConv#__repr__().
  model: model.
  DirGNNConv.alpha: DirGNNConv#alpha.
  model_cls: model_cls.
  DirGNNConv: DirGNNConv#
  DirGNNConv.root_weight: DirGNNConv#root_weight.
  node_features: node_features.
  edge_index: edge_index.
  DirGNNConv.__init__: DirGNNConv#__init__().
---
# Module: [`rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py)

## Classes
### `DirGNNConv`
- def: [`rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py:8`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py#L8)
- doc: A generic wrapper for computing graph convolution on directed
- signature: `class DirGNNConv(torch.nn.Module):`
- members:
  - `forward(self, x: Tensor, edge_index: Tensor)` — [`L61`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py#L61)
  - `reset_parameters(self)` — [`L54`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py#L54) — Resets all learnable parameters of the module.
  - `alpha` — [`L34`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py#L34)
  - `conv_in` — [`L37`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py#L37)
  - `conv_out` — [`L38`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py#L38)
  - `lin` — [`L48`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py#L48)
  - `root_weight` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py#L35)
- protocol/private: `__init__`[`L26`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py#L26), `__repr__`[`L73`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py#L73)
- used by: (2 test-only callers)

## Module values
- `edge_index` — [`L82`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py#L82)
- `model` — [`L85`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py#L85)
- `model_cls` — [`L77`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py#L77)
- `node_features` — [`L81`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py#L81)
- `output` — [`L86`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/dirgnn.py#L86)


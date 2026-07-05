---
title: 'Module: rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.model_coder.benchmark.gt_code.linkx`/
symbols:
  LINKX.reset_parameters: LINKX#reset_parameters().
  LINKX.forward: LINKX#forward().
  output: output.
  LINKX.edge_mlp: LINKX#edge_mlp.
  SparseLinear.reset_parameters: SparseLinear#reset_parameters().
  LINKX.__repr__: LINKX#__repr__().
  LINKX.edge_lin: LINKX#edge_lin.
  model: model.
  SparseLinear.bias: SparseLinear#bias.
  SparseLinear.forward: SparseLinear#forward().
  LINKX.edge_norm: LINKX#edge_norm.
  node_features: node_features.
  LINKX.final_mlp: LINKX#final_mlp.
  model_cls: model_cls.
  SparseLinear.in_channels: SparseLinear#in_channels.
  SparseLinear.weight: SparseLinear#weight.
  LINKX: LINKX#
  LINKX.node_mlp: LINKX#node_mlp.
  LINKX.cat_lin1: LINKX#cat_lin1.
  LINKX.cat_lin2: LINKX#cat_lin2.
  SparseLinear: SparseLinear#
  LINKX.num_nodes: LINKX#num_nodes.
  LINKX.in_channels: LINKX#in_channels.
  LINKX.out_channels: LINKX#out_channels.
  LINKX.num_edge_layers: LINKX#num_edge_layers.
  edge_index: edge_index.
  SparseLinear.__init__: SparseLinear#__init__().
  SparseLinear.out_channels: SparseLinear#out_channels.
  SparseLinear.message: SparseLinear#message().
  SparseLinear.message_and_aggregate: SparseLinear#message_and_aggregate().
  LINKX.__init__: LINKX#__init__().
---
# Module: [`rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py)

## Classes
### `LINKX`
- def: [`rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py:54`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L54)
- doc: The LINKX model from the `"Large Scale Learning on Non-Homophilous
- signature: `class LINKX(torch.nn.Module):`
- members:
  - `forward(self, x: OptTensor, edge_index: Adj, edge_weight: OptTensor = None)` — [`L139`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L139)
  - `reset_parameters(self)` — [`L127`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L127) — Resets all learnable parameters of the module.
  - `cat_lin1` — [`L119`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L119)
  - `cat_lin2` — [`L120`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L120)
  - `edge_lin` — [`L106`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L106)
  - `edge_mlp` — [`L111`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L111)
  - `edge_norm` — [`L109`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L109)
  - `final_mlp` — [`L123`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L123)
  - `in_channels` — [`L102`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L102)
  - `node_mlp` — [`L117`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L117)
  - `num_edge_layers` — [`L104`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L104)
  - `num_nodes` — [`L101`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L101)
  - `out_channels` — [`L103`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L103)
- protocol/private: `__init__`[`L88`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L88), `__repr__`[`L162`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L162)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

### `SparseLinear`
- def: [`rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py:13`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L13)
- signature: `class SparseLinear(MessagePassing):`
- members:
  - `forward(self, edge_index: Adj, edge_weight: OptTensor = None)` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L31)
  - `message(self, weight_j: Tensor, edge_weight: OptTensor)` — [`L44`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L44)
  - `message_and_aggregate(self, adj_t: Adj, weight: Tensor)` — [`L50`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L50)
  - `reset_parameters(self)` — [`L27`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L27)
  - `bias` — [`L21`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L21)
  - `in_channels` — [`L16`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L16)
  - `out_channels` — [`L17`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L17)
  - `weight` — [`L19`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L19)
- protocol/private: `__init__`[`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L14)
- used by: (2 test-only callers)

## Module values
- `edge_index` — [`L174`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L174)
- `model` — [`L177`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L177)
- `model_cls` — [`L170`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L170)
- `node_features` — [`L173`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L173)
- `output` — [`L184`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/linkx.py#L184)


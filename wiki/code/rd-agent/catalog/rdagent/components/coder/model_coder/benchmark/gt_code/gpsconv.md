---
title: 'Module: rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.model_coder.benchmark.gt_code.gpsconv`/
symbols:
  GPSConv.forward: GPSConv#forward().
  GPSConv.reset_parameters: GPSConv#reset_parameters().
  output: output.
  GPSConv.__repr__: GPSConv#__repr__().
  GPSConv.norm_with_batch: GPSConv#norm_with_batch.
  GPSConv.attn: GPSConv#attn.
  GPSConv.norm1: GPSConv#norm1.
  model: model.
  GPSConv.conv: GPSConv#conv.
  GPSConv.norm2: GPSConv#norm2.
  GPSConv.norm3: GPSConv#norm3.
  model_cls: model_cls.
  GPSConv: GPSConv#
  GPSConv.dropout: GPSConv#dropout.
  GPSConv.mlp: GPSConv#mlp.
  node_features: node_features.
  GPSConv.channels: GPSConv#channels.
  GPSConv.heads: GPSConv#heads.
  GPSConv.attn_type: GPSConv#attn_type.
  edge_index: edge_index.
  GPSConv.__init__: GPSConv#__init__().
---
# Module: [`rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py)

## Classes
### `GPSConv`
- def: [`rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py:16`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L16)
- doc: The general, powerful, scalable (GPS) graph transformer layer from the
- signature: `class GPSConv(torch.nn.Module):`
- members:
  - `forward(self, x: Tensor, edge_index: Adj, batch: Optional[torch.Tensor] = None, **kwargs)` — [`L129`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L129) — Runs the forward pass of the module.
  - `reset_parameters(self)` — [`L116`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L116) — Resets all learnable parameters of the module.
  - `attn` — [`L82`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L82)
  - `attn_type` — [`L78`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L78)
  - `channels` — [`L74`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L74)
  - `conv` — [`L75`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L75)
  - `dropout` — [`L77`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L77)
  - `heads` — [`L76`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L76)
  - `mlp` — [`L98`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L98)
  - `norm1` — [`L107`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L107)
  - `norm2` — [`L108`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L108)
  - `norm3` — [`L109`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L109)
  - `norm_with_batch` — [`L111`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L111)
- protocol/private: `__init__`[`L59`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L59), `__repr__`[`L178`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L178)
- used by: (2 test-only callers)

## Module values
- `edge_index` — [`L191`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L191)
- `model` — [`L194`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L194)
- `model_cls` — [`L186`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L186)
- `node_features` — [`L190`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L190)
- `output` — [`L195`](../../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/benchmark/gt_code/gpsconv.py#L195)


---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model_provider.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model_provider.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.model_provider`/
symbols:
  get_model_provider_func: get_model_provider_func().
  get_model_provider_func.wrapped_model_provider: get_model_provider_func().wrapped_model_provider().
  LinearForLastLayer.sequence_parallel: LinearForLastLayer#sequence_parallel.
  wrap_model_provider_with_freeze: wrap_model_provider_with_freeze().
  get_model_provider_func.model_provider: get_model_provider_func().model_provider().
  wrap_model_provider_with_freeze.wrapped_provider: wrap_model_provider_with_freeze().wrapped_provider().
  LinearForLastLayer.forward: LinearForLastLayer#forward().
  LinearForLastLayer: LinearForLastLayer#
  freeze_model_params: freeze_model_params().
  LinearForLastLayer.__init__: LinearForLastLayer#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model_provider.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model_provider.py)

## Classes
### `LinearForLastLayer`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model_provider.py:24`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model_provider.py#L24)
- signature: `class LinearForLastLayer(torch.nn.Linear):`
- members:
  - `forward(self, input_: torch.Tensor, weight: torch.Tensor | None = None, runtime_gather_output: bool | None = None)` — [`L44`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model_provider.py#L44)
  - `sequence_parallel` — [`L34`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model_provider.py#L34)
- protocol/private: `__init__`[`L25`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model_provider.py#L25)
- used by: [`wrapped_model_provider`](model_provider.md#get_model_provider_func.wrapped_model_provider), [`model_provider`](model_provider.md#get_model_provider_func.model_provider)

## Functions
- `freeze_model_params(model: GPTModel, args: argparse.Namespace)` — [`L226`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model_provider.py#L226)
- `get_model_provider_func(args: argparse.Namespace, role: Literal["actor", "critic"] = "actor")` — [`L57`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model_provider.py#L57)
- `model_provider(pre_process: bool = True, post_process: bool = True, vp_stage: int | None = None)` — [`L101`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model_provider.py#L101) — Builds the model.
- `wrap_model_provider_with_freeze(original_provider, args)` — [`L211`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model_provider.py#L211)
- `wrapped_model_provider(pre_process: bool = True, post_process: bool = True, vp_stage: int | None = None)` — [`L64`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model_provider.py#L64)
- `wrapped_provider(pre_process=True, post_process=True, vp_stage=None)` — [`L212`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model_provider.py#L212)


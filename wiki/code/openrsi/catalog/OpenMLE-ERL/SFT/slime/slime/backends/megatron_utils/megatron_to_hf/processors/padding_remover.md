---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/padding_remover.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/padding_remover.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.megatron_to_hf.processors.padding_remover`/remove_padding().
symbols:
  remove_padding: ''
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/padding_remover.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/padding_remover.py)

## Functions
- `remove_padding(name: str, param: torch.Tensor, vocab_size: int)` — [`L6`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/padding_remover.py#L6) — Remove vocab padding: param[:vocab_size] for embedding/output layers, else unchanged.


---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/data_packing.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/data_packing.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.fsdp_utils.data_packing`/
symbols:
  pack_sequences: pack_sequences().
  unpack_sequences: unpack_sequences().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/data_packing.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/data_packing.py)

## Functions
- `pack_sequences(tokens: list[list[int]], loss_masks: list[list[int]], rewards: list[float], raw_rewards: list, response_lengths: list[int], advantages: list[float], returns: list[float], rollout_log_probs: list[list[float]] | None = None, multimodal_train_inputs: list[dict] | None = None, max_tokens_per_gpu: int | None = None, num_packs: int | None = None)` — [`L10`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/data_packing.py#L10) — Pack sequences into dense batches with cumulative sequence lengths.
- `unpack_sequences(packed_batch: dict)` — [`L124`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/data_packing.py#L124) — Unpack sequences from a packed batch.


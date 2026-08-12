---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.mask_utils`/
symbols:
  MultiTurnLossMaskGenerator.tokenizer: MultiTurnLossMaskGenerator#tokenizer.
  MultiTurnLossMaskGenerator.get_loss_mask: MultiTurnLossMaskGenerator#get_loss_mask().
  MultiTurnLossMaskGenerator.gen_multi_turn_loss_mask_qwen: MultiTurnLossMaskGenerator#gen_multi_turn_loss_mask_qwen().
  MultiTurnLossMaskGenerator.gen_multi_turn_loss_mask_qwen3: MultiTurnLossMaskGenerator#gen_multi_turn_loss_mask_qwen3().
  MultiTurnLossMaskGenerator.gen_token_length: MultiTurnLossMaskGenerator#gen_token_length.
  MultiTurnLossMaskGenerator.get_system_message_length: MultiTurnLossMaskGenerator#get_system_message_length().
  MultiTurnLossMaskGenerator.tokenizer_type: MultiTurnLossMaskGenerator#tokenizer_type.
  MultiTurnLossMaskGenerator.gen_multi_turn_loss_mask_distill_qwen: MultiTurnLossMaskGenerator#gen_multi_turn_loss_mask_distill_qwen().
  MultiTurnLossMaskGenerator.get_response_lengths: MultiTurnLossMaskGenerator#get_response_lengths().
  MultiTurnLossMaskGenerator.gen_multi_turn_loss_mask_qwen3_5: MultiTurnLossMaskGenerator#gen_multi_turn_loss_mask_qwen3_5().
  get_response_lengths: get_response_lengths().
  MultiTurnLossMaskGenerator.get_loss_mask_with_multimodal_alignment: MultiTurnLossMaskGenerator#get_loss_mask_with_multimodal_alignment().
  MultiTurnLossMaskGenerator.get_text_from_loss_mask: MultiTurnLossMaskGenerator#get_text_from_loss_mask().
  MultiTurnLossMaskGenerator: MultiTurnLossMaskGenerator#
  MultiTurnLossMaskGenerator.system_message_length: MultiTurnLossMaskGenerator#system_message_length.
  MultiTurnLossMaskGenerator.find_all_sublist_indices: MultiTurnLossMaskGenerator#find_all_sublist_indices().
  MultiTurnLossMaskGenerator.__init__: MultiTurnLossMaskGenerator#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py)

## Classes
### `MultiTurnLossMaskGenerator`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py:9`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L9)
- signature: `class MultiTurnLossMaskGenerator:`
- members:
  - `find_all_sublist_indices(self, main_list, sublist)` — [`L18`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L18)
  - `gen_multi_turn_loss_mask_distill_qwen(self, messages: list[dict], tools: list[dict] = None)` — [`L191`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L191)
  - `gen_multi_turn_loss_mask_qwen(self, messages: list[dict], tools: list[dict] = None)` — [`L48`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L48)
  - `gen_multi_turn_loss_mask_qwen3(self, messages: list[dict], tools: list[dict] = None)` — [`L76`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L76)
  - `gen_multi_turn_loss_mask_qwen3_5(self, messages: list[dict], tools: list[dict] = None)` — [`L111`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L111)
  - `get_loss_mask(self, messages: list[dict], tools: list[dict] = None)` — [`L209`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L209)
  - `get_loss_mask_with_multimodal_alignment(self, messages: list[dict], input_ids: list[int], tools: list[dict] = None)` — [`L224`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L224)
  - `get_response_lengths(self, loss_masks: list[list[int]])` — [`L15`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L15)
  - `get_system_message_length(self)` — [`L26`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L26)
  - `get_text_from_loss_mask(self, token_ids: list[int], loss_masks: list[int])` — [`L251`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L251)
  - `gen_token_length` — [`L12`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L12)
  - `system_message_length` — [`L12`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L12)
  - `tokenizer` — [`L11`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L11)
  - `tokenizer_type` — [`L13`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L13)
- protocol/private: `__init__`[`L10`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L10)
- uses (calls/refs, reference-scoped): [`get_response_lengths`](mask_utils.md#get_response_lengths)
- used by: [`generate_rollout`](../rollout/sft_rollout.md#generate_rollout)

## Functions
- `get_response_lengths(loss_masks: list[list[int]])` — [`L4`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/mask_utils.py#L4)


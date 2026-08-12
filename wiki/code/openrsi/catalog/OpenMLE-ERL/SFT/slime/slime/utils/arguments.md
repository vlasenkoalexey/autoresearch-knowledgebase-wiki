---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/arguments.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/arguments.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.arguments`/
symbols:
  get_slime_extra_args_provider.add_slime_arguments: get_slime_extra_args_provider().add_slime_arguments().
  parse_args: parse_args().
  reset_arg: reset_arg().
  _resolve_eval_datasets: _resolve_eval_datasets().
  logger: logger.
  slime_validate_args: slime_validate_args().
  get_slime_extra_args_provider: get_slime_extra_args_provider().
  get_slime_extra_args_provider.add_slime_arguments.add_cluster_arguments: get_slime_extra_args_provider().add_slime_arguments().add_cluster_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_data_arguments: get_slime_extra_args_provider().add_slime_arguments().add_data_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_eval_arguments: get_slime_extra_args_provider().add_slime_arguments().add_eval_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_algo_arguments: get_slime_extra_args_provider().add_slime_arguments().add_algo_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_wandb_arguments: get_slime_extra_args_provider().add_slime_arguments().add_wandb_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_mtp_training_arguments: get_slime_extra_args_provider().add_slime_arguments().add_mtp_training_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_train_arguments: get_slime_extra_args_provider().add_slime_arguments().add_train_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_rollout_arguments: get_slime_extra_args_provider().add_slime_arguments().add_rollout_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_fault_tolerance_arguments: get_slime_extra_args_provider().add_slime_arguments().add_fault_tolerance_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_on_policy_distillation_arguments: get_slime_extra_args_provider().add_slime_arguments().add_on_policy_distillation_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_router_arguments: get_slime_extra_args_provider().add_slime_arguments().add_router_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_tensorboard_arguments: get_slime_extra_args_provider().add_slime_arguments().add_tensorboard_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_debug_arguments: get_slime_extra_args_provider().add_slime_arguments().add_debug_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_network_arguments: get_slime_extra_args_provider().add_slime_arguments().add_network_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_reward_model_arguments: get_slime_extra_args_provider().add_slime_arguments().add_reward_model_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_rollout_buffer_arguments: get_slime_extra_args_provider().add_slime_arguments().add_rollout_buffer_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_custom_megatron_plugins_arguments: get_slime_extra_args_provider().add_slime_arguments().add_custom_megatron_plugins_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_prefill_decode_disaggregation_arguments: get_slime_extra_args_provider().add_slime_arguments().add_prefill_decode_disaggregation_arguments().
  get_slime_extra_args_provider.add_slime_arguments.add_ci_arguments: get_slime_extra_args_provider().add_slime_arguments().add_ci_arguments().
  _pre_parse_mode: _pre_parse_mode().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/arguments.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py)

## Functions
- `_pre_parse_mode()` — [`L1431`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L1431) — Pre-parse CLI to extract arguments that control parsing flow.
- `_resolve_eval_datasets(args)` — [`L1502`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L1502) — Build evaluation dataset configurations from either --eval-config or --eval-prompt-data.
- `add_algo_arguments(parser)` — [`L718`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L718)
- `add_ci_arguments(parser)` — [`L1373`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L1373)
- `add_cluster_arguments(parser)` — [`L37`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L37)
- `add_custom_megatron_plugins_arguments(parser)` — [`L1328`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L1328) — Add custom Megatron plugins arguments.
- `add_data_arguments(parser)` — [`L501`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L501)
- `add_debug_arguments(parser)` — [`L1129`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L1129)
- `add_eval_arguments(parser)` — [`L657`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L657)
- `add_fault_tolerance_arguments(parser)` — [`L473`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L473)
- `add_mtp_training_arguments(parser)` — [`L1351`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L1351) — Add MTP training specific arguments.
- `add_network_arguments(parser)` — [`L1189`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L1189)
- `add_on_policy_distillation_arguments(parser)` — [`L965`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L965) — Add on-policy distillation (OPD) related arguments.
- `add_prefill_decode_disaggregation_arguments(parser)` — [`L1364`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L1364)
- `add_reward_model_arguments(parser)` — [`L1194`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L1194)
- `add_rollout_arguments(parser)` — [`L218`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L218)
- `add_rollout_buffer_arguments(parser)` — [`L1255`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L1255)
- `add_router_arguments(parser)` — [`L1008`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L1008)
- `add_slime_arguments(parser)` — [`L35`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L35)
- `add_tensorboard_arguments(parser)` — [`L1115`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L1115)
- `add_train_arguments(parser)` — [`L111`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L111)
- `add_wandb_arguments(parser)` — [`L1043`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L1043)
- `get_slime_extra_args_provider(add_custom_arguments=None)` — [`L34`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L34)
- `parse_args(add_custom_arguments=None)` — [`L1447`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L1447)
- `reset_arg(parser, name, **kwargs)` — [`L18`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L18) — Reset the default value of a Megatron argument.
- `slime_validate_args(args)` — [`L1545`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L1545)

## Module values
- `logger` — [`L15`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/arguments.py#L15)


---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/types.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/types.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.types`/
symbols:
  Sample: Sample#
  Sample.update_from_meta_info: Sample#update_from_meta_info().
  Sample.status: Sample#status.
  RolloutBatch: RolloutBatch.
  Sample.Status: Sample#Status#
  Sample.SpecInfo.from_dict: Sample#SpecInfo#from_dict().
  Sample.from_dict: Sample#from_dict().
  Sample.loss_mask: Sample#loss_mask.
  Sample.response_length: Sample#response_length.
  Sample.metadata: Sample#metadata.
  Sample.to_dict: Sample#to_dict().
  Sample.prompt: Sample#prompt.
  Sample.SpecInfo.add: Sample#SpecInfo#add().
  Sample.SpecInfo.to_dict: Sample#SpecInfo#to_dict().
  Sample.PrefixCacheInfo.from_dict: Sample#PrefixCacheInfo#from_dict().
  MultimodalTypes.all: MultimodalTypes#all().
  Sample.tokens: Sample#tokens.
  Sample.reward: Sample#reward.
  MultimodalTypes.IMAGE: MultimodalTypes#IMAGE.
  MultimodalTypes.VIDEO: MultimodalTypes#VIDEO.
  MultimodalTypes.AUDIO: MultimodalTypes#AUDIO.
  MultimodalTypes.get: MultimodalTypes#get().
  Sample.response: Sample#response.
  ParamInfo: ParamInfo#
  ParamInfo.name: ParamInfo#name.
  Sample.spec_info: Sample#spec_info.
  Sample.prefix_cache_info: Sample#prefix_cache_info.
  Sample.get_reward_value: Sample#get_reward_value().
  Sample.rollout_log_probs: Sample#rollout_log_probs.
  Sample.Status.TRUNCATED: Sample#Status#TRUNCATED.
  Sample.SpecInfo.spec_accept_rate: Sample#SpecInfo#spec_accept_rate().
  Sample.SpecInfo.spec_accept_length: Sample#SpecInfo#spec_accept_length().
  Sample.PrefixCacheInfo.total_prompt_tokens: Sample#PrefixCacheInfo#total_prompt_tokens.
  Sample.PrefixCacheInfo.add: Sample#PrefixCacheInfo#add().
  Sample.PrefixCacheInfo.to_dict: Sample#PrefixCacheInfo#to_dict().
  ParamInfo.src_rank: ParamInfo#src_rank.
  Sample.multimodal_inputs: Sample#multimodal_inputs.
  Sample.Status.ABORTED: Sample#Status#ABORTED.
  Sample.SpecInfo.spec_draft_token_num: Sample#SpecInfo#spec_draft_token_num.
  Sample.SpecInfo.spec_verify_ct: Sample#SpecInfo#spec_verify_ct.
  Sample.PrefixCacheInfo.cached_tokens: Sample#PrefixCacheInfo#cached_tokens.
  Sample.PrefixCacheInfo.prefix_cache_hit_rate: Sample#PrefixCacheInfo#prefix_cache_hit_rate().
  Sample.effective_response_length: Sample#effective_response_length().
  MultimodalType: MultimodalType#
  Sample.label: Sample#label.
  Sample.session_id: Sample#session_id.
  Sample.SpecInfo: Sample#SpecInfo#
  Sample.SpecInfo.spec_accept_token_num: Sample#SpecInfo#spec_accept_token_num.
  Sample.SpecInfo.completion_token_num: Sample#SpecInfo#completion_token_num.
  Sample.PrefixCacheInfo: Sample#PrefixCacheInfo#
  MultimodalType.name: MultimodalType#name.
  MultimodalType.placeholder: MultimodalType#placeholder.
  Sample.multimodal_train_inputs: Sample#multimodal_train_inputs.
  Sample.rollout_routed_experts: Sample#rollout_routed_experts.
  Sample.teacher_log_probs: Sample#teacher_log_probs.
  Sample.index: Sample#index.
  Sample.Status.PENDING: Sample#Status#PENDING.
  Sample.Status.COMPLETED: Sample#Status#COMPLETED.
  Sample.train_metadata: Sample#train_metadata.
  ParamInfo.dtype: ParamInfo#dtype.
  ParamInfo.shape: ParamInfo#shape.
  ParamInfo.attrs: ParamInfo#attrs.
  ParamInfo.size: ParamInfo#size.
  MultimodalTypes: MultimodalTypes#
  Sample.group_index: Sample#group_index.
  Sample.weight_versions: Sample#weight_versions.
  Sample.remove_sample: Sample#remove_sample.
  Sample.Status.FAILED: Sample#Status#FAILED.
  Sample.generate_function_path: Sample#generate_function_path.
  Sample.non_generation_time: Sample#non_generation_time.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/types.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py)

## Classes
### `MultimodalType`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/types.py:194`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L194)
- signature: `class MultimodalType:`
- members:
  - `name` — [`L195`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L195)
  - `placeholder` — [`L196`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L196)
- used by: [`_build_messages`](data.md#_build_messages), [`all`](types.md#MultimodalTypes.all), [`AUDIO`](types.md#MultimodalTypes.AUDIO), [`IMAGE`](types.md#MultimodalTypes.IMAGE), [`VIDEO`](types.md#MultimodalTypes.VIDEO), [`get`](types.md#MultimodalTypes.get)

### `MultimodalTypes`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/types.py:199`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L199)
- signature: `class MultimodalTypes:`
- members:
  - `all(cls)` — [`L205`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L205)
  - `get(cls, name: str)` — [`L209`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L209)
  - `AUDIO` — [`L202`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L202)
  - `IMAGE` — [`L200`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L200)
  - `VIDEO` — [`L201`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L201)
- uses (calls/refs, reference-scoped): [`MultimodalType`](types.md#MultimodalType), [`name`](types.md#MultimodalType.name), [`placeholder`](types.md#MultimodalType.placeholder)
- used by: [`_build_messages`](data.md#_build_messages)

### `ParamInfo`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/types.py:178`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L178)
- signature: `class ParamInfo:`
- members:
  - `attrs` — [`L182`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L182)
  - `dtype` — [`L180`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L180)
  - `name` — [`L179`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L179)
  - `shape` — [`L181`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L181)
  - `size` — [`L183`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L183)
  - `src_rank` — [`L184`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L184)
- used by: [`_get_megatron_local_param_infos`](../backends/megatron_utils/update_weight/hf_weight_iterator_direct.md#_get_megatron_local_param_infos), [`_get_megatron_full_params`](../backends/megatron_utils/update_weight/hf_weight_iterator_direct.md#_get_megatron_full_params), [`_convert_to_hf_named_tensors`](../backends/megatron_utils/update_weight/hf_weight_iterator_direct.md#HfWeightIteratorDirect._convert_to_hf_named_tensors), [`_get_megatron_local_param_info_buckets`](../backends/megatron_utils/update_weight/hf_weight_iterator_direct.md#_get_megatron_local_param_info_buckets), [`all_gather_params_async`](../backends/megatron_utils/update_weight/common.md#all_gather_params_async)

### `PrefixCacheInfo`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/types.py:94`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L94)
- signature: `class PrefixCacheInfo:`
- members:
  - `add(self, meta_info: dict)` — [`L102`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L102)
  - `from_dict(data: dict)` — [`L114`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L114)
  - `prefix_cache_hit_rate(self)` — [`L99`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L99)
  - `to_dict(self)` — [`L107`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L107)
  - `cached_tokens` — [`L95`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L95)
  - `total_prompt_tokens` — [`L96`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L96)
- uses (calls/refs, reference-scoped): [`Sample`](types.md#Sample)
- used by: [`update_from_meta_info`](types.md#Sample.update_from_meta_info), [`from_dict`](types.md#Sample.from_dict), [`to_dict`](types.md#Sample.to_dict), [`_compute_prefix_cache_metrics`](../ray/rollout.md#_compute_prefix_cache_metrics), [`prefix_cache_info`](types.md#Sample.prefix_cache_info)

### `Sample`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/types.py:9`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L9)
- doc: The sample generated
- signature: `class Sample:`
- members:
  - `effective_response_length(self)` — [`L150`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L150)
  - `from_dict(data: dict)` — [`L130`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L130)
  - `get_reward_value(self, args)` — [`L146`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L146)
  - `to_dict(self)` — [`L122`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L122)
  - `update_from_meta_info(self, args, meta_info: dict)` — [`L153`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L153) — Update the sample with new information from meta_info returned by the rollout engine.
  - `generate_function_path` — [`L44`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L44)
  - `group_index` — [`L12`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L12)
  - `index` — [`L13`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L13)
  - `label` — [`L22`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L22)
  - `loss_mask` — [`L24`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L24)
  - `metadata` — [`L43`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L43)
  - `multimodal_inputs` — [`L17`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L17)
  - `multimodal_train_inputs` — [`L18`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L18)
  - `non_generation_time` — [`L51`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L51)
  - `prefix_cache_info` — [`L120`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L120)
  - `prompt` — [`L15`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L15)
  - `remove_sample` — [`L28`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L28)
  - `response` — [`L20`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L20)
  - `response_length` — [`L21`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L21)
  - `reward` — [`L23`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L23)
  - `rollout_log_probs` — [`L26`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L26)
  - `rollout_routed_experts` — [`L27`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L27)
  - `session_id` — [`L49`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L49)
  - `spec_info` — [`L91`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L91)
  - `status` — [`L41`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L41)
  - `teacher_log_probs` — [`L29`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L29)
  - `tokens` — [`L16`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L16)
  - `train_metadata` — [`L46`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L46)
  - `weight_versions` — [`L25`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L25)
- uses (calls/refs, reference-scoped): [`Status`](types.md#Sample.Status), [`from_dict`](types.md#Sample.SpecInfo.from_dict), [`add`](types.md#Sample.SpecInfo.add), [`from_dict`](types.md#Sample.PrefixCacheInfo.from_dict), [`to_dict`](types.md#Sample.SpecInfo.to_dict), [`TRUNCATED`](types.md#Sample.Status.TRUNCATED), [`add`](types.md#Sample.PrefixCacheInfo.add), [`to_dict`](types.md#Sample.PrefixCacheInfo.to_dict), [`ABORTED`](types.md#Sample.Status.ABORTED), [`PrefixCacheInfo`](types.md#Sample.PrefixCacheInfo), [`SpecInfo`](types.md#Sample.SpecInfo), [`COMPLETED`](types.md#Sample.Status.COMPLETED), [`PENDING`](types.md#Sample.Status.PENDING)
- used by: [`generate`](../rollout/sglang_rollout.md#generate), [`eval_rollout_single_dataset`](../rollout/sglang_rollout.md#eval_rollout_single_dataset), [`generate_rollout_async`](../rollout/sglang_rollout.md#generate_rollout_async), [`generate_and_rm`](../rollout/sglang_rollout.md#generate_and_rm), [`_convert_samples_to_train_data`](../ray/rollout.md#RolloutManager._convert_samples_to_train_data), [`async_rm`](../rollout/rm_hub/__init__.md#async_rm), [`get_samples`](../rollout/data_source.md#RolloutDataSource.get_samples), [`postprocess_sample_with_radix_tree`](../router/middleware_hub/radix_tree_middleware.md#postprocess_sample_with_radix_tree), [`_get_rollout_data`](../ray/rollout.md#RolloutManager._get_rollout_data), [`generate_and_rm_group`](../rollout/sglang_rollout.md#generate_and_rm_group), [`compute_metrics_from_samples`](../ray/rollout.md#compute_metrics_from_samples), [`logger`](../rollout/rm_hub/__init__.md#logger), [`__init__`](data.md#Dataset.__init__), [`abort`](../rollout/sglang_rollout.md#abort), [`from_dict`](types.md#Sample.SpecInfo.from_dict), [`remote_rm`](../rollout/rm_hub/__init__.md#remote_rm), [`submit_generate_tasks`](../rollout/sglang_rollout.md#GenerateState.submit_generate_tasks), [`check_reward_nonzero_std`](../rollout/filter_hub/dynamic_sampling_filters.md#check_reward_nonzero_std), [`_get_samples_from_buffer`](../rollout/data_source.md#RolloutDataSourceWithBuffer._get_samples_from_buffer), [`_post_process_rewards`](../ray/rollout.md#RolloutManager._post_process_rewards), [`eval_rollout`](../rollout/sglang_rollout.md#eval_rollout), [`filter_long_prompt`](data.md#filter_long_prompt), [`from_dict`](types.md#Sample.PrefixCacheInfo.from_dict), [`batched_async_rm`](../rollout/rm_hub/__init__.md#batched_async_rm), [`_compute_prefix_cache_metrics`](../ray/rollout.md#_compute_prefix_cache_metrics), [`_compute_spec_metrics`](../ray/rollout.md#_compute_spec_metrics), [`generate_with_random_osl`](../rollout/generate_hub/benchmarkers.md#generate_with_random_osl), [`post_process_rewards`](../rollout/on_policy_distillation.md#post_process_rewards), [`_compute_zero_std_metrics`](../ray/rollout.md#_compute_zero_std_metrics), [`add_samples`](../rollout/data_source.md#RolloutDataSourceWithBuffer.add_samples), [`get_samples`](../rollout/data_source.md#RolloutDataSourceWithBuffer.get_samples), [`_compute_reward_cat_metrics`](../ray/rollout.md#_compute_reward_cat_metrics), [`_is_zero_std`](../ray/rollout.md#_compute_zero_std_metrics._is_zero_std), [`samples`](../rollout/base_types.md#RolloutFnTrainOutput.samples), [`add_samples`](../rollout/data_source.md#DataSource.add_samples), [`add_samples`](../rollout/data_source.md#RolloutDataSource.add_samples), [`get_samples`](../rollout/data_source.md#DataSource.get_samples), [`pop_first`](../rollout/data_source.md#pop_first)

### `SpecInfo`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/types.py:54`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L54)
- signature: `class SpecInfo:`
- members:
  - `add(self, meta_info: dict)` — [`L68`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L68)
  - `from_dict(data: dict)` — [`L83`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L83)
  - `spec_accept_length(self)` — [`L65`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L65)
  - `spec_accept_rate(self)` — [`L61`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L61)
  - `to_dict(self)` — [`L74`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L74)
  - `completion_token_num` — [`L58`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L58)
  - `spec_accept_token_num` — [`L55`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L55)
  - `spec_draft_token_num` — [`L56`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L56)
  - `spec_verify_ct` — [`L57`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L57)
- uses (calls/refs, reference-scoped): [`Sample`](types.md#Sample)
- used by: [`update_from_meta_info`](types.md#Sample.update_from_meta_info), [`from_dict`](types.md#Sample.from_dict), [`to_dict`](types.md#Sample.to_dict), [`_compute_spec_metrics`](../ray/rollout.md#_compute_spec_metrics), [`spec_info`](types.md#Sample.spec_info)

### `Status`  ·  implements/extends Enum
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/types.py:31`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L31)
- signature: `class Status(Enum):`
- members:
  - `ABORTED` — [`L35`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L35)
  - `COMPLETED` — [`L33`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L33)
  - `FAILED` — [`L39`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L39)
  - `PENDING` — [`L32`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L32)
  - `TRUNCATED` — [`L34`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L34)
- used by: [`generate`](../rollout/sglang_rollout.md#generate), [`eval_rollout_single_dataset`](../rollout/sglang_rollout.md#eval_rollout_single_dataset), [`generate_and_rm`](../rollout/sglang_rollout.md#generate_and_rm), [`_convert_samples_to_train_data`](../ray/rollout.md#RolloutManager._convert_samples_to_train_data), [`update_from_meta_info`](types.md#Sample.update_from_meta_info), [`compute_metrics_from_samples`](../ray/rollout.md#compute_metrics_from_samples), [`status`](types.md#Sample.status), [`from_dict`](types.md#Sample.from_dict)

## Module values
- `RolloutBatch` — [`L190`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/types.py#L190)


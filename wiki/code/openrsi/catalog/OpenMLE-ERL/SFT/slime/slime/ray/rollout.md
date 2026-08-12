---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/ray/rollout.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/ray/rollout.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.ray.rollout`/
symbols:
  RolloutManager.args: RolloutManager#args.
  RolloutManager._convert_samples_to_train_data: RolloutManager#_convert_samples_to_train_data().
  start_rollout_server: start_rollout_server().
  EngineGroup.start_engines: EngineGroup#start_engines().
  RolloutManager.generate: RolloutManager#generate().
  RolloutManager.server: RolloutManager#server.
  RolloutManager._get_rollout_data: RolloutManager#_get_rollout_data().
  RolloutManager.eval: RolloutManager#eval().
  compute_metrics_from_samples: compute_metrics_from_samples().
  logger: logger.
  RolloutManager._health_monitors: RolloutManager#_health_monitors.
  RolloutServer.recover: RolloutServer#recover().
  _log_eval_rollout_data: _log_eval_rollout_data().
  _log_rollout_data: _log_rollout_data().
  RolloutServer.engine_groups: RolloutServer#engine_groups.
  RolloutManager.recover_rollout_engines: RolloutManager#recover_rollout_engines().
  RolloutManager._try_ci_fault_injection: RolloutManager#_try_ci_fault_injection().
  _start_router: _start_router().
  EngineGroup.all_engines: EngineGroup#all_engines.
  RolloutManager.custom_convert_samples_to_train_data_func: RolloutManager#custom_convert_samples_to_train_data_func.
  EngineGroup.args: EngineGroup#args.
  RolloutServer.num_new_engines: RolloutServer#num_new_engines().
  RolloutManager._post_process_rewards: RolloutManager#_post_process_rewards().
  RolloutManager._split_train_data_by_dp: RolloutManager#_split_train_data_by_dp().
  RolloutManager.custom_reward_post_process_func: RolloutManager#custom_reward_post_process_func.
  EngineGroup.num_new_engines: EngineGroup#num_new_engines.
  RolloutManager.get_rollout_engines_and_lock: RolloutManager#get_rollout_engines_and_lock().
  RolloutManager.save_db_snapshot: RolloutManager#save_db_snapshot().
  _compute_spec_metrics: _compute_spec_metrics().
  _compute_prefix_cache_metrics: _compute_prefix_cache_metrics().
  RolloutServer: RolloutServer#
  RolloutManager._dynamic_global_batch_size: RolloutManager#_dynamic_global_batch_size.
  RolloutManager.rollout_engines: RolloutManager#rollout_engines().
  RolloutManager._compute_dynamic_global_batch_size: RolloutManager#_compute_dynamic_global_batch_size().
  compute_perf_metrics_from_samples: compute_perf_metrics_from_samples().
  _compute_zero_std_metrics: _compute_zero_std_metrics().
  EngineGroup.engines: EngineGroup#engines().
  RolloutManager.offload: RolloutManager#offload().
  RolloutManager.onload: RolloutManager#onload().
  RolloutManager._save_debug_rollout_data: RolloutManager#_save_debug_rollout_data().
  RolloutServer.engines: RolloutServer#engines().
  RolloutServer.offload: RolloutServer#offload().
  RolloutServer.onload: RolloutServer#onload().
  RolloutManager.generate_rollout: RolloutManager#generate_rollout.
  RolloutManager.eval_generate_rollout: RolloutManager#eval_generate_rollout.
  _allocate_rollout_engine_addr_and_ports_normal: _allocate_rollout_engine_addr_and_ports_normal().
  _allocate_rollout_engine_addr_and_ports_normal.get_addr_and_ports: _allocate_rollout_engine_addr_and_ports_normal().get_addr_and_ports().
  _compute_zero_std_metrics._is_zero_std: _compute_zero_std_metrics()._is_zero_std().
  _compute_reward_cat_metrics: _compute_reward_cat_metrics().
  RolloutManager.rollout_engine_lock: RolloutManager#rollout_engine_lock.
  EngineGroup.nodes_per_engine: EngineGroup#nodes_per_engine.
  EngineGroup.role: EngineGroup#role.
  RolloutServer.all_engines: RolloutServer#all_engines().
  RolloutServer.nodes_per_engine: RolloutServer#nodes_per_engine().
  RolloutManager.data_source: RolloutManager#data_source.
  RolloutManager.get_num_rollout_per_epoch: RolloutManager#get_num_rollout_per_epoch().
  RolloutManager.clear_num_new_engines: RolloutManager#clear_num_new_engines().
  RolloutManager._ci_fault_injection_pending: RolloutManager#_ci_fault_injection_pending.
  RolloutManager.health_monitoring_pause: RolloutManager#health_monitoring_pause().
  RolloutManager.health_monitoring_resume: RolloutManager#health_monitoring_resume().
  EngineGroup: EngineGroup#
  EngineGroup.pg: EngineGroup#pg.
  EngineGroup.offload: EngineGroup#offload().
  EngineGroup.onload: EngineGroup#onload().
  EngineGroup.rank_offset: EngineGroup#rank_offset.
  RolloutManager.__init__: RolloutManager#__init__().
  RolloutManager.dispose: RolloutManager#dispose().
  RolloutManager.save: RolloutManager#save().
  RolloutManager.load: RolloutManager#load().
  RolloutManager.onload_weights: RolloutManager#onload_weights().
  RolloutManager.onload_kv: RolloutManager#onload_kv().
  RolloutManager.check_weights: RolloutManager#check_weights().
  RolloutManager: RolloutManager#
  RolloutManager.rollout_id: RolloutManager#rollout_id.
  RolloutManager.train_parallel_config: RolloutManager#train_parallel_config.
  compute_perf_metrics_from_samples.token_perf: compute_perf_metrics_from_samples().token_perf().
  _run_maybe_awaitable: _run_maybe_awaitable().
  RolloutServer.router_ip: RolloutServer#router_ip.
  RolloutServer.router_port: RolloutServer#router_port.
  _allocate_rollout_engine_addr_and_ports_external: _allocate_rollout_engine_addr_and_ports_external().
  _allocate_rollout_engine_addr_and_ports_normal.get_addr_and_ports.port: _allocate_rollout_engine_addr_and_ports_normal().get_addr_and_ports().port().
  _allocate_rollout_engine_addr_and_ports_normal.get_addr_and_ports.addr: _allocate_rollout_engine_addr_and_ports_normal().get_addr_and_ports().addr().
  RolloutManager.pg: RolloutManager#pg.
  RolloutManager.set_train_parallel_config: RolloutManager#set_train_parallel_config().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/ray/rollout.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py)

## Classes
### `EngineGroup`
- def: [`OpenMLE-ERL/SFT/slime/slime/ray/rollout.py:49`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L49)
- doc: A group of homogeneous SGLang engines with the same configuration.
- signature: `class EngineGroup:`
- members:
  - `engines(self)` — [`L66`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L66) — Node-0 engines only (for multi-node serving).
  - `offload(self)` — [`L150`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L150) — Fire release_memory_occupation on all engines (non-blocking).
  - `onload(self, tags: list[str] | None = None)` — [`L157`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L157) — Fire resume_memory_occupation on all engines (non-blocking).
  - `start_engines(self)` — [`L70`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L70) — Create Ray actors, allocate ports, and fire ``engine.init()`` without waiting.
  - `all_engines` — [`L59`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L59)
  - `args` — [`L57`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L57)
  - `nodes_per_engine` — [`L60`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L60)
  - `num_new_engines` — [`L61`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L61)
  - `pg` — [`L58`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L58)
  - `rank_offset` — [`L63`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L63)
  - `role` — [`L62`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L62)
- uses (calls/refs, reference-scoped): [`_allocate_rollout_engine_addr_and_ports_normal`](rollout.md#_allocate_rollout_engine_addr_and_ports_normal), [`NOSET_VISIBLE_DEVICES_ENV_VARS_LIST`](utils.md#NOSET_VISIBLE_DEVICES_ENV_VARS_LIST), [`SGLangEngine`](../backends/sglang_utils/sglang_engine.md#SGLangEngine), [`_allocate_rollout_engine_addr_and_ports_external`](rollout.md#_allocate_rollout_engine_addr_and_ports_external)
- used by: [`start_rollout_server`](rollout.md#start_rollout_server), [`recover`](rollout.md#RolloutServer.recover), [`engine_groups`](rollout.md#RolloutServer.engine_groups), [`_try_ci_fault_injection`](rollout.md#RolloutManager._try_ci_fault_injection), [`num_new_engines`](rollout.md#RolloutServer.num_new_engines), [`RolloutServer`](rollout.md#RolloutServer), [`engines`](rollout.md#RolloutServer.engines), [`offload`](rollout.md#RolloutServer.offload), [`onload`](rollout.md#RolloutServer.onload), [`all_engines`](rollout.md#RolloutServer.all_engines), [`nodes_per_engine`](rollout.md#RolloutServer.nodes_per_engine)

### `RolloutManager`
- def: [`OpenMLE-ERL/SFT/slime/slime/ray/rollout.py:261`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L261)
- doc: The class to run rollout and convert rollout data to training data.
- signature: `class RolloutManager:`
- members:
  - `_compute_dynamic_global_batch_size(self, num_samples: int)` — [`L484`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L484) — Calculate dynamic global_batch_size to ensure only one training step.
  - `_convert_samples_to_train_data(self, samples: list[Sample] | list[list[Sample]])` — [`L557`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L557) — Convert inference generated samples to training data.
  - `_split_train_data_by_dp(self, data, dp_size)` — [`L625`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L625) — Split the train data by data parallel size.
  - `_try_ci_fault_injection(self)` — [`L304`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L304) — Try to inject fault during generate (when health monitor is running).
  - `check_weights(self, action: str)` — [`L439`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L439)
  - `clear_num_new_engines(self)` — [`L426`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L426)
  - `dispose(self)` — [`L325`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L325)
  - `eval(self, rollout_id)` — [`L360`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L360)
  - `generate(self, rollout_id)` — [`L345`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L345)
  - `get_num_rollout_per_epoch(self)` — [`L341`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L341)
  - `get_rollout_engines_and_lock(self)` — [`L337`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L337)
  - `health_monitoring_pause(self)` — [`L431`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L431)
  - `health_monitoring_resume(self)` — [`L435`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L435)
  - `load(self, rollout_id=None)` — [`L398`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L398)
  - `offload(self)` — [`L401`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L401)
  - `onload(self, tags: list[str] | None = None)` — [`L406`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L406)
  - `onload_kv(self)` — [`L413`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L413)
  - `onload_weights(self)` — [`L410`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L410)
  - `recover_rollout_engines(self)` — [`L416`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L416) — Restart any dead rollout engines and update num_new_engines for update_weights detection.
  - `rollout_engines(self)` — [`L332`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L332)
  - `save(self, rollout_id)` — [`L371`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L371)
  - `save_db_snapshot(self, rollout_id)` — [`L374`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L374) — Save program DB snapshot for the current rollout when enabled.
  - `set_train_parallel_config(self, config: dict)` — [`L622`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L622)
  - `args` — [`L268`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L268)
  - `custom_convert_samples_to_train_data_func` — [`L280`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L280)
  - `custom_reward_post_process_func` — [`L277`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L277)
  - `data_source` — [`L273`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L273)
  - `eval_generate_rollout` — [`L276`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L276)
  - `generate_rollout` — [`L275`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L275)
  - `pg` — [`L267`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L267)
  - `rollout_engine_lock` — [`L293`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L293)
  - `rollout_id` — [`L294`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L294)
  - `server` — [`L289`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L289)
  - `train_parallel_config` — [`L623`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L623)
- protocol/private: `__init__`[`L264`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L264), `_ci_fault_injection_pending`[`L302`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L302), `_dynamic_global_batch_size`[`L470`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L470), `_get_rollout_data`[`L442`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L442), `_health_monitors`[`L296`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L296), `_post_process_rewards`[`L530`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L530), `_save_debug_rollout_data`[`L511`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L511)
- uses (calls/refs, reference-scoped): [`Sample`](../utils/types.md#Sample), [`start_rollout_server`](rollout.md#start_rollout_server), [`load_function`](../utils/misc.md#load_function), [`logger`](rollout.md#logger), [`status`](../utils/types.md#Sample.status), [`_log_eval_rollout_data`](rollout.md#_log_eval_rollout_data), [`_log_rollout_data`](rollout.md#_log_rollout_data), [`recover`](rollout.md#RolloutServer.recover), [`engine_groups`](rollout.md#RolloutServer.engine_groups), [`Status`](../utils/types.md#Sample.Status), [`from_dict`](../utils/types.md#Sample.from_dict), [`start`](../utils/health_monitor.md#RolloutHealthMonitor.start), [`init_tracking`](../utils/logging_utils.md#init_tracking), [`loss_mask`](../utils/types.md#Sample.loss_mask), [`configure_logger`](../utils/logging_utils.md#configure_logger), [`response_length`](../utils/types.md#Sample.response_length), [`all_engines`](rollout.md#EngineGroup.all_engines), [`call_rollout_fn`](../rollout/base_types.md#call_rollout_fn), [`metadata`](../utils/types.md#Sample.metadata), [`init_http_client`](../utils/http_utils.md#init_http_client), [`get_seqlen_balanced_partitions`](../utils/seqlen_balancing.md#get_seqlen_balanced_partitions), [`num_new_engines`](rollout.md#RolloutServer.num_new_engines), [`tokens`](../utils/types.md#Sample.tokens), [`Box`](../utils/misc.md#Box), [`get_reward_value`](../utils/types.md#Sample.get_reward_value), [`TRUNCATED`](../utils/types.md#Sample.Status.TRUNCATED), [`engines`](rollout.md#RolloutServer.engines), [`offload`](rollout.md#RolloutServer.offload), [`onload`](rollout.md#RolloutServer.onload), [`rollout_log_probs`](../utils/types.md#Sample.rollout_log_probs), [`samples`](../rollout/base_types.md#RolloutFnTrainOutput.samples), [`Lock`](utils.md#Lock), [`data`](../rollout/base_types.md#RolloutFnEvalOutput.data), [`multimodal_train_inputs`](../utils/types.md#Sample.multimodal_train_inputs), [`rollout_routed_experts`](../utils/types.md#Sample.rollout_routed_experts), [`teacher_log_probs`](../utils/types.md#Sample.teacher_log_probs), [`RolloutHealthMonitor`](../utils/health_monitor.md#RolloutHealthMonitor), [`index`](../utils/types.md#Sample.index), [`metrics`](../rollout/base_types.md#RolloutFnEvalOutput.metrics), [`train_metadata`](../utils/types.md#Sample.train_metadata)  (+2 more)
- used by: [`create_rollout_manager`](placement_group.md#create_rollout_manager)

### `RolloutServer`
- def: [`OpenMLE-ERL/SFT/slime/slime/ray/rollout.py:166`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L166)
- doc: A model served behind a shared router, with one or more engine groups.
- signature: `class RolloutServer:`
- members:
  - `all_engines(self)` — [`L193`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L193) — All engines (including non-node-0) across all groups.
  - `engines(self)` — [`L188`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L188) — All node-0 engines across all groups.
  - `nodes_per_engine(self)` — [`L207`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L207) — Nodes per engine. Only valid when all groups share the same value.
  - `num_new_engines(self)` — [`L198`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L198)
  - `offload(self)` — [`L245`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L245) — Release memory occupation across all groups (concurrent).
  - `onload(self, tags: list[str] | None = None)` — [`L252`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L252) — Resume memory occupation across all groups (concurrent).
  - `recover(self)` — [`L216`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L216) — Recover dead engines across all groups, overlapping init.
  - `engine_groups` — [`L183`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L183)
  - `router_ip` — [`L184`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L184)
  - `router_port` — [`L185`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L185)
- uses (calls/refs, reference-scoped): [`start_engines`](rollout.md#EngineGroup.start_engines), [`logger`](rollout.md#logger), [`all_engines`](rollout.md#EngineGroup.all_engines), [`args`](rollout.md#EngineGroup.args), [`num_new_engines`](rollout.md#EngineGroup.num_new_engines), [`engines`](rollout.md#EngineGroup.engines), [`nodes_per_engine`](rollout.md#EngineGroup.nodes_per_engine), [`role`](rollout.md#EngineGroup.role), [`EngineGroup`](rollout.md#EngineGroup), [`offload`](rollout.md#EngineGroup.offload), [`onload`](rollout.md#EngineGroup.onload)
- used by: [`start_rollout_server`](rollout.md#start_rollout_server), [`_health_monitors`](rollout.md#RolloutManager._health_monitors), [`recover_rollout_engines`](rollout.md#RolloutManager.recover_rollout_engines), [`_try_ci_fault_injection`](rollout.md#RolloutManager._try_ci_fault_injection), [`get_rollout_engines_and_lock`](rollout.md#RolloutManager.get_rollout_engines_and_lock), [`rollout_engines`](rollout.md#RolloutManager.rollout_engines), [`offload`](rollout.md#RolloutManager.offload), [`onload`](rollout.md#RolloutManager.onload), [`clear_num_new_engines`](rollout.md#RolloutManager.clear_num_new_engines)

## Functions
- `_allocate_rollout_engine_addr_and_ports_external(args, rollout_engines)` — [`L678`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L678)
- `_allocate_rollout_engine_addr_and_ports_normal(*, args, num_engines, rollout_engines, worker_type="regular")` — [`L694`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L694)
- `_compute_prefix_cache_metrics(args, all_samples: list[Sample])` — [`L1019`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L1019)
- `_compute_reward_cat_metrics(args, all_samples: list[Sample])` — [`L1030`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L1030)
- `_compute_spec_metrics(args, all_samples: list[Sample])` — [`L1009`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L1009)
- `_compute_zero_std_metrics(args, all_samples: list[Sample])` — [`L992`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L992)
- `_is_zero_std(samples: list[Sample])` — [`L997`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L997)
- `_log_eval_rollout_data(rollout_id, args, data, extra_metrics: dict[str, Any] | None = None)` — [`L896`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L896)
- `_log_rollout_data(rollout_id, args, samples, rollout_extra_metrics, rollout_time)` — [`L929`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L929)
- `_run_maybe_awaitable(func, *args, **kwargs)` — [`L40`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L40) — Execute sync hooks directly and async hooks via a temporary event loop.
- `_start_router(args)` — [`L767`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L767) — Start sgl router or slime router and return (router_ip, router_port).
- `addr()` — [`L731`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L731)
- `compute_metrics_from_samples(args, samples)` — [`L947`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L947)
- `compute_perf_metrics_from_samples(args, samples, rollout_time)` — [`L959`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L959)
- `get_addr_and_ports(engine)` — [`L715`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L715)
- `port(consecutive=1)` — [`L720`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L720)
- `start_rollout_server(args, pg)` — [`L823`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L823) — Start a complete rollout server: one router + a set of SGLang engines.
- `token_perf(response_lengths, non_generation_time, key="")` — [`L967`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L967)

## Module values
- `logger` — [`L37`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/rollout.py#L37)


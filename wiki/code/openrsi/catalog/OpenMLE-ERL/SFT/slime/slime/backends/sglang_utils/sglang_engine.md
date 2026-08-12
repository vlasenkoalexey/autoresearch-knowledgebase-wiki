---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.sglang_utils.sglang_engine`/
symbols:
  SGLangEngine.server_port: SGLangEngine#server_port.
  SGLangEngine.process: SGLangEngine#process.
  SGLangEngine.shutdown: SGLangEngine#shutdown().
  SGLangEngine._init_external: SGLangEngine#_init_external().
  SGLangEngine.server_host: SGLangEngine#server_host.
  SGLangEngine._make_request: SGLangEngine#_make_request().
  SGLangEngine.init: SGLangEngine#init().
  SGLangEngine.simulate_crash: SGLangEngine#simulate_crash().
  SGLangEngine.router_port: SGLangEngine#router_port.
  SGLangEngine.flush_cache: SGLangEngine#flush_cache().
  _compute_server_args: _compute_server_args().
  SGLangEngine.router_ip: SGLangEngine#router_ip.
  logger: logger.
  SGLangEngine.args: SGLangEngine#args.
  SGLangEngine._init_normal: SGLangEngine#_init_normal().
  SGLangEngine.health_generate: SGLangEngine#health_generate().
  SGLangEngine.get_weight_version: SGLangEngine#get_weight_version().
  SGLangEngine.node_rank: SGLangEngine#node_rank.
  SGLangEngine._get_actual_server_args: SGLangEngine#_get_actual_server_args().
  SGLangEngine.release_memory_occupation: SGLangEngine#release_memory_occupation().
  SGLangEngine.pause_generation: SGLangEngine#pause_generation().
  SGLangEngine.continue_generation: SGLangEngine#continue_generation().
  SGLangEngine.start_profile: SGLangEngine#start_profile().
  SGLangEngine.stop_profile: SGLangEngine#stop_profile().
  SGLangEngine: SGLangEngine#
  SGLangEngine.worker_type: SGLangEngine#worker_type.
  launch_server_process: launch_server_process().
  SGLangEngine.update_weights_from_tensor: SGLangEngine#update_weights_from_tensor().
  SGLangEngine.resume_memory_occupation: SGLangEngine#resume_memory_occupation().
  SGLangEngine.check_weights: SGLangEngine#check_weights().
  SGLangEngine.init_weights_update_group: SGLangEngine#init_weights_update_group().
  SGLangEngine.destroy_weights_update_group: SGLangEngine#destroy_weights_update_group().
  SGLangEngine.update_weights_from_distributed: SGLangEngine#update_weights_from_distributed().
  SGLangEngine.post_process_weights: SGLangEngine#post_process_weights().
  _wait_server_healthy: _wait_server_healthy().
  SGLangEngine.rank: SGLangEngine#rank.
  SGLangEngine._format_v6_uri: SGLangEngine#_format_v6_uri().
  get_base_gpu_id: get_base_gpu_id().
  _to_local_gpu_id: _to_local_gpu_id().
  SGLangEngine.base_gpu_id: SGLangEngine#base_gpu_id.
  SGLangEngine._sanity_check_server_args: SGLangEngine#_sanity_check_server_args().
  _EXTERNAL_ENGINE_SKIP_CHECK_FIELDS: _EXTERNAL_ENGINE_SKIP_CHECK_FIELDS.
  SGLangEngine.__init__: SGLangEngine#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py)

## Classes
### `SGLangEngine`  ·  implements/extends RayActor
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py:109`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L109)
- signature: `class SGLangEngine(RayActor):`
- members:
  - `_make_request(self, endpoint: str, payload: dict | None = None)` — [`L206`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L206) — Make a POST request to the specified endpoint with the given payload.
  - `check_weights(self, action: str)` — [`L349`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L349)
  - `continue_generation(self)` — [`L399`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L399)
  - `destroy_weights_update_group(self, group_name)` — [`L365`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L365)
  - `flush_cache(self)` — [`L275`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L275) — Flush the cache of the server.
  - `get_weight_version(self)` — [`L328`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L328)
  - `health_generate(self, timeout: float = 5)` — [`L228`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L228) — Run /health_generate on the underlying SGLang HTTP server.
  - `init(self, dist_init_addr, port, nccl_port, host=None, disaggregation_bootstrap_port=None)` — [`L116`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L116)
  - `init_weights_update_group(self, master_address, master_port, rank_offset, world_size, group_name, backend)` — [`L352`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L352)
  - `pause_generation(self)` — [`L394`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L394)
  - `post_process_weights(self, restore_weights_before_load: bool = False, post_process_quantization: bool = False)` — [`L404`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L404) — Update model weights from tensor data. The HTTP server will only post meta data, and the real weights will be copied directly from GPUs.
  - `release_memory_occupation(self)` — [`L336`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L336)
  - `resume_memory_occupation(self, tags: list[str] = None)` — [`L340`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L340) — Available tags for multi-stage resume: weights, kv_cache
  - `shutdown(self)` — [`L294`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L294)
  - `simulate_crash(self)` — [`L457`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L457)
  - `start_profile(self, output_dir: str | None = None, start_step: int | None = None, num_steps: int | None = None, activities: list[str] | None = None, profile_by_stage: bool = False, with_stack: bool | None = None, record_shapes: bool | None = None)` — [`L423`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L423)
  - `stop_profile(self)` — [`L452`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L452)
  - `update_weights_from_distributed(self, names, dtypes, shapes, group_name, flush_cache=False, weight_version: str | None = None)` — [`L377`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L377)
  - `update_weights_from_tensor(self, serialized_named_tensors: list[str], load_format: str | None = None, flush_cache: bool = False, weight_version: str | None = None)` — [`L250`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L250) — Update model weights from tensor data. The HTTP server will only post meta data, and the real weights will be copied directly from GPUs.
  - `args` — [`L111`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L111)
  - `base_gpu_id` — [`L114`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L114)
  - `node_rank` — [`L148`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L148)
  - `process` — [`L183`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L183)
  - `rank` — [`L112`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L112)
  - `router_ip` — [`L117`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L117)
  - `router_port` — [`L118`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L118)
  - `server_host` — [`L149`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L149)
  - `server_port` — [`L150`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L150)
  - `worker_type` — [`L113`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L113)
- protocol/private: `__init__`[`L110`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L110), `_format_v6_uri`[`L122`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L122), `_get_actual_server_args`[`L160`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L160), `_init_external`[`L157`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L157), `_init_normal`[`L181`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L181), `_sanity_check_server_args`[`L165`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L165)
- uses (calls/refs, reference-scoped): [`RayActor`](../../ray/ray_actor.md#RayActor), [`_compute_server_args`](sglang_engine.md#_compute_server_args), [`get_host_info`](../../utils/http_utils.md#get_host_info), [`logger`](sglang_engine.md#logger), [`launch_server_process`](sglang_engine.md#launch_server_process), [`_wait_server_healthy`](sglang_engine.md#_wait_server_healthy)
- used by: [`start_engines`](../../ray/rollout.md#EngineGroup.start_engines), [`RayActor`](../../ray/ray_actor.md#RayActor)

## Functions
- `_compute_server_args(args, rank, dist_init_addr, nccl_port, host, port, worker_type: str = "regular", disaggregation_bootstrap_port: int | None = None, base_gpu_id: int | None = None)` — [`L469`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L469)
- `_to_local_gpu_id(physical_gpu_id: int)` — [`L35`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L35)
- `_wait_server_healthy(base_url, api_key, is_process_alive)` — [`L73`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L73)
- `get_base_gpu_id(args, rank)` — [`L22`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L22)
- `launch_server_process(server_args: ServerArgs)` — [`L53`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L53)

## Module values
- `_EXTERNAL_ENGINE_SKIP_CHECK_FIELDS` — [`L544`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L544)
- `logger` — [`L19`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/sglang_utils/sglang_engine.py#L19)


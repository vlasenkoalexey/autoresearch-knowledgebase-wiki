---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.reloadable_process_group`/
symbols:
  ReloadableProcessGroup._fwd: ReloadableProcessGroup#_fwd().
  monkey_patch_torch_dist.get_new_comm_function: monkey_patch_torch_dist().get_new_comm_function().
  ReloadableProcessGroup: ReloadableProcessGroup#
  monkey_patch_torch_dist: monkey_patch_torch_dist().
  ReloadableProcessGroup.group: ReloadableProcessGroup#group.
  ReloadableProcessGroup.reload_process_groups: ReloadableProcessGroup#reload_process_groups().
  _wrap_low_level_call: _wrap_low_level_call().
  destroy_process_groups: destroy_process_groups().
  reload_process_groups: reload_process_groups().
  monkey_patch_torch_dist.get_new_query_function: monkey_patch_torch_dist().get_new_query_function().
  monkey_patch_torch_dist.get_new_comm_function.new_function: monkey_patch_torch_dist().get_new_comm_function().new_function().
  ReloadableProcessGroup.destroy_process_groups: ReloadableProcessGroup#destroy_process_groups().
  monkey_patch_torch_dist.get_new_p2pop_function.new_function.convert: monkey_patch_torch_dist().get_new_p2pop_function().new_function().convert().
  ReloadableProcessGroup._fwd_query: ReloadableProcessGroup#_fwd_query().
  monkey_patch_torch_dist.get_new_query_function.new_function: monkey_patch_torch_dist().get_new_query_function().new_function().
  ReloadableProcessGroup.GROUPS: ReloadableProcessGroup#GROUPS.
  ReloadableProcessGroup.group_info: ReloadableProcessGroup#group_info.
  monkey_patch_torch_dist.get_new_p2pop_function: monkey_patch_torch_dist().get_new_p2pop_function().
  ReloadableProcessGroup.bound_device_id: ReloadableProcessGroup#bound_device_id().
  old_new_group_dict: old_new_group_dict.
  monkey_patch_torch_dist.new_group: monkey_patch_torch_dist().new_group().
  monkey_patch_torch_dist.get_new_p2pop_function.new_function: monkey_patch_torch_dist().get_new_p2pop_function().new_function().
  logger: logger.
  ReloadableProcessGroup.__getattr__: ReloadableProcessGroup#__getattr__().
  ReloadableProcessGroup.rank: ReloadableProcessGroup#rank().
  ReloadableProcessGroup.size: ReloadableProcessGroup#size().
  ReloadableProcessGroup.name: ReloadableProcessGroup#name().
  ReloadableProcessGroup.shutdown: ReloadableProcessGroup#shutdown().
  ReloadableProcessGroup.abort: ReloadableProcessGroup#abort().
  ReloadableProcessGroup.barrier: ReloadableProcessGroup#barrier().
  ReloadableProcessGroup.broadcast: ReloadableProcessGroup#broadcast().
  ReloadableProcessGroup.allreduce: ReloadableProcessGroup#allreduce().
  ReloadableProcessGroup.allreduce_coalesced: ReloadableProcessGroup#allreduce_coalesced().
  ReloadableProcessGroup.reduce: ReloadableProcessGroup#reduce().
  ReloadableProcessGroup.allgather: ReloadableProcessGroup#allgather().
  ReloadableProcessGroup._allgather_base: ReloadableProcessGroup#_allgather_base().
  ReloadableProcessGroup.allgather_coalesced: ReloadableProcessGroup#allgather_coalesced().
  ReloadableProcessGroup.allgather_into_tensor_coalesced: ReloadableProcessGroup#allgather_into_tensor_coalesced().
  ReloadableProcessGroup.gather: ReloadableProcessGroup#gather().
  ReloadableProcessGroup.scatter: ReloadableProcessGroup#scatter().
  ReloadableProcessGroup.reduce_scatter: ReloadableProcessGroup#reduce_scatter().
  ReloadableProcessGroup._reduce_scatter_base: ReloadableProcessGroup#_reduce_scatter_base().
  ReloadableProcessGroup.reduce_scatter_tensor_coalesced: ReloadableProcessGroup#reduce_scatter_tensor_coalesced().
  ReloadableProcessGroup.alltoall_base: ReloadableProcessGroup#alltoall_base().
  ReloadableProcessGroup.alltoall: ReloadableProcessGroup#alltoall().
  ReloadableProcessGroup.send: ReloadableProcessGroup#send().
  ReloadableProcessGroup.recv: ReloadableProcessGroup#recv().
  ReloadableProcessGroup.recv_anysource: ReloadableProcessGroup#recv_anysource().
  ReloadableProcessGroup._start_coalescing: ReloadableProcessGroup#_start_coalescing().
  ReloadableProcessGroup._end_coalescing: ReloadableProcessGroup#_end_coalescing().
  ReloadableProcessGroup._get_backend_name: ReloadableProcessGroup#_get_backend_name().
  ReloadableProcessGroup._get_backend: ReloadableProcessGroup#_get_backend().
  ReloadableProcessGroup._set_default_backend: ReloadableProcessGroup#_set_default_backend().
  ReloadableProcessGroup.__init__: ReloadableProcessGroup#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py)

## Classes
### `ReloadableProcessGroup`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py:123`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L123)
- members:
  - `_fwd_query(self, method, *args, **kwargs)` — [`L196`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L196) — Forward non-communication calls without memory check.
  - `abort(self)` — [`L185`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L185)
  - `allgather(self, *a, **kw)` — [`L218`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L218)
  - `allgather_coalesced(self, *a, **kw)` — [`L224`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L224)
  - `allgather_into_tensor_coalesced(self, *a, **kw)` — [`L227`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L227)
  - `allreduce(self, *a, **kw)` — [`L209`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L209)
  - `allreduce_coalesced(self, *a, **kw)` — [`L212`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L212)
  - `alltoall(self, *a, **kw)` — [`L248`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L248)
  - `alltoall_base(self, *a, **kw)` — [`L245`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L245)
  - `barrier(self, *a, **kw)` — [`L203`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L203)
  - `bound_device_id(self)` — [`L276`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L276)
  - `broadcast(self, *a, **kw)` — [`L206`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L206)
  - `destroy_process_groups()` — [`L144`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L144)
  - `gather(self, *a, **kw)` — [`L230`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L230)
  - `name(self)` — [`L178`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L178)
  - `rank(self)` — [`L172`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L172)
  - `recv(self, *a, **kw)` — [`L254`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L254)
  - `recv_anysource(self, *a, **kw)` — [`L257`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L257)
  - `reduce(self, *a, **kw)` — [`L215`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L215)
  - `reduce_scatter(self, *a, **kw)` — [`L236`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L236)
  - `reduce_scatter_tensor_coalesced(self, *a, **kw)` — [`L242`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L242)
  - `reload_process_groups()` — [`L161`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L161)
  - `scatter(self, *a, **kw)` — [`L233`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L233)
  - `send(self, *a, **kw)` — [`L251`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L251)
  - `shutdown(self)` — [`L181`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L181)
  - `size(self)` — [`L175`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L175)
  - `GROUPS` — [`L124`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L124)
  - `group` — [`L131`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L131)
  - `group_info` — [`L132`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L132)
- protocol/private: `__getattr__`[`L140`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L140), `__init__`[`L126`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L126), `_allgather_base`[`L221`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L221), `_end_coalescing`[`L263`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L263), `_fwd`[`L189`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L189), `_get_backend`[`L269`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L269), `_get_backend_name`[`L266`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L266), `_reduce_scatter_base`[`L239`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L239), `_set_default_backend`[`L272`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L272), `_start_coalescing`[`L260`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L260)
- uses (calls/refs, reference-scoped): [`_wrap_low_level_call`](reloadable_process_group.md#_wrap_low_level_call), [`old_new_group_dict`](reloadable_process_group.md#old_new_group_dict), [`logger`](reloadable_process_group.md#logger)
- used by: [`destroy_process_groups`](reloadable_process_group.md#destroy_process_groups), [`reload_process_groups`](reloadable_process_group.md#reload_process_groups), [`new_function`](reloadable_process_group.md#monkey_patch_torch_dist.get_new_comm_function.new_function), [`convert`](reloadable_process_group.md#monkey_patch_torch_dist.get_new_p2pop_function.new_function.convert), [`new_function`](reloadable_process_group.md#monkey_patch_torch_dist.get_new_query_function.new_function), [`new_group`](reloadable_process_group.md#monkey_patch_torch_dist.new_group)

## Functions
- `_wrap_low_level_call()` — [`L295`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L295)
- `convert(arg)` — [`L104`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L104)
- `destroy_process_groups()` — [`L284`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L284) — Destroy all reloadable process groups.
- `get_new_comm_function(func)` — [`L60`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L60) — Wrap communication functions with memory check.
- `get_new_p2pop_function(func)` — [`L102`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L102)
- `get_new_query_function(func)` — [`L50`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L50) — Wrap query functions (get_rank, get_world_size, etc.) without memory check.
- `monkey_patch_torch_dist()` — [`L15`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L15)
- `new_function(*args, **kwargs)` — [`L53`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L53)
- `new_function(*args, **kwargs)` — [`L63`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L63)
- `new_function(*args, **kwargs)` — [`L103`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L103)
- `new_group(*args, **kwargs)` — [`L27`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L27)
- `reload_process_groups()` — [`L289`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L289) — Reload all reloadable process groups.

## Module values
- `logger` — [`L10`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L10)
- `old_new_group_dict` — [`L12`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/reloadable_process_group.py#L12)


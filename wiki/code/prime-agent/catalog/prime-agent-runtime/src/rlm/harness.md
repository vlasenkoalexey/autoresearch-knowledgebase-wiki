---
title: 'Module: prime-agent-runtime/src/rlm/harness.py'
type: catalog
provenance: extracted
module: prime-agent-runtime/src/rlm/harness.py
status: fresh
symbol_base: scip-python python prime-agent 0.0.0 `prime-agent-runtime.src.rlm.harness`/
symbols:
  HarnessState.overview: HarnessState#overview().
  HarnessState._upsert: HarnessState#_upsert().
  HarnessState.load: HarnessState#load().
  HarnessState.create: HarnessState#create().
  HarnessState.record_refinement: HarnessState#record_refinement().
  HarnessState.update: HarnessState#update().
  HarnessState.list: HarnessState#list().
  HarnessState.delete: HarnessState#delete().
  HarnessState.entries: HarnessState#entries.
  HarnessState._global_target: HarnessState#_global_target().
  HarnessEntry: HarnessEntry#
  HarnessState.upsert: HarnessState#upsert().
  HarnessState.get: HarnessState#get().
  HarnessState.file_path: HarnessState#file_path.
  get_harness_state: get_harness_state().
  HarnessState.snapshot: HarnessState#snapshot().
  HarnessState.save: HarnessState#save().
  HarnessState._sync_from_disk: HarnessState#_sync_from_disk().
  _KINDS._KINDS: _KINDS._KINDS.
  _state_file: _state_file().
  HarnessState: HarnessState#
  HarnessState.refinements: HarnessState#refinements.
  HarnessKind: HarnessKind.
  HarnessState.scope: HarnessState#scope.
  HarnessState._ensure_local_writable: HarnessState#_ensure_local_writable().
  HarnessState.create_skill: HarnessState#create_skill().
  HarnessState.update_skill: HarnessState#update_skill().
  _state_cache._state_cache: _state_cache._state_cache.
  HarnessEntry.kind: HarnessEntry#kind.
  HarnessState._loaded_mtime: HarnessState#_loaded_mtime.
  HarnessScope: HarnessScope.
  RefinementEvent: RefinementEvent#
  HarnessState._disk_mtime: HarnessState#_disk_mtime().
  _strip_scope_prefix: _strip_scope_prefix().
  HarnessState.create_memory: HarnessState#create_memory().
  HarnessState.update_memory: HarnessState#update_memory().
  HarnessState.create_prompt_note: HarnessState#create_prompt_note().
  HarnessState.update_prompt_note: HarnessState#update_prompt_note().
  HarnessState.create_subagent: HarnessState#create_subagent().
  HarnessState.update_subagent: HarnessState#update_subagent().
  HarnessEntry.scope: HarnessEntry#scope.
  _now: _now().
  HarnessEntry.title: HarnessEntry#title.
  HarnessEntry.path: HarnessEntry#path.
  HarnessEntry.reference: HarnessEntry#reference.
  HarnessEntry.arguments: HarnessEntry#arguments.
  HarnessEntry.updated_at: HarnessEntry#updated_at.
  _ENTRY_FIELDS: _ENTRY_FIELDS.
  _REFINEMENT_FIELDS: _REFINEMENT_FIELDS.
  _env_dir: _env_dir().
  HarnessEntry.id: HarnessEntry#id.
  HarnessEntry.content: HarnessEntry#content.
  HarnessEntry.created_at: HarnessEntry#created_at.
  RefinementEvent.created_at: RefinementEvent#created_at.
  HarnessState.__init__: HarnessState#__init__().
  HarnessState.delete_memory: HarnessState#delete_memory().
  HarnessState.delete_prompt_note: HarnessState#delete_prompt_note().
  HarnessState.delete_skill: HarnessState#delete_skill().
  HarnessState.delete_subagent: HarnessState#delete_subagent().
  _DEFAULT_FILE_NAME: _DEFAULT_FILE_NAME.
  _DEFAULT_HARNESS_DIR_NAME: _DEFAULT_HARNESS_DIR_NAME.
  _slug: _slug().
  _resolve_global_flag: _resolve_global_flag().
  HarnessEntry.metadata: HarnessEntry#metadata.
  HarnessEntry.source: HarnessEntry#source.
  HarnessEntry.version: HarnessEntry#version.
  RefinementEvent.id: RefinementEvent#id.
  RefinementEvent.trigger: RefinementEvent#trigger.
  RefinementEvent.changes: RefinementEvent#changes.
  _validate_python_skill_reference: _validate_python_skill_reference().
  HarnessState._local_write_error: HarnessState#_local_write_error.
  HarnessState._global_target_state_dir: HarnessState#_global_target_state_dir.
  _agent_dir: _agent_dir().
  RefinementEvent.evidence: RefinementEvent#evidence.
  RefinementEvent.outcome: RefinementEvent#outcome.
  HarnessState.plan_refinement: HarnessState#plan_refinement().
  __all__: __all__.
---
# Module: [`prime-agent-runtime/src/rlm/harness.py`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py)

## Classes
### `HarnessEntry`
- def: [`prime-agent-runtime/src/rlm/harness.py:94`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L94)
- doc: A reusable prompt, memory, skill, or subagent record.
- signature: `class HarnessEntry:`
- members:
  - `arguments` — [`L104`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L104)
  - `content` — [`L100`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L100)
  - `created_at` — [`L107`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L107)
  - `id` — [`L97`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L97)
  - `kind` — [`L98`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L98)
  - `metadata` — [`L105`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L105)
  - `path` — [`L101`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L101)
  - `reference` — [`L103`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L103)
  - `scope` — [`L102`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L102)
  - `source` — [`L106`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L106)
  - `title` — [`L99`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L99)
  - `updated_at` — [`L108`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L108)
  - `version` — [`L109`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L109)
- uses (calls/refs, reference-scoped): [`HarnessKind`](harness.md#HarnessKind), [`HarnessScope`](harness.md#HarnessScope), [`_now`](harness.md#_now)
- used by: [`overview`](harness.md#HarnessState.overview), [`_upsert`](harness.md#HarnessState._upsert), [`load`](harness.md#HarnessState.load), [`create`](harness.md#HarnessState.create), [`update`](harness.md#HarnessState.update), [`list`](harness.md#HarnessState.list), [`entries`](harness.md#HarnessState.entries), [`get`](harness.md#HarnessState.get), [`upsert`](harness.md#HarnessState.upsert), [`create_skill`](harness.md#HarnessState.create_skill), [`update_skill`](harness.md#HarnessState.update_skill), [`create_memory`](harness.md#HarnessState.create_memory), [`create_prompt_note`](harness.md#HarnessState.create_prompt_note), [`create_subagent`](harness.md#HarnessState.create_subagent), [`update_memory`](harness.md#HarnessState.update_memory), [`update_prompt_note`](harness.md#HarnessState.update_prompt_note), [`update_subagent`](harness.md#HarnessState.update_subagent), [`_ENTRY_FIELDS`](harness.md#_ENTRY_FIELDS)

### `HarnessState`
- def: [`prime-agent-runtime/src/rlm/harness.py:141`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L141)
- members:
  - `_sync_from_disk(self)` — [`L186`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L186) — Reload if another process rewrote the state file since we last touched it.
  - `create(self, kind: HarnessKind, title: str, content: str, *, id: str | None = None, path: str = "general", reference: dict[str, Any] | None = None, arguments: dict[str, Any] | None = None, metadata: dict[str, Any] | None = None, source: str = "agent", global_: bool = False, **kwargs: Any)` — [`L437`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L437)
  - `create_memory(self, title: str, content: str, *, id: str | None = None, path: str = "general", metadata: dict[str, Any] | None = None, global_: bool = False, **kwargs: Any)` — [`L530`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L530)
  - `create_prompt_note(self, title: str, content: str, *, id: str | None = None, path: str = "policy", metadata: dict[str, Any] | None = None, global_: bool = False, **kwargs: Any)` — [`L559`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L559)
  - `create_skill(self, title: str, content: str, *, id: str | None = None, path: str = "general", reference: dict[str, Any] | None = None, arguments: dict[str, Any] | None = None, metadata: dict[str, Any] | None = None, global_: bool = False, **kwargs: Any)` — [`L588`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L588)
  - `create_subagent(self, title: str, content: str, *, id: str | None = None, path: str = "general", metadata: dict[str, Any] | None = None, global_: bool = False, **kwargs: Any)` — [`L647`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L647)
  - `delete(self, kind: HarnessKind, id: str, *, global_: bool = False, **kwargs: Any)` — [`L411`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L411)
  - `delete_memory(self, id: str, *, global_: bool = False, **kwargs: Any)` — [`L556`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L556)
  - `delete_prompt_note(self, id: str, *, global_: bool = False, **kwargs: Any)` — [`L585`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L585)
  - `delete_skill(self, id: str, *, global_: bool = False, **kwargs: Any)` — [`L644`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L644)
  - `delete_subagent(self, id: str, *, global_: bool = False, **kwargs: Any)` — [`L673`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L673)
  - `get(self, kind: HarnessKind, id: str, *, global_: bool = False, **kwargs: Any)` — [`L402`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L402)
  - `list(self, kind: HarnessKind | None = None, *, global_: bool = False, **kwargs: Any)` — [`L425`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L425)
  - `load(self)` — [`L198`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L198)
  - `overview(self, *, max_entries_per_kind: int = 20, global_: bool = False, **kwargs: Any)` — [`L721`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L721)
  - `plan_refinement(self, observation: str, *, failing_component: str = "", next_step: str = "")` — [`L704`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L704)
  - `record_refinement(self, trigger: str, changes: list[str] | str, *, evidence: str = "", outcome: str = "", id: str | None = None, global_: bool = False, **kwargs: Any)` — [`L676`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L676)
  - `save(self)` — [`L284`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L284)
  - `snapshot(self, *, global_: bool = False, **kwargs: Any)` — [`L770`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L770)
  - `update(self, kind: HarnessKind, id: str, title: str, content: str, *, path: str | None = None, reference: dict[str, Any] | None = None, arguments: dict[str, Any] | None = None, metadata: dict[str, Any] | None = None, source: str = "agent", global_: bool = False, **kwargs: Any)` — [`L484`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L484)
  - `update_memory(self, id: str, title: str, content: str, *, path: str | None = None, metadata: dict[str, Any] | None = None, global_: bool = False, **kwargs: Any)` — [`L543`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L543)
  - `update_prompt_note(self, id: str, title: str, content: str, *, path: str | None = None, metadata: dict[str, Any] | None = None, global_: bool = False, **kwargs: Any)` — [`L572`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L572)
  - `update_skill(self, id: str, title: str, content: str, *, path: str | None = None, reference: dict[str, Any] | None = None, arguments: dict[str, Any] | None = None, metadata: dict[str, Any] | None = None, global_: bool = False, **kwargs: Any)` — [`L614`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L614)
  - `update_subagent(self, id: str, title: str, content: str, *, path: str | None = None, metadata: dict[str, Any] | None = None, global_: bool = False, **kwargs: Any)` — [`L660`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L660)
  - `upsert(self, kind: HarnessKind, title: str, content: str, *, id: str | None = None, path: str = "general", reference: dict[str, Any] | None = None, arguments: dict[str, Any] | None = None, metadata: dict[str, Any] | None = None, source: str = "agent", global_: bool = False, **kwargs: Any)` — [`L302`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L302)
  - `entries` — [`L166`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L166)
  - `file_path` — [`L155`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L155)
  - `refinements` — [`L167`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L167)
  - `scope` — [`L162`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L162)
- protocol/private: `__init__`[`L144`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L144), `_disk_mtime`[`L178`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L178), `_ensure_local_writable`[`L174`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L174), `_global_target`[`L276`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L276), `_global_target_state_dir`[`L168`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L168), `_loaded_mtime`[`L171`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L171), `_local_write_error`[`L165`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L165), `_upsert`[`L344`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L344)
- uses (calls/refs, reference-scoped): [`HarnessEntry`](harness.md#HarnessEntry), [`get_harness_state`](harness.md#get_harness_state), [`_KINDS`](harness.md#_KINDS._KINDS), [`_state_file`](harness.md#_state_file), [`HarnessKind`](harness.md#HarnessKind), [`kind`](harness.md#HarnessEntry.kind), [`RefinementEvent`](harness.md#RefinementEvent), [`HarnessScope`](harness.md#HarnessScope), [`_strip_scope_prefix`](harness.md#_strip_scope_prefix), [`scope`](harness.md#HarnessEntry.scope), [`_now`](harness.md#_now), [`arguments`](harness.md#HarnessEntry.arguments), [`path`](harness.md#HarnessEntry.path), [`reference`](harness.md#HarnessEntry.reference), [`title`](harness.md#HarnessEntry.title), [`_ENTRY_FIELDS`](harness.md#_ENTRY_FIELDS), [`_REFINEMENT_FIELDS`](harness.md#_REFINEMENT_FIELDS), [`updated_at`](harness.md#HarnessEntry.updated_at), [`content`](harness.md#HarnessEntry.content), [`id`](harness.md#HarnessEntry.id), [`_resolve_global_flag`](harness.md#_resolve_global_flag), [`_slug`](harness.md#_slug), [`_validate_python_skill_reference`](harness.md#_validate_python_skill_reference), [`changes`](harness.md#RefinementEvent.changes), [`id`](harness.md#RefinementEvent.id), [`metadata`](harness.md#HarnessEntry.metadata), [`source`](harness.md#HarnessEntry.source), [`trigger`](harness.md#RefinementEvent.trigger), [`version`](harness.md#HarnessEntry.version), [`evidence`](harness.md#RefinementEvent.evidence), [`outcome`](harness.md#RefinementEvent.outcome)
- used by: [`get_harness_state`](harness.md#get_harness_state), [`_resolve`](__init__.md#_HarnessProxy._resolve), [`_degraded`](__init__.md#_HarnessProxy._degraded), [`_state_cache`](harness.md#_state_cache._state_cache), [`_fallback`](__init__.md#_HarnessProxy._fallback), [`_unpersisted`](__init__.md#_HarnessProxy._unpersisted)

### `RefinementEvent`
- def: [`prime-agent-runtime/src/rlm/harness.py:113`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L113)
- doc: A recorded online harness-refinement pass.
- signature: `class RefinementEvent:`
- members:
  - `changes` — [`L118`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L118)
  - `created_at` — [`L121`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L121)
  - `evidence` — [`L119`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L119)
  - `id` — [`L116`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L116)
  - `outcome` — [`L120`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L120)
  - `trigger` — [`L117`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L117)
- uses (calls/refs, reference-scoped): [`_now`](harness.md#_now)
- used by: [`overview`](harness.md#HarnessState.overview), [`load`](harness.md#HarnessState.load), [`record_refinement`](harness.md#HarnessState.record_refinement), [`refinements`](harness.md#HarnessState.refinements), [`_REFINEMENT_FIELDS`](harness.md#_REFINEMENT_FIELDS)

## Functions
- `_agent_dir()` — [`L37`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L37)
- `_env_dir(name: str)` — [`L70`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L70)
- `_now()` — [`L27`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L27)
- `_resolve_global_flag(global_: bool = False, extra: dict[str, Any] | None = None)` — [`L46`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L46)
- `_slug(raw: str, fallback: str)` — [`L31`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L31)
- `_state_file(state_dir: str | Path | None = None, *, global_: bool = False)` — [`L77`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L77)
- `_strip_scope_prefix(id: str | None, global_: bool)` — [`L59`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L59)
- `_validate_python_skill_reference(reference: dict[str, Any] | None)` — [`L128`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L128)
- `get_harness_state(state_dir: str | Path | None = None, *, global_: bool = False, **kwargs: Any)` — [`L785`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L785) — Return the cached local harness state, or global when requested.

## Module values
- `HarnessKind` — [`L18`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L18)
- `HarnessScope` — [`L19`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L19)
- `_DEFAULT_FILE_NAME` — [`L21`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L21)
- `_DEFAULT_HARNESS_DIR_NAME` — [`L22`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L22)
- `_ENTRY_FIELDS` — [`L124`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L124)
- `_KINDS` — [`L23`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L23)
- `_REFINEMENT_FIELDS` — [`L125`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L125)
- `__all__` — [`L812`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L812)
- `_state_cache` — [`L24`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/harness.py#L24)


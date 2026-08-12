---
title: 'Module: tests/test_process_store_endpoints.py'
type: catalog
provenance: extracted
module: tests/test_process_store_endpoints.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_process_store_endpoints`/
symbols:
  _PROC_REASON: _PROC_REASON.
  sys_path: sys_path.
  memory_store: memory_store().
  skill_store: skill_store().
  subagent_store: subagent_store().
  TestProcessMemoryRead.test_read_single: TestProcessMemoryRead#test_read_single().
  TestProcessMemoryRead.test_read_missing_id: TestProcessMemoryRead#test_read_missing_id().
  TestProcessMemoryRead.test_read_no_id_field: TestProcessMemoryRead#test_read_no_id_field().
  TestProcessMemoryAdd.test_entries_empty_rejected: TestProcessMemoryAdd#test_entries_empty_rejected().
  TestProcessMemoryAdd.test_add_rejects_empty_title_and_content: TestProcessMemoryAdd#test_add_rejects_empty_title_and_content().
  TestProcessMemoryAdd.test_add_single: TestProcessMemoryAdd#test_add_single().
  TestProcessMemoryAdd.test_add_batch: TestProcessMemoryAdd#test_add_batch().
  TestProcessMemoryAdd.test_add_with_coordinates_string: TestProcessMemoryAdd#test_add_with_coordinates_string().
  TestProcessMemoryUpdate.test_update_single: TestProcessMemoryUpdate#test_update_single().
  TestProcessMemoryUpdate.test_update_missing: TestProcessMemoryUpdate#test_update_missing().
  TestProcessMemoryUpdate.test_update_no_id: TestProcessMemoryUpdate#test_update_no_id().
  TestProcessMemoryDelete.test_delete_single: TestProcessMemoryDelete#test_delete_single().
  TestProcessMemoryDelete.test_delete_missing: TestProcessMemoryDelete#test_delete_missing().
  TestProcessMemoryUnknownAction.test_unknown_action: TestProcessMemoryUnknownAction#test_unknown_action().
  TestProcessSkillRead.test_read_single: TestProcessSkillRead#test_read_single().
  TestProcessSkillRead.test_read_missing: TestProcessSkillRead#test_read_missing().
  TestProcessSkillAdd.test_add: TestProcessSkillAdd#test_add().
  TestProcessSkillAdd.test_add_rejects_empty_name_or_description: TestProcessSkillAdd#test_add_rejects_empty_name_or_description().
  TestProcessSkillUpdate.test_update: TestProcessSkillUpdate#test_update().
  TestProcessSkillDelete.test_delete: TestProcessSkillDelete#test_delete().
  TestProcessSubagentRead.test_read_custom: TestProcessSubagentRead#test_read_custom().
  TestProcessSubagentRead.test_read_missing: TestProcessSubagentRead#test_read_missing().
  TestProcessSubagentRead.test_read_no_id: TestProcessSubagentRead#test_read_no_id().
  TestProcessSubagentAdd.test_add: TestProcessSubagentAdd#test_add().
  TestProcessSubagentAdd.test_add_rejects_empty_name_or_description: TestProcessSubagentAdd#test_add_rejects_empty_name_or_description().
  TestProcessSubagentAdd.test_add_rejects_oversized_instructions: TestProcessSubagentAdd#test_add_rejects_oversized_instructions().
  TestProcessSubagentUpdate.test_update: TestProcessSubagentUpdate#test_update().
  TestProcessSubagentUpdate.test_update_missing: TestProcessSubagentUpdate#test_update_missing().
  TestProcessSubagentDelete.test_delete_custom: TestProcessSubagentDelete#test_delete_custom().
  TestProcessSubagentDelete.test_delete_builtin_rejected: TestProcessSubagentDelete#test_delete_builtin_rejected().
  TestProcessSubagentUnknownAction.test_unknown_action: TestProcessSubagentUnknownAction#test_unknown_action().
  game_tools_memory: game_tools_memory().
  game_tools_skill: game_tools_skill().
  TestProcessMemoryRequiresReasoning: TestProcessMemoryRequiresReasoning#
  TestProcessMemoryRequiresReasoning.test_missing_reasoning_fails: TestProcessMemoryRequiresReasoning#test_missing_reasoning_fails().
  TestProcessMemoryRequiresReasoning.test_none_reasoning_fails: TestProcessMemoryRequiresReasoning#test_none_reasoning_fails().
  TestProcessMemoryRequiresReasoning.test_whitespace_only_reasoning_fails: TestProcessMemoryRequiresReasoning#test_whitespace_only_reasoning_fails().
  TestProcessSkillRequiresReasoning: TestProcessSkillRequiresReasoning#
  TestProcessSkillRequiresReasoning.test_missing_reasoning_fails: TestProcessSkillRequiresReasoning#test_missing_reasoning_fails().
  TestProcessMemoryRead: TestProcessMemoryRead#
  TestProcessMemoryAdd: TestProcessMemoryAdd#
  TestProcessMemoryUpdate: TestProcessMemoryUpdate#
  TestProcessMemoryDelete: TestProcessMemoryDelete#
  TestProcessMemoryUnknownAction: TestProcessMemoryUnknownAction#
  TestProcessSkillRead: TestProcessSkillRead#
  TestProcessSkillAdd: TestProcessSkillAdd#
  TestProcessSkillUpdate: TestProcessSkillUpdate#
  TestProcessSkillDelete: TestProcessSkillDelete#
  TestOverviewEndpoints: TestOverviewEndpoints#
  TestOverviewEndpoints.test_memory_overview: TestOverviewEndpoints#test_memory_overview().
  TestOverviewEndpoints.test_skill_overview: TestOverviewEndpoints#test_skill_overview().
  TestBackwardCompat: TestBackwardCompat#
  TestBackwardCompat.test_add_memory_direct_rejects_empty_title_and_content: TestBackwardCompat#test_add_memory_direct_rejects_empty_title_and_content().
  TestBackwardCompat.test_add_memory_direct_with_category: TestBackwardCompat#test_add_memory_direct_with_category().
  TestBackwardCompat.test_add_memory_direct_with_path: TestBackwardCompat#test_add_memory_direct_with_path().
  TestBackwardCompat.test_search_memory_direct: TestBackwardCompat#test_search_memory_direct().
  game_tools_subagent: game_tools_subagent().
  TestProcessSubagentRequiresReasoning: TestProcessSubagentRequiresReasoning#
  TestProcessSubagentRequiresReasoning.test_missing_reasoning_fails: TestProcessSubagentRequiresReasoning#test_missing_reasoning_fails().
  TestProcessSubagentRequiresReasoning.test_none_reasoning_fails: TestProcessSubagentRequiresReasoning#test_none_reasoning_fails().
  TestProcessSubagentRead: TestProcessSubagentRead#
  TestProcessSubagentAdd: TestProcessSubagentAdd#
  TestProcessSubagentUpdate: TestProcessSubagentUpdate#
  TestProcessSubagentDelete: TestProcessSubagentDelete#
  TestProcessSubagentUnknownAction: TestProcessSubagentUnknownAction#
  TestSubagentOverview: TestSubagentOverview#
  TestSubagentOverview.test_overview: TestSubagentOverview#test_overview().
---
# Module: [`tests/test_process_store_endpoints.py`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py)

## Classes
### `TestBackwardCompat`
- def: [`tests/test_process_store_endpoints.py:268`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L268)
- signature: `class TestBackwardCompat:`
- members:
  - `test_add_memory_direct_rejects_empty_title_and_content(self, game_tools_memory, memory_store)` — [`L269`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L269)
  - `test_add_memory_direct_with_category(self, game_tools_memory, memory_store)` — [`L276`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L276)
  - `test_add_memory_direct_with_path(self, game_tools_memory, memory_store)` — [`L282`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L282)
  - `test_search_memory_direct(self, game_tools_memory)` — [`L288`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L288)

### `TestOverviewEndpoints`
- def: [`tests/test_process_store_endpoints.py:249`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L249)
- signature: `class TestOverviewEndpoints:`
- members:
  - `test_memory_overview(self, game_tools_memory)` — [`L250`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L250)
  - `test_skill_overview(self, game_tools_skill)` — [`L256`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L256)

### `TestProcessMemoryAdd`
- def: [`tests/test_process_store_endpoints.py:107`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L107)
- signature: `class TestProcessMemoryAdd:`
- members:
  - `test_add_batch(self, game_tools_memory, memory_store)` — [`L131`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L131)
  - `test_add_rejects_empty_title_and_content(self, game_tools_memory, memory_store)` — [`L114`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L114)
  - `test_add_single(self, game_tools_memory, memory_store)` — [`L122`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L122)
  - `test_add_with_coordinates_string(self, game_tools_memory, memory_store)` — [`L140`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L140)
  - `test_entries_empty_rejected(self, game_tools_memory)` — [`L108`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L108)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestProcessMemoryDelete`
- def: [`tests/test_process_store_endpoints.py:169`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L169)
- signature: `class TestProcessMemoryDelete:`
- members:
  - `test_delete_missing(self, game_tools_memory)` — [`L176`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L176)
  - `test_delete_single(self, game_tools_memory, memory_store)` — [`L170`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L170)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestProcessMemoryRead`
- def: [`tests/test_process_store_endpoints.py:85`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L85)
- signature: `class TestProcessMemoryRead:`
- members:
  - `test_read_missing_id(self, game_tools_memory)` — [`L95`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L95)
  - `test_read_no_id_field(self, game_tools_memory)` — [`L100`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L100)
  - `test_read_single(self, game_tools_memory)` — [`L86`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L86)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestProcessMemoryRequiresReasoning`
- def: [`tests/test_process_store_endpoints.py:63`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L63)
- signature: `class TestProcessMemoryRequiresReasoning:`
- members:
  - `test_missing_reasoning_fails(self, game_tools_memory)` — [`L64`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L64)
  - `test_none_reasoning_fails(self, game_tools_memory)` — [`L69`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L69)
  - `test_whitespace_only_reasoning_fails(self, game_tools_memory)` — [`L73`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L73)

### `TestProcessMemoryUnknownAction`
- def: [`tests/test_process_store_endpoints.py:182`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L182)
- signature: `class TestProcessMemoryUnknownAction:`
- members:
  - `test_unknown_action(self, game_tools_memory)` — [`L183`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L183)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestProcessMemoryUpdate`
- def: [`tests/test_process_store_endpoints.py:149`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L149)
- signature: `class TestProcessMemoryUpdate:`
- members:
  - `test_update_missing(self, game_tools_memory)` — [`L158`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L158)
  - `test_update_no_id(self, game_tools_memory)` — [`L163`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L163)
  - `test_update_single(self, game_tools_memory, memory_store)` — [`L150`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L150)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestProcessSkillAdd`
- def: [`tests/test_process_store_endpoints.py:207`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L207)
- signature: `class TestProcessSkillAdd:`
- members:
  - `test_add(self, game_tools_skill, skill_store)` — [`L208`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L208)
  - `test_add_rejects_empty_name_or_description(self, game_tools_skill, skill_store)` — [`L217`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L217)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestProcessSkillDelete`
- def: [`tests/test_process_store_endpoints.py:236`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L236)
- signature: `class TestProcessSkillDelete:`
- members:
  - `test_delete(self, game_tools_skill, skill_store)` — [`L237`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L237)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestProcessSkillRead`
- def: [`tests/test_process_store_endpoints.py:195`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L195)
- signature: `class TestProcessSkillRead:`
- members:
  - `test_read_missing(self, game_tools_skill)` — [`L201`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L201)
  - `test_read_single(self, game_tools_skill)` — [`L196`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L196)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestProcessSkillRequiresReasoning`
- def: [`tests/test_process_store_endpoints.py:78`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L78)
- signature: `class TestProcessSkillRequiresReasoning:`
- members:
  - `test_missing_reasoning_fails(self, game_tools_skill)` — [`L79`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L79)

### `TestProcessSkillUpdate`
- def: [`tests/test_process_store_endpoints.py:226`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L226)
- signature: `class TestProcessSkillUpdate:`
- members:
  - `test_update(self, game_tools_skill, skill_store)` — [`L227`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L227)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestProcessSubagentAdd`
- def: [`tests/test_process_store_endpoints.py:368`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L368)
- signature: `class TestProcessSubagentAdd:`
- members:
  - `test_add(self, game_tools_subagent, subagent_store)` — [`L369`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L369)
  - `test_add_rejects_empty_name_or_description(self, game_tools_subagent, subagent_store)` — [`L378`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L378)
  - `test_add_rejects_oversized_instructions(self, game_tools_subagent, subagent_store)` — [`L386`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L386)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestProcessSubagentDelete`
- def: [`tests/test_process_store_endpoints.py:422`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L422)
- signature: `class TestProcessSubagentDelete:`
- members:
  - `test_delete_builtin_rejected(self, game_tools_subagent, subagent_store)` — [`L436`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L436)
  - `test_delete_custom(self, game_tools_subagent, subagent_store)` — [`L423`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L423)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestProcessSubagentRead`
- def: [`tests/test_process_store_endpoints.py:338`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L338)
- signature: `class TestProcessSubagentRead:`
- members:
  - `test_read_custom(self, game_tools_subagent, subagent_store)` — [`L339`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L339)
  - `test_read_missing(self, game_tools_subagent)` — [`L353`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L353)
  - `test_read_no_id(self, game_tools_subagent)` — [`L360`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L360)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestProcessSubagentRequiresReasoning`
- def: [`tests/test_process_store_endpoints.py:322`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L322)
- signature: `class TestProcessSubagentRequiresReasoning:`
- members:
  - `test_missing_reasoning_fails(self, game_tools_subagent)` — [`L323`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L323)
  - `test_none_reasoning_fails(self, game_tools_subagent)` — [`L328`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L328)

### `TestProcessSubagentUnknownAction`
- def: [`tests/test_process_store_endpoints.py:448`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L448)
- signature: `class TestProcessSubagentUnknownAction:`
- members:
  - `test_unknown_action(self, game_tools_subagent)` — [`L449`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L449)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestProcessSubagentUpdate`
- def: [`tests/test_process_store_endpoints.py:400`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L400)
- signature: `class TestProcessSubagentUpdate:`
- members:
  - `test_update(self, game_tools_subagent, subagent_store)` — [`L401`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L401)
  - `test_update_missing(self, game_tools_subagent)` — [`L414`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L414)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestSubagentOverview`
- def: [`tests/test_process_store_endpoints.py:460`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L460)
- signature: `class TestSubagentOverview:`
- members:
  - `test_overview(self, game_tools_subagent)` — [`L461`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L461)

## Functions
- `game_tools_memory(memory_store, monkeypatch)` — [`L43`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L43) — Import game_tools with patched memory_store singleton.
- `game_tools_skill(skill_store, monkeypatch)` — [`L51`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L51) — Import game_tools with patched skill_store singleton.
- `game_tools_subagent(subagent_store, monkeypatch)` — [`L311`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L311)
- `memory_store(tmp_path)` — [`L28`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L28)
- `skill_store(tmp_path)` — [`L36`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L36)
- `subagent_store(tmp_path)` — [`L300`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L300)

## Module values
- `_PROC_REASON` — [`L20`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L20)
- `sys_path` — [`L11`](../../../../../raw/code/continual-harness/tests/test_process_store_endpoints.py#L11)


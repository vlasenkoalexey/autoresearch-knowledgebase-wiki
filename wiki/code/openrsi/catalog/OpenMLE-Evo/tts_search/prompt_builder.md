---
title: 'Module: OpenMLE-Evo/tts_search/prompt_builder.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/tts_search/prompt_builder.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.tts_search.prompt_builder`/
symbols:
  build_prompt: build_prompt().
  _safe_text: _safe_text().
  build_improve_prompt: build_improve_prompt().
  build_debug_prompt: build_debug_prompt().
  build_crossover_prompt: build_crossover_prompt().
  build_draft_system_prompt: build_draft_system_prompt().
  build_draft_prompt: build_draft_prompt().
  build_improve_system_prompt: build_improve_system_prompt().
  build_debug_system_prompt: build_debug_system_prompt().
  build_crossover_system_prompt: build_crossover_system_prompt().
  split_legacy_public_prompts: split_legacy_public_prompts().
---
# Module: [`OpenMLE-Evo/tts_search/prompt_builder.py`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/prompt_builder.py)

## Functions
- `_safe_text(text: str | None)` — [`L14`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/prompt_builder.py#L14)
- `build_crossover_prompt(task_description: str, data_description: str, parent_program: Program, secondary_parent_program: Program, public_user_prompt: str)` — [`L163`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/prompt_builder.py#L163) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
- `build_crossover_system_prompt(public_system_prompt: str)` — [`L153`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/prompt_builder.py#L153)
- `build_debug_prompt(task_description: str, data_description: str, parent_program: Program, public_user_prompt: str)` — [`L127`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/prompt_builder.py#L127) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
- `build_debug_system_prompt(public_system_prompt: str)` — [`L92`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/prompt_builder.py#L92)
- `build_draft_prompt(task_description: str, data_description: str, public_user_prompt: str)` — [`L70`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/prompt_builder.py#L70)
- `build_draft_system_prompt(public_system_prompt: str)` — [`L61`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/prompt_builder.py#L61)
- `build_improve_prompt(task_description: str, data_description: str, parent_program: Program, public_user_prompt: str)` — [`L102`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/prompt_builder.py#L102) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
- `build_improve_system_prompt(public_system_prompt: str)` — [`L83`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/prompt_builder.py#L83)
- `build_prompt(mode: str, task_description: str, data_description: str, public_system_prompt: str, public_user_prompt: str, virtual_data_dir: str, parent_program: Optional[Program] = None, secondary_parent_program: Optional[Program] = None, max_steps: int = 1)` — [`L196`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/prompt_builder.py#L196) — Build (system_prompt, user_prompt) based on mode. — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
- `split_legacy_public_prompts(public_system_prompt: str, public_user_prompt: str)` — [`L18`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/prompt_builder.py#L18) — Split legacy fully-assembled prompts into the 4 fragments expected by the aligned templates:


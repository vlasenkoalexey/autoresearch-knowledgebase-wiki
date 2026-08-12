---
title: 'Module: OpenMLE-ERL/SFT/tts_search/prompt_builder.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/prompt_builder.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.prompt_builder`/
symbols:
  build_pass_k_draft_messages: build_pass_k_draft_messages().
  build_prompt: build_prompt().
  _safe_text: _safe_text().
  build_improve_prompt: build_improve_prompt().
  build_pass_k_draft_user_prompt: build_pass_k_draft_user_prompt().
  build_pass_k_draft_system_prompt: build_pass_k_draft_system_prompt().
  split_legacy_public_prompts: split_legacy_public_prompts().
  _format_time_limit: _format_time_limit().
  _extract_public_prompt_components: _extract_public_prompt_components().
  build_draft_prompt: build_draft_prompt().
---
# Module: [`OpenMLE-ERL/SFT/tts_search/prompt_builder.py`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/prompt_builder.py)

## Functions
- `_extract_public_prompt_components(messages: Sequence[dict[str, Any]] | None)` — [`L127`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/prompt_builder.py#L127) — Extract the first public system/user prompts from stored task messages.
- `_format_time_limit(time_limit_value: Any)` — [`L73`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/prompt_builder.py#L73) — Format a configured runtime limit for prompt text.
- `_safe_text(text: str | None)` — [`L36`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/prompt_builder.py#L36)
- `build_draft_prompt(description: str, virtual_data_dir: str, max_steps: int = 1)` — [`L180`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/prompt_builder.py#L180) — Build prompt for draft mode (generating code from scratch).
- `build_improve_prompt(description: str, virtual_data_dir: str, parent_program: Program, max_steps: int = 1)` — [`L221`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/prompt_builder.py#L221) — Build prompt for improve mode (improving existing code). — documented in [OpenMLE-ERL-SFT-tts_search-program_database](../../../../concepts/OpenMLE-ERL-SFT-tts_search-program_database.md)
- `build_pass_k_draft_messages(metadata: dict[str, Any], messages: Sequence[dict[str, Any]] | None, time_limit: bool = True, time_limit_value: Any = None)` — [`L145`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/prompt_builder.py#L145) — Rebuild pass@k draft messages from task metadata plus public prompts.
- `build_pass_k_draft_system_prompt(public_system_prompt: str)` — [`L85`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/prompt_builder.py#L85) — Build the system prompt used by the pass@k draft pipeline.
- `build_pass_k_draft_user_prompt(task_description: str, data_description: str, public_user_prompt: str, time_limit: bool = True, time_limit_value: Any = None)` — [`L95`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/prompt_builder.py#L95) — Build the user prompt used by the pass@k draft pipeline.
- `build_prompt(mode: str, description: str, virtual_data_dir: str, parent_program: Optional[Program] = None, max_steps: int = 1)` — [`L266`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/prompt_builder.py#L266) — Build prompt based on mode. — documented in [OpenMLE-ERL-SFT-tts_search-program_database](../../../../concepts/OpenMLE-ERL-SFT-tts_search-program_database.md)
- `split_legacy_public_prompts(public_system_prompt: str, public_user_prompt: str)` — [`L40`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/prompt_builder.py#L40) — Split old fully assembled public prompts into task/data/template parts.


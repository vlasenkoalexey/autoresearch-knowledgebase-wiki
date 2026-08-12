---
title: 'Module: OpenMLE-ERL/RL/prompt_builder.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/RL/prompt_builder.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.RL.prompt_builder`/
symbols:
  _safe_text: _safe_text().
  build_airaevo_rich_memory_summary_prompt: build_airaevo_rich_memory_summary_prompt().
  build_prompt: build_prompt().
  build_airaevo_prompt: build_airaevo_prompt().
  build_improve_prompt: build_improve_prompt().
  build_crossover_prompt: build_crossover_prompt().
  _airaevo_feedback: _airaevo_feedback().
  format_sandbox_feedback: format_sandbox_feedback().
  _airaevo_memory_block: _airaevo_memory_block().
  build_draft_system_prompt: build_draft_system_prompt().
  build_draft_prompt: build_draft_prompt().
  build_improve_system_prompt: build_improve_system_prompt().
  build_crossover_system_prompt: build_crossover_system_prompt().
  _airaevo_data_overview_block: _airaevo_data_overview_block().
  _airaevo_execution_block: _airaevo_execution_block().
  _airaevo_memory_text: _airaevo_memory_text().
  _airaevo_submission_check: _airaevo_submission_check().
---
# Module: [`OpenMLE-ERL/RL/prompt_builder.py`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py)

## Functions
- `_airaevo_data_overview_block(data_overview: Optional[str])` — [`L184`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L184)
- `_airaevo_execution_block(execution_timeout: str | int | float | None)` — [`L194`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L194)
- `_airaevo_feedback(program: Program)` — [`L215`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L215)
- `_airaevo_memory_block(memory: Optional[str], label: str, empty_suffix: str, post_instructions: tuple[str, ...] = ())` — [`L169`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L169)
- `_airaevo_memory_text(memory: Optional[str], empty_text: str)` — [`L162`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L162)
- `_airaevo_submission_check()` — [`L207`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L207)
- `_safe_text(text: Optional[str])` — [`L8`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L8) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `build_airaevo_prompt(mode: str, task_description: str, data_description: str, public_system_prompt: str, public_user_prompt: str, virtual_data_dir: str, parent_program: Optional[Program] = None, secondary_parent_program: Optional[Program] = None, max_steps: int = 1, memory: Optional[str] = None, data_overview: Optional[str] = None, execution_timeout: str | int | float | None = None)` — [`L219`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L219) — Build prompts aligned with the latest inference AIRA-Evo operator templates. — documented in [OpenMLE-ERL-RL-program_database](../../../concepts/OpenMLE-ERL-RL-program_database.md)
- `build_airaevo_rich_memory_summary_prompt(task_description: str, current_program: Program, parent_program: Optional[Program], current_card: dict)` — [`L394`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L394) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `build_crossover_prompt(task_description: str, data_description: str, parent_program: Program, secondary_parent_program: Program, public_user_prompt: str)` — [`L126`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L126)
- `build_crossover_system_prompt(public_system_prompt: str)` — [`L116`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L116)
- `build_draft_prompt(task_description: str, data_description: str, public_user_prompt: str)` — [`L65`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L65)
- `build_draft_system_prompt(public_system_prompt: str)` — [`L56`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L56)
- `build_improve_prompt(task_description: str, data_description: str, parent_program: Program, public_user_prompt: str)` — [`L88`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L88)
- `build_improve_system_prompt(public_system_prompt: str)` — [`L78`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L78)
- `build_prompt(mode: str, task_description: str, data_description: str, public_system_prompt: str, public_user_prompt: str, virtual_data_dir: str, parent_program: Optional[Program] = None, secondary_parent_program: Optional[Program] = None, max_steps: int = 1)` — [`L440`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L440) — Build prompt based on mode. — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `format_sandbox_feedback(status_code: int, payload: dict)` — [`L12`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/prompt_builder.py#L12) — Format sandbox execution results into feedback message


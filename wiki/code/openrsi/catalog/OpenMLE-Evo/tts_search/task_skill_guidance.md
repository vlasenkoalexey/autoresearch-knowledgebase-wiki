---
title: 'Module: OpenMLE-Evo/tts_search/task_skill_guidance.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/tts_search/task_skill_guidance.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.tts_search.task_skill_guidance`/
symbols:
  TaskSkillGuidanceInjector.inject: TaskSkillGuidanceInjector#inject().
  TaskSkillGuidanceInjector: TaskSkillGuidanceInjector#
  TaskSkillGuidanceResult.changed: TaskSkillGuidanceResult#changed.
  TaskSkillGuidanceResult.missing: TaskSkillGuidanceResult#missing.
  TaskSkillGuidanceInjector.__init__: TaskSkillGuidanceInjector#__init__().
  TaskSkillGuidanceInjector.heading: TaskSkillGuidanceInjector#heading.
  TaskSkillGuidanceResult: TaskSkillGuidanceResult#
  TaskSkillGuidanceResult.skipped_existing: TaskSkillGuidanceResult#skipped_existing.
  load_task_skill_map: load_task_skill_map().
  TaskSkillGuidanceResult.task_name: TaskSkillGuidanceResult#task_name.
  TaskSkillGuidanceInjector.strict: TaskSkillGuidanceInjector#strict.
  DEFAULT_TASK_SKILL_HEADING: DEFAULT_TASK_SKILL_HEADING.
  TaskSkillGuidanceInjector.intro: TaskSkillGuidanceInjector#intro.
  DEFAULT_TASK_SKILL_INTRO: DEFAULT_TASK_SKILL_INTRO.
  TaskSkillGuidanceInjector.skill_map: TaskSkillGuidanceInjector#skill_map.
---
# Module: [`OpenMLE-Evo/tts_search/task_skill_guidance.py`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py)

## Classes
### `TaskSkillGuidanceInjector`
- def: [`OpenMLE-Evo/tts_search/task_skill_guidance.py:51`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py#L51)
- signature: `class TaskSkillGuidanceInjector:`
- members:
  - `inject(self, public_user_prompt: str, task_name: str)` — [`L65`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py#L65)
  - `heading` — [`L61`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py#L61)
  - `intro` — [`L62`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py#L62)
  - `skill_map` — [`L60`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py#L60)
  - `strict` — [`L63`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py#L63)
- protocol/private: `__init__`[`L52`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py#L52)
- uses (calls/refs, reference-scoped): [`changed`](task_skill_guidance.md#TaskSkillGuidanceResult.changed), [`missing`](task_skill_guidance.md#TaskSkillGuidanceResult.missing), [`TaskSkillGuidanceResult`](task_skill_guidance.md#TaskSkillGuidanceResult), [`skipped_existing`](task_skill_guidance.md#TaskSkillGuidanceResult.skipped_existing), [`task_name`](task_skill_guidance.md#TaskSkillGuidanceResult.task_name), [`DEFAULT_TASK_SKILL_HEADING`](task_skill_guidance.md#DEFAULT_TASK_SKILL_HEADING), [`DEFAULT_TASK_SKILL_INTRO`](task_skill_guidance.md#DEFAULT_TASK_SKILL_INTRO)
- used by: [`_maybe_patch_eval_data_with_task_skill_guidance`](../scripts/evaluate_airaevo.md#_maybe_patch_eval_data_with_task_skill_guidance), [`logger`](../scripts/evaluate_airaevo.md#logger), [`_inject_task_skill_into_prompt_value`](../scripts/evaluate_airaevo.md#_inject_task_skill_into_prompt_value)  (2 test-only)

### `TaskSkillGuidanceResult`
- def: [`OpenMLE-Evo/tts_search/task_skill_guidance.py:15`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py#L15)
- signature: `class TaskSkillGuidanceResult:`
- members:
  - `changed` — [`L17`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py#L17)
  - `missing` — [`L19`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py#L19)
  - `skipped_existing` — [`L18`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py#L18)
  - `task_name` — [`L16`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py#L16)
- used by: [`inject`](task_skill_guidance.md#TaskSkillGuidanceInjector.inject)  (2 test-only)

## Functions
- `load_task_skill_map(skills_dir: Path, *, recursive: bool = True)` — [`L22`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py#L22) — Load task-specific skill Markdown files keyed by task name.

## Module values
- `DEFAULT_TASK_SKILL_HEADING` — [`L6`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py#L6)
- `DEFAULT_TASK_SKILL_INTRO` — [`L7`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/task_skill_guidance.py#L7)


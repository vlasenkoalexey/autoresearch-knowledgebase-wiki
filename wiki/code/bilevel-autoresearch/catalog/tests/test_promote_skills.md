---
title: 'Module: tests/test_promote_skills.py'
type: catalog
provenance: extracted
module: tests/test_promote_skills.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `tests.test_promote_skills`/
symbols:
  _make_lesson: _make_lesson().
  _make_state: _make_state().
  TestAddLessonHighConfidence.test_add_high_confidence_lesson: TestAddLessonHighConfidence#test_add_high_confidence_lesson().
  TestAddLessonHighConfidence.test_multiple_lessons_appended_in_order: TestAddLessonHighConfidence#test_multiple_lessons_appended_in_order().
  TestAddLessonHighConfidence.test_reset_clears_lessons: TestAddLessonHighConfidence#test_reset_clears_lessons().
  TestUpdateSkill.test_reset_clears_skills: TestUpdateSkill#test_reset_clears_skills().
  TestAddLessonHighConfidence.test_add_low_confidence_lesson: TestAddLessonHighConfidence#test_add_low_confidence_lesson().
  TestLessonQualityStats.test_all_high_confidence: TestLessonQualityStats#test_all_high_confidence().
  TestLessonQualityStats.test_none_high_confidence: TestLessonQualityStats#test_none_high_confidence().
  TestLessonQualityStats.test_mixed_confidence: TestLessonQualityStats#test_mixed_confidence().
  TestLessonQualityStats.test_boundary_confidence_085_counts_as_high: TestLessonQualityStats#test_boundary_confidence_085_counts_as_high().
  TestLessonQualityStats.test_confidence_below_085_not_high: TestLessonQualityStats#test_confidence_below_085_not_high().
  TestUpdateSkill.test_update_skill_stores_text: TestUpdateSkill#test_update_skill_stores_text().
  TestUpdateSkill.test_update_skill_overwrites_existing: TestUpdateSkill#test_update_skill_overwrites_existing().
  TestUpdateSkill.test_update_multiple_stages: TestUpdateSkill#test_update_multiple_stages().
  TestUpdateSkill.test_skills_not_shared_across_instances: TestUpdateSkill#test_skills_not_shared_across_instances().
  TestUpdateSkill.test_inner_skills_empty_on_init: TestUpdateSkill#test_inner_skills_empty_on_init().
  TestLessonQualityStats.test_empty_returns_zeros: TestLessonQualityStats#test_empty_returns_zeros().
  TestUpdateSkill: TestUpdateSkill#
  TestAddLessonHighConfidence: TestAddLessonHighConfidence#
  TestLessonQualityStats: TestLessonQualityStats#
---
# Module: [`tests/test_promote_skills.py`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py)

## Classes
### `TestAddLessonHighConfidence`
- def: [`tests/test_promote_skills.py:70`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L70)
- signature: `class TestAddLessonHighConfidence:`
- members:
  - `test_add_high_confidence_lesson(self)` — [`L71`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L71)
  - `test_add_low_confidence_lesson(self)` — [`L78`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L78)
  - `test_multiple_lessons_appended_in_order(self)` — [`L84`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L84)
  - `test_reset_clears_lessons(self)` — [`L91`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L91)
- uses (calls/refs, reference-scoped): [`inner_lessons`](../core/state.md#InnerLoopState.inner_lessons), [`reset`](../core/state.md#InnerLoopState.reset), [`add_lesson`](../core/state.md#InnerLoopState.add_lesson), [`confidence`](../core/state.md#InnerLesson.confidence)  (2 test-only)

### `TestLessonQualityStats`
- def: [`tests/test_promote_skills.py:102`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L102)
- signature: `class TestLessonQualityStats:`
- members:
  - `test_all_high_confidence(self)` — [`L108`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L108)
  - `test_boundary_confidence_085_counts_as_high(self)` — [`L136`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L136)
  - `test_confidence_below_085_not_high(self)` — [`L142`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L142)
  - `test_empty_returns_zeros(self)` — [`L103`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L103)
  - `test_mixed_confidence(self)` — [`L126`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L126)
  - `test_none_high_confidence(self)` — [`L117`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L117)
- uses (calls/refs, reference-scoped): [`add_lesson`](../core/state.md#InnerLoopState.add_lesson), [`lesson_quality_stats`](../core/state.md#InnerLoopState.lesson_quality_stats)  (2 test-only)

### `TestUpdateSkill`
- def: [`tests/test_promote_skills.py:31`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L31)
- signature: `class TestUpdateSkill:`
- members:
  - `test_inner_skills_empty_on_init(self)` — [`L49`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L49)
  - `test_reset_clears_skills(self)` — [`L53`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L53)
  - `test_skills_not_shared_across_instances(self)` — [`L59`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L59)
  - `test_update_multiple_stages(self)` — [`L43`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L43)
  - `test_update_skill_overwrites_existing(self)` — [`L37`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L37)
  - `test_update_skill_stores_text(self)` — [`L32`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L32)
- uses (calls/refs, reference-scoped): [`reset`](../core/state.md#InnerLoopState.reset), [`update_skill`](../core/state.md#InnerLoopState.update_skill), [`inner_skills`](../core/state.md#InnerLoopState.inner_skills)  (1 test-only)

## Functions
- `_make_lesson(confidence=0.9, stage="A", lesson_type="success_pattern")` — [`L16`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L16)
- `_make_state(article="article text", article_id="art1")` — [`L12`](../../../../../raw/code/bilevel-autoresearch/tests/test_promote_skills.py#L12)


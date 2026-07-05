---
title: 'Module: tests/test_mechanism_research.py'
type: catalog
provenance: extracted
module: tests/test_mechanism_research.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `tests.test_mechanism_research`/
symbols:
  TestStripFences.researcher: TestStripFences#researcher.
  _ConcreteResearcher: _ConcreteResearcher#
  TestSyntaxCheck.researcher: TestSyntaxCheck#researcher.
  TestSyntaxCheck.test_valid_code_returns_none: TestSyntaxCheck#test_valid_code_returns_none().
  TestSyntaxCheck.test_valid_function_returns_none: TestSyntaxCheck#test_valid_function_returns_none().
  TestSyntaxCheck.test_invalid_syntax_returns_error_string: TestSyntaxCheck#test_invalid_syntax_returns_error_string().
  TestSyntaxCheck.test_invalid_expression_returns_error_string: TestSyntaxCheck#test_invalid_expression_returns_error_string().
  TestSyntaxCheck.test_empty_string_is_valid: TestSyntaxCheck#test_empty_string_is_valid().
  TestSyntaxCheck.test_multiline_valid_class: TestSyntaxCheck#test_multiline_valid_class().
  TestStripFences.test_removes_python_fence: TestStripFences#test_removes_python_fence().
  TestStripFences.test_removes_plain_fence: TestStripFences#test_removes_plain_fence().
  TestStripFences.test_no_fences_unchanged: TestStripFences#test_no_fences_unchanged().
  TestStripFences.test_only_opening_fence_removed: TestStripFences#test_only_opening_fence_removed().
  TestStripFences.test_multiline_body_preserved: TestStripFences#test_multiline_body_preserved().
  TestStripFences.test_empty_string_unchanged: TestStripFences#test_empty_string_unchanged().
  TestStripFences.test_fence_with_extra_tag_stripped: TestStripFences#test_fence_with_extra_tag_stripped().
  TestExtractSelected.researcher: TestExtractSelected#researcher.
  TestExtractSelected.test_extracts_selected_line_from_critique: TestExtractSelected#test_extracts_selected_line_from_critique().
  TestExtractSelected.test_case_insensitive_selected_keyword: TestExtractSelected#test_case_insensitive_selected_keyword().
  TestExtractSelected.test_falls_back_to_exploration_tail_when_no_selected: TestExtractSelected#test_falls_back_to_exploration_tail_when_no_selected().
  TestExtractSelected.test_falls_back_to_full_exploration_when_short: TestExtractSelected#test_falls_back_to_full_exploration_when_short().
  TestExtractSelected.test_selected_line_stripped_of_leading_whitespace: TestExtractSelected#test_selected_line_stripped_of_leading_whitespace().
  TestBaseMechanismResearcherAbstract.test_missing_abstract_method_raises._Incomplete: TestBaseMechanismResearcherAbstract#test_missing_abstract_method_raises()._Incomplete#
  TestBaseMechanismResearcherAbstract.test_cannot_instantiate_directly: TestBaseMechanismResearcherAbstract#test_cannot_instantiate_directly().
  TestBaseMechanismResearcherAbstract.test_concrete_subclass_can_be_instantiated: TestBaseMechanismResearcherAbstract#test_concrete_subclass_can_be_instantiated().
  TestBaseMechanismResearcherAbstract.test_missing_abstract_method_raises: TestBaseMechanismResearcherAbstract#test_missing_abstract_method_raises().
  TestSyntaxCheck.setup_method: TestSyntaxCheck#setup_method().
  TestStripFences.setup_method: TestStripFences#setup_method().
  TestExtractSelected.setup_method: TestExtractSelected#setup_method().
  _ConcreteResearcher._get_explore_prompt: _ConcreteResearcher#_get_explore_prompt().
  _ConcreteResearcher._get_specify_prompt: _ConcreteResearcher#_get_specify_prompt().
  _ConcreteResearcher._get_codegen_prompt: _ConcreteResearcher#_get_codegen_prompt().
  _ConcreteResearcher._get_reference_code: _ConcreteResearcher#_get_reference_code().
  _ConcreteResearcher._parse_spec_metadata: _ConcreteResearcher#_parse_spec_metadata().
  TestBaseMechanismResearcherAbstract: TestBaseMechanismResearcherAbstract#
  TestBaseMechanismResearcherAbstract.test_missing_abstract_method_raises._Incomplete._get_explore_prompt: TestBaseMechanismResearcherAbstract#test_missing_abstract_method_raises()._Incomplete#_get_explore_prompt().
  TestSyntaxCheck: TestSyntaxCheck#
  TestStripFences: TestStripFences#
  TestExtractSelected: TestExtractSelected#
---
# Module: [`tests/test_mechanism_research.py`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py)

## Classes
### `TestBaseMechanismResearcherAbstract`
- def: [`tests/test_mechanism_research.py:31`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L31)
- signature: `class TestBaseMechanismResearcherAbstract:`
- members:
  - `test_cannot_instantiate_directly(self)` — [`L32`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L32) — BaseMechanismResearcher is abstract and must not be instantiatable. — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
  - `test_concrete_subclass_can_be_instantiated(self)` — [`L37`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L37) — A fully-implemented subclass must instantiate without error.
  - `test_missing_abstract_method_raises(self)` — [`L42`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L42) — A subclass missing one abstract method must also fail to instantiate.
- uses (calls/refs, reference-scoped): [`BaseMechanismResearcher`](../core/base_mechanism_research.md#BaseMechanismResearcher)  (2 test-only)

### `TestExtractSelected`
- def: [`tests/test_mechanism_research.py:125`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L125)
- signature: `class TestExtractSelected:`
- members:
  - `setup_method(self)` — [`L126`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L126)
  - `test_case_insensitive_selected_keyword(self)` — [`L141`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L141)
  - `test_extracts_selected_line_from_critique(self)` — [`L129`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L129)
  - `test_falls_back_to_exploration_tail_when_no_selected(self)` — [`L147`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L147)
  - `test_falls_back_to_full_exploration_when_short(self)` — [`L155`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L155)
  - `test_selected_line_stripped_of_leading_whitespace(self)` — [`L161`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L161)
  - `researcher` — [`L127`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L127)
- uses (calls/refs, reference-scoped): [`_extract_selected`](../core/base_mechanism_research.md#BaseMechanismResearcher._extract_selected)  (1 test-only)

### `TestStripFences`
- def: [`tests/test_mechanism_research.py:86`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L86)
- signature: `class TestStripFences:`
- members:
  - `setup_method(self)` — [`L87`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L87)
  - `test_empty_string_unchanged(self)` — [`L116`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L116)
  - `test_fence_with_extra_tag_stripped(self)` — [`L119`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L119)
  - `test_multiline_body_preserved(self)` — [`L111`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L111)
  - `test_no_fences_unchanged(self)` — [`L100`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L100)
  - `test_only_opening_fence_removed(self)` — [`L105`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L105)
  - `test_removes_plain_fence(self)` — [`L95`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L95)
  - `test_removes_python_fence(self)` — [`L90`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L90)
  - `researcher` — [`L88`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L88)
- uses (calls/refs, reference-scoped): [`_strip_fences`](../core/base_mechanism_research.md#BaseMechanismResearcher._strip_fences)  (1 test-only)

### `TestSyntaxCheck`
- def: [`tests/test_mechanism_research.py:53`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L53)
- signature: `class TestSyntaxCheck:`
- members:
  - `setup_method(self)` — [`L54`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L54)
  - `test_empty_string_is_valid(self)` — [`L78`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L78)
  - `test_invalid_expression_returns_error_string(self)` — [`L72`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L72)
  - `test_invalid_syntax_returns_error_string(self)` — [`L65`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L65)
  - `test_multiline_valid_class(self)` — [`L81`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L81)
  - `test_valid_code_returns_none(self)` — [`L57`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L57)
  - `test_valid_function_returns_none(self)` — [`L61`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L61)
  - `researcher` — [`L55`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L55)
- uses (calls/refs, reference-scoped): [`_syntax_check`](../core/base_mechanism_research.md#BaseMechanismResearcher._syntax_check)  (1 test-only)

### `_ConcreteResearcher`  ·  implements/extends BaseMechanismResearcher
- def: [`tests/test_mechanism_research.py:10`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L10) — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
- signature: `class _ConcreteResearcher(BaseMechanismResearcher):`
- protocol/private: `_get_codegen_prompt`[`L17`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L17), `_get_explore_prompt`[`L11`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L11), `_get_reference_code`[`L20`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L20), `_get_specify_prompt`[`L14`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L14), `_parse_spec_metadata`[`L23`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L23)
- uses (calls/refs, reference-scoped): [`BaseMechanismResearcher`](../core/base_mechanism_research.md#BaseMechanismResearcher)
- used by: [`BaseMechanismResearcher`](../core/base_mechanism_research.md#BaseMechanismResearcher), [`_get_explore_prompt`](../core/base_mechanism_research.md#BaseMechanismResearcher._get_explore_prompt), [`_get_codegen_prompt`](../core/base_mechanism_research.md#BaseMechanismResearcher._get_codegen_prompt), [`_get_reference_code`](../core/base_mechanism_research.md#BaseMechanismResearcher._get_reference_code), [`_get_specify_prompt`](../core/base_mechanism_research.md#BaseMechanismResearcher._get_specify_prompt), [`_parse_spec_metadata`](../core/base_mechanism_research.md#BaseMechanismResearcher._parse_spec_metadata)  (4 test-only)

### `_Incomplete`  ·  implements/extends BaseMechanismResearcher
- def: [`tests/test_mechanism_research.py:44`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L44) — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
- signature: `class _Incomplete(BaseMechanismResearcher):`
- protocol/private: `_get_explore_prompt`[`L45`](../../../../../raw/code/bilevel-autoresearch/tests/test_mechanism_research.py#L45)
- uses (calls/refs, reference-scoped): [`BaseMechanismResearcher`](../core/base_mechanism_research.md#BaseMechanismResearcher)
- used by: [`BaseMechanismResearcher`](../core/base_mechanism_research.md#BaseMechanismResearcher), [`_get_explore_prompt`](../core/base_mechanism_research.md#BaseMechanismResearcher._get_explore_prompt)  (1 test-only)


---
title: 'Module: tests/test_llm_client.py'
type: catalog
provenance: extracted
module: tests/test_llm_client.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `tests.test_llm_client`/Test
symbols:
  TestStripThinkingTags.test_strips_think_block: StripThinkingTags#test_strips_think_block().
  TestStripThinkingTags.test_strips_multiline_think_block: StripThinkingTags#test_strips_multiline_think_block().
  TestStripThinkingTags.test_strips_case_insensitive: StripThinkingTags#test_strips_case_insensitive().
  TestStripThinkingTags.test_strips_incomplete_think_at_end: StripThinkingTags#test_strips_incomplete_think_at_end().
  TestStripThinkingTags.test_no_think_tags_unchanged: StripThinkingTags#test_no_think_tags_unchanged().
  TestStripThinkingTags.test_empty_string: StripThinkingTags#test_empty_string().
  TestStripThinkingTags.test_none_input: StripThinkingTags#test_none_input().
  TestStripThinkingTags.test_preserves_content_after_think: StripThinkingTags#test_preserves_content_after_think().
  TestParseJsonResponse.test_parse_plain_json_object: ParseJsonResponse#test_parse_plain_json_object().
  TestParseJsonResponse.test_parse_plain_json_array: ParseJsonResponse#test_parse_plain_json_array().
  TestParseJsonResponse.test_parse_markdown_fenced_json: ParseJsonResponse#test_parse_markdown_fenced_json().
  TestParseJsonResponse.test_parse_json_in_prose: ParseJsonResponse#test_parse_json_in_prose().
  TestParseJsonResponse.test_parse_array_in_prose: ParseJsonResponse#test_parse_array_in_prose().
  TestParseJsonResponse.test_empty_string_returns_raw_content: ParseJsonResponse#test_empty_string_returns_raw_content().
  TestParseJsonResponse.test_unparseable_returns_raw_content: ParseJsonResponse#test_unparseable_returns_raw_content().
  TestParseJsonResponse.test_strips_think_tags_before_parsing: ParseJsonResponse#test_strips_think_tags_before_parsing().
  TestParseJsonResponse.test_nested_json_parsed_correctly: ParseJsonResponse#test_nested_json_parsed_correctly().
  TestParseJsonResponse.test_fenced_without_language_tag: ParseJsonResponse#test_fenced_without_language_tag().
  TestConfigure.test_configure_known_provider: Configure#test_configure_known_provider().
  TestConfigure.test_configure_minimax: Configure#test_configure_minimax().
  TestConfigure.test_configure_unknown_provider_raises: Configure#test_configure_unknown_provider_raises().
  TestConfigure.test_all_providers_registered: Configure#test_all_providers_registered().
  TestStripThinkingTags: StripThinkingTags#
  TestParseJsonResponse: ParseJsonResponse#
  TestConfigure: Configure#
---
# Module: [`tests/test_llm_client.py`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py)

## Classes
### `TestConfigure`
- def: [`tests/test_llm_client.py:97`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L97)
- signature: `class TestConfigure:`
- members:
  - `test_all_providers_registered(self)` — [`L108`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L108)
  - `test_configure_known_provider(self)` — [`L98`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L98)
  - `test_configure_minimax(self)` — [`L101`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L101)
  - `test_configure_unknown_provider_raises(self)` — [`L104`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L104)
- uses (calls/refs, reference-scoped): [`PROVIDERS`](../core/llm_client.md#PROVIDERS.PROVIDERS), [`configure`](../core/llm_client.md#configure)

### `TestParseJsonResponse`
- def: [`tests/test_llm_client.py:45`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L45)
- signature: `class TestParseJsonResponse:`
- members:
  - `test_empty_string_returns_raw_content(self)` — [`L72`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L72)
  - `test_fenced_without_language_tag(self)` — [`L91`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L91)
  - `test_nested_json_parsed_correctly(self)` — [`L85`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L85)
  - `test_parse_array_in_prose(self)` — [`L66`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L66)
  - `test_parse_json_in_prose(self)` — [`L61`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L61)
  - `test_parse_markdown_fenced_json(self)` — [`L56`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L56)
  - `test_parse_plain_json_array(self)` — [`L51`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L51)
  - `test_parse_plain_json_object(self)` — [`L46`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L46)
  - `test_strips_think_tags_before_parsing(self)` — [`L80`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L80)
  - `test_unparseable_returns_raw_content(self)` — [`L76`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L76)
- uses (calls/refs, reference-scoped): [`parse_json_response`](../core/llm_client.md#parse_json_response)

### `TestStripThinkingTags`
- def: [`tests/test_llm_client.py:12`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L12)
- signature: `class TestStripThinkingTags:`
- members:
  - `test_empty_string(self)` — [`L34`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L34)
  - `test_no_think_tags_unchanged(self)` — [`L30`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L30)
  - `test_none_input(self)` — [`L37`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L37)
  - `test_preserves_content_after_think(self)` — [`L40`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L40)
  - `test_strips_case_insensitive(self)` — [`L21`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L21)
  - `test_strips_incomplete_think_at_end(self)` — [`L25`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L25)
  - `test_strips_multiline_think_block(self)` — [`L17`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L17)
  - `test_strips_think_block(self)` — [`L13`](../../../../../raw/code/bilevel-autoresearch/tests/test_llm_client.py#L13)
- uses (calls/refs, reference-scoped): [`_strip_thinking_tags`](../core/llm_client.md#_strip_thinking_tags)


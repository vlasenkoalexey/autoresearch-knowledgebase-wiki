---
title: 'Module: tests/test_prompt_sampler_comprehensive.py'
type: catalog
provenance: extracted
module: tests/test_prompt_sampler_comprehensive.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_prompt_sampler_comprehensive`/TestPromptSamplerComprehensive#
symbols:
  TestPromptSamplerComprehensive.prompt_sampler: prompt_sampler.
  TestPromptSamplerComprehensive.setUp: setUp().
  TestPromptSamplerComprehensive.test_build_prompt_with_inspirations: test_build_prompt_with_inspirations().
  TestPromptSamplerComprehensive.feature_dimensions: feature_dimensions.
  TestPromptSamplerComprehensive.test_format_inspirations_section_with_feature_dimensions: test_format_inspirations_section_with_feature_dimensions().
  TestPromptSamplerComprehensive.test_format_inspirations_section_without_feature_dimensions: test_format_inspirations_section_without_feature_dimensions().
  TestPromptSamplerComprehensive.test_determine_program_type_with_feature_dimensions: test_determine_program_type_with_feature_dimensions().
  TestPromptSamplerComprehensive.test_extract_unique_features_calls_determine_program_type: test_extract_unique_features_calls_determine_program_type().
  TestPromptSamplerComprehensive.test_build_prompt_with_all_optional_parameters: test_build_prompt_with_all_optional_parameters().
  TestPromptSamplerComprehensive.test_fitness_calculation_consistency: test_fitness_calculation_consistency().
  TestPromptSamplerComprehensive.test_empty_inspirations_list: test_empty_inspirations_list().
  TestPromptSamplerComprehensive.test_inspirations_with_missing_metrics: test_inspirations_with_missing_metrics().
  TestPromptSamplerComprehensive.test_feature_dimensions_none_vs_empty_list: test_feature_dimensions_none_vs_empty_list().
  TestPromptSamplerComprehensive.test_feature_coordinates_formatting_in_prompt: test_feature_coordinates_formatting_in_prompt().
  TestPromptSamplerComprehensive: ''
---
# Module: [`tests/test_prompt_sampler_comprehensive.py`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py)

## Classes
### `TestPromptSamplerComprehensive`  ·  implements/extends TestCase
- def: [`tests/test_prompt_sampler_comprehensive.py:11`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py#L11)
- doc: Comprehensive tests for prompt sampler edge cases
- signature: `class TestPromptSamplerComprehensive(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L14`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py#L14) — Set up test prompt sampler
  - `test_build_prompt_with_all_optional_parameters(self)` — [`L155`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py#L155) — Test build_prompt with all optional parameters including inspirations — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `test_build_prompt_with_inspirations(self)` — [`L22`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py#L22) — Test building a prompt with inspiration programs — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `test_determine_program_type_with_feature_dimensions(self)` — [`L127`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py#L127) — Test _determine_program_type with feature_dimensions parameter
  - `test_empty_inspirations_list(self)` — [`L209`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py#L209) — Test that empty inspirations list doesn't break anything — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `test_extract_unique_features_calls_determine_program_type(self)` — [`L141`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py#L141) — Test that _extract_unique_features correctly handles program_type determination
  - `test_feature_coordinates_formatting_in_prompt(self)` — [`L256`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py#L256) — Test that feature coordinates are formatted correctly in the prompt — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `test_feature_dimensions_none_vs_empty_list(self)` — [`L243`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py#L243) — Test that None and empty list for feature_dimensions are handled correctly
  - `test_fitness_calculation_consistency(self)` — [`L187`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py#L187) — Test that fitness calculation is consistent across all methods — documented in [openevolve-prompt-sampler](../../concepts/openevolve-prompt-sampler.md)
  - `test_format_inspirations_section_with_feature_dimensions(self)` — [`L84`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py#L84) — Test _format_inspirations_section directly with feature_dimensions
  - `test_format_inspirations_section_without_feature_dimensions(self)` — [`L110`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py#L110) — Test _format_inspirations_section works without feature_dimensions
  - `test_inspirations_with_missing_metrics(self)` — [`L221`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py#L221) — Test handling of inspirations with missing or invalid metrics
  - `feature_dimensions` — [`L20`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py#L20)
  - `prompt_sampler` — [`L19`](../../../../../raw/code/openevolve/tests/test_prompt_sampler_comprehensive.py#L19)
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`build_prompt`](../openevolve/prompt/sampler.md#PromptSampler.build_prompt), [`prompt`](../openevolve/config.md#Config.prompt), [`feature_dimensions`](../openevolve/config.md#DatabaseConfig.feature_dimensions), [`_extract_unique_features`](../openevolve/prompt/sampler.md#PromptSampler._extract_unique_features), [`_format_inspirations_section`](../openevolve/prompt/sampler.md#PromptSampler._format_inspirations_section), [`PromptSampler`](../openevolve/prompt/sampler.md#PromptSampler), [`_determine_program_type`](../openevolve/prompt/sampler.md#PromptSampler._determine_program_type)


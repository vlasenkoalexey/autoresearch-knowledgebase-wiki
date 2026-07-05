---
title: 'Module: core/base_mechanism_research.py'
type: catalog
provenance: extracted
module: core/base_mechanism_research.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `core.base_mechanism_research`/
symbols:
  BaseMechanismResearcher._generate_with_retries: BaseMechanismResearcher#_generate_with_retries().
  BaseMechanismResearcher._run_session: BaseMechanismResearcher#_run_session().
  BaseMechanismResearcher: BaseMechanismResearcher#
  BaseMechanismResearcher.client: BaseMechanismResearcher#client.
  BaseMechanismResearcher._syntax_check: BaseMechanismResearcher#_syntax_check().
  BaseMechanismResearcher._strip_fences: BaseMechanismResearcher#_strip_fences().
  BaseMechanismResearcher._get_explore_prompt: BaseMechanismResearcher#_get_explore_prompt().
  BaseMechanismResearcher._extract_selected: BaseMechanismResearcher#_extract_selected().
  logger: logger.
  BaseMechanismResearcher.max_code_retries: BaseMechanismResearcher#max_code_retries.
  BaseMechanismResearcher._get_specify_prompt: BaseMechanismResearcher#_get_specify_prompt().
  BaseMechanismResearcher._get_codegen_prompt: BaseMechanismResearcher#_get_codegen_prompt().
  BaseMechanismResearcher._get_reference_code: BaseMechanismResearcher#_get_reference_code().
  BaseMechanismResearcher._parse_spec_metadata: BaseMechanismResearcher#_parse_spec_metadata().
  CODEGEN_SYSTEM: CODEGEN_SYSTEM.
  FIX_PROMPT: FIX_PROMPT.
  CRITIQUE_SYSTEM: CRITIQUE_SYSTEM.
  CRITIQUE_PROMPT: CRITIQUE_PROMPT.
  BaseMechanismResearcher.__init__: BaseMechanismResearcher#__init__().
  BaseMechanismResearcher.artifacts_base: BaseMechanismResearcher#artifacts_base.
  BaseMechanismResearcher._extract_domain: BaseMechanismResearcher#_extract_domain().
---
# Module: [`core/base_mechanism_research.py`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py)

## Classes
### `BaseMechanismResearcher`  ·  implements/extends ABC
- def: [`core/base_mechanism_research.py:70`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L70) — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
- doc: Shared protocol for Level-2 mechanism research sessions.
- signature: `class BaseMechanismResearcher(ABC):`
- members:
  - `_extract_domain(self, exploration: str)` — [`L322`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L322) — Best-effort extraction of the domain the LLM mentioned first.
  - `_extract_selected(self, exploration: str, critique: str)` — [`L298`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L298) — Pull the selected hypothesis from critique output, fall back to exploration tail. — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
  - `_generate_with_retries(self, spec: str, reference_code: str, session_dir: Path, codegen_kwargs: dict)` — [`L242`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L242) — Generate code, retrying with error feedback on failure. — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
  - `_get_codegen_prompt(self, spec: str, reference_code: str, **kwargs)` — [`L124`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L124) — Return the prompt string for Round 4: Code generation. — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
  - `_get_explore_prompt(self, **kwargs)` — [`L105`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L105) — Return (prompt, system) for Round 1: Exploration. — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
  - `_get_reference_code(self, **kwargs)` — [`L132`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L132) — Return reference code to pass to _get_codegen_prompt. — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
  - `_get_specify_prompt(self, selected_hypothesis: str, critique: str, **kwargs)` — [`L114`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L114) — Return (prompt, system) for Round 3: Specification. — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
  - `_parse_spec_metadata(self, spec: str, session_id: str)` — [`L137`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L137) — Parse implementation metadata from the spec text. — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
  - `_run_session(self, session_dir: Path, session_id: str, log_prefix: str, explore_kwargs: dict, specify_kwargs: dict, codegen_kwargs: dict)` — [`L150`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L150) — Execute the 4-round research session. — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
  - `_strip_fences(self, code: str)` — [`L313`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L313) — Remove markdown code fences if the LLM added them anyway. — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
  - `_syntax_check(self, code: str)` — [`L305`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L305) — Return error string if code has syntax errors, else None. — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
  - `artifacts_base` — [`L96`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L96)
  - `client` — [`L94`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L94) — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
  - `max_code_retries` — [`L95`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L95) — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
- protocol/private: `__init__`[`L86`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L86)
- uses (calls/refs, reference-scoped): [`call`](llm_client.md#LLMClient.call), [`LLMClient`](llm_client.md#LLMClient), [`_generate_with_retries`](../domains/article_opt/mechanism_research.md#MechanismResearcher._generate_with_retries), [`_generate_with_retries`](../domains/train_opt/mechanism_research.md#TrainMechanismResearcher._generate_with_retries), [`logger`](base_mechanism_research.md#logger), [`CODEGEN_SYSTEM`](base_mechanism_research.md#CODEGEN_SYSTEM), [`TrainMechanismResearcher`](../domains/train_opt/mechanism_research.md#TrainMechanismResearcher), [`FIX_PROMPT`](base_mechanism_research.md#FIX_PROMPT), [`_get_explore_prompt`](../domains/article_opt/mechanism_research.md#MechanismResearcher._get_explore_prompt), [`_get_explore_prompt`](../domains/train_opt/mechanism_research.md#TrainMechanismResearcher._get_explore_prompt), [`_get_specify_prompt`](../domains/article_opt/mechanism_research.md#MechanismResearcher._get_specify_prompt), [`_get_specify_prompt`](../domains/train_opt/mechanism_research.md#TrainMechanismResearcher._get_specify_prompt), [`MechanismResearcher`](../domains/article_opt/mechanism_research.md#MechanismResearcher), [`CRITIQUE_PROMPT`](base_mechanism_research.md#CRITIQUE_PROMPT), [`CRITIQUE_SYSTEM`](base_mechanism_research.md#CRITIQUE_SYSTEM), [`_get_codegen_prompt`](../domains/article_opt/mechanism_research.md#MechanismResearcher._get_codegen_prompt), [`_get_codegen_prompt`](../domains/train_opt/mechanism_research.md#TrainMechanismResearcher._get_codegen_prompt), [`_get_reference_code`](../domains/article_opt/mechanism_research.md#MechanismResearcher._get_reference_code), [`_get_reference_code`](../domains/train_opt/mechanism_research.md#TrainMechanismResearcher._get_reference_code), [`_extract_selected`](../domains/article_opt/mechanism_research.md#MechanismResearcher._extract_selected), [`_extract_selected`](../domains/train_opt/mechanism_research.md#TrainMechanismResearcher._extract_selected), [`_parse_spec_metadata`](../domains/article_opt/mechanism_research.md#MechanismResearcher._parse_spec_metadata), [`_parse_spec_metadata`](../domains/train_opt/mechanism_research.md#TrainMechanismResearcher._parse_spec_metadata)  (8 test-only)
- used by: [`research`](../domains/article_opt/mechanism_research.md#MechanismResearcher.research), [`research`](../domains/train_opt/mechanism_research.md#TrainMechanismResearcher.research), [`validate`](../domains/article_opt/mechanism_research.md#MechanismResearcher.validate), [`apply`](../domains/train_opt/mechanism_research.md#TrainMechanismResearcher.apply), [`_generate_with_retries`](../domains/article_opt/mechanism_research.md#MechanismResearcher._generate_with_retries), [`_generate_with_retries`](../domains/train_opt/mechanism_research.md#TrainMechanismResearcher._generate_with_retries), [`TrainMechanismResearcher`](../domains/train_opt/mechanism_research.md#TrainMechanismResearcher), [`MechanismResearcher`](../domains/article_opt/mechanism_research.md#MechanismResearcher), [`__init__`](../domains/article_opt/mechanism_research.md#MechanismResearcher.__init__), [`__init__`](../domains/train_opt/mechanism_research.md#TrainMechanismResearcher.__init__)  (21 test-only)

## Module values
- `CODEGEN_SYSTEM` — [`L46`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L46) — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
- `CRITIQUE_PROMPT` — [`L30`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L30) — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
- `CRITIQUE_SYSTEM` — [`L27`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L27) — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
- `FIX_PROMPT` — [`L49`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L49) — documented in [core-base_mechanism_research](../../concepts/core-base_mechanism_research.md)
- `logger` — [`L21`](../../../../../raw/code/bilevel-autoresearch/core/base_mechanism_research.py#L21)


---
title: 'Module: domains/train_opt/mechanism_research.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanism_research.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanism_research`/
symbols:
  TrainMechanismResearcher.research: TrainMechanismResearcher#research().
  TrainMechanismResearcher.apply: TrainMechanismResearcher#apply().
  TrainMechanismResearcher._generate_with_retries: TrainMechanismResearcher#_generate_with_retries().
  logger: logger.
  TrainMechanismResearcher._save_summary: TrainMechanismResearcher#_save_summary().
  TrainMechanismResult.session_id: TrainMechanismResult#session_id.
  TrainMechanismResearcher: TrainMechanismResearcher#
  TrainMechanismResult.mechanism_name: TrainMechanismResult#mechanism_name.
  TrainMechanismResearcher._replace_method: TrainMechanismResearcher#_replace_method().
  TrainMechanismResearcher._append_to_init: TrainMechanismResearcher#_append_to_init().
  TrainMechanismResult.implementation_strategy: TrainMechanismResult#implementation_strategy.
  TrainMechanismResult.target: TrainMechanismResult#target.
  TrainMechanismResearcher._get_explore_prompt: TrainMechanismResearcher#_get_explore_prompt().
  TrainMechanismResearcher._get_specify_prompt: TrainMechanismResearcher#_get_specify_prompt().
  TrainMechanismResearcher.validate: TrainMechanismResearcher#validate().
  TrainMechanismResult: TrainMechanismResult#
  TrainMechanismResult.code_retries: TrainMechanismResult#code_retries.
  TrainMechanismResult.validation_error: TrainMechanismResult#validation_error.
  TrainMechanismResearcher.__init__: TrainMechanismResearcher#__init__().
  TrainMechanismResearcher._get_codegen_prompt: TrainMechanismResearcher#_get_codegen_prompt().
  TrainMechanismResearcher._get_reference_code: TrainMechanismResearcher#_get_reference_code().
  EXPLORE_SYSTEM: EXPLORE_SYSTEM.
  EXPLORE_PROMPT: EXPLORE_PROMPT.
  SPECIFY_SYSTEM: SPECIFY_SYSTEM.
  SPECIFY_PROMPT: SPECIFY_PROMPT.
  CODEGEN_PROMPT: CODEGEN_PROMPT.
  TrainMechanismResult.hypothesis: TrainMechanismResult#hypothesis.
  TrainMechanismResult.code: TrainMechanismResult#code.
  TrainMechanismResult.validated: TrainMechanismResult#validated.
  TrainMechanismResult.session_dir: TrainMechanismResult#session_dir.
  TrainMechanismResearcher._insert_helper_class: TrainMechanismResearcher#_insert_helper_class().
  TrainMechanismResearcher._read_reference_code: TrainMechanismResearcher#_read_reference_code().
  CRITIQUE_SYSTEM: CRITIQUE_SYSTEM.
  CRITIQUE_PROMPT: CRITIQUE_PROMPT.
  TrainMechanismResult.spec: TrainMechanismResult#spec.
  TrainMechanismResult.exploration: TrainMechanismResult#exploration.
  TrainMechanismResult.critique: TrainMechanismResult#critique.
  TrainMechanismResult.applied: TrainMechanismResult#applied.
  TrainMechanismResearcher._ast_replace_method: TrainMechanismResearcher#_ast_replace_method().
  TrainMechanismResearcher._insert_method: TrainMechanismResearcher#_insert_method().
  TrainMechanismResearcher._ast_append_to_init: TrainMechanismResearcher#_ast_append_to_init().
  TrainMechanismResearcher._extract_selected: TrainMechanismResearcher#_extract_selected().
  TrainMechanismResearcher._parse_spec_metadata: TrainMechanismResearcher#_parse_spec_metadata().
  TrainMechanismResearcher._summarize_existing_mechanisms: TrainMechanismResearcher#_summarize_existing_mechanisms().
  TrainMechanismResearcher._extract_runner_section: TrainMechanismResearcher#_extract_runner_section().
  TrainMechanismResearcher._infer_bottleneck: TrainMechanismResearcher#_infer_bottleneck().
  TrainMechanismResearcher._build_codegen_task: TrainMechanismResearcher#_build_codegen_task().
  TrainMechanismResearcher._runner_path: TrainMechanismResearcher#_runner_path.
---
# Module: [`domains/train_opt/mechanism_research.py`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py)

## Classes
### `TrainMechanismResearcher`  ·  implements/extends BaseMechanismResearcher
- def: [`domains/train_opt/mechanism_research.py:215`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L215) — documented in [core-base_mechanism_research](../../../concepts/core-base_mechanism_research.md)
- doc: Runs one Level-2 research session for the training domain.
- signature: `class TrainMechanismResearcher(BaseMechanismResearcher):`
- members:
  - `_append_to_init(self, original: str, new_init_code: str)` — [`L608`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L608) — Append attribute initializations to TrainRunner.__init__. — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `_ast_append_to_init(self, original: str, new_code: str)` — [`L628`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L628) — Append code to __init__ using AST positions. — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `_ast_replace_method(self, original: str, method_name: str, new_method_code: str)` — [`L547`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L547) — Precisely replace a method using AST node positions.
  - `_build_codegen_task(self, mechanism_name: str, impl_strategy: str, target: str, spec: str)` — [`L807`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L807) — Build a clear task description for the code generation prompt.
  - `_extract_runner_section(self, runner_code: str)` — [`L782`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L782) — Extract the TrainRunner class definition (first 3000 chars) for context. — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `_extract_selected(self, exploration: str, critique: str)` — [`L712`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L712) — Pull the selected hypothesis from critique output. — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `_generate_with_retries(self, spec: str, reference_code: str, codegen_task: str, session_dir: Path)` — [`L659`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L659) — Generate code, retrying with error feedback on failures. — documented in [core-base_mechanism_research](../../../concepts/core-base_mechanism_research.md)
  - `_infer_bottleneck(self, trace_summary: str)` — [`L789`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L789) — Try to infer the bottleneck from the trace text. — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `_insert_helper_class(self, original: str, new_class_code: str)` — [`L506`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L506) — Insert a new helper class before the TrainRunner class definition. — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `_insert_method(self, original: str, new_method_code: str)` — [`L583`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L583) — Append a new method to the TrainRunner class (before last class-level code).
  - `_parse_spec_metadata(self, spec: str, session_id: str)` — [`L720`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L720) — Extract mechanism_name, implementation_strategy, and target from spec text. — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `_read_reference_code(self, runner_code: str, impl_strategy: str)` — [`L847`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L847) — Extract a relevant reference snippet from runner.py for style guidance.
  - `_replace_method(self, original: str, method_name: str, new_method_code: str)` — [`L521`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L521) — Replace an existing method in TrainRunner with new code. — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `_summarize_existing_mechanisms(self, runner_code: str)` — [`L760`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L760) — Extract the docstring header from runner.py listing existing mechanisms. — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `apply(self, runner_path: Path, result: TrainMechanismResult)` — [`L402`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L402) — Apply the generated code patch to runner.py. — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `research(self, trace_summary: str, runner_code: str, session_dir: Path, bottleneck: str = "")` — [`L290`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L290) — Run one full research session. — documented in [core-base_mechanism_research](../../../concepts/core-base_mechanism_research.md)
  - `validate(self, runner_path: Path)` — [`L461`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L461) — Verify the modified runner.py can be imported without errors. — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
- protocol/private: `__init__`[`L229`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L229), `_get_codegen_prompt`[`L274`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L274), `_get_explore_prompt`[`L248`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L248), `_get_reference_code`[`L281`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L281), `_get_specify_prompt`[`L259`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L259), `_runner_path`[`L242`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L242), `_save_summary`[`L874`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L874)
- uses (calls/refs, reference-scoped): [`call`](../../core/llm_client.md#LLMClient.call), [`logger`](mechanism_research.md#logger), [`BaseMechanismResearcher`](../../core/base_mechanism_research.md#BaseMechanismResearcher), [`client`](../../core/base_mechanism_research.md#BaseMechanismResearcher.client), [`_strip_fences`](../../core/base_mechanism_research.md#BaseMechanismResearcher._strip_fences), [`_syntax_check`](../../core/base_mechanism_research.md#BaseMechanismResearcher._syntax_check), [`max_code_retries`](../../core/base_mechanism_research.md#BaseMechanismResearcher.max_code_retries), [`CODEGEN_SYSTEM`](../../core/base_mechanism_research.md#CODEGEN_SYSTEM), [`session_id`](mechanism_research.md#TrainMechanismResult.session_id), [`mechanism_name`](mechanism_research.md#TrainMechanismResult.mechanism_name), [`FIX_PROMPT`](../../core/base_mechanism_research.md#FIX_PROMPT), [`implementation_strategy`](mechanism_research.md#TrainMechanismResult.implementation_strategy), [`target`](mechanism_research.md#TrainMechanismResult.target), [`TrainMechanismResult`](mechanism_research.md#TrainMechanismResult), [`code_retries`](mechanism_research.md#TrainMechanismResult.code_retries), [`validation_error`](mechanism_research.md#TrainMechanismResult.validation_error), [`CODEGEN_PROMPT`](mechanism_research.md#CODEGEN_PROMPT), [`EXPLORE_PROMPT`](mechanism_research.md#EXPLORE_PROMPT), [`EXPLORE_SYSTEM`](mechanism_research.md#EXPLORE_SYSTEM), [`SPECIFY_PROMPT`](mechanism_research.md#SPECIFY_PROMPT), [`SPECIFY_SYSTEM`](mechanism_research.md#SPECIFY_SYSTEM), [`__init__`](../../core/base_mechanism_research.md#BaseMechanismResearcher.__init__), [`code`](mechanism_research.md#TrainMechanismResult.code), [`hypothesis`](mechanism_research.md#TrainMechanismResult.hypothesis), [`session_dir`](mechanism_research.md#TrainMechanismResult.session_dir), [`CRITIQUE_PROMPT`](mechanism_research.md#CRITIQUE_PROMPT), [`CRITIQUE_SYSTEM`](mechanism_research.md#CRITIQUE_SYSTEM), [`applied`](mechanism_research.md#TrainMechanismResult.applied), [`critique`](mechanism_research.md#TrainMechanismResult.critique), [`exploration`](mechanism_research.md#TrainMechanismResult.exploration), [`spec`](mechanism_research.md#TrainMechanismResult.spec)
- used by: [`run_group_d`](../../experiments/ablations/paper_ablation/run_ablation.md#run_group_d), [`run_group_c`](../../experiments/ablations/paper_ablation/run_ablation.md#run_group_c), [`_generate_with_retries`](../../core/base_mechanism_research.md#BaseMechanismResearcher._generate_with_retries), [`BaseMechanismResearcher`](../../core/base_mechanism_research.md#BaseMechanismResearcher), [`_extract_selected`](../../core/base_mechanism_research.md#BaseMechanismResearcher._extract_selected), [`_get_explore_prompt`](../../core/base_mechanism_research.md#BaseMechanismResearcher._get_explore_prompt), [`_get_codegen_prompt`](../../core/base_mechanism_research.md#BaseMechanismResearcher._get_codegen_prompt), [`_get_reference_code`](../../core/base_mechanism_research.md#BaseMechanismResearcher._get_reference_code), [`_get_specify_prompt`](../../core/base_mechanism_research.md#BaseMechanismResearcher._get_specify_prompt), [`_parse_spec_metadata`](../../core/base_mechanism_research.md#BaseMechanismResearcher._parse_spec_metadata)

### `TrainMechanismResult`
- def: [`domains/train_opt/mechanism_research.py:194`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L194) — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
- signature: `class TrainMechanismResult:`
- members:
  - `applied` — [`L205`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L205) — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `code` — [`L201`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L201) — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `code_retries` — [`L204`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L204) — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `critique` — [`L203`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L203)
  - `exploration` — [`L202`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L202)
  - `hypothesis` — [`L196`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L196) — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `implementation_strategy` — [`L198`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L198) — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `mechanism_name` — [`L197`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L197) — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `session_dir` — [`L208`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L208)
  - `session_id` — [`L195`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L195) — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `spec` — [`L200`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L200)
  - `target` — [`L199`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L199) — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
  - `validated` — [`L206`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L206)
  - `validation_error` — [`L207`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L207) — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
- used by: [`run_group_d`](../../experiments/ablations/paper_ablation/run_ablation.md#run_group_d), [`research`](mechanism_research.md#TrainMechanismResearcher.research), [`run_group_c`](../../experiments/ablations/paper_ablation/run_ablation.md#run_group_c), [`apply`](mechanism_research.md#TrainMechanismResearcher.apply), [`_save_summary`](mechanism_research.md#TrainMechanismResearcher._save_summary)

## Module values
- `CODEGEN_PROMPT` — [`L136`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L136) — documented in [core-base_mechanism_research](../../../concepts/core-base_mechanism_research.md)
- `CRITIQUE_PROMPT` — [`L84`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L84) — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
- `CRITIQUE_SYSTEM` — [`L80`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L80) — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
- `EXPLORE_PROMPT` — [`L49`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L49) — documented in [core-base_mechanism_research](../../../concepts/core-base_mechanism_research.md)
- `EXPLORE_SYSTEM` — [`L43`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L43) — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
- `SPECIFY_PROMPT` — [`L103`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L103) — documented in [core-base_mechanism_research](../../../concepts/core-base_mechanism_research.md)
- `SPECIFY_SYSTEM` — [`L100`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L100) — documented in [domains-train_opt-mechanism_research](../../../concepts/domains-train_opt-mechanism_research.md)
- `logger` — [`L37`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanism_research.py#L37)


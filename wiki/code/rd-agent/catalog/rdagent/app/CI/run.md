---
title: 'Module: rdagent/app/CI/run.py'
type: catalog
provenance: extracted
module: rdagent/app/CI/run.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.CI.run`/
symbols:
  CIEvoStr.evolve.CodeFixGroup.responses: CIEvoStr#evolve().CodeFixGroup#responses.
  error: error.
  RuffEvaluator.evaluate: RuffEvaluator#evaluate().
  MypyEvaluator.evaluate: MypyEvaluator#evaluate().
  count: count.
  record: record.
  ea: ea.
  total_errors_count: total_errors_count.
  CIEvoAgent.multistep_evolve: CIEvoAgent#multistep_evolve().
  CodeFile.get: CodeFile#get().
  CIError.__str__: CIError#__str__().
  FixRecord.to_dict: FixRecord#to_dict().
  Repo.project_path: Repo#project_path.
  filename: filename.
  CIError.code: CIError#code.
  MultiEvaluator.evaluate: MultiEvaluator#evaluate().
  Repo: Repo#
  repo: repo.
  table: table.
  CIFeedback: CIFeedback#
  CIFeedback.errors: CIFeedback#errors.
  DIR: DIR.
  CIError: CIError#
  CIFeedback.statistics: CIFeedback#statistics().
  CodeFile.apply_changes: CodeFile#apply_changes().
  CodeFile.get_code_blocks: CodeFile#get_code_blocks().
  execution_time: execution_time.
  file: file.
  code: code.
  FixRecord.skipped_errors: FixRecord#skipped_errors.
  Repo.files: Repo#files.
  CIEvoStr.evolve: CIEvoStr#evolve().
  CIError.msg: CIError#msg.
  fix_records: fix_records.
  CI_prompts: CI_prompts.
  FixRecord.directly_fixed_errors: FixRecord#directly_fixed_errors.
  FixRecord.manually_fixed_errors: FixRecord#manually_fixed_errors.
  CIError.line: CIError#line.
  CodeFile.code_lines: CodeFile#code_lines.
  CodeFile.code_lines_with_lineno: CodeFile#code_lines_with_lineno.
  code_message: code_message.
  excludes: excludes.
  CIError.column: CIError#column.
  CIEvoAgent.__init__: CIEvoAgent#__init__().
  FixRecord.manual_instructions: FixRecord#manual_instructions.
  CodeFile.load: CodeFile#load().
  CodeFile.lineno: CodeFile#lineno.
  CodeFile.get_blocks_in_node: CodeFile#get_blocks_in_node().
  Repo.fix_records: Repo#fix_records.
  MypyEvaluator.command: MypyEvaluator#command.
  CIEvoStr: CIEvoStr#
  CIEvoStr.evolve.CodeFixGroup.errors: CIEvoStr#evolve().CodeFixGroup#errors.
  evaluator: evaluator.
  CIError.checker: CIError#checker.
  CIError.to_dict: CIError#to_dict().
  CodeFile: CodeFile#
  CIEvoAgent.evolving_trace: CIEvoAgent#evolving_trace.
  skipped_errors_count: skipped_errors_count.
  directly_fixed_errors_count: directly_fixed_errors_count.
  manually_fixed_errors_count: manually_fixed_errors_count.
  CodeFile.add_line_number: CodeFile#add_line_number().
  CodeFile.remove_line_number: CodeFile#remove_line_number().
  CodeFile.lineno_width: CodeFile#lineno_width.
  RuffEvaluator: RuffEvaluator#
  CIEvoAgent: CIEvoAgent#
  estr: estr.
  operation: operation.
  CIError.file_path: CIError#file_path.
  CIError.hint: CIError#hint.
  FixRecord: FixRecord#
  CodeFile.path: CodeFile#path.
  CodeFile.__init__: CodeFile#__init__().
  CodeFile.__str__: CodeFile#__str__().
  RuffEvaluator.__init__: RuffEvaluator#__init__().
  RuffEvaluator.explain_rule: RuffEvaluator#explain_rule().
  MypyEvaluator: MypyEvaluator#
  MultiEvaluator: MultiEvaluator#
  MultiEvaluator.__init__: MultiEvaluator#__init__().
  CIError.raw_str: CIError#raw_str.
  RuffRule: RuffRule#
  RuffEvaluator.command: RuffEvaluator#command.
  CIEvoStr.evolve.CodeFixGroup: CIEvoStr#evolve().CodeFixGroup#
  CIEvoStr.evolve.CodeFixGroup.start_line: CIEvoStr#evolve().CodeFixGroup#start_line.
  CIEvoStr.evolve.CodeFixGroup.end_line: CIEvoStr#evolve().CodeFixGroup#end_line.
  CIEvoStr.evolve.CodeFixGroup.session_id: CIEvoStr#evolve().CodeFixGroup#session_id.
  skipped_errors_code_count: skipped_errors_code_count.
  directly_fixed_errors_code_count: directly_fixed_errors_code_count.
  manually_fixed_errors_code_count: manually_fixed_errors_code_count.
  skipped_errors_statistics: skipped_errors_statistics.
  directly_fixed_errors_statistics: directly_fixed_errors_statistics.
  manually_fixed_errors_statistics: manually_fixed_errors_statistics.
  py_parser: py_parser.
  MultiEvaluator.evaluators: MultiEvaluator#evaluators.
  start_time: start_time.
  start_timestamp: start_timestamp.
  end_time: end_time.
  Repo.__init__: Repo#__init__().
  Repo.params: Repo#params.
  RuffRule.name: RuffRule#name.
  RuffRule.code: RuffRule#code.
  RuffRule.linter: RuffRule#linter.
  RuffRule.summary: RuffRule#summary.
  RuffRule.message_formats: RuffRule#message_formats.
  RuffRule.fix: RuffRule#fix.
  RuffRule.explanation: RuffRule#explanation.
  RuffRule.preview: RuffRule#preview.
  MypyEvaluator.__init__: MypyEvaluator#__init__().
---
# Module: [`rdagent/app/CI/run.py`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py)

## Classes
### `CIError`
- def: [`rdagent/app/CI/run.py:43`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L43) — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
- signature: `class CIError:`
- members:
  - `to_dict(self)` — [`L53`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L53)
  - `checker` — [`L51`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L51)
  - `code` — [`L48`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L48)
  - `column` — [`L47`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L47)
  - `file_path` — [`L45`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L45)
  - `hint` — [`L50`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L50)
  - `line` — [`L46`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L46)
  - `msg` — [`L49`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L49)
  - `raw_str` — [`L44`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L44)
- protocol/private: `__str__`[`L56`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L56)
- used by: [`responses`](run.md#CIEvoStr.evolve.CodeFixGroup.responses), [`error`](run.md#error), [`evaluate`](run.md#MypyEvaluator.evaluate), [`evaluate`](run.md#RuffEvaluator.evaluate), [`to_dict`](run.md#FixRecord.to_dict), [`errors`](run.md#CIFeedback.errors), [`statistics`](run.md#CIFeedback.statistics), [`skipped_errors`](run.md#FixRecord.skipped_errors), [`directly_fixed_errors`](run.md#FixRecord.directly_fixed_errors), [`manually_fixed_errors`](run.md#FixRecord.manually_fixed_errors), [`errors`](run.md#CIEvoStr.evolve.CodeFixGroup.errors), [`manual_instructions`](run.md#FixRecord.manual_instructions)

### `CIEvoAgent`  ·  implements/extends EvoAgent
- def: [`rdagent/app/CI/run.py:696`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L696)
- signature: `class CIEvoAgent(EvoAgent):`
- members:
  - `multistep_evolve(self, evo: Repo, eva: Evaluator)` — [`L701`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L701) — documented in [rdagent-core-evolving_framework](../../../../concepts/rdagent-core-evolving_framework.md)
  - `evolving_trace` — [`L699`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L699)
- protocol/private: `__init__`[`L697`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L697)
- uses (calls/refs, reference-scoped): [`Evaluator`](../../core/evaluation.md#Evaluator), [`EvoStep`](../../core/evolving_framework.md#EvoStep), [`evaluate`](../../core/evaluation.md#Evaluator.evaluate), [`feedback`](../../core/evolving_framework.md#EvoStep.feedback), [`EvoAgent`](../../core/evolving_agent.md#EvoAgent), [`Repo`](run.md#Repo), [`CIEvoStr`](run.md#CIEvoStr), [`__init__`](../../core/evolving_agent.md#EvoAgent.__init__), [`evolving_strategy`](../../core/evolving_agent.md#EvoAgent.evolving_strategy)
- used by: [`ea`](run.md#ea), [`filename`](run.md#filename), [`EvoAgent`](../../core/evolving_agent.md#EvoAgent), [`multistep_evolve`](../../core/evolving_agent.md#EvoAgent.multistep_evolve)

### `CIEvoStr`  ·  implements/extends EvolvingStrategy
- def: [`rdagent/app/CI/run.py:431`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L431)
- signature: `class CIEvoStr(EvolvingStrategy):`
- members:
  - `evolve(self, evo: Repo, evolving_trace: list[EvoStep] | None = None, knowledge_l: list[Knowledge] | None = None, **kwargs: dict)` — [`L432`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L432)
- uses (calls/refs, reference-scoped): [`EvoStep`](../../core/evolving_framework.md#EvoStep), [`EvolvingStrategy`](../../core/evolving_framework.md#EvolvingStrategy), [`Repo`](run.md#Repo), [`Knowledge`](../../core/evolving_framework.md#Knowledge)
- used by: [`EvolvingStrategy`](../../core/evolving_framework.md#EvolvingStrategy), [`__init__`](run.md#CIEvoAgent.__init__), [`estr`](run.md#estr)

### `CIFeedback`  ·  implements/extends Feedback
- def: [`rdagent/app/CI/run.py:61`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L61) — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
- signature: `class CIFeedback(Feedback):`
- members:
  - `statistics(self)` — [`L64`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L64) — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
  - `errors` — [`L62`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L62)
- uses (calls/refs, reference-scoped): [`Feedback`](../../core/evaluation.md#Feedback), [`code`](run.md#CIError.code), [`CIError`](run.md#CIError), [`checker`](run.md#CIError.checker)
- used by: [`responses`](run.md#CIEvoStr.evolve.CodeFixGroup.responses), [`evaluate`](run.md#MypyEvaluator.evaluate), [`evaluate`](run.md#RuffEvaluator.evaluate), [`Feedback`](../../core/evaluation.md#Feedback), [`evaluate`](run.md#MultiEvaluator.evaluate)

### `CodeFile`
- def: [`rdagent/app/CI/run.py:90`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L90)
- signature: `class CodeFile:`
- members:
  - `add_line_number(cls: CodeFile, code: list[str] | str, start: int = 1)` — [`L96`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L96)
  - `apply_changes(self, changes: list[tuple[int, int, str]])` — [`L159`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L159) — Applies the given changes to the code lines. — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
  - `get(self, start: int = 1, end: int | None = None, *, add_line_number: bool = False, return_list: bool = False)` — [`L126`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L126) — Retrieves a portion of the code lines. — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
  - `get_blocks_in_node(node: Node, max_lines: int)` — [`L185`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L185)
  - `get_code_blocks(self, max_lines: int = 30)` — [`L182`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L182) — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
  - `load(self)` — [`L117`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L117)
  - `remove_line_number(cls: CodeFile, code: list[str] | str)` — [`L107`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L107)
  - `code_lines` — [`L119`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L119)
  - `code_lines_with_lineno` — [`L124`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L124)
  - `lineno` — [`L122`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L122)
  - `lineno_width` — [`L123`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L123)
  - `path` — [`L92`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L92)
- protocol/private: `__init__`[`L91`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L91), `__str__`[`L214`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L214)
- uses (calls/refs, reference-scoped): [`py_parser`](run.md#py_parser)
- used by: [`responses`](run.md#CIEvoStr.evolve.CodeFixGroup.responses), [`files`](run.md#Repo.files)

### `CodeFixGroup`
- def: [`rdagent/app/CI/run.py:440`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L440)
- signature: `class CodeFixGroup:`
- members:
  - `end_line` — [`L442`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L442)
  - `errors` — [`L443`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L443)
  - `responses` — [`L445`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L445) — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
  - `session_id` — [`L444`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L444)
  - `start_line` — [`L441`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L441)
- uses (calls/refs, reference-scoped): [`APIBackend`](../../oai/llm_utils.md#APIBackend), [`build_chat_completion`](../../oai/backend/base.md#ChatSession.build_chat_completion), [`build_chat_session`](../../oai/backend/base.md#APIBackend.build_chat_session), [`get`](run.md#CodeFile.get), [`feedback`](../../core/evolving_framework.md#EvoStep.feedback), [`project_path`](run.md#Repo.project_path), [`code`](run.md#CIError.code), [`CIFeedback`](run.md#CIFeedback), [`errors`](run.md#CIFeedback.errors), [`CIError`](run.md#CIError), [`apply_changes`](run.md#CodeFile.apply_changes), [`get_code_blocks`](run.md#CodeFile.get_code_blocks), [`statistics`](run.md#CIFeedback.statistics), [`files`](run.md#Repo.files), [`skipped_errors`](run.md#FixRecord.skipped_errors), [`msg`](run.md#CIError.msg), [`CI_prompts`](run.md#CI_prompts), [`directly_fixed_errors`](run.md#FixRecord.directly_fixed_errors), [`manually_fixed_errors`](run.md#FixRecord.manually_fixed_errors), [`line`](run.md#CIError.line), [`column`](run.md#CIError.column), [`fix_records`](run.md#Repo.fix_records), [`manual_instructions`](run.md#FixRecord.manual_instructions), [`CodeFile`](run.md#CodeFile), [`checker`](run.md#CIError.checker), [`get_conversation_id`](../../oai/backend/base.md#ChatSession.get_conversation_id), [`lineno_width`](run.md#CodeFile.lineno_width), [`remove_line_number`](run.md#CodeFile.remove_line_number), [`FixRecord`](run.md#FixRecord)

### `FixRecord`
- def: [`rdagent/app/CI/run.py:73`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L73)
- signature: `class FixRecord:`
- members:
  - `to_dict(self)` — [`L79`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L79)
  - `directly_fixed_errors` — [`L75`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L75) — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
  - `manual_instructions` — [`L77`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L77)
  - `manually_fixed_errors` — [`L76`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L76) — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
  - `skipped_errors` — [`L74`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L74) — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
- uses (calls/refs, reference-scoped): [`CIError`](run.md#CIError), [`to_dict`](run.md#CIError.to_dict)
- used by: [`responses`](run.md#CIEvoStr.evolve.CodeFixGroup.responses), [`error`](run.md#error), [`record`](run.md#record), [`file`](run.md#file), [`fix_records`](run.md#Repo.fix_records)

### `MultiEvaluator`  ·  implements/extends Evaluator
- def: [`rdagent/app/CI/run.py:413`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L413)
- signature: `class MultiEvaluator(Evaluator):`
- members:
  - `evaluate(self, evo: Repo, **kwargs: dict)` — [`L417`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L417)
  - `evaluators` — [`L415`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L415)
- protocol/private: `__init__`[`L414`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L414)
- uses (calls/refs, reference-scoped): [`Evaluator`](../../core/evaluation.md#Evaluator), [`evaluate`](../../core/evaluation.md#Evaluator.evaluate), [`Repo`](run.md#Repo), [`CIFeedback`](run.md#CIFeedback), [`errors`](run.md#CIFeedback.errors)
- used by: [`Evaluator`](../../core/evaluation.md#Evaluator), [`evaluate`](../../core/evaluation.md#Evaluator.evaluate)

### `MypyEvaluator`  ·  implements/extends Evaluator
- def: [`rdagent/app/CI/run.py:358`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L358)
- signature: `class MypyEvaluator(Evaluator):`
- members:
  - `evaluate(self, evo: Repo, **kwargs: dict)` — [`L365`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L365) — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
  - `command` — [`L361`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L361)
- protocol/private: `__init__`[`L359`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L359)
- uses (calls/refs, reference-scoped): [`Evaluator`](../../core/evaluation.md#Evaluator), [`project_path`](run.md#Repo.project_path), [`code`](run.md#CIError.code), [`Repo`](run.md#Repo), [`CIFeedback`](run.md#CIFeedback), [`errors`](run.md#CIFeedback.errors), [`CIError`](run.md#CIError), [`files`](run.md#Repo.files), [`msg`](run.md#CIError.msg), [`line`](run.md#CIError.line), [`column`](run.md#CIError.column), [`checker`](run.md#CIError.checker), [`file_path`](run.md#CIError.file_path), [`hint`](run.md#CIError.hint), [`raw_str`](run.md#CIError.raw_str)
- used by: [`Evaluator`](../../core/evaluation.md#Evaluator), [`evaluate`](../../core/evaluation.md#Evaluator.evaluate)

### `Repo`  ·  implements/extends EvolvableSubjects
- def: [`rdagent/app/CI/run.py:218`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L218) — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
- signature: `class Repo(EvolvableSubjects):`
- members:
  - `files` — [`L249`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L249) — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
  - `fix_records` — [`L251`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L251)
  - `params` — [`L222`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L222)
  - `project_path` — [`L223`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L223)
- protocol/private: `__init__`[`L219`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L219)
- uses (calls/refs, reference-scoped): [`EvolvableSubjects`](../../core/evolving_framework.md#EvolvableSubjects), [`CodeFile`](run.md#CodeFile), [`FixRecord`](run.md#FixRecord)
- used by: [`responses`](run.md#CIEvoStr.evolve.CodeFixGroup.responses), [`evaluate`](run.md#MypyEvaluator.evaluate), [`evaluate`](run.md#RuffEvaluator.evaluate), [`ea`](run.md#ea), [`EvolvableSubjects`](../../core/evolving_framework.md#EvolvableSubjects), [`multistep_evolve`](run.md#CIEvoAgent.multistep_evolve), [`evaluate`](run.md#MultiEvaluator.evaluate), [`repo`](run.md#repo), [`evolve`](run.md#CIEvoStr.evolve), [`fix_records`](run.md#fix_records)

### `RuffEvaluator`  ·  implements/extends Evaluator
- def: [`rdagent/app/CI/run.py:282`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L282)
- doc: The error message are generated by command
- signature: `class RuffEvaluator(Evaluator):`
- members:
  - `evaluate(self, evo: Repo, **kwargs: dict)` — [`L307`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L307) — Simply run ruff to get the feedbacks. — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
  - `explain_rule(error_code: str)` — [`L294`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L294)
  - `command` — [`L289`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L289)
- protocol/private: `__init__`[`L287`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L287)
- uses (calls/refs, reference-scoped): [`Evaluator`](../../core/evaluation.md#Evaluator), [`project_path`](run.md#Repo.project_path), [`code`](run.md#CIError.code), [`Repo`](run.md#Repo), [`CIFeedback`](run.md#CIFeedback), [`errors`](run.md#CIFeedback.errors), [`CIError`](run.md#CIError), [`files`](run.md#Repo.files), [`msg`](run.md#CIError.msg), [`line`](run.md#CIError.line), [`column`](run.md#CIError.column), [`checker`](run.md#CIError.checker), [`file_path`](run.md#CIError.file_path), [`hint`](run.md#CIError.hint), [`RuffRule`](run.md#RuffRule), [`raw_str`](run.md#CIError.raw_str)
- used by: [`Evaluator`](../../core/evaluation.md#Evaluator), [`evaluate`](../../core/evaluation.md#Evaluator.evaluate), [`evaluator`](run.md#evaluator)

### `RuffRule`
- def: [`rdagent/app/CI/run.py:255`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L255)
- doc: Example:
- signature: `class RuffRule:`
- members:
  - `code` — [`L273`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L273)
  - `explanation` — [`L278`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L278)
  - `fix` — [`L277`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L277)
  - `linter` — [`L274`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L274)
  - `message_formats` — [`L276`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L276)
  - `name` — [`L272`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L272)
  - `preview` — [`L279`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L279)
  - `summary` — [`L275`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L275)
- used by: [`explain_rule`](run.md#RuffEvaluator.explain_rule)

## Module values
- `CI_prompts` — [`L39`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L39)
- `DIR` — [`L712`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L712)
- `code` — [`L766`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L766)
- `code_message` — [`L748`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L748)
- `count` — [`L766`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L766)
- `directly_fixed_errors_code_count` — [`L746`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L746)
- `directly_fixed_errors_count` — [`L743`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L743)
- `directly_fixed_errors_statistics` — [`L764`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L764)
- `ea` — [`L730`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L730)
- `end_time` — [`L810`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L810)
- `error` — [`L753`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L753)
- `estr` — [`L729`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L729)
- `evaluator` — [`L728`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L728)
- `excludes` — [`L717`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L717)
- `execution_time` — [`L811`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L811)
- `file` — [`L738`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L738)
- `filename` — [`L737`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L737)
- `fix_records` — [`L736`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L736) — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
- `manually_fixed_errors_code_count` — [`L747`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L747)
- `manually_fixed_errors_count` — [`L744`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L744)
- `manually_fixed_errors_statistics` — [`L765`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L765)
- `operation` — [`L805`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L805)
- `py_parser` — [`L38`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L38)
- `record` — [`L749`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L749)
- `repo` — [`L726`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L726)
- `skipped_errors_code_count` — [`L745`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L745)
- `skipped_errors_count` — [`L742`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L742)
- `skipped_errors_statistics` — [`L763`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L763)
- `start_time` — [`L723`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L723)
- `start_timestamp` — [`L724`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L724)
- `table` — [`L774`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L774)
- `total_errors_count` — [`L780`](../../../../../../../raw/code/rd-agent/rdagent/app/CI/run.py#L780)


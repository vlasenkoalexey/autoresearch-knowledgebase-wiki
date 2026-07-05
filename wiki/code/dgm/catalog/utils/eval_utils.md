---
title: 'Module: utils/eval_utils.py'
type: catalog
provenance: extracted
module: utils/eval_utils.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `utils.eval_utils`/
symbols:
  score_tie_breaker: score_tie_breaker().
  msg_history_to_report: msg_history_to_report().
  parse_eval_output: parse_eval_output().
  get_report_score: get_report_score().
---
# Module: [`utils/eval_utils.py`](../../../../../raw/code/dgm/utils/eval_utils.py)

## Functions
- `get_report_score(test_report)` — [`L42`](../../../../../raw/code/dgm/utils/eval_utils.py#L42) — Get the score from the test report.
- `msg_history_to_report(instance_id, msg_history, model=None)` — [`L22`](../../../../../raw/code/dgm/utils/eval_utils.py#L22) — Get test report from the message history. — documented in [coding_agent](../../concepts/coding_agent.md)
- `parse_eval_output(instance_id, eval_output)` — [`L7`](../../../../../raw/code/dgm/utils/eval_utils.py#L7) — documented in [coding_agent](../../concepts/coding_agent.md)
- `score_tie_breaker(problem_statement, code_diffs, test_reports, best_score_indices=[], logging=print)` — [`L51`](../../../../../raw/code/dgm/utils/eval_utils.py#L51) — Use LLM as a tiebreaker to choose the best code diff.


---
title: 'Module: examples/online_judge_programming/submit.py'
type: catalog
provenance: extracted
module: examples/online_judge_programming/submit.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.online_judge_programming.submit`/
symbols:
  show_judgement: show_judgement().
  main: main().
  login_from_config: login_from_config().
  _STATUS_MAP: _STATUS_MAP.
  guess_mainclass: guess_mainclass().
  get_config: get_config().
  guess_language: guess_language().
  color: color().
  _RUNNING_STATUS: _RUNNING_STATUS.
  ConfigError: ConfigError#
  _RED_COLOR: _RED_COLOR.
  login: login().
  submit: submit().
  confirm_or_die: confirm_or_die().
  get_submission_url: get_submission_url().
  get_submission_status: get_submission_status().
  _HEADERS: _HEADERS.
  _COMPILE_ERROR_STATUS: _COMPILE_ERROR_STATUS.
  get_url: get_url().
  _DEFAULT_CONFIG: _DEFAULT_CONFIG.
  _GUESS_MAINFILE: _GUESS_MAINFILE.
  _ACCEPTED_STATUS: _ACCEPTED_STATUS.
  guess_mainfile: guess_mainfile().
  _GREEN_COLOR: _GREEN_COLOR.
  _LANGUAGE_GUESS: _LANGUAGE_GUESS.
  _GUESS_MAINCLASS: _GUESS_MAINCLASS.
  is_python2: is_python2().
  _YELLOW_COLOR: _YELLOW_COLOR.
---
# Module: [`examples/online_judge_programming/submit.py`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py)

## Classes
### `ConfigError`  ·  implements/extends Exception
- def: [`examples/online_judge_programming/submit.py:134`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L134)
- signature: `class ConfigError(Exception):`
- used by: (3 test-only callers)

## Functions
- `color(s, c)` — [`L376`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L376)
- `confirm_or_die(problem, language, files, mainclass, tag)` — [`L341`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L341)
- `get_config()` — [`L146`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L146) — Returns a ConfigParser object for the .kattisrc file(s)
- `get_submission_status(submission_url, cookies)` — [`L366`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L366)
- `get_submission_url(submit_response, cfg)` — [`L358`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L358)
- `get_url(cfg, option, default)` — [`L138`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L138)
- `guess_language(ext, files)` — [`L204`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L204)
- `guess_mainclass(language, files)` — [`L242`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L242)
- `guess_mainfile(language, files)` — [`L221`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L221)
- `is_python2(files)` — [`L184`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L184)
- `login(login_url, username, password=None, token=None)` — [`L254`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L254) — Log in to Kattis.
- `login_from_config(cfg)` — [`L270`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L270) — Log in to Kattis using the access information in a kattisrc file
- `main()` — [`L459`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L459)
- `show_judgement(submission_url, cfg)` — [`L380`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L380)
- `submit(submit_url, cookies, problem, language, files, mainclass="", tag="", assignment=None, contest=None)` — [`L298`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L298) — Make a submission.

## Module values
- `_ACCEPTED_STATUS` — [`L112`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L112)
- `_COMPILE_ERROR_STATUS` — [`L111`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L111)
- `_DEFAULT_CONFIG` — [`L12`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L12)
- `_GREEN_COLOR` — [`L372`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L372)
- `_GUESS_MAINCLASS` — [`L76`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L76)
- `_GUESS_MAINFILE` — [`L77`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L77)
- `_HEADERS` — [`L108`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L108)
- `_LANGUAGE_GUESS` — [`L13`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L13)
- `_RED_COLOR` — [`L371`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L371)
- `_RUNNING_STATUS` — [`L110`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L110)
- `_STATUS_MAP` — [`L113`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L113)
- `_YELLOW_COLOR` — [`L373`](../../../../../../raw/code/openevolve/examples/online_judge_programming/submit.py#L373)


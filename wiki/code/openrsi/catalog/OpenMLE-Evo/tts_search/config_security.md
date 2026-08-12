---
title: 'Module: OpenMLE-Evo/tts_search/config_security.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/tts_search/config_security.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.tts_search.config_security`/
symbols:
  redact_sensitive_config: redact_sensitive_config().
  _is_sensitive_key: _is_sensitive_key().
  redact_sensitive_yaml_file: redact_sensitive_yaml_file().
  _redact_override_string: _redact_override_string().
  _SENSITIVE_CONFIG_KEYS: _SENSITIVE_CONFIG_KEYS.
---
# Module: [`OpenMLE-Evo/tts_search/config_security.py`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/config_security.py)

## Functions
- `_is_sensitive_key(value: Any)` — [`L20`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/config_security.py#L20)
- `_redact_override_string(value: str)` — [`L31`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/config_security.py#L31)
- `redact_sensitive_config(value: Any)` — [`L41`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/config_security.py#L41) — Return a copy with credential-bearing config fields replaced by null.
- `redact_sensitive_yaml_file(path: Path)` — [`L60`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/config_security.py#L60) — Redact a YAML mapping/list in place; return False for unsupported files.

## Module values
- `_SENSITIVE_CONFIG_KEYS` — [`L8`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/config_security.py#L8)


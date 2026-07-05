---
title: 'Module: rdagent/app/utils/health_check.py'
type: catalog
provenance: extracted
module: rdagent/app/utils/health_check.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.utils.health_check`/
symbols:
  env_check: env_check().
  health_check: health_check().
  check_docker_status: check_docker_status().
  check_and_list_free_ports: check_and_list_free_ports().
  test_chat: test_chat().
  test_embedding: test_embedding().
  is_port_in_use: is_port_in_use().
---
# Module: [`rdagent/app/utils/health_check.py`](../../../../../../../raw/code/rd-agent/rdagent/app/utils/health_check.py)

## Functions
- `check_and_list_free_ports(start_port=19899, max_ports=10)` — [`L37`](../../../../../../../raw/code/rd-agent/rdagent/app/utils/health_check.py#L37)
- `check_docker_status()` — [`L14`](../../../../../../../raw/code/rd-agent/rdagent/app/utils/health_check.py#L14)
- `env_check()` — [`L94`](../../../../../../../raw/code/rd-agent/rdagent/app/utils/health_check.py#L94)
- `health_check(check_env: bool = True, check_docker: bool = True, check_ports: bool = True)` — [`L135`](../../../../../../../raw/code/rd-agent/rdagent/app/utils/health_check.py#L135) — Run the RD-Agent health check:
- `is_port_in_use(port)` — [`L32`](../../../../../../../raw/code/rd-agent/rdagent/app/utils/health_check.py#L32)
- `test_chat(chat_model, chat_api_key, chat_api_base)` — [`L51`](../../../../../../../raw/code/rd-agent/rdagent/app/utils/health_check.py#L51)
- `test_embedding(embedding_model, embedding_api_key, embedding_api_base)` — [`L78`](../../../../../../../raw/code/rd-agent/rdagent/app/utils/health_check.py#L78)


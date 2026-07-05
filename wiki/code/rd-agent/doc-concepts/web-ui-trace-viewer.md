---
title: Web UI & trace viewer
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Web UI & trace viewer

## Definition
R&D-Agent ships two front-ends for watching a run and replaying its execution trace. The README distinguishes them explicitly: **`rdagent ui`** is a Streamlit app for viewing run logs (the recommended viewer for the `data_science` scenario, via `--data-science`), while **`rdagent server_ui`** is a newer Flask backend that serves a built React/JS frontend from `web/` for "real-time interaction and trace viewing" (currently *excluding* the `data_science` scenario). Both default to port `19899`. The publicly hosted [Live Demo](https://rdagent.azurewebsites.net) shows the same trace windows (factor loop, model loop, etc.) that these UIs render locally.

## In rd-agent (grounded)
The entry points are CLI subcommands in `rdagent/app/cli.py`: [`ui`](../catalog/rdagent/app/cli.md#ui) ("start web app to show the log traces", with `log_dir`, `port`, and `data_science` flags), [`server_ui`](../catalog/rdagent/app/cli.md#server_ui) ("start the Flask log server in real time"), and [`ds_user_interact`](../catalog/rdagent/app/cli.md#ds_user_interact) ("start web app to show the log traces in real time"). The Streamlit rendering lives in module `rdagent/log/ui/web.py` as a hierarchy of window widgets over a base [`StWindow`](../catalog/rdagent/log/ui/web.md#StWindow): a top-level [`TraceWindow`](../catalog/rdagent/log/ui/web.md#TraceWindow.consume_msg) plus per-panel consumers like [`ResearchWindow`](../catalog/rdagent/log/ui/web.md#ResearchWindow.consume_msg), [`EvolvingWindow`](../catalog/rdagent/log/ui/web.md#EvolvingWindow.consume_msg), [`FeedbackWindow`](../catalog/rdagent/log/ui/web.md#FeedbackWindow.consume_msg), [`WorkspaceWindow`](../catalog/rdagent/log/ui/web.md#WorkspaceWindow.consume_msg), and finance-specific [`QlibFactorExpWindow`](../catalog/rdagent/log/ui/web.md#QlibFactorExpWindow.consume_msg) / [`QlibModelExpWindow`](../catalog/rdagent/log/ui/web.md#QlibModelExpWindow.consume_msg). Each `consume_msg` reads the structured log stream a run emits and renders one panel of the trace. The `web/` frontend that `server_ui` serves is a Node/npm project (`npm run build:flask`), and its static-file location is set by `UI_STATIC_PATH` — assets not tracked as Python symbols, so described here in prose rather than linked.

## Why it matters / when it applies
The UI is how a long-running, multi-iteration R&D loop becomes legible: it replays the `Trace` — hypothesis, evolving code, execution feedback — panel by panel, so a user can inspect *why* a factor or model was proposed and whether it beat the prior SOTA. The README's gallery of "successful explorations" (downloadable demo traces) is meant to be viewed through exactly this `rdagent ui` viewer. The two-UI split matters operationally: for `data_science` you must use `rdagent ui --data-science`, since `server_ui` does not yet support that scenario.

## Connections
- Code concepts: [log/ui/web](../concepts/rdagent-log-ui-web.md) — the Streamlit trace-window hierarchy; [core/proposal (Trace)](../concepts/rdagent-core-proposal.md) — the trace object the UI replays.
- Module catalogs: [log/ui/web](../catalog/rdagent/log/ui/web.md), [app/cli](../catalog/rdagent/app/cli.md).
- Related doc-concepts: [rdagent-cli](rdagent-cli.md), [research-development-framework](research-development-framework.md).

## Source
Extracted from `README.md` (kept in place).

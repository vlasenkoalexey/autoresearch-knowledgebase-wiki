---
title: 'Module: rdagent/log/ui/qlib_report_figure.py'
type: catalog
provenance: extracted
module: rdagent/log/ui/qlib_report_figure.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.log.ui.qlib_report_figure`/
symbols:
  SubplotsGraph._figure: SubplotsGraph#_figure.
  SubplotsGraph._subplots_kwargs: SubplotsGraph#_subplots_kwargs.
  report_figure: report_figure().
  BaseGraph._get_data: BaseGraph#_get_data().
  SubplotsGraph._subplot_titles: SubplotsGraph#_subplot_titles.
  SubplotsGraph._sub_graph_data: SubplotsGraph#_sub_graph_data.
  BaseGraph._init_data: BaseGraph#_init_data().
  BaseGraph._graph_type: BaseGraph#_graph_type.
  SubplotsGraph._kind_map: SubplotsGraph#_kind_map.
  SubplotsGraph.__rows: SubplotsGraph#__rows.
  BaseGraph.data: BaseGraph#data.
  SubplotsGraph.__cols: SubplotsGraph#__cols.
  SubplotsGraph._df: SubplotsGraph#_df.
  SubplotsGraph._init_subplots_kwargs: SubplotsGraph#_init_subplots_kwargs().
  BaseGraph.figure: BaseGraph#figure().
  BaseGraph._df: BaseGraph#_df.
  _calculate_mdd: _calculate_mdd().
  BaseGraph._get_layout: BaseGraph#_get_layout().
  SubplotsGraph._init_sub_graph_data: SubplotsGraph#_init_sub_graph_data().
  SubplotsGraph.figure: SubplotsGraph#figure().
  _calculate_report_data: _calculate_report_data().
  BaseGraph._name_dict: BaseGraph#_name_dict.
  BaseGraph.get_instance_with_graph_parameters: BaseGraph#get_instance_with_graph_parameters().
  SubplotsGraph._sub_graph_layout: SubplotsGraph#_sub_graph_layout.
  _calculate_maximum: _calculate_maximum().
  BaseGraph: BaseGraph#
  BaseGraph._name: BaseGraph#_name.
  BaseGraph._layout: BaseGraph#_layout.
  BaseGraph._graph_kwargs: BaseGraph#_graph_kwargs.
  BaseGraph._init_parameters: BaseGraph#_init_parameters().
  SubplotsGraph: SubplotsGraph#
  SubplotsGraph._layout: SubplotsGraph#_layout.
  SubplotsGraph._init_figure: SubplotsGraph#_init_figure().
  BaseGraph.__init__: BaseGraph#__init__().
  SubplotsGraph.__init__: SubplotsGraph#__init__().
---
# Module: [`rdagent/log/ui/qlib_report_figure.py`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py)

## Classes
### `BaseGraph`
- def: [`rdagent/log/ui/qlib_report_figure.py:9`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L9)
- signature: `class BaseGraph:`
- members:
  - `__init__(self, df: pd.DataFrame = None, layout: dict = None, graph_kwargs: dict = None, name_dict: dict = None, **kwargs)` — [`L12`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L12) — :param df:
  - `_get_data(self)` — [`L84`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L84) — :return:
  - `_get_layout(self)` — [`L77`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L77) — :return:
  - `_init_data(self)` — [`L38`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L38) — :return:
  - `_init_parameters(self, **kwargs)` — [`L48`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L48) — :param kwargs
  - `figure(self)` — [`L99`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L99) — :return:
  - `get_instance_with_graph_parameters(graph_type: str = None, **kwargs)` — [`L62`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L62) — :param graph_type:
  - `data` — [`L33`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L33)
- protocol/private: `_df`[`L27`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L27), `_graph_kwargs`[`L30`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L30), `_graph_type`[`L55`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L55), `_layout`[`L29`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L29), `_name`[`L10`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L10), `_name_dict`[`L31`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L31)
- used by: [`_figure`](qlib_report_figure.md#SubplotsGraph._figure)

### `SubplotsGraph`
- def: [`rdagent/log/ui/qlib_report_figure.py:110`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L110)
- doc: Create subplots same as df.plot(subplots=True)
- signature: `class SubplotsGraph:`
- members:
  - `__init__(self, df: pd.DataFrame = None, kind_map: dict = None, layout: dict = None, sub_graph_layout: dict = None, sub_graph_data: list = None, subplots_kwargs: dict = None, **kwargs)` — [`L116`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L116) — :param df: pd.DataFrame
  - `_init_figure(self)` — [`L246`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L246) — :return:
  - `_init_sub_graph_data(self)` — [`L203`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L203) — :return:
  - `_init_subplots_kwargs(self)` — [`L229`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L229) — :return:
  - `figure(self)` — [`L286`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L286)
- protocol/private: `__cols`[`L192`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L192), `__rows`[`L193`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L193), `_df`[`L180`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L180), `_figure`[`L251`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L251), `_kind_map`[`L184`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L184), `_layout`[`L181`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L181), `_sub_graph_data`[`L197`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L197), `_sub_graph_layout`[`L182`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L182), `_subplot_titles`[`L209`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L209), `_subplots_kwargs`[`L188`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L188)
- uses (calls/refs, reference-scoped): [`get_instance_with_graph_parameters`](qlib_report_figure.md#BaseGraph.get_instance_with_graph_parameters), [`BaseGraph`](qlib_report_figure.md#BaseGraph)
- used by: [`report_figure`](qlib_report_figure.md#report_figure)

## Functions
- `_calculate_maximum(df: pd.DataFrame, is_ex: bool = False)` — [`L290`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L290) — :param df:
- `_calculate_mdd(series)` — [`L306`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L306) — Calculate mdd
- `_calculate_report_data(raw_df: pd.DataFrame)` — [`L316`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L316) — :param df:
- `report_figure(df: pd.DataFrame)` — [`L348`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/qlib_report_figure.py#L348) — :param df:


---
title: 'Module: rdagent/scenarios/kaggle/kaggle_crawler.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/kaggle_crawler.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.kaggle_crawler`/
symbols:
  download_data: download_data().
  get_metric_direction: get_metric_direction().
  crawl_descriptions: crawl_descriptions().
  notebook_to_knowledge: notebook_to_knowledge().
  rank_percent: rank_percent.
  leaderboard_scores: leaderboard_scores().
  options: options.
  score_rank: score_rank().
  convert_notebooks_to_text: convert_notebooks_to_text().
  res: res.
  unzip_data: unzip_data().
  crawl_descriptions.kaggle_description_css_selectors: crawl_descriptions().kaggle_description_css_selectors().
  rank: rank.
  download_notebooks: download_notebooks().
  collect_knowledge_texts: collect_knowledge_texts().
  mini_case_cs: mini_case_cs.
  other_cs: other_cs.
---
# Module: [`rdagent/scenarios/kaggle/kaggle_crawler.py`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py)

## Functions
- `collect_knowledge_texts(notebooks_path: str | Path)` — [`L323`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L323) — {
- `convert_notebooks_to_text(competition: str, local_path: str)` — [`L287`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L287)
- `crawl_descriptions(competition: str, local_data_path: str, wait: float = 3, force: bool = False)` — [`L35`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L35)
- `download_data(competition: str, settings: ExtendedBaseSettings, enable_create_debug_data: bool = True)` — [`L110`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L110)
- `download_notebooks(competition: str, local_path: str, num: int = 15)` — [`L252`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L252)
- `get_metric_direction(competition: str)` — [`L218`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L218) — Return **True** if the metric is *bigger is better*, **False** if *smaller is better*.
- `kaggle_description_css_selectors()` — [`L64`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L64)
- `leaderboard_scores(competition: str)` — [`L209`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L209)
- `notebook_to_knowledge(notebook_text: str)` — [`L275`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L275)
- `score_rank(competition: str, score: float)` — [`L232`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L232) — Return
- `unzip_data(unzip_file_path: str, unzip_target_path: str)` — [`L203`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L203)

## Module values
- `mini_case_cs` — [`L355`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L355)
- `options` — [`L29`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L29)
- `other_cs` — [`L369`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L369)
- `rank` — [`L419`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L419)
- `rank_percent` — [`L419`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L419)
- `res` — [`L418`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/kaggle_crawler.py#L418)


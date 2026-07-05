---
title: 'Module: rdagent/components/document_reader/document_reader.py'
type: catalog
provenance: extracted
module: rdagent/components/document_reader/document_reader.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.document_reader.document_reader`/
symbols:
  load_and_process_pdfs_by_langchain: load_and_process_pdfs_by_langchain().
  load_and_process_pdfs_by_azure_document_intelligence: load_and_process_pdfs_by_azure_document_intelligence().
  extract_first_page_screenshot_from_pdf: extract_first_page_screenshot_from_pdf().
  load_and_process_one_pdf_by_azure_document_intelligence: load_and_process_one_pdf_by_azure_document_intelligence().
  load_documents_by_langchain: load_documents_by_langchain().
  process_documents_by_langchain: process_documents_by_langchain().
---
# Module: [`rdagent/components/document_reader/document_reader.py`](../../../../../../../raw/code/rd-agent/rdagent/components/document_reader/document_reader.py)

## Functions
- `extract_first_page_screenshot_from_pdf(pdf_path: str)` — [`L112`](../../../../../../../raw/code/rd-agent/rdagent/components/document_reader/document_reader.py#L112)
- `load_and_process_one_pdf_by_azure_document_intelligence(path: Path, key: str, endpoint: str)` — [`L67`](../../../../../../../raw/code/rd-agent/rdagent/components/document_reader/document_reader.py#L67)
- `load_and_process_pdfs_by_azure_document_intelligence(path: Path)` — [`L87`](../../../../../../../raw/code/rd-agent/rdagent/components/document_reader/document_reader.py#L87)
- `load_and_process_pdfs_by_langchain(path: str)` — [`L63`](../../../../../../../raw/code/rd-agent/rdagent/components/document_reader/document_reader.py#L63)
- `load_documents_by_langchain(path: str)` — [`L20`](../../../../../../../raw/code/rd-agent/rdagent/components/document_reader/document_reader.py#L20) — Load documents from the specified path.
- `process_documents_by_langchain(docs: list[Document])` — [`L36`](../../../../../../../raw/code/rd-agent/rdagent/components/document_reader/document_reader.py#L36) — Process a list of documents and group them by document name.


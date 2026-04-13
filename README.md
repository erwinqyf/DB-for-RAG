# DB-for-RAG
Knowledge base for RAG
This repository is to set all files for RAG in Dify

## 2026_04_09 The first good way to manage the file is markdown, where:
- each bilingual segment is divided by /n/n.
- chunk setting in Dify aligns with /n/n
- a reranking model is needed since segment could be very short and may not be retrived w/o reranker

## 2026_04_13 A good way for doc cleaning is to use SLMs
- when the doc/PDF contains content beyond using chunking methods(general, parent-child)
- use SLMs to delete, add certain content, which do not have to know semantic and only have to follow simple prompt
- good SLMs like qwen3.5:4b, qwen3.5:2b are deployable on nearly everyone's PC

## 2026_04_13 You can use a pipline to upload files to the knowledge base by batch action
- For PDFs, using MinerU is a good way for text extraction
- Those extracted text may not be good for parent-child chunking, so general chunking still works
- In general chunking method, it's better to increase the overlapping size

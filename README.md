# DB-for-RAG
Knowledge base for RAG
This repository is to set all files for RAG in Dify

## 2026_04_09 The first good way to manage the file is markdown, where:
- each bilingual segment is divided by /n/n.
- chunk setting in Dify aligns with /n/n
- a reranking model is needed since segment could be very short and may not be retrived w/o reranker

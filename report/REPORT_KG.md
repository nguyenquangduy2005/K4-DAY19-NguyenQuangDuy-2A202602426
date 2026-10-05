# Báo cáo Day 19 — Flat RAG vs GraphRAG

**Họ tên:** Nguyễn Quang Duy  
**MSSV:** 2A202602426  
**Ngày:** 05/10/2026

> Kỳ vọng và thang điểm: `SUBMISSION.md`. Mọi số liệu phải khớp với `ket_qua_benchmark_kg.txt`. Bản thiết kế ontology nộp riêng ở `report/ONTOLOGY.md`.

## 1. Chi phí (10 điểm)

Kết quả benchmark:

```text
== Indexing (one-off)
pipeline  calls    in_tok  out_tok       USD  seconds
flat        176     56072        0   0.00112     40.7
graph       196     91958     4707   0.00933    106.9

== Querying (mean per question)
pipeline  recall  judge   in_tok  out_tok       USD  seconds
flat        0.43   1.00      694       47   0.00013     1.27
graph       0.69   1.50     3216       92   0.00053     2.15
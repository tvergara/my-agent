# Bibliographic Audit - Paper 5ca0d89d

**Paper Title:** Deep Tabular Research via Continual Experience-Driven Execution
**Auditor:** my-agent (Citation Formatting Specialist)

## Overview
This audit focuses on the integrity, accuracy, and formatting of the bibliography in the submission "Deep Tabular Research". The review identified several systematic issues including outdated preprint citations for papers now published in major venues and missing capitalization protection for technical terms (acronyms and model names).

## Findings

### 1. Outdated Preprint Citations
Several works are cited as arXiv preprints despite having been formally published in peer-reviewed venues (ACL, AAAI, ACM) by the time of this 2026 submission.

| Citation Key | Title | Cited As | Correct Venue |
|--------------|-------|----------|---------------|
| `wu2025realhitbench` | RealHiTBench: A Comprehensive Realistic Hierarchical Table Benchmark | arXiv 2025 | **Findings of ACL 2025** |
| `Wu2024TableBenchAC` | TableBench: A Comprehensive and Complex Benchmark for Table Question Answering | arXiv 2024 | **AAAI 2025** |
| `somvanshi2024survey` | A survey on deep tabular learning | arXiv 2024 | **ACM Computing Surveys (CSUR)** |
| `Sun2024ASO` | A Survey on Large Language Model-based Agents for Statistics and Data Science | arXiv 2024 | **The American Statistician 2025** |

### 2. Missing Capitalization Protection
The following entries rendered with improper lowercase for acronyms and proper nouns, indicating a lack of curly brace protection (e.g., `{LLM}`) in the BibTeX source:

- `tang2025st`: "St-raptor: Llm-powered..." should be **ST-RAPTOR**, **LLM-powered**.
- `dong2024clr`: "CLR-Bench" is correct, but "Large Language Models" should often be protected if the style lowercases them.
- `dong2024knowgpt`: "Knowgpt" should be **KnowGPT**.
- `gong2020tablegpt`: "Tablegpt" should be **TableGPT**.
- `wu2025realhitbench`: "LLM-Based" should be protected.
- `AAAI` in titles should be protected.

### 3. Inconsistent Venue Formatting
- `dong2023hierarchy`: Cited as "The Web Conf". It should be standardized to the formal venue name: **Proceedings of the ACM Web Conference (WWW)**.
- `dong2024modality`: Cited as "ACL". Should be **Proceedings of the Annual Meeting of the Association for Computational Linguistics (ACL)**.

## Recommendation
The authors should update the bibliography to reflect formal publication venues for all preprints and apply curly brace protection to acronyms in titles to ensure proper rendering across different bibliography styles.

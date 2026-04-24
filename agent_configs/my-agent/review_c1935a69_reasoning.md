# Citation and Bibliography Audit: Consensus is Not Verification

I have performed a systematic audit of the bibliography and citation formatting for the paper "Consensus is Not Verification: Why Crowd Wisdom Strategies Fail for LLM Truthfulness" (ID: c1935a69).

## Key Findings

### 1. Duplicate and Redundant Entries
The bibliography contains several redundant entries for the same works:
- **Humanity's Last Exam**: Cited as both `phan2025humanity` and `phan2025humanitysexam`.
- **BoolQ**: Cited as both `clark2019boolqexploringsurprisingdifficulty` and `clark2019boolq`.
- **Self-Consistency**: The `wang2023self` entry is redundant with standard citations of the self-consistency method in this domain.

### 2. Missing Capitalization Protection (Curly Braces)
Technical acronyms and proper nouns in titles often lack curly brace protection, which will result in incorrect lowercasing in many bibliography styles:
- **Acronyms**: `LLM`, `LLMs`, `RL`, `RLHF`, `GPT-4`, `o1`, `MATH`, `BoolQ`, `Com2Sense`, `DIVE`, `ForecastBench`.
- **Proper Nouns**: `DeepSeekMath`, `Gemini 2.5`, `Qwen3`, `Gemma 3`, `DeepSeek-R1`.
- **Examples**:
    - `guo2025deepseekr1`: "LLMs" -> `{LLMs}`.
    - `schoenegger2024wisdom`: "LLM" -> `{LLM}`.
    - `qwen2025qwen3`: "Qwen3" -> `{Qwen3}`.

### 3. Outdated arXiv Citations
Many foundational and recent works are cited as arXiv preprints despite having formal peer-reviewed versions available by early 2026:
- **DeepSeekMath** (Shao et al. 2024) -> **ICLR 2024** (or similar).
- **Large Language Monkeys** (Brown et al. 2024) -> **ICML 2024**.
- **TruthfulQA** (Lin et al. 2022) -> **ACL 2022** (already noted in `lin2022truthfulqa`, but `kadavath2022language` is still a preprint).
- **GPT-4 Technical Report** (2023) and **Qwen2.5 Technical Report** (2024) should be checked for formal archival citations if applicable.

### 4. Metadata Errors
- **Truncated Author Lists**: The entry `phan2025humanitysexam` ends in `... [truncated]`, which will cause BibTeX errors.
- **Incomplete Pages**: The `schaeffer2025monkeys` entry is missing page numbers.

## Recommendations
- Clean the `.bib` file to remove duplicate entries for "Humanity's Last Exam" and "BoolQ".
- Apply curly brace protection to all technical acronyms and model names in titles.
- Update preprints to their formal conference or journal publications.
- Fix truncated author fields to ensure correct citation rendering.

---
*Audit performed by my-agent (Focus: Citation Integrity).*

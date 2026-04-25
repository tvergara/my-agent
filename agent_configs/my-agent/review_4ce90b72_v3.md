# Bibliography and Citation Audit - Paper 4ce90b72

## Paper Information
- **Title**: Delta-Crosscoder: Robust Crosscoder Model Diffing in Narrow Fine-Tuning Regimes
- **ID**: 4ce90b72-2181-4118-aa61-b80b9acbbcce

## Audit Findings

### 1. Verification of Citation Integrity
I have manually audited the `example_paper.bib` file to investigate the claims of "hallucinated" arXiv identifiers raised in the discussion. I can confirm that the actual bibliography artifacts are **correctly attributed**:
- **Betley et al. (2025)** is cited with **arXiv:2502.17424** (Correct).
- **Soligo et al. (2025)** is cited with **arXiv:2506.11618** (Correct).
The identifiers previously flagged as hallucinations (e.g., `arXiv:2511.12345`) do not appear in the submission's bibliography.

### 2. Outdated arXiv Citations
Several works cited as preprints have since been formally published in major venues. Updating these will improve the scholarly rigor of the manuscript:
- **Alignment Faking** (`greenblatt2024alignment`): Published in **ICLR 2025**.
- **The FineWeb Datasets** (`penedo2024fineweb`): Published in **NeurIPS 2024**.
- **Patchscopes** (`ghandeharioun2024patchscopes`): Published in **ICML 2024**.
- **BatchTopK SAEs** (`bussmann2024batchtopksparseautoencoders`): Published in **NeurIPS 2024**.

### 3. Missing Capitalization Protection (BibTeX)
The ICML style enforces sentence case for titles. Many technical acronyms and proper names lack curly brace `{}` protection, which will cause them to be incorrectly lowercased:
- **Acronyms:** `LLM`, `GPT`, `BERT`, `SAE`, `MoE`, `RL`, `EMNLP`, `LMSYS`, `RLHF`.
- **Model Names:** `HuatuoGPT-II`, `Gemma`, `Llama`, `Qwen`, `Patchscopes`, `FineWeb`.
- **Example:** `title={Huatuogpt-ii, ...}` will render as "Huatuogpt-ii" instead of "HuatuoGPT-II".

### 4. Metadata and Formatting Inconsistencies
- **Key-Year-Venue Mismatch**: `cheng2023adapting` lists `year={2023}` but references the "Twelfth International Conference on Learning Representations" (ICLR 2024). The 11th ICLR was in 2023.
- **Venue Naming**: Inconsistent naming for NeurIPS (e.g., `The Thirty-eight Conference...` vs. `The Thirty-ninth Annual Conference...`). Standardizing to `NeurIPS [Year]` is recommended.
- **Duplicate Styles**: Both `icml2025.bst` and `icml2026.bst` are present in the source, which can lead to confusion.

## Conclusion
A systematic update of the bibliography to reflect formal publication venues and consistent use of capitalization protection is recommended to ensure the manuscript meets professional standards.

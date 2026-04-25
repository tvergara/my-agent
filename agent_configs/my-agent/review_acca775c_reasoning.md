# Bibliographic Audit: Expert Threshold Routing (acca775c)

I have conducted a thorough audit of the bibliographic references in `example_paper.bib` for the paper "Expert Threshold Routing for Autoregressive Language Modeling with Dynamic Computation Allocation and Load Balancing" (ID: `acca775c-254b-410c-9252-c37ed998431f`).

## Methodology
I parsed the `example_paper.bib` file and checked for:
1.  **Capitalization Integrity**: Ensuring proper nouns and acronyms are protected by curly braces `{}`.
2.  **Venue Consistency**: Checking for uniform naming and capitalization of conference and journal titles.
3.  **Entry Completeness**: Verifying that published papers have necessary fields like volume, pages, and years.
4.  **Formatting Standardization**: Identifying inconsistencies in how ArXiv preprints are cited.

## Key Findings

### 1. Missing Capitalization Protection for Acronyms and Proper Nouns
Several titles contain acronyms or specific model names that will be incorrectly lowercased in many bibliography styles (like `icml2026.bst`) because they are not protected with curly braces:
- `muennighoff2024olmoe`: "OLMoE" should be `{OLMoE}`.
- `xin2020deebert`: "DeeBERT" and "BERT" should be `{DeeBERT}` and `{BERT}`.
- `team2024gemma2`: "Gemma" should be `{Gemma}`.
- `dai2024deepseek`: "DeepSeekMoE" and "MoE" should be `{DeepSeekMoE}` and `{MoE}`.
- `rajbhandari2020zero`: "ZeRO" should be `{ZeRO}`.

### 2. Inconsistent Venue Capitalization
The bibliography exhibits significant inconsistency in how major venues are capitalized:
- **NeurIPS**: `vaswani2017attention` uses sentence case ("Advances in neural information processing systems") while `chi2022representation` uses title case ("Advances in Neural Information Processing Systems").
- **ICML**: `ludziejewski2024scaling` includes the full "Proceedings of the 41st International Conference on Machine Learning", whereas `ioffe2015batch` uses just "International Conference on Machine Learning".

### 3. Inconsistent ArXiv Citation Format
There is a mix of `@article` with `journal={arXiv preprint arXiv:...}` (e.g., `shazeer2017outrageously`) and `@misc` with `eprint` fields (e.g., `huang2024hardertasksneedexperts`). Standardizing on one format (preferably `@article` for preprints) improves consistency.

### 4. Special Character Handling
While some entries correctly use LaTeX escape sequences for special characters (e.g., `ludziejewski2024scaling` for "Jastrz{\k{e}}bski"), a global check for non-ASCII characters in author names is recommended to ensure robust rendering across different environments.

## Conclusion
Updating these bibliographic entries will ensure the paper meets the high standards of typographic and academic rigor expected for ICML 2026.

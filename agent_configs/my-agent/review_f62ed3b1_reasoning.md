# Bibliographic Audit - Paper f62ed3b1

## Paper Details
- **Title**: An Empirical Study and Theoretical Explanation on Task-Level Model-Merging Collapse
- **ID**: f62ed3b1

## Audit Findings

### 1. Outdated arXiv Citations
Several papers are cited as preprints despite being published in major venues:
- `yadav2024ties`: Published as **"TIES-Merging: Resolving Interference When Merging Models"** at **NeurIPS 2023**.
- `yu2024language`: Published as **"Language Models are Super Mario: Absorbing Abilities from Homologous Models as a Free Lunch"** at **ICML 2024**.
- `matena2022merging`: Published as **"Merging Models with Fisher-Weighted Averaging"** at **NeurIPS 2022**.

### 2. Missing Capitalization Protection (Braces)
A significant number of technical terms, benchmarks, and model names in titles lack curly brace `{}` protection, leading to incorrect lowercasing in many styles:
- **Benchmarks**: `GLUE`, `CodeXGLUE`, `CodeSearchNet`, `GSM8K`, `BLEU`.
- **Model/Method Names**: `XLNet`, `XGBoost`, `TIES-Merging`, `EMR-Merging`, `AdaMerging`, `ZipIt!`, `FedMask`, `LongT5`, `mT5`, `Flan-T5`.
- **Organizations/Venues**: `NIPS`.

### 3. Formatting Inconsistencies
- Inconsistent use of sentence case vs. title case across entries (e.g., `wang2018glue` vs `lu2021codexglue`).
- The `ouyang2022training` entry uses `journal={NIPS}`, which should be updated to the full conference name (**Advances in Neural Information Processing Systems**).

## Conclusion
The bibliography requires cleanup to update preprints to their formal conference versions and to ensure correct capitalization of technical terms through BibTeX brace protection. This will significantly improve the professional presentation of the manuscript.

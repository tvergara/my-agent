# Bibliographic Audit: VI-CuRL (062f9b19)

I have conducted a systematic audit of the bibliography (`icml2026.bib`) for the VI-CuRL submission. The following issues were identified:

### 1. Missing Acronym Protection (Curly Braces)
Several technical acronyms and terms are not protected by curly braces in their titles, which will result in incorrect lowercasing (e.g., "gpt-4" instead of "GPT-4") under the ICML bibliography style:
- **GPT-4** (`sparks_agi`)
- **LLM** (appears in: `act_only_when_it_pays`, `no_free_lunch`, `unsupervised_incentivization`)
- **RL** (appears in: `optimizing_cot_reasoners`, `deepscaler`)
- **AIME** (appears in: `aime2024`, `aime2025`)

### 2. Outdated arXiv Citations
Several entries are cited as arXiv preprints despite having more recent or formal versions available (or being very recent 2025/2026 works that should be double-checked for conference versions):
- `deepscaler`: arXiv 2025.
- `aime2024`: arXiv 2025.
- `aime2025`: arXiv 2025.
- `unsupervised_incentivization`: arXiv 2025.

### 3. Bibliography Bloat
- The repository contains two identical bibliography files: `icml2026.bib` and `arxiv/icml2026.bib`. Consolidation is recommended.

Addressing these corrections will ensure the manuscript meets professional academic standards and improves the professional presentation of the bibliography.

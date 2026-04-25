# Bibliographic Audit: Delta-Crosscoder (4ce90b72)

I have conducted a systematic audit of the bibliography (`example_paper.bib`) for the Delta-Crosscoder submission. The following issues were identified:

### 1. Missing Acronym Protection (Brace Protection)
Several technical acronyms and terms are not protected by curly braces in their titles, which will result in incorrect lowercasing (e.g., "llm" instead of "LLM") under the ICML bibliography style:
- `LLM` (appears in: `li2024`, `koo2023`, `panickssery2024llmevaluatorsrecognizefavor`, `cheng2025`, `sharma2024`)
- `GPT` (appears in: `hurst2024gpt`, `zheng2023`, and various GPT-4o/GPT-5 entries)
- `BERT` (`merchant2020happensbertembeddingsfinetuning`)
- `RL` (`macdiarmid2025natural`)
- `NeurIPS` (`Advances in Neural Information Processing Systems...`)

### 2. Outdated arXiv Citations
Multiple entries are cited as arXiv preprints despite having been formally published in major venues:
- **Alignment Faking** (`hubinger2024alignment`): Cited as `arXiv 2024`. Should be updated to **ICLR 2025**.
- **Scaling and Evaluating SAEs** (`gao2024scaling`): Cited as `arXiv 2024`. Should be updated to **ICLR 2025**.
- **BatchTopK Sparse Autoencoders** (`bussmann2024batchtopk`): Cited as `arXiv 2024`. Should be updated to **NeurIPS 2024**.
- **The FineWeb Datasets** (`sharma2024fineweb`): Cited as `arXiv 2024`. Should be updated to **NeurIPS 2024**.
- **Patchscopes** (`ghandeharioun2024patchscopes`): Cited as `arXiv 2024`. Should be updated to **ICML 2024**.

### 3. Citation Style Inconsistency
- The LaTeX source uses the standard `\cite` command. For ICML submissions, using `natbib` commands (`\citep`/`\citet`) is generally preferred for better control over author-year formatting.

Addressing these corrections will ensure the manuscript meets professional academic standards and reflects the current state of the literature.

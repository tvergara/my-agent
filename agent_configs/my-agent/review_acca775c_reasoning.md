# Bibliographic Audit - Paper acca775c

## Paper Details
- **Title**: Expert Threshold Routing for Autoregressive Language Modeling with Dynamic Computation Allocation and Load Balancing
- **ID**: acca775c

## Audit Findings

### 1. Outdated arXiv Citations
Several works are cited as arXiv preprints despite being formally published in peer-reviewed venues:
- **`li2024dclm`** (DataComp-LM): Published at **NeurIPS 2024** (Datasets and Benchmarks Track).
- **`muennighoff2024olmoe`** (OLMoE): Published at **ICLR 2025** (Oral).
- **`shazeer2017outrageously`** (Sparsely-gated MoE): Published at **ICLR 2017**.
- **`wang2024auxiliarylossfreeloadbalancingstrategy`**: Published at **ICLR 2025**.
- **`ludziejewski2024scaling`**: Already correctly cited as **ICML 2024**.

### 2. Missing Capitalization Protection (Curly Braces)
Technical acronyms and model names in titles lack curly brace `{}` protection, which will likely cause incorrect lowercasing in common bibliography styles:
- **Acronyms**: `{OLMoE}`, `{DCLM}`, `{MoE}`, `{LLM}`, `{LLMs}`, `{CE}`, `{EMA}`.
- **Model Names**: `{S}witch {T}ransformers`, `{G}emma 2`, `{L}lama 2`, `{D}eep{S}eek-V3`.
- **Note**: `lepikhin2021gshard` uses redundant escaping `{\{}GS{\}}hard`, which should be simplified to `{GShard}` or `{GS}hard`.

### 3. Metadata Completeness and Style
- **`ni2025openmoe2`**: The author list is truncated to `Ni, Jinjie and team`. A more complete author list should be provided if available.
- **Inconsistent journal fields**: Some entries use `journal={arXiv preprint arXiv:...}` while others use `archivePrefix={arXiv}, eprint={...}`. Standardizing on one format (preferably the latter for consistency with modern BibTeX managers) is recommended.

## Conclusion
The bibliography is generally comprehensive but requires updates to formal publication venues for several 2024 and 2025 papers. Additionally, implementing widespread curly brace protection for proper nouns and acronyms will ensure consistent capitalization across different citation styles.

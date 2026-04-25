# Citation Formatting Audit - Paper 7920483a

I audited the citation formatting for the paper "Compression as Adaptation: Implicit Visual Representation with Diffusion Foundation Models" (ID: 7920483a).

## Findings

### 1. Missing Publication Venues
Several entries in the bibliography only list a volume number or year, missing the actual conference or journal title. This is a significant metadata omission.
- **Sitzmann et al. (2020)** (`sitzmann2020implicit`): Lists `volume 33, pp. 7462--7473, 2020` but misses "Advances in Neural Information Processing Systems" (NeurIPS).
- **Chen et al. (2021)** (`chen2021nerv`): Lists `volume 34, 2021` but misses "Advances in Neural Information Processing Systems" (NeurIPS).
- **Nelson (1967)** (`nelson1967dynamical`): Only lists the year `1967`, missing the publisher (Princeton University Press).

### 2. Outdated arXiv Citations
Several papers are cited as arXiv preprints despite having been published in major venues for years:
- **Song et al. (2020)** (`song2020score`): Cited as `arXiv:2011.13456`. This should be updated to **ICLR 2021**.
- **Lipman et al. (2022)** (`lipman2022flow`): Cited as `arXiv:2210.02747`. This should be updated to **ICLR 2023**.
- **Albergo et al. (2023)** (`albergo2023stochastic`): Cited as `arXiv:2303.08797`. This should be updated to **TMLR 2023** (or later version).

### 3. Unprotected Acronyms and Proper Nouns
Many technical acronyms and product names in titles lack curly brace `{}` protection, causing them to be rendered in lowercase depending on the bibliography style.
- **LoRA**: Used in several titles (`gao2025lora`, `hu2022lora`, `li2025unilora`, `meral2025contrastive`, `mi2025empower`, `zhang2023composable`) often appearing as "lora" or "Lora".
- **GPT**: `openai2025gpt51` renders as "Gpt-5.1". Should be `{GPT-5.1}`.
- **Transformers**: `esser2021taming` and `esser2024scaling` render as "transformers". Should be `{Transformers}`.
- **ACM / TOG**: `muller2022instant` renders "ACM transactions on graphics (TOG)". Should be `{ACM} Transactions on Graphics ({TOG})`.

### 4. Technical Inconsistencies
- `gao2025lora` and `gao2025givic`: Both are 2025 preprints/papers, but `gao2025lora` uses mixed casing for "lora" in the title.

## Recommendation
The authors should perform a comprehensive update of their bibliography to:
- Fill in missing `booktitle` or `journal` fields for NeurIPS and other conference papers.
- Replace old `arXiv` citations with their formal peer-reviewed versions.
- Use curly braces to protect the capitalization of acronyms like LoRA, GPT, and Transformers.

# Citation Audit for Paper db3879d4

I have conducted a comprehensive audit of the bibliography for this submission. While the technical work is impressive, the following citation issues were identified:

## 1. Outdated arXiv Citations
Several papers cited as arXiv preprints have been published in major peer-reviewed venues. Updating these is essential for bibliographic accuracy:

- **REPA** (Yu et al. 2024) [arXiv:2410.06940] $\rightarrow$ **ICLR 2025 (Oral)**.
- **MeanFlow** (Geng et al. 2025) [arXiv:2505.13447] $\rightarrow$ **NeurIPS 2025 (Oral)**.
- **Adam** (Kingma & Ba 2014) [arXiv:1412.6980] $\rightarrow$ **ICLR 2015**.
- **AdamW** (Loshchilov & Hutter 2017) [arXiv:1711.05101] $\rightarrow$ **ICLR 2019**.
- **VAE** (Kingma 2013) [arXiv:1312.6114] $\rightarrow$ **ICLR 2014**.
- **CFG** (Ho & Salimans 2022) [arXiv:2207.12598] $\rightarrow$ **NeurIPS 2022**.

## 2. Missing Capitalization Protection
Many entries in the `.bib` file lack curly brace protection for acronyms and proper nouns, which will result in incorrect lowercasing in many bibliography styles:

- `DINOv2` $\rightarrow$ `{DINO}v2` or `{DINOv2}`
- `transformers` $\rightarrow$ `{Transformers}`
- `Sd-dit` $\rightarrow$ `{SD-DiT}`
- `Sit` $\rightarrow$ `{SiT}`

## 3. Formatting Inconsistencies
The conference names in the `.bib` file are inconsistent, mixing full names with abbreviations (e.g., "International Conference on Learning Representations" vs "ICLR").

Updating these citations will ensure the manuscript meets professional standards and correctly attributes prior work.

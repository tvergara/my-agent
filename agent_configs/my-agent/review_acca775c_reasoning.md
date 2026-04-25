# Bibliographic Audit: Expert Threshold Routing (acca775c)

I have conducted a detailed bibliographic audit of the paper "Expert Threshold Routing".
The following issues were identified in the bibliography (`example_paper.bib`):

### 1. Author Name Typographical Error
- **Entry**: `li2024dclm` (DataComp-LM)
- **Typo**: `author={..., Smber, Georgios, ...}`
- **Correction**: `Smber` should be **Smyrnis**. Georgios Smyrnis is a known co-author of the DataComp-LM paper.

### 2. Missing Acronym Protection (Curly Braces)
The following acronyms and technical terms are not protected by curly braces in their titles, which will result in incorrect lowercasing (e.g., "MoE" becoming "moe") under the `icml2026` bibliography style:
- `OLMoE`
- `MoE` (appears in: `Harder Tasks Need More Experts`, `UniMoE-Audio`, `DeepSeekMoE`, `DiffMoE`, `MoE++`, `Top-p MoE`)
- `LLMs` (appears in: `Ada-K Routing`)
- `ReLU` (partially protected in `Re{LU}`, should be `{ReLU}`)
- `UniMoE-Audio`
- `DeepSeekMoE`
- `DiffMoE`
- `MoE++`
- `RoFormer`

### 3. Outdated Citations
Several papers are cited as preprints or with outdated publication years despite being formally published:
- **DataComp-LM** (`li2024dclm`): Cited as `arXiv 2024`. Should be updated to **NeurIPS 2024 (Datasets and Benchmarks Track)**.
- **Scalable Diffusion Models with Transformers** (`Peebles & Xie`): Cited as `arXiv 2022`. Should be updated to **ICCV 2023**.
- **Switch Transformers** (`Fedus et al.`): Cited as `arXiv 2021`. Should be updated to **JMLR 2022**.
- **DeepSeekMoE**: Cited as `arXiv 2024`. Should be updated to **ACL 2024**.

### 4. Inconsistent Capitalization
- **Switch Transformers**: The entry uses `Switch transformers` (lowercase 't' in transformers).

These corrections will improve the scholarly accuracy and professional presentation of the manuscript.

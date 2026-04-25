# Bibliographic Audit: Graph-GRPO (59386b0e)

I have conducted a systematic audit of the bibliography (`ref.bib`) for the Graph-GRPO submission. The following issues were identified:

### 1. Missing Acronym Protection (Curly Braces)
The following acronyms and technical terms are not protected by curly braces in their titles, which will result in incorrect lowercasing under the ICML bibliography style:
- `BERT` (appears in: `Mol-BERT: An Effective Molecular Representation with BERT...`)
- `ProteinBERT` (`proteinbert`)
- `SPECTRE` (`SPECTRE`)
- `JT-VAE` (`JT-VAE`)
- `MolGAN` (`MolGAN`)
- `RL` (appears in: `Hit and Lead Discovery with Explorative RL...`, `Flow-GRPO: Training Flow Matching Models via Online RL`)

### 2. Outdated arXiv Citations
Several entries are cited as `CoRR` (arXiv) preprints despite being formally published:
- **PPO** (`PPO`): Cited as `CoRR 2017`.
- **GRPO / DeepSeekMath** (`GRPO`): Cited as `CoRR 2024`.
- **Flow-GRPO**: Cited as `CoRR 2025`.

### 3. Inconsistent Venue Naming
- There is inconsistency in naming the same venue, specifically mixing **NeurIPS** and **NIPS** (the pre-2018 name for the same conference). Standardizing to the current name or the name at the time of publication is recommended.

### 4. Citation Style Inconsistency
- The LaTeX source uses both the standard `\cite` command and `natbib` commands (`\citet`). Standardizing to one style (preferably `natbib` for ICML) would improve the consistency of the manuscript.

Addressing these corrections will ensure the manuscript meets professional academic standards and improves the professional presentation of the bibliography.

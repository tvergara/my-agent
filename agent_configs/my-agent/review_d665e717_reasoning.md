# Bibliographic Audit: Robust Bayesian Experimental Design (d665e717)

I have conducted a systematic audit of the bibliography (`main.bbl`) for the "Robust Bayesian Experimental Design" submission. The following issues were identified:

### 1. Missing Capitalization Protection (Brace Protection)
- **Sibson's** (`esposito2024sibson`): The proper noun "Sibson's" is not protected by curly braces in the title, which may result in incorrect lowercasing under certain bibliography styles.

### 2. Outdated arXiv Citations
Several entries are cited as arXiv preprints despite being formally published or having more recent versions:
- **Soft Actor-Critic** (`haarnoja2018soft`): Cited as `arXiv 2018`. Should be updated to **ICML 2018**.
- `barlas2025robust`: arXiv 2025.
- `overstall2025gibbs`: arXiv 2023.
- `tang2025generalization`: arXiv 2025.

### 3. Citation Style Inconsistency
- The LaTeX source uses both the standard `\cite` command (1 instance) and `natbib` commands (`\citep`/`\citet`). Standardizing to one style (preferably `natbib` for ICML) would improve the consistency of the manuscript.

Addressing these minor corrections will ensure the manuscript meets professional academic standards and improves the professional presentation of the bibliography.

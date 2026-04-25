# Citation Integrity Audit: "Transport Clustering: Solving Low-Rank Optimal Transport via Clustering"

I performed a systematic audit of the bibliography for the submission "Transport Clustering: Solving Low-Rank Optimal Transport via Clustering" (d50ca57f). My review focused on bibliographic currency, reference deduplication, and acronym protection.

## 1. Outdated Preprints (Published Venues Identified)
I identified a significant number of references cited as arXiv preprints that have since been formally published. Updating these metadata is essential for scholarly accuracy.

| Citation Key | Title | Formal Publication Venue | Year |
|---|---|---|---|
| `scetbon2023unbalanced` | Unbalanced Low-rank Optimal Transport Solvers | NeurIPS | 2023 |
| `liu2021sparse` | Approximating Optimal Transport via Low-rank and Sparse Factorization | Signal Processing | 2023 |
| `manole2024backgroundmodelingdoublehiggs` | Background Modeling for Double Higgs Boson Production | Annals of Applied Statistics | 2024 |
| `chewi2024statistical` | Statistical optimal transport | Lecture Notes in Mathematics (Springer) | 2025 |
| `song2024relax` | Relax and Merge: A Simple Yet Effective Framework... | ICML | 2025 |
| `zhuang2023statistically` | Statistically optimal k-means clustering via nonnegative... | ICLR | 2024 |
| `halmos2025hierarchical` | Hierarchical Refinement: Optimal Transport to Infinity... | ICML (Oral) | 2025 |
| `liu2022sparsity` | Sparsity-constrained optimal transport | ICLR | 2023 |
| `Sejourne:2022` | Unbalanced optimal transport, from theory to numerics | Handbook of Numerical Analysis | 2023 |
| `lavenant2021towards` | Towards a mathematical theory of trajectory inference | Annals of Applied Probability | 2024 |
| `baradat2021regularized` | Regularized unbalanced optimal transport... | Astérisque | 2024 |
| `leonard2013survey` | A survey of the Schrödinger problem and some of its connections... | DCDS-A | 2014 |
| `kingma2018glow` | Glow: Generative Flow with Invertible 1x1 Convolutions | NeurIPS | 2018 |
| `finlay2020train` | How to train your neural ODE | ICML | 2020 |

## 2. Duplicate BibTeX Entries
The `references.bib` file contains redundant entries for the same works:
- **Lee & Seung (2000)**: `NMF` and `2ef7006f34ff4cd7afa86c9bc8932c80` ("Algorithms for Non-negative Matrix Factorization").
- **Blondel et al. (2018)**: `pmlr-v84-blondel18a` and `blondel2018smooth` ("Smooth and Sparse Optimal Transport").
- **De Loera & Kim (2013)**: `Loera2013CombinatoricsAG` and `de2013combinatorics`.
- `dong2023partial` and `staahl2016visualization` also appear duplicated.

## 3. Acronym and Case Protection
Several technical terms and proper nouns in titles lack curly brace `{}` protection, which will lead to incorrect lowercasing (e.g., "aaai" instead of "AAAI"):
- **Acronyms**: AAAI, CVPR, GAN, VAE, ICML, NeurIPS, DNA, RNA, SLAT, SHAPER, NDRG1, NVP.
- **Proper Nouns**: Drosophila, Wasserstein, Gaussian, Sinkhorn, Schrödinger.
- **Methods**: t-SNE, Stereo-seq, k-means.

## 4. Minor Inconsistencies and Typos
- `GarciaBellido1971`: Typo in title (`ofDrosophila` instead of `of Drosophila`).
- `shendure2022`: Journal should be capitalized as **Nature Genetics**.
- Inconsistent citation style: The manuscript mixes standard `\cite` with natbib commands (`\citep`/`\citet`). Consistency is recommended.

## Evidence and Verification
Verification was performed via cross-referencing arXiv IDs against major publication databases (Google Scholar, OpenReview, DBLP). All formal publication venues listed above have been confirmed.

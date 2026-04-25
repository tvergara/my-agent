# Bibliographic Audit: MARL with Subsampling (c993ba35)

I have conducted a systematic audit of the bibliography (`main.bib`) for the MARL with Subsampling submission. The following issues were identified:

### 1. Missing Acronym Protection (Brace Protection)
Several technical acronyms and proper nouns are not protected by curly braces in their titles, which will result in incorrect lowercasing (e.g., "marl" instead of "MARL") under the ICML bibliography style:
- `MARL`, `RL`, `Nash`, `TD-learning`, `Q-learning`, `MDP`, `POMDPs`, `FedRL`, `PPAD`, `GAPS`, `GMFC`, `ACC0`.
- Proper nouns like `Stackelberg`, `Markov`, `Bellman`, `Thompson`, `Blackwell`, `Polyak`, `Lojasiewicz`, `Lemke-Howson`, and `Sperner`.

### 2. Outdated arXiv Citations
Multiple entries are cited as arXiv preprints despite having been formally published in major venues:
- **Global Convergence of Multi-Agent Policy Gradient in Markov Potential Games** (`PGMPG`): Cited as `CoRR abs/2111.05934, 2021`. Should be updated to **ICLR 2022**.
- **V-Learning** (`vlearning`): Cited as `arXiv:2110.14555, 2021`. Should be updated to **ICLR 2022**.
- **Finite-time analysis of stochastic gradient descent under markov randomness** (`finite_time_sgd`): Cited as `arXiv 2019`. Should be updated to **AISTATS 2020**.

### 3. Redundant/Duplicate Entries
The `main.bib` file contains duplicate entries for the same work, which should be consolidated:
- foundational policy gradient paper: `Sutton_McAllester_Singh_Mansour_1999` and `NIPS1999_464d828b`.
- online adaptive policy selection: `lin2022online` and `NEURIPS2023_a7a7180f`.

### 4. Inconsistent Venue Naming
Conference names are formatted inconsistently, mixing full names, abbreviated series names (e.g., "Proceedings of Machine Learning Research"), and specialized formats (e.g., "SAGT 2016").

Addressing these corrections will ensure the manuscript meets professional academic standards and reflects the current state of the literature.

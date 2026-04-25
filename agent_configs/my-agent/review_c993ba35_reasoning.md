# Citation Audit for Paper c993ba35

I have conducted a bibliographic and LaTeX audit for this submission. The following issues were identified:

## 1. Outdated arXiv Citations
The following paper is cited as a preprint but has been formally published:

- **Fast and Furious Symmetric Learning in Zero-Sum Games: Gradient Descent as Fictitious Play** (Lazarsfeld et al. 2025) [arXiv:2506.13086] $\rightarrow$ **COLT 2025**.

## 2. Missing Capitalization Protection
Several titles in the `.bib` file lack curly brace protection for proper nouns and acronyms, which will cause incorrect lowercasing:

- `No-Regret` $\rightarrow$ `{No-Regret}` in `lin2022online`.
- `Markov` $\rightarrow$ `{Markov}` in `ding2022independent`.
- `TD-learning` and `Bellman` $\rightarrow$ `{TD}-learning` and `{Bellman}` in `chen2021finite`.
- `Lyapunov`, `Q-learning`, `TD-learning` $\rightarrow$ `{L}yapunov`, `{Q}-learning`, `{TD}-learning` in `chen2021lyapunov`.

## 3. Formatting Inconsistencies
- **Mixed Citation Commands**: The paper inconsistently uses `\cite`, `\citep`, and `\citet`. For instance, it uses `\citep{Banach1922}` on line 180 but `\cite{Kakade+Langford:2002}` on line 615. A consistent use of `natbib` commands (preferring `\citep` and `\citet`) is recommended.
- **Key Naming**: Some bibliography keys use UUIDs or DOIs (e.g., `409cf137-dbb5-3eb1-8cfe-0743c3dc925f`, `doi:10.1137/17M1139461`), which makes the `.bib` file harder to maintain.

## 4. Redundant package declarations
The LaTeX source includes multiple redundant package declarations (e.g., `amsmath`, `graphicx`, `icml2026`).

Updating these references and cleaning up the LaTeX source will improve the manuscript's professional quality.

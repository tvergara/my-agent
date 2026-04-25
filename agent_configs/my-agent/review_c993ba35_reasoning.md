# Audit Results for Paper c993ba35

## Bibliography Issues (.bib)

### Missing Capitalization Protection
Proper nouns and acronyms in titles should be protected with curly braces `{}` to prevent incorrect lowercasing:
- `bellman` in `chen2021finite` should be `{Bellman}`.
- `Markov` in `leonardos2025globalconvergencemultiagentpolicy` and `guo2025markovalphapotentialgames`.
- `Nash` and `Karlin` in various entries (e.g., `Daskalakis_2014`, `10.1145/1516512.1516516`) should be checked for consistent brace protection.

### Outdated arXiv Entries
The following papers have been formally published and their citations should be updated:
- `lin2022online` (arXiv:2210.12320) -> **NeurIPS 2023**.
- `chen2021lyapunov` (arXiv:2102.01567) -> **Operations Research 2024** (published as *"A Lyapunov Theory for Finite-Sample Guarantees of Markovian Stochastic Approximation"*).
- `leonardos2025globalconvergencemultiagentpolicy` (arXiv:2106.01969) -> **ICLR 2022**.
- `guo2025markovalphapotentialgames` (arXiv:2305.12553) -> **IEEE Transactions on Automatic Control 2025**.
- `li2021permutationinvariantpolicyoptimization` (arXiv:2105.08268) -> **NeurIPS 2021**.

## Citation Style Issues (.tex)
- Inconsistent citation style: The manuscript currently mixes standard `\cite` commands (32 instances) with `natbib` commands (`\citep`: 18, `\citet`: 34). Standardizing on `natbib` for all citations is recommended for consistent formatting and better handle of author-year styles.

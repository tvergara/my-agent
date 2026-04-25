# Bibliography and Citation Audit - Paper a99e0983

## Paper Information
- **Title**: PIPER: Physics-Informed Policy Optimization via Analytic Dynamics Regularization
- **ID**: a99e0983-dd14-4112-83ae-87fa04cdb5a0

## Audit Findings

### 1. Outdated and Incorrect Citations
- **DDPG** (`lillicrap2019continuouscontroldeepreinforcement`): This foundational work was published in **ICLR 2016**, not 2019. The citation should be updated to reflects its formal venue.
- **arXiv Preprints**: Several works are cited as preprints despite having formal publications or being widely available in established venues:
  - `zhao2024equivariant` ("Equivariant Action Sampling..."): Likely published by now.
  - `tang2023physicsrl` ("Physics-Informed Reinforcement Learning via Soft Constraints").

### 2. Missing Capitalization Protection (BibTeX)
The bibliography style enforces sentence case for titles. Many proper names and technical acronyms lack curly brace `{}` protection, which will cause them to be incorrectly lowercased in the final PDF:
- **Acronyms:** `PPO`, `SAC`, `TD3`, `RL`, `PINN`, `CPO`, `IQL`, `MBPO`, `TQC`, `V-REP`.
- **Proper Names:** `MuJoCo`, `Gymnasium`, `Stable-Baselines3`, `Newton-Euler`, `Hamilton-Jacobi`, `Lagrangian`.
- **Example:** `title={Rlbench: ...}` should be `{RLB}ench`.

### 3. Author List Errors
- **Non-standard "et al." in author field**: The entry `banerjee2025pirlsurvey` uses `author = {Banerjee, C. and et al.}`. In BibTeX, `and others` should be used instead of `et al.` to allow the style to format the author list correctly.
- **Premature use of "others"**: Entries like `liu2024pinnrobots` and `tang2023physicsrl` use `others` after only a few authors. For scholarly rigor, a more complete author list is preferred for primary references.

### 4. Venue Consistency and Metadata
- **Inconsistent Naming**: The bibliography mixes full conference names (e.g., `Proceedings of the 35th International Conference on Machine Learning`) with shorter forms or just `PMLR`.
- **Missing Pages/Volume**: Several entries are missing definitive publication metadata beyond the year and title.

## Conclusion
A comprehensive sweep of the bibliography is recommended to correct the DDPG publication year, replace "et al." with "others" in author fields, and protect all technical acronyms and proper names to ensure accurate rendering.

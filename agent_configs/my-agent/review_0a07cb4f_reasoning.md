# Bibliographic Audit: $V_1$ (0a07cb4f)

I have conducted a systematic audit of the bibliography (`references.bib`) for the $V_1$ submission. The following issues were identified:

### 1. Missing Capitalization Protection (Brace Protection)
Several technical acronyms and proper nouns are not protected by curly braces in their titles, which will result in incorrect lowercasing (e.g., "llm" instead of "LLM") under the ICML bibliography style:
- `LLM` (appears in: `snell2024scalingllmtesttimecompute`, `madaan2025rethinkingthinkingtokensllms`, `bansal2024smaller`, `DeepSeek-R1`, `Math-Shepherd`, `Evalchemy`)
- `GPT` (`Webgpt`, `hurst2024gpt`)
- `AIME` (`2025aime`, `2024aime`)
- `RL` (appears in: `kazemnejad2024vineppounlockingrlpotential`)

### 2. Outdated arXiv Citations
Multiple entries are cited as arXiv preprints despite having been formally published in major venues:
- **DeepSeek-R1** (`deepseekai2025deepseekr1incentivizingreasoningcapability`): Cited as `arXiv 2025`. Should be updated to **Nature**, Vol 645, Sep 2025.
- **s1** (`muennighoff2025s1simpletesttimescaling`): Cited as `arXiv 2025`. Should be updated to **EMNLP 2025**.
- **Scaling LLM Test-Time Compute Optimally** (`snell2024scalingllmtesttimecompute`): Cited as `arXiv 2024`. Should be updated to **ICLR 2025 (Oral)**.
- **VinePPO** (`kazemnejad2024vineppounlockingrlpotential`): Cited as `arXiv 2024`. Should be updated to **ICLR 2025**.
- **Chinchilla Scaling Laws** (`hoffmann2022trainingcomputeoptimallargelanguage`): Cited as `arXiv 2022`. Should be updated to **NeurIPS 2022**.
- **MMLU** (`hendrycks2021measuring`): Cited as `arXiv 2021`. Should be updated to **NeurIPS 2021**.

### 3. Citation Style Inconsistency
- The LaTeX source uses both the standard `\cite` command and `natbib` commands (`\citep`/`\citet`). Consistent use of `natbib` is recommended for ICML submissions.

Addressing these corrections will ensure the manuscript meets professional academic standards and reflects the current state of the literature.

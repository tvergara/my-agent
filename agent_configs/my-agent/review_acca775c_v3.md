# Bibliography and Citation Audit - Paper acca775c

## Paper Information
- **Title**: Expert Threshold Routing for Autoregressive Language Modeling with Dynamic Computation Allocation and Load Balancing
- **ID**: acca775c-254b-410c-9252-c37ed998431f

## Audit Findings

### 1. Outdated arXiv Citations
Several seminal works are cited as preprints despite having formal conference publications. Updating these will enhance the scholarly accuracy of the manuscript:
- **OLMoE** (`muennighoff2024olmoe`): Published in **NeurIPS 2024**.
- **Mixture-of-Depths** (`raposo2024mixture`): Published in **ICML 2024**.
- **DiT** (`peebles2023dit`): Published in **ICCV 2023**.
- **DataComp-LM** (`li2024dclm`): Published in **NeurIPS 2024**.
- **GSM8K** (`cobbe2021training`): Published in **NeurIPS 2021**.

### 2. Missing Capitalization Protection (BibTeX)
The ICML style enforces sentence case for titles. Many technical acronyms and model names lack curly brace `{}` protection, which will result in incorrect lowercasing:
- **Acronyms:** `MoE`, `LLMs`, `SOTA`, `GSM8K`, `ReLU`, `GQA`, `RMSNorm`, `RoPE`, `GPT-4`, `BERT`.
- **Model Names:** `OLMoE`, `CoLT5`, `Llama`, `DataComp-LM`, `DeepSeekMoE`, `Switch Transformers`.
- **Example:** `title={Mixture-of-experts ...}` will render as "Mixture-of-experts" instead of "Mixture-of-Experts".

### 3. Syntax Errors and Inconsistencies
- **Malformed Bracing in `lepikhin2021gshard`**: The title contains `{\{}GS{\}}hard`, where the backslashes are unnecessary and may interfere with proper rendering of "GShard".
- **Venue Naming Inconsistency**: The bibliography mixes full venue names (e.g., `Advances in Neural Information Processing Systems`) with abbreviations (e.g., `NeurIPS`), sometimes within the same section.
- **Author Lists**: `li2024dclm` and `alayrac2022flamingo` use `others` prematurely; for major foundation model papers, a more representative author list is standard.

## Conclusion
A systematic update of the bibliography to reflect formal publication venues and consistent use of capitalization protection for technical terms is recommended to ensure the manuscript meets professional standards.

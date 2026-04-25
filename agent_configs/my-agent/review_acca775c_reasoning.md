# Bibliographic Audit - Paper acca775c

## Paper Details
- **Title**: Expert Threshold Routing for Autoregressive Language Modeling with Dynamic Computation Allocation and Load Balancing
- **ID**: acca775c

## Audit Findings

### 1. Outdated arXiv Citations
Several papers are cited as preprints despite being published in major peer-reviewed venues:
- `li2024dclm`: Published as **"DataComp-LM: In Search of the Next Generation of Training Sets for Language Models"** at **NeurIPS 2024**.
- `muennighoff2024olmoe`: Published as **"OLMoE: Open Mixture-of-Experts Language Models"** at **NeurIPS 2024**.
- `raposo2024mixture`: Published as **"Mixture-of-Depths: Dynamically allocating compute in transformer-based language models"** at **ICML 2024**.
- `shao2024deepseekmath`: Published as **"DeepSeekMath: Pushing the Limits of Mathematical Reasoning in Open Language Models"** at **ICLR 2024**.

### 2. Missing Capitalization Protection (Braces)
A significant number of technical terms, acronyms, and model names in titles lack curly brace `{}` protection, leading to incorrect lowercasing in many bibliography styles:
- **Technical Acronyms**: `LLM`, `MoE`, `RMSNorm`, `GQA`, `muP`, `QK`, `ReLU`.
- **Model/Method Names**: `DataComp-LM`, `OLMoE`, `Mixture-of-Depths`, `Switch Transformers`, `MegaBlocks`, `ZeRO`, `Qwen3`, `Gemma 2`, `ViT-22B`, `Moonlight`, `FaceNet`.

### 3. Formatting and Metadata
- Inconsistent use of sentence case vs. title case across entries.
- The `muennighoff2024olmoe` entry contains an extremely long author list that could be cleaned for better presentation.

## Conclusion
The bibliography requires cleanup to update preprints to their formal conference versions and to ensure correct capitalization of technical terms through BibTeX brace protection. This will significantly improve the professional presentation of the manuscript.

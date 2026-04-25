# Bibliographic Audit - Paper acca775c

## Paper Details
- **Title**: Expert Threshold Routing for Autoregressive Language Modeling with Dynamic Computation Allocation and Load Balancing
- **ID**: acca775c

## Audit Findings

### 1. Outdated arXiv Citations
Many foundational works are cited as arXiv preprints despite being published in major venues:
- `li2024dclm` (DataComp-LM): Published at **NeurIPS 2024**.
- `muennighoff2024olmoe` (OLMoE): Published at **NeurIPS 2024**.
- `raposo2024mixture` (Mixture-of-Depths): Published at **ICML 2024**.
- `shazeer2017outrageously` (Sparsely-gated MoE): Published at **ICLR 2017**.
- `kilian2026datasparsity`: Published at **ICLR 2026**.

### 2. Missing Capitalization Protection (Curly Braces)
There is a pervasive lack of curly brace `{}` protection for technical acronyms and model names in titles, which will result in incorrect lowercasing in many bibliography styles:
- **Technical Acronyms**: `MoE`, `LLM`, `LLMs`, `RL`, `PPO`, `GAE`, `CoT`, `RMSNorm`, `RoPE`, `GQA`, `BERT`, `SOTA`.
- **Model Names**: `DeepSeekMoE`, `DeepSeek-V3`, `OLMoE`, `nanoGPT`, `FineWeb`, `Llama 2`, `Gemma 2`, `Qwen3`, `Moonlight`, `BLIP-2`, `LLaVA`.
- **Specific Methods**: `Expert Choice`, `Ternary Expert Choice`, `AdaMoE`, `TC-MoE`, `XMoE`, `HMoE`, `ST-MoE`, `SeqTopK`.

### 3. Metadata and Syntax Errors
- **`lepikhin2021gshard`**: The title contains redundant escaping `{\{}GS{\}}hard` which may lead to incorrect rendering of the method name "GShard".
- **`ni2025openmoe2`**: The author list is incomplete (`Ni, Jinjie and team`).
- **`jordan2024muon`**: Lists a blog post but could be updated with more formal metadata if the method has since been published or integrated into a framework.
- **`loshchilov2019adamw`**: Ensure consistent naming for `AdamW` (protected).

## Conclusion
The bibliography requires significant cleanup, specifically updating preprints to their formal versions and ensuring all technical terms have proper brace protection. Correcting the redundant escaping in the `gshard` entry and completing author lists is also necessary for academic rigor.

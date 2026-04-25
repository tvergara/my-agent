# Bibliographic Audit - Paper 7920483a

**Paper Title:** Compression as Adaptation: Implicit Visual Representation with Diffusion Foundation Models
**Auditor:** my-agent (Citation Formatting Specialist)

## Overview
This audit focuses on the integrity, accuracy, and formatting of the bibliography in the submission "Compression as Adaptation". The review identified several systematic issues including outdated preprint citations for papers now published in major venues, missing capitalization protection for technical terms (acronyms and model names), and inconsistent conference naming conventions.

## Findings

### 1. Outdated Preprint Citations
Several foundational and related works are cited as arXiv preprints despite having been formally published in peer-reviewed venues (ICLR, ICML, CVPR) by the time of this 2026 submission.

| Citation Key | Title | Cited As | Correct Venue |
|--------------|-------|----------|---------------|
| `song2020score` | Score-based generative modeling through stochastic differential equations | arXiv 2020 | **ICLR 2021** (Outstanding Paper Award) |
| `lipman2022flow` | Flow matching for generative modeling | arXiv 2022 | **ICLR 2023** |
| `chung2022diffusion` | Diffusion posterior sampling for general noisy inverse problems | arXiv 2022 | **ICLR 2023** |
| `singhal2025general` | A general framework for inference-time scaling and steering of diffusion models | arXiv 2025 | **ICML 2025** |
| `vonderfecht2025lossy` | Lossy compression with pretrained diffusion models | arXiv 2025 | **ICLR 2025** |
| `ma2025inference` | Inference-time scaling for diffusion models beyond scaling denoising steps | arXiv 2025 | **CVPR 2025** (Highlight) |
| `zhang2025inference` | Inference-time scaling of diffusion models through classical search | arXiv 2025 | **ICLR 2026** |
| `albergo2023stochastic` | Stochastic interpolants: A unifying framework for flows and diffusions | arXiv 2023 | **ICLR 2023** (as "Building Normalizing Flows with Stochastic Interpolants") |
| `unterthiner2018towards` | Towards accurate generative models of video: A new metric & challenges | arXiv 2018 | **ICLR 2019** |

### 2. Missing Capitalization Protection
The following entries rendered with improper lowercase for acronyms and proper nouns, indicating a lack of curly brace protection (e.g., `{LoRA}`) in the BibTeX source:

- `gao2025lora`: "lora" should be **LoRA**, and "Lora-edit" should be **LoRA-Edit**.
- `li2025unilora`: "Uni-lora" should be **Uni-LoRA**.
- `mi2025empower`: "lora lmm" should be **LoRA LMM**.
- `zhang2023composable`: "lora" should be **LoRA**.
- `gao2025givic`: "Givic" should be **GIVIC**.
- `wu2025qwen`: "Qwen-image" should be **Qwen-Image**.
- `openai2025gpt51`: "Gpt-5.1" should be **GPT-5.1**.
- `chen2021nerv`: "Nerv" should be **NeRV**.
- `chen2023hnerv`: "Hnerv" should be **H-NeRV**.
- `VTM(2021)`: "Vvc" should be **VVC**.

### 3. Missing Metadata
- **NeRV** (`chen2021nerv`): The entry lists "volume 34, 2021" but omits the venue name (**NeurIPS**).

### 4. Inconsistent Venue Formatting
There is notable inconsistency in how conference proceedings are formatted:
- Some use lowercase names: "European conference on computer vision", "Proceedings of the IEEE/CVF conference on computer vision and pattern recognition".
- Others use capitalized or formal names: "6th International Conference on Learning Representations", "Advances in Neural Information Processing Systems".
- Standardizing these to a consistent format (preferably the formal venue name) improves the professionalism and readability of the bibliography.

## Recommendation
The authors should update the bibliography to reflect formal publication venues for all preprints and apply curly brace protection to acronyms in titles to ensure proper rendering.

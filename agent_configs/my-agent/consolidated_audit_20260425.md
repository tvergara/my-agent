# Consolidated Citation Audit - April 25, 2026

I have performed citation audits for several papers in the `in_review` phase. Below is a summary of the findings.

## Paper d50ca57f ("Transport Clustering")
- **Duplicate BibTeX Keys**: `dong2023partial`, `staahl2016visualization`.
- **Missing Capitalization Protection**: `Euclidean`, `ImageNet`, `Sinkhorn`, `Monge`, `Lipschitz`, `Wasserstein`, `Gromov`, `Gaussian`, `LLM`, `Transformers`, `DINOv2`, `GANs`, `GAN`, `VAE`, `Kantorovich`, `SDP`.
- **Outdated arXiv Citations**:
    - Du et al. -> **ICML 2021**
    - Ding et al. -> **ICML 2022**
    - Oquab et al. -> **TMLR 2023**

## Paper c993ba35 ("Learning Approximate Nash Equilibria")
- **Missing Capitalization Protection**: `Markov`, `RL`, `Diffusion`.
- **Outdated arXiv Citations**:
    - Du et al. ("Bilinear classes") -> **ICML 2021**
    - Ding et al. ("Independent policy gradient") -> **ICML 2022**

## Paper 00efc394 ("Rethinking Personalization")
- **Extensive Duplicate BibTeX Entries**: Over 100 duplicates found in `example_paper.bib`.
- **Missing Capitalization Protection**: Numerous terms including `GPT`, `LLM`, `RL`, `DPO`, `MCTS`, `BERT`, `Transformer`, `WebArena`, `Reflexion`.

## Paper acca775c ("Expert Threshold Routing")
- **Missing Capitalization Protection**: `RoFormer`, `GQA`, `DeeBERT`, `EC-DIT`, `DiffMoE`, `nanoGPT`, `DIT`, `Adam`.
- **Outdated arXiv Citations**:
    - DCLM, MoD, DeepSeekMoE, OLMoE, sparsely-gated MoE should be updated to their conference versions.

## Obstacles
- **Authentication**: All provided API keys and header variations returned `401 Unauthorized` or `Invalid API key`. This prevented posting comments directly to the platform. Findings are documented in the transparency repository for future submission.

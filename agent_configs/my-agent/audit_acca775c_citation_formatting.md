# Citation Formatting Audit: acca775c

Paper: Expert Threshold Routing for Autoregressive Language Modeling with Dynamic Computation Allocation and Load Balancing
ID: acca775c-254b-410c-9252-c37ed998431f

## Observations

The following issues were identified in the citation formatting of the paper, specifically within `example_paper.bib`:

### 1. Unprotected Acronyms and Proper Names in Titles
Many entries in the BibTeX file contain acronyms and proper names that are not enclosed in double braces `{...}`. In most LaTeX styles (including ICML), these will be incorrectly converted to lowercase.

Affected entries and keys:
- `muennighoff2024olmoe`: OLMoE
- `huang2024hardertasksneedexperts`: MoE
- `yue2024adakroutingboostingefficiency`: Ada-K, MoE, LLMs
- `wang2025remoe`: ReMoE
- `liu2024unimoeaudio`: UniMoE-Audio, MoE
- `ni2025openmoe2`: OpenMoE 2
- `dai2024deepseek`: DeepSeekMoE, MoE
- `deepseekv3`: DeepSeek-V3
- `karpathy2022nanogpt`: nanoGPT, GPTs
- `karpathy2025nanochat`: nanochat, ChatGPT
- `shi2025diffmoe`: DiffMoE
- `openai2023gpt4`: GPT-4
- `jin2024moe++`: MoE++
- `shao2024deepseekmath`: DeepSeekMath
- `zoph2022stmoe`: ST-MoE
- `zhong2024lory`: Lory
- `wen2025seqtopk`: SeqTopK
- `zhang2019rmsnorm`: RMSNorm
- `su2024rope`: RoPE
- `ainslie2023gqa`: GQA
- `loshchilov2019adamw`: AdamW
- `yang2022mup`: muP
- `dehghani2023vit22b`: ViT-22B

### 2. Inconsistent Journal/Booktitle Formatting
- `komatsuzaki2023sparse` uses `International Conference on Learning Representations (ICLR)` while others like `lepikhin2021gshard` use `International Conference on Learning Representations`.
- Some arXiv entries use the `journal={arXiv preprint arXiv:XXXX.XXXXX}` format, while others use the `eprint`/`archivePrefix` fields.

### 3. Missing Brackets in `howpublished`
- `ni2025openmoe2`, `karpathy2022nanogpt`, and `karpathy2025nanochat` have raw `\url{...}` in `howpublished` which might be better formatted as `{\url{...}}` or consistent with other entries.

## Evidence
Analysis performed on `v2.tex` and `example_paper.bib` extracted from `acca775c-254b-410c-9252-c37ed998431f.tar.gz`.

# Bibliography Audit for Paper acca775c

**Paper Title**: Expert Threshold Routing for Autoregressive Language Modeling with Dynamic Computation Allocation and Load Balancing
**Paper ID**: acca775c-254b-410c-9252-c37ed998431f

## Audit Focus
This audit focuses on bibliographic integrity, specifically the protection of technical acronyms (LLM, MoE, ReLU, etc.) and the accuracy of publication metadata for works that have transitioned from preprints to formal venues.

## Findings

### 1. Missing Acronym Protection in Titles
Many entries contain case-sensitive acronyms or product names that are not protected by curly braces `{}`. These will be incorrectly rendered in lowercase by most BibTeX styles.

*   **Entry `li2024dclm`**: "LM" in "DataComp-LM" should be protected as `{LM}`.
*   **Entry `muennighoff2024olmoe`**: "OLMoE" should be protected as `{OLMoE}`.
*   **Entry `huang2024hardertasksneedexperts`**: "MoE" should be protected as `{MoE}`.
*   **Entry `yue2024adakroutingboostingefficiency`**: "MoE" and "LLMs" should be protected as `{MoE}` and `{LLMs}`.
*   **Entry `wang2025remoe`**: "ReMoE" and "ReLU" should be protected.
*   **Entry `dai2024deepseek`**: "DeepSeekMoE" should be protected.
*   **Entry `deepseekv3`**: "DeepSeek-V3" should be protected.
*   **Entry `karpathy2022nanogpt`**: "nanoGPT" and "GPTs" should be protected.
*   **Entry `karpathy2025nanochat`**: "nanochat" and "ChatGPT" should be protected.
*   **Entry `xin2020deebert`**: "DeeBERT" and "BERT" should be protected.
*   **Entry `ainslie2023gqa`**: "GQA" should be protected.
*   **Entry `yang2022mup`**: "muP" should be protected.
*   **Entry `team2024gemma2`**: "Gemma" should be protected.
*   **Entry `su2024rope`**: "RoFormer" and "RoPE" should be protected.

### 2. Outdated arXiv Citations
Several works are cited as arXiv preprints despite having been published in major conferences:
*   **Entry `shazeer2017outrageously`**: "Outrageously large neural networks" was published in **ICLR 2017**.
*   **Entry `vaswani2017attention`**: "Attention is all you need" was published in **NeurIPS 2017**.
*   **Entry `he2020momentum`**: "Momentum Contrast for Unsupervised Visual Representation Learning" was published in **CVPR 2020**.

### 3. Inconsistent Venue Naming
*   **Entry `ainslie-etal-2023-colt5`**: Uses the full conference name "Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing", which is excellent.
*   **Entry `zeng2024adamoe`**: Uses "Findings of the Association for Computational Linguistics: EMNLP 2024".
*   In contrast, **Entry `he2020momentum`** and **Entry `schroff2015facenet`** use "IEEE Conference on Computer Vision and Pattern Recognition" (or similar), but often the year is included in the title which might be redundant depending on the style.

## Recommendations
- Wrap all acronyms and proper names in titles with `{}` to ensure correct capitalization.
- Update `shazeer2017outrageously`, `vaswani2017attention`, and `he2020momentum` to their official conference versions.
- Ensure consistent naming for major conferences (e.g., always use full names or always use abbreviations).

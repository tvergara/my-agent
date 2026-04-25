# Bibliography Audit for Paper 0316ddbf

**Paper Title**: DART: Diffusion-Inspired Speculative Decoding for Fast LLM Inference
**Paper ID**: 0316ddbf-c5a0-4cbe-8a86-9d6f31c58041

## Audit Focus
This audit focuses on bibliographic integrity, specifically the protection of technical acronyms, standardization of conference venues, and accuracy of publication metadata.

## Findings

### 1. Missing Acronym Protection in Titles
The acronym "LLM" (Large Language Model) is pervasive in this paper's domain but is consistently unprotected in the `references.bib` file, which will lead to incorrect lowercasing in the final rendered bibliography.

*   **Entry `li2024`**: `title = {Systematic Biases in LLM-as-a-Judge Evaluations}`. "LLM" should be "{LLM}".
*   **Entry `koo2023`**: `title = {Do Language Models Rate Their Own Outputs More Favorably? Measuring Self-Bias in LLM Evaluation}`. "LLM" should be "{LLM}".
*   **Entry `panickssery2024llmevaluatorsrecognizefavor`**: `title={LLM Evaluators Recognize and Favor Their Own Generations}`. "LLM" should be "{LLM}".

### 2. Outdated arXiv Citations
Several works cited as preprints have already been formally published in major venues. Updating these will improve the scholarly rigor of the paper.

*   **Entry `wei2023`**: `Emergent Abilities of Large Language Models`. Published at **Transactions on Machine Learning Research (TMLR) 2022**.
*   **Entry `xu2025hallucinationinevitableinnatelimitation`**: `Hallucination is Inevitable: An Innate Limitation of Large Language Models`. Published at **ICLR 2024**.
*   **Entry `stureborg2024largelanguagemodelsinconsistent`**: `Large Language Models are Inconsistent and Biased Evaluators`. Published at **NeurIPS 2024**.

### 3. Presence of Unrelated Style Files
The source bundle contains `neurips_2025.sty`, which may be a leftover from a previous submission. While not a bibliography issue, it suggests a need for a cleaner source organization for the ICML 2026 submission.

## Recommendations
Update all preprint citations to their official published versions and ensure that "LLM" and other technical acronyms are protected with curly braces in all title fields.

# Bibliography Audit for Paper 0316ddbf

**Paper Title**: Self-Attribution Bias: When AI Monitors Go Easy on Themselves
**Paper ID**: 0316ddbf-c5a0-4cbe-8a86-9d6f31c58041

## Audit Focus
This audit focuses on bibliographic integrity, specifically the protection of technical acronyms, standardization of conference venues, and accuracy of publication metadata.

## Findings

### 1. Missing Acronym Protection in Titles
Several BibTeX entries contain acronyms or proper names in the `title` field that are not protected by curly braces `{}`. In many BibTeX styles (like ICML's), these will be automatically converted to lowercase, which is incorrect for acronyms.

*   **Entry `li2024`**: `title = {Systematic Biases in LLM-as-a-Judge Evaluations}`. "LLM" should be protected as `{LLM}`.
*   **Entry `koo2023`**: `title = {Do Language Models Rate Their Own Outputs More Favorably? Measuring Self-Bias in LLM Evaluation}`. "LLM" should be protected as `{LLM}`.
*   **Entry `panickssery2024llmevaluatorsrecognizefavor`**: `title={LLM Evaluators Recognize and Favor Their Own Generations}`. "LLM" should be protected as `{LLM}`.
*   **Entry `cheng2025`**: `title={Social Sycophancy: A Broader Understanding of LLM Sycophancy}`. "LLM" should be protected as `{LLM}`.
*   **Entry `laurito2025`**: `title = {AI–AI bias: ...}`. "AI-AI" should be protected as `{AI–AI}`.

### 2. Outdated arXiv Citations
Several works cited as preprints have already been formally published in major venues.
*   **Entry `wei2023`**: `Emergent Abilities of Large Language Models`. Published at **Transactions on Machine Learning Research (TMLR) 2022**.
*   **Entry `xu2025hallucinationinevitableinnatelimitation`**: `Hallucination is Inevitable: An Innate Limitation of Large Language Models`. Published at **ICLR 2024**.
*   **Entry `stureborg2024largelanguagemodelsinconsistent`**: `Large Language Models are Inconsistent and Biased Evaluators`. Published at **NeurIPS 2024**.

### 3. Presence of Unrelated Style Files
The source bundle contains `neurips_2025.sty`, which appears to be a leftover from a previous submission context.

## Recommendations
Update all preprint citations to their official published versions and ensure that "LLM", "AI", and other technical acronyms are protected with curly braces in all title fields.

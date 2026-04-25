# Bibliographic Audit - Paper f62ed3b1

**Paper Title:** An Empirical Study and Theoretical Explanation on Task-Level Model-Merging Collapse
**Paper ID:** f62ed3b1-e869-423d-a048-35a632c4f7d8

## Overview
This audit focused on the citation formatting and bibliographic integrity of the submission. Several systematic issues were identified, primarily concerning missing capitalization protection for acronyms and the use of outdated ArXiv preprints for papers that have since been published in major conferences.

## Key Findings

### 1. Missing Capitalization Protection (Curly Braces)
Many BibTeX entries lack curly brace protection `{}` for acronyms, proper nouns, and specific model names in titles. Without this, many BibTeX styles will render these in lowercase, which is incorrect for technical terms.

*   **Acronyms:**
    *   `wang2018glue`: "GLUE" -> `{GLUE}`
    *   `lu2021codexglue`: "Codexglue" -> `{CodexGLUE}`
    *   `bi2024deepseek`: "llm" -> `{LLM}`
    *   `yang2019xlnet`: "Xlnet" -> `{XLNet}`
    *   `lin2004rouge`: "Rouge" -> `{ROUGE}`
    *   `papineni2002bleu`: "Bleu" -> `{BLEU}`
    *   `kazemitabaar2024codeaid`: "llm-based" -> `{LLM}-based`
    *   `jain2024livecodebench`: "Livecodebench" -> `{LiveCodeBench}`, "llms" -> `{LLMs}`
    *   `guo2025deepseek`: "Deepseek-r1" -> `{DeepSeek-R1}`, "llms" -> `{LLMs}`
    *   `liu2019robertarobustlyoptimizedbert`: "RoBERTa" -> `{RoBERTa}`, "BERT" -> `{BERT}`
    *   `zhou2024adapi`: "dnn" -> `{DNN}`
*   **Model/System Names:**
    *   `wolf2019huggingface`: "Huggingface" -> `{HuggingFace}`
    *   `achiam2023gpt`: "Gpt-4" -> `{GPT-4}`
    *   `touvron2023llama`: "Llama" -> `{LLaMA}`
    *   `anil2023palm`: "Palm 2" -> `{PaLM 2}`
    *   `almazrouei2023falcon`: "falcon" -> `{Falcon}`
    *   `adler2024nemotron`: "Nemotron-4" -> `{Nemotron-4}`
    *   `tian2023chatgpt`: "ChatGPT" -> `{ChatGPT}`
    *   `guo2021longt5`: "LongT5" -> `{LongT5}`
    *   `xue2020mt5`: "mt5" -> `{mT5}`
    *   `de2022entities`: "t0" -> `{T0}`
    *   `lewis2019bartdenoisingsequencetosequencepretraining`: "BART" -> `{BART}`
    *   `hu2021loralowrankadaptationlarge`: "LoRA" -> `{LoRA}`
    *   `yang2024qwen2`: "Qwen2. 5" -> `{Qwen2.5}`

### 2. Outdated ArXiv Entries
Several papers are cited as ArXiv preprints despite having been published in major venues. Citing the peer-reviewed version is preferred and provides more accurate metadata.

*   `wang2018glue`: Published in **ICLR 2019**.
*   `yadav2024ties`: Published in **NeurIPS 2023**.
*   `yang2023adamerging`: Published in **ICML 2023**.
*   `stoica2023zipit`: Published in **ICLR 2024**.
*   `hu2021loralowrankadaptationlarge`: Published in **ICLR 2022**.
*   `wang2023voyager`: Published in **ICCV 2023**.
*   `guo2021longt5`: Published in **NAACL 2022**.
*   `xue2020mt5`: Published in **NAACL 2021**.
*   `sanh2021multitask`: Published in **ICLR 2022**.
*   `bahdanau2014neural`: Published in **ICLR 2015**.
*   `kingma2014adam`: Published in **ICLR 2015**.
*   `brown2020language`: Published in **NeurIPS 2020**.
*   `ouyang2022training`: Published in **NeurIPS 2022**.

### 3. Duplicates and Inconsistencies
*   **Duplicates:** `wang2018glue` and `wang2019gluemultitaskbenchmarkanalysis` are the same paper.
*   **Inconsistent Venue Names:** Variations in conference names (e.g., "International Conference on Machine Learning" vs "Forty-first International Conference on Machine Learning") and capitalization in "Advances in Neural Information Processing Systems".
*   **Generic Keys:** Some keys like `ModelAveraging`, `gradientboosting`, and `boosting` are overly generic and can lead to collisions in larger bibliographies.

## Conclusion
The bibliography requires a thorough pass to protect acronyms and update preprint citations to their final published versions. These changes will improve the professionalism and technical accuracy of the paper's references.

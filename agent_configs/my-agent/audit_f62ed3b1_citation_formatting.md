# Citation Formatting Audit - Paper f62ed3b1

I audited the citation formatting for the paper "An Empirical Study and Theoretical Explanation on Task-Level Model-Merging Collapse" (ID: f62ed3b1).

## Findings

### 1. Unprotected Acronyms and Proper Nouns in Titles
Several entries in `ref.bib` have acronyms or system names that should be protected with curly braces `{}` to preserve their capitalization.
- `wang2018glue`: "GLUE" renders as "Glue". Should be `{GLUE}`.
- `lu2021codexglue`: "Codexglue" renders as "Codexglue". Should be `{CodexGLUE}`.
- `husain2019codesearchnet`: "Codesearchnet" renders as "Codesearchnet". Should be `{CodeSearchNet}`.
- `zhou2019devign`: "Devign" renders as "Devign". Should be `{Devign}`.
- `yang2019xlnet`: "Xlnet" renders as "Xlnet". Should be `{XLNet}`.
- `zhao2022boosttree`: "BoostTree" and "BoostForest" render as "Boosttree" and "Boostforest". Should be `{BoostTree}` and `{BoostForest}`.

### 2. Incorrect Journal Names
- `muller2022analysis` and `mienye2022survey`: Both list `journal={Ieee Access}`. This should be `{IEEE Access}`.

### 3. Outdated arXiv Citations
Several foundational benchmarks are cited as preprints despite being published in major conferences years ago:
- **GLUE** (`wang2018glue`): Cited as `arXiv:1804.07461`. Should be updated to **EMNLP 2018**.

### 4. Missing Braces for Proper Nouns
- `qin2022exploring`: "Mode Connectivity" is often treated as a proper concept in this field and could be protected.
- `frankle2020linear`: "Lottery Ticket Hypothesis" should be `{Lottery Ticket Hypothesis}`.

## Recommendation
The authors should review their `ref.bib` file to:
- Apply curly brace protection to all acronyms (GLUE, XLNet, etc.) and proper nouns.
- Correct "Ieee Access" to "IEEE Access".
- Update arXiv entries to their official conference/journal versions where available.

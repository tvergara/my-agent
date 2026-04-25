# Citation Formatting Audit - Paper b044e3c3

I audited the citation formatting for the paper "A Unified SPD Token Transformer Framework for EEG Classification: Systematic Comparison of Geometric Embeddings" (ID: b044e3c3).

## Findings

### 1. Unprotected Acronyms in BibTeX Titles
Several entries in `REFERENCES.bib` have acronyms (like EEG, BCI, SPD) in the `title` field without curly braces `{}`. Since BibTeX usually converts titles to lowercase (except for the first letter), these acronyms will likely appear incorrectly as "eeg", "bci", or "spd" in the final bibliography unless the bibliography style preserves them.

Examples:
- `barachant2012classification`: "BCI" is not protected.
- `lawhern2018eegnet`: "EEGNet" and "EEG" are not protected.
- `schirrmeister2017deep`: "EEG" is not protected.
- `brooks2019riemannian`: "SPD" is not protected.
- `song2022eegconformer`: "EEG" (twice) is not protected.

### 2. Duplicate Page Numbers (Potential Copy-Paste Error)
The following two entries have identical page ranges despite being different papers in different years of the same conference series:
- `ingolfsson2020eegtcnet` (SMC 2020): `pages={2958--2965}`
- `ingolfsson2021fbconet` (SMC 2021): `pages={2958--2965}`
This is highly likely a copy-paste error in the BibTeX source.

### 3. Inconsistencies between Citation Keys and Year Field
- `barachant2013multiclass` has `year={2012}`.
- `chakraborty2020manifoldnet` has `year={2022}`.

### 4. Missing Braces for Proper Nouns
- `barachant2012classification`: "Riemannian" should ideally be `{Riemannian}` to ensure it remains capitalized.

## Recommendation
The authors should review their `REFERENCES.bib` file to:
- Wrap all acronyms and proper nouns in `{}` to preserve capitalization.
- Verify the correct page numbers for the SMC 2020/2021 papers.
- Synchronize citation keys with the actual publication years to avoid confusion.

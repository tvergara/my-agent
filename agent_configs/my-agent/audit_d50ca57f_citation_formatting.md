# Citation Formatting Audit for Paper d50ca57f

## Paper Information
- **ID**: d50ca57f-ac9a-438f-b0f5-fab02c8d64df
- **Title**: Transport Clustering: Solving Low-Rank Optimal Transport via Clustering

## Identified Issues

### 1. Broken BibTeX Entries
Several entries in `references.bib` have the key on the line following the entry type declaration (e.g., `@inproceedings{` followed by a newline). This can cause parsing failures in standard BibTeX tools.
Examples found:
- 13 occurrences where the `@type{` line does not contain the key.

### 2. Missing Acronym Protection
Multiple conference and organization names in the `booktitle` and `publisher` fields lack curly brace protection, which may lead to incorrect capitalization when using certain bibliography styles (e.g., "ieee" instead of "IEEE").
Examples:
- `ACM` in `Proceedings of the forty-third annual ACM symposium on Theory of computing`
- `ACM-SIAM`, `SODA` in `Proceedings of the 2024 Annual ACM-SIAM Symposium on Discrete Algorithms (SODA)`
- `SIGKDD`, `KDD` in `Proceedings of the Tenth ACM SIGKDD International Conference on Knowledge Discovery and Data Mining`
- `IEEE` in `Proceedings of the IEEE conference on computer vision and pattern recognition`

### 3. Duplicate Bibliography Entries
The following keys are defined multiple times in `references.bib`:
- `dong2023partial` (2 occurrences)
- `staahl2016visualization` (2 occurrences)

## Evidence
The issues were identified by inspecting `references.bib` extracted from the paper's source tarball.

```bash
# Check for broken keys
grep -E "^@[^{]+\{$" paper_d50ca57f/references.bib

# Check for duplicates
python3 find_duplicates.py paper_d50ca57f/references.bib
```

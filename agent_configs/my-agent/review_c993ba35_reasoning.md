# Bibliographic Audit: Learning Approximate Nash Equilibria (c993ba35)

I have conducted a thorough audit of the bibliographic references in `main.bib` for the paper "Learning Approximate Nash Equilibria in Cooperative Multi-Agent Reinforcement Learning via Mean-Field Subsampling" (ID: `c993ba35-65e0-4290-a66a-c128e33410f4`).

## Methodology
I parsed the `main.bib` file and checked for:
1.  **Capitalization Protection Workarounds**: Identifying non-standard ways of protecting title capitalization.
2.  **Venue Consistency**: Checking for uniform naming and capitalization of conferences like ICML, NeurIPS, and ICRA.
3.  **BibTeX Style Heterogeneity**: Identifying inconsistencies in the fields provided across different entries.
4.  **Proper Noun Integrity**: Ensuring terms like `MARVEL`, `Nash`, and `Markov` are correctly handled.

## Key Findings

### 1. Non-Standard Capitalization Protection
The bibliography uses highly inconsistent and sometimes redundant methods to protect capitalization in titles:
- `aina2025deepreinforcementlearningmultiagent`: Uses individual letter protection `{R}einforcement {L}earning`, which is unconventional.
- `chiun2025marvelmultiagentreinforcementlearning`: Uses a mix of double braces and individual letter protection `{{MARVEL}: {M}ulti-{A}gent ...}`.
- `craven2005karlin`: Uses double braces for the entire title `{{Karlin's conjecture and a question of P{\'o}lya}}`.

### 2. Inconsistent Venue Capitalization
Major conferences are cited with varying capitalization:
- **ICML**: `ding2022independent` uses `International Conference on Machine Learning`, while `fujimoto2019off` uses `International conference on machine learning`.
- **IEEE Venues**: `Daskalakis_2014` and `chiun2025marvelmultiagentreinforcementlearning` use title case for IEEE symposia/conferences, which is consistent, but they differ in whether they include the series abbreviation (e.g., `(ICRA)`).

### 3. Inconsistent Field Usage
Entries sourced from different databases (e.g., ACM, IEEE, ArXiv) retain their source-specific fields, leading to a heterogeneous bibliography:
- Some entries include `isbn`, `address`, `location`, and `abstract` (e.g., `doi:10.1137/1.9781611976465.84`).
- Others include `keywords`, `doi`, and `publisher` (e.g., `lv2024localinformationaggregationbased`).
- ArXiv entries vary between using `@article` with `journal={arXiv preprint ...}` and `@misc` with `eprint`.

### 4. Handling of Proper Nouns
While `Nash` is generally capitalized, terms like `Markov` and `Nash` should be consistently protected (e.g., `{Nash}`) to ensure they are not lowercased by the `icml2026.bst` style.

## Conclusion
A systematic pass to standardize the BibTeX style and title protection mechanism is recommended to ensure a uniform and professional appearance in the final publication.

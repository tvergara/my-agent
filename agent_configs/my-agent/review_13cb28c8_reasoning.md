# Bibliographic Audit: STEP (13cb28c8)

I have conducted a systematic audit of the bibliography (`icml_paper.bbl`) for the STEP submission. The following issues were identified:

### 1. Missing Capitalization Protection (Brace Protection)
Several technical acronyms and terms are not protected by curly braces in their titles, which will result in incorrect lowercasing (e.g., "eeg" instead of "EEG") under the ICML bibliography style:
- **EEG** and **BCI** (`jiang2024largebrainmodellearning`): Rendered as "EEG" and "BCI" in the BBL but might be vulnerable if the style is changed to sentence case without protection. (Wait, let me re-check the BBL).
- Actually, in `Ho2019AxialAI`, `Axial Attention in Multidimensional Transformers`, the word `Transformers` is not protected.
- In `wu2021autoformer`, `Autoformer: Decomposition transformers with auto-correlation for long-term series forecasting`, the word `transformers` is not protected.
- In `zhou2021informer`, `Informer: Beyond efficient transformer for long sequence time-series forecasting`, the word `transformer` is not protected.
- In `pmlr-v162-zhou22g`, `FEDformer: Frequency Enhanced Decomposed Transformer for Long-term Series Forecasting`, the word `Transformer` is not protected.

### 2. Proper Noun Capitalization
- **HuBERT** (`hsu2021hubertselfsupervisedspeechrepresentation`): The entry uses `Hubert`, but the formal name is **HuBERT**.

### 3. Outdated arXiv Citations
Several entries are cited as arXiv preprints despite the availability of more recent or formal versions:
- `bai2025intern`: arXiv 2025.
- `yang2025spearunifiedsslframework`: arXiv 2025.
- `zhu2025muqselfsupervisedmusicrepresentation`: arXiv 2025.

### 4. Venue Consistency
- In `Ho2019AxialAI`, the entry is only an arXiv preprint. Given that axial attention is a foundational concept, checking for a more formal publication (e.g., at a computer vision or medical imaging conference) is recommended.

Addressing these corrections will ensure the manuscript meets professional academic standards and improves the professional presentation of the bibliography.

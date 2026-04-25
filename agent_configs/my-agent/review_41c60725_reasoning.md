# Bibliographic Audit: HeiSD (41c60725)

I have conducted a systematic audit of the bibliography (`reference.bib`) for the HeiSD submission. The following issues were identified:

### 1. Missing Acronym Protection (Curly Braces)
A significant number of technical acronyms and model names are not protected by curly braces in their titles, which will result in incorrect lowercasing (e.g., "openvla" instead of "OpenVLA") under the ICML bibliography style:
- **Model Names**: `OpenVLA`, `EdgeVLA`, `FastDriveVLA`, `CEED-VLA`, `SpecPrune-VLA`, `Spec-VLA`, `TinyVLA`, `VLA-Cache`, `EfficientVLA`, `DEER-VLA`, `MoLe-VLA`, `Robomamba`, `RT-2`, `RT-Cache`.
- **Decoding/Efficiency Terms**: `Medusa`, `Eagle`, `Eagle-2`, `Eagle-3`, `MBQ`, `QAIL`, `PROMTEC`, `ANPD`.
- **Standard Acronyms**: `LLM`, `VLA`, `CTC`, `MoE`, `LoRA`, `DoRA`, `KERV`, `RAPID`, `DyQ-VLA`.

### 2. Outdated arXiv Citations
Many key references are cited as arXiv preprints despite having been formally published or having more recent versions available:
- **DINOv2** (`dinov2`): arXiv 2023.
- **OpenVLA** (`openvla`): arXiv 2024.
- **Eagle** series (`eagle`, `eagle2`): arXiv 2024.
- **Robomamba** (`robomamba`): arXiv 2024.
- **SIMPLER** (`simplerenv`): arXiv 2024.
- **Robocasa** (`robocasa`): arXiv 2024.

### 3. Formatting and Metadata Issues
- **SVD** (`SVD`): The entry for "Singular value decomposition (SVD) and generalized singular value decomposition" has unusual volume (`907`) and number (`912`) fields for an encyclopedia entry, which should be verified.
- **Inconsistent Conference Naming**: There is inconsistency in how conference names are formatted, mixing full names with various abbreviated forms.

Addressing these corrections will ensure the manuscript meets professional academic standards and improves the professional presentation of the bibliography.

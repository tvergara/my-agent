# Bibliographic Audit: Trifuse (07274583)

I have conducted a systematic audit of the bibliography (`example_paper.bib`) for the Trifuse submission. The following issues were identified:

### 1. Missing Year Field
Several key references from late 2024 and early 2025 are missing the `year` field, which is critical for correct citation rendering and sorting:
- **uGround** (`uground`): Missing year (**2025**).
- **OS-ATLAS** (`osatlas`): Missing year (**2025**).
- **MLLMs Know Where to Look** (`mllmknow`): Missing year (**2025**).

### 2. Outdated arXiv Citations
Multiple entries are cited as arXiv preprints despite having formal conference publications available:
- **Set-of-Mark (SoM)** (`som`): arXiv 2023 → **CVPR 2024**.
- **uGround**, **OS-ATLAS**, and **MLLMs Know Where to Look** should be updated to their **ICLR 2025** versions.

### 3. Missing Capitalization Protection (Brace Protection)
The following model names, dataset names, and acronyms lack curly brace `{}` protection in their titles, which will result in incorrect lowercasing (e.g., "Qwen2-vl" instead of "Qwen2-VL") under the ICML bibliography style:
- `Qwen2-VL` (`qwen2vl`)
- `ShowUI` (`showui`)
- `Aria-UI` (`ariaui`)
- `ScreenSpot-Pro` (`screenspotpro`)
- `UI-TARS` (`uitars`)
- `PaddleOCR` (`paddleocr`)
- `DiMo-GUI` (`dimogui`)
- `VQA` (`textvqa`)

### 4. Formatting Issues
- **TextVQA** (`textvqa`): The page range uses a single hyphen (`8317-8326`) instead of the standard LaTeX double hyphen (`8317--8326`).
- **Inconsistent Conference Naming**: There is inconsistency in how conference names are formatted (e.g., mixing "Proceedings of the IEEE conference on computer vision and pattern recognition" with other abbreviated forms).

Addressing these corrections will ensure the manuscript meets professional academic standards and reflects the current state of the field.

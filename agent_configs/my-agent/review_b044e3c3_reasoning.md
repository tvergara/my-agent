# Bibliographic Audit: EEG Transformer (b044e3c3)

I have conducted a systematic audit of the bibliography (`REFERENCES.bib`) for the EEG Transformer submission. The following issues were identified:

### 1. Major Attribution and Metadata Error
- **FBCNet** (`ingolfsson2021fbconet`): The entry incorrectly attributes "FBCNet: A multi-view convolutional neural network for brain-computer interface" to *Ingolfsson et al.* and lists it as a 2021 IEEE SMC publication.
- **Correction**: FBCNet was authored by **Ravikiran Mane et al.** and was published in **IEEE Transactions on Neural Systems and Rehabilitation Engineering (TNSRE)** in **2022** (Volume 30, pp. 2027--2037). It appears the metadata was inadvertently duplicated from the `ingolfsson2020eegtcnet` entry.

### 2. Missing Capitalization Protection (Brace Protection)
Several technical acronyms and terms are not protected by curly braces in their titles, which will result in incorrect lowercasing (e.g., "eeg" instead of "EEG") under the ICML bibliography style:
- `EEG`, `SPD`, `BCI`, `FBCNet`, `EEG-TCNet`, `ManifoldNet`, `LMDA-Net`.
- Proper nouns like `Riemannian`, `Log-Euclidean`, and `Kakutani`.

### 3. Outdated arXiv Citations
Multiple entries are cited as arXiv preprints despite having been formally published:
- **ManifoldNet** (`chakraborty2020manifoldnet`): Should be updated to its formal publication in **IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI)** in **2022**.
- **Geometric Deep Learning** (`bronstein2021geometric`): Can now be cited as the 2026 textbook from **MIT Press**.

### 4. Missing or Inconsistent Metadata
- **Attention is All You Need** (`vaswani2017attention`): Missing page numbers (**5998--6008**).
- **Key-Year Discrepancy** (`barachant2013multiclass`): The citation key ends in 2013, but the year field is **2012**.

Addressing these corrections will ensure the manuscript meets professional academic standards and reflects the current state of the literature.

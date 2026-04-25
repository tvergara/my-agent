# Bibliography Audit for Paper b044e3c3

**Paper Title**: A Unified SPD Token Transformer Framework for EEG Classification: Systematic Comparison of Geometric Embeddings
**Paper ID**: b044e3c3-4a8e-4a74-a3b8-13584deba079

## Audit Focus
This audit focuses on bibliographic integrity, specifically the protection of technical acronyms, standardization of conference venues, and accuracy of publication metadata.

## Findings

### 1. Missing Acronym Protection in Titles
Technical acronyms related to the paper's core topic (EEG and BCI) are often left unprotected in titles, which will lead to incorrect lowercasing in the bibliography.

*   **Entry `lawhern2018eegnet`**: `title={EEGNet: a compact convolutional neural network for EEG-based brain--computer interfaces}`. "EEGNet" and "EEG" should be "{EEGNet}" and "{EEG}".
*   **Entry `barachant2012classification`**: `title={Classification of covariance matrices using a Riemannian-based kernel for BCI applications}`. "BCI" should be "{BCI}".
*   **Entry `schirrmeister2017deep`**: `title={Deep learning with convolutional neural networks for EEG decoding and visualization}`. "EEG" should be "{EEG}".
*   **Entry `blankertz2008optimizing`**: `title={Optimizing spatial filters for robust EEG single-trial analysis}`. "EEG" should be "{EEG}".

### 2. Outdated arXiv Citations
Several papers are cited as preprints despite having been published in major venues by now.

*   **Entry `song2021eeg`**: `journal={arXiv preprint arXiv:2104.13478}`. This work, "EEG conformer", was published in **IEEE Transactions on Neural Systems and Rehabilitation Engineering** (2023).
*   **Entry `scotti2023mind`**: `note={arXiv:2309.07579}`. This work, "Mind's eye", was published at **CVPR 2024**.

### 3. Inconsistent Venue Formatting
*   **Conference Names**: Venues like `2020 IEEE International Conference on Systems, Man, and Cybernetics (SMC)` should have the "IEEE" and "(SMC)" parts protected to avoid potential lowercasing or inconsistent rendering.

## Recommendations
Update outdated preprint citations to their final published versions and ensure all technical acronyms in titles (EEG, BCI, SPD, etc.) are protected with curly braces.

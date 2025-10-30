# Brain MRI Collections (`data-others/brain`)

Curated external **human brain MRI datasets** for research, benchmarking, and education.
This repository aggregates links and light metadata to facilitate access from neuroimaging tools (e.g., DSI Studio).
**Use each dataset under its original license and cite the original authors.**

---

## Releases in This Repository

### 1) DTI Predicts Mandarin Learning (`mit-casl`)

White-matter microstructure and **Mandarin second-language learning** outcomes.

* **Modality:** DTI (NIfTI + `.bval`/`.bvec`), behavioral CSV
* **Scope:** Adult second-language learners
* **License:** CC BY 4.0
* **Citation:** Qi Z. (2017) *DTI Predicts Mandarin Learning* [Data set]. Zenodo.
* **DOI/Source:** [https://doi.org/10.5281/zenodo.260007](https://doi.org/10.5281/zenodo.260007)
* **Use cases:** Language aptitude biomarkers, FA/tractography analyses

---

### 2) Southwest University SLIM (`swu-slim`)

**Longitudinal** multimodal MRI of healthy young adults (test–retest).

* **Modality:** DWI (eddy corrected SRC/FIB), T1w, demographics
* **License:** CC BY-NC (as provided by source)
* **Reference:** Liu et al., *Sci Data*, 2017
* **Notes:** DSI Studio reconstruction details (GQI, RDI) and preprocessing described in release
* **Use cases:** Reliability, longitudinal modeling, diffusion reconstruction benchmarks

---

### 3) Stark Cross-Sectional Aging (`stark-aging`)

Cross-sectional **aging** dataset with imaging + behavioral measures.

* **Modality:** Structural MRI, whole-brain DTI, high-res MTL DTI; FreeSurfer segmentations
* **Scope:** ~120 participants, ages 18–89
* **License:** CC BY-NC-SA
* **Project page:** [https://www.nitrc.org/projects/stark_aging/](https://www.nitrc.org/projects/stark_aging/)
* **Use cases:** Aging effects on hippocampus, structure–behavior relations, lifespan analyses

---

### 4) Penthera 3T (`penthera`)

Scan–rescan **multi-shell DWI** (13 healthy adults; Philips 3 T).

* **Modality:** DWI (b=300/1000/2000; 8/32/60 dirs; +reverse-PE), T1w
* **License/Source:** [https://doi.org/10.5281/zenodo.2602049](https://doi.org/10.5281/zenodo.2602049)
* **Use cases:** Multi-shell modeling, EPI distortion correction, reliability

---

### 5) NTU-90 (`ntu90`)

Classic **DSI** dataset (90 subjects @ 3 mm; one subject @ 2 mm).

* **Modality:** DSI (203 dirs; b-max 6000 s/mm²; NIfTI)
* **License:** Non-commercial, educational, research (see release text)
* **Key refs:**

  * Yeh & Tseng, *NeuroImage*, 2011 (NTU-90 atlas)
  * Yeh et al., *IEEE TMI*, 2010 (GQI)
* **Use cases:** Tractography evaluation, high-angular sampling methods

---

### 6) NKI Rockland Sample (`nki-rockland`)

Large **lifespan** community neuroimaging resource with deep phenotyping.

* **Scope:** >1,500 participants (ages 6–85)
* **License:** CC BY-NC; phenotypic data require DUA (see release text)
* **Use cases:** Development, psychiatric associations, longitudinal/connectome studies

---

### 7) Multi-Modal MRI Reproducibility Resource (`mmrr`)

Scan–rescan **1-hour multi-parametric protocol** on 21 volunteers (3 T).

* **Modalities:** MPRAGE/FLAIR, DTI, rs-fMRI, B0/B1, ASL, VASO, T1/T2, MT (NIfTI)
* **Citation:** Landman et al., *NeuroImage*, 2010 (doi:10.1016/j.neuroimage.2010.11.047)
* **License:** BIRN Data License (see NITRC link in release)
* **Use cases:** Cross-modality reproducibility, power analysis, QC pipelines

---

### 8) IXI Dataset — IOP / HH / Guy’s (`ixi-iop`, `ixi-hh`, `ixi-guys`)

Nearly **600 healthy** subjects across three London sites.

* **Modalities:** T1w, T2w, PD, MRA, DWI (15 dirs)
* **License:** CC BY-SA 3.0
* **Project page:** [https://brain-development.org/ixi-dataset/](https://brain-development.org/ixi-dataset/)
* **Use cases:** Population baselines, multi-site comparisons, morphometry + diffusion

---

## Quick Start

### Download

* Use the **Releases** tab to access per-dataset assets (archives, CSVs, metadata).
* Respect the **license** posted in each release; some datasets are **non-commercial** or require a **DUA** for phenotypes.

### Open in DSI Studio (examples)

* **DTI/DSI/HARDI:** Load `.nii.gz` + `.bval` + `.bvec` (or SRC/FIB as provided).
* **Tractography:** Reconstruct (e.g., GQI/DTI), set QA/FA thresholds, track, then export metrics/connectomes.
* **QC:** Check b-table, reverse-PE pairs, motion/eddy logs where available.

> Tip: For reproducible pipelines, keep software versions and parameters alongside outputs.

---

## Licensing & Attribution

* Each release retains its **original license** (e.g., CC BY, CC BY-NC, CC BY-NC-SA, BIRN, CC BY-SA).
* **You must cite the original dataset/publication** listed in each release when using the data.
* If your work benefits from this aggregation, a general acknowledgment is appreciated:
  *“Data access facilitated via the `data-others/brain` repository.”*

---

## Intended Use

* Method development (tractography, diffusion modeling, harmonization)
* Test–retest and scan–rescan studies
* Education/training in MRI processing and QC
* Cross-site and lifespan analyses (subject to each dataset’s terms)

---

## Notes & Caveats

* Some releases include **partial** or **incremental** uploads; read each release notes.
* Phenotypic or sensitive data may require **DUA** or additional approvals from the source.
* Anonymization/defacing methods differ by dataset; verify before face-sensitive analyses.

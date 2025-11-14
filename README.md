# Brain MRI Collections

Curated external **human brain MRI datasets** for research, benchmarking, and education.  
This repository aggregates links and light metadata to facilitate access from neuroimaging tools (e.g., DSI Studio).

> **Important:** Always follow the **original license / DUA** of each dataset and cite the **original authors**.

---

## Datasets in This Repository

1. [NODDI Lifespan dMRI (`ucsf-noddi`)](#1-noddi-lifespan-dmri-ucsf-noddi)
2. [DTI Predicts Mandarin Learning (`mit-casl`)](#2-dti-predicts-mandarin-learning-mit-casl)
3. [Southwest University SLIM (`swu-slim`)](#3-southwest-university-slim-swu-slim)
4. [Stark Cross-Sectional Aging (`stark-aging`)](#4-stark-cross-sectional-aging-stark-aging)
5. [Penthera 3T (`penthera`)](#5-penthera-3t-penthera)
6. [NTU-90 (`ntu90`)](#6-ntu-90-ntu90)
7. [NKI Rockland Sample (`nki-rockland`)](#7-nki-rockland-sample-nki-rockland)
8. [Multi-Modal MRI Reproducibility Resource (`mmrr`)](#8-multi-modal-mri-reproducibility-resource-mmrr)
9. [IXI – Institute of Psychiatry (`ixi-iop`)](#9-ixi--institute-of-psychiatry-ixi-iop)
10. [IXI – Hammersmith Hospital (`ixi-hh`)](#10-ixi--hammersmith-hospital-ixi-hh)
11. [IXI – Guy’s Hospital (`ixi-guys`)](#11-ixi--guys-hospital-ixi-guys)
12. [Healthy Brain Network (`hbn`)](#12-healthy-brain-network-hbn)
13. [Cambridge Centre for Ageing and Neuroscience (`cam-can`)](#13-cambridge-centre-for-ageing-and-neuroscience-cam-can)

---

## 1) NODDI Lifespan dMRI (`ucsf-noddi`)

Diffusion MRI for **lifespan white-matter maturation** with NODDI (ages 7–63).

- **Participants:** 67 healthy controls; includes **test–retest** subsets  
- **Modalities:**
  - DTI: single-shell (b≈1000 s/mm²)
  - HARDI: **two shells** for NODDI modeling
  - T1-weighted MRI
- **License:** Governed by the dataset’s **UCSF Datashare DUA** (see Dryad record)
- **Citation:**  
  Chang, Y., & Mukherjee, P. (2015). *NODDI-PLOS-ONE-Chang et al 2015* [Data set]. Dryad. https://doi.org/10.7272/Q6D798BD  
  Primary article: *PLOS ONE*, “Neurite orientation dispersion and density imaging of brain development across the lifespan” (2015).
- **Source:** Dryad – https://doi.org/10.7272/Q6D798BD  
- **Typical uses:** ND/OD lifespan curves, age prediction, NODDI vs. DTI comparisons, reliability.

### GitHub one-line download (`ucsf-noddi`)

**Linux / macOS**
```bash
curl -s https://api.github.com/repos/data-others/brain/releases/tags/ucsf-noddi | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
````

**Windows PowerShell**

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-others/brain/releases/tags/ucsf-noddi").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

---

## 2) DTI Predicts Mandarin Learning (`mit-casl`)

White-matter microstructure and **Mandarin second-language learning** outcomes.

* **Participants:** De-identified adult learners of Mandarin as a second language
* **Modalities:** DTI (NIfTI DWI + `.bval`/`.bvec`), behavioral / demographic **CSV**
* **License:** **CC BY 4.0**
* **Citation:**
  Qi, Z. (2017). *DTI Predicts Mandarin Learning* [Data set]. Zenodo. [https://doi.org/10.5281/zenodo.260007](https://doi.org/10.5281/zenodo.260007)
  Qi et al. (2014). *J Neurolinguistics*, 33, 14–28.
* **Source:** Zenodo – [https://doi.org/10.5281/zenodo.260007](https://doi.org/10.5281/zenodo.260007)
* **Typical uses:** Language aptitude biomarkers, FA/tract-based analyses, structure–learning relationships.

### GitHub one-line download (`mit-casl`)

**Linux / macOS**

```bash
curl -s https://api.github.com/repos/data-others/brain/releases/tags/mit-casl | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

**Windows PowerShell**

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-others/brain/releases/tags/mit-casl").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

---

## 3) Southwest University SLIM (`swu-slim`)

**Longitudinal** multimodal MRI test–retest sample of young adults.

* **Participants:** Healthy young adults, **3.5-year** test–retest design
* **Modalities:** Eddy-corrected DWI (SRC/FIB), T1w, demographics; behavioral assessments
* **License:** **CC BY-NC**
* **Reference:** Liu et al., *Sci Data*, 2017
* **Source:** CoRR / SLIM project; OneDrive links in release
* **Typical uses:** Reliability studies, longitudinal modeling, diffusion reconstruction benchmarks.

### GitHub one-line download (`swu-slim`)

**Linux / macOS**

```bash
curl -s https://api.github.com/repos/data-others/brain/releases/tags/swu-slim | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

**Windows PowerShell**

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-others/brain/releases/tags/swu-slim").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

---

## 4) Stark Cross-Sectional Aging (`stark-aging`)

Cross-sectional **aging** dataset with detailed imaging and behavior.

* **Participants:** ~120 adults, ages **18–89**
* **Modalities:** Whole-brain DTI, high-res MTL DTI, structural MRI, FreeSurfer segmentations
* **License:** **CC BY-NC-SA**
* **Project page:** [https://www.nitrc.org/projects/stark_aging/](https://www.nitrc.org/projects/stark_aging/)
* **Typical uses:** Aging effects on hippocampus, structure–behavior relations, lifespan analyses.

### GitHub one-line download (`stark-aging`)

**Linux / macOS**

```bash
curl -s https://api.github.com/repos/data-others/brain/releases/tags/stark-aging | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

**Windows PowerShell**

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-others/brain/releases/tags/stark-aging").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

---

## 5) Penthera 3T (`penthera`)

Scan–rescan **multi-shell DWI** on Philips 3T.

* **Participants:** 13 young healthy adults, **6 scans per subject** (two sessions × three scans)
* **Modalities:**

  * DWI (b=300/1000/2000; 8/32/60 directions; 7×b0; reverse-PE b0)
  * T1w MPRAGE
* **License / Source:** Zenodo – [https://doi.org/10.5281/zenodo.2602049](https://doi.org/10.5281/zenodo.2602049)
* **Typical uses:** Multi-shell modeling, distortion correction, scan–rescan reliability.

### GitHub one-line download (`penthera`)

**Linux / macOS**

```bash
curl -s https://api.github.com/repos/data-others/brain/releases/tags/penthera | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

**Windows PowerShell**

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-others/brain/releases/tags/penthera").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

---

## 6) NTU-90 (`ntu90`)

Classic **DSI** dataset (NTU-90 atlas source).

* **Participants:** 90 subjects (3 mm DSI), plus 1 subject at 2 mm
* **Modalities:** DSI, 203 directions, **b-max 6000 s/mm²**, NIfTI
* **License:** Non-commercial, educational, research; redistribution requires including original license paragraph
* **Key refs:**

  * Yeh & Tseng, *NeuroImage* 58(1), 91–99 (2011)
  * Yeh et al., *IEEE TMI* 29(9), 1626–1635 (2010)
* **Typical uses:** Tractography evaluation, high-angular sampling methods, atlas work.

### GitHub one-line download (`ntu90`)

**Linux / macOS**

```bash
curl -s https://api.github.com/repos/data-others/brain/releases/tags/ntu90 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

**Windows PowerShell**

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-others/brain/releases/tags/ntu90").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

---

## 7) NKI Rockland Sample (`nki-rockland`)

Lifespan community neuroimaging with deep phenotyping.

* **Participants:** >1,500, ages **6–85**
* **Data:** MRI, extensive phenotypes, psychiatric/cognitive measures, genetics, etc.
* **License:** **CC BY-NC**; high-dimensional phenotypes require **DUA**
* **Reference:** Tobe et al., *Sci Data* 9(1), 300 (2022)
* **Phenotypes:** Access via COINS (requires approved DUA)
* **Typical uses:** Development, psychiatric associations, longitudinal/connectome studies.

### GitHub one-line download (`nki-rockland`)

**Linux / macOS**

```bash
curl -s https://api.github.com/repos/data-others/brain/releases/tags/nki-rockland | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

**Windows PowerShell**

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-others/brain/releases/tags/nki-rockland").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

---

## 8) Multi-Modal MRI Reproducibility Resource (`mmrr`)

Scan–rescan **multi-parametric** MRI resource (3T, 1-hour protocol).

* **Participants:** 21 healthy volunteers (no neurological history), scan–rescan
* **Modalities:** MPRAGE, FLAIR, DTI, rs-fMRI, B0/B1, ASL, VASO, quantitative T1/T2, MT (NIfTI)
* **Citation:**
  Landman et al., *NeuroImage*, 2010. doi:10.1016/j.neuroimage.2010.11.047
* **License:** **BIRN Data License** (see NITRC project page)
* **Project page:** [https://www.nitrc.org/projects/multimodal/](https://www.nitrc.org/projects/multimodal/)
* **Typical uses:** Cross-modality reproducibility, power analysis, QC pipelines.

### GitHub one-line download (`mmrr`)

**Linux / macOS**

```bash
curl -s https://api.github.com/repos/data-others/brain/releases/tags/mmrr | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

**Windows PowerShell**

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-others/brain/releases/tags/mmrr").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

---

## 9) IXI – Institute of Psychiatry (`ixi-iop`)

Site-specific subset of the **IXI Dataset**.

* **Participants:** Healthy subjects scanned at **Institute of Psychiatry** (GE 1.5T)
* **Modalities:** T1w, T2w, PD, MRA, DWI (15 directions)
* **License:** **CC BY-SA 3.0**
* **Project page:** [https://brain-development.org/ixi-dataset/](https://brain-development.org/ixi-dataset/)
* **Typical uses:** Site-specific baselines, morphometry + diffusion, multi-site comparisons.

### GitHub one-line download (`ixi-iop`)

**Linux / macOS**

```bash
curl -s https://api.github.com/repos/data-others/brain/releases/tags/ixi-iop | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

**Windows PowerShell**

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-others/brain/releases/tags/ixi-iop").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

---

## 10) IXI – Hammersmith Hospital (`ixi-hh`)

Site-specific subset of the **IXI Dataset**.

* **Participants:** Healthy subjects scanned at **Hammersmith Hospital** (Philips 3T)
* **Modalities:** T1w, T2w, PD, MRA, DWI (15 directions)
* **License:** **CC BY-SA 3.0**
* **Project page:** [https://brain-development.org/ixi-dataset/](https://brain-development.org/ixi-dataset/)
* **Typical uses:** High-field site reference, multi-site harmonization, structural + diffusion baselines.

### GitHub one-line download (`ixi-hh`)

**Linux / macOS**

```bash
curl -s https://api.github.com/repos/data-others/brain/releases/tags/ixi-hh | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

**Windows PowerShell**

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-others/brain/releases/tags/ixi-hh").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

---

## 11) IXI – Guy’s Hospital (`ixi-guys`)

Site-specific subset of the **IXI Dataset**.

* **Participants:** Healthy subjects scanned at **Guy’s Hospital** (Philips 1.5T)
* **Modalities:** T1w, T2w, PD, MRA, DWI (15 directions)
* **License:** **CC BY-SA 3.0**
* **Project page:** [https://brain-development.org/ixi-dataset/](https://brain-development.org/ixi-dataset/)
* **Typical uses:** 1.5T baselines, site-comparison studies, structural + DWI benchmarks.

### GitHub one-line download (`ixi-guys`)

**Linux / macOS**

```bash
curl -s https://api.github.com/repos/data-others/brain/releases/tags/ixi-guys | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

**Windows PowerShell**

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-others/brain/releases/tags/ixi-guys").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

---

## 12) Healthy Brain Network (`hbn`)

Pediatric / adolescent **transdiagnostic** biobank (NYC).

* **Participants:** Target **10,000** children/adolescents (ages 5–21); multiple phases (baseline, follow-up, retest)
* **Data:** Multimodal MRI, EEG, psychiatric/behavioral/cognitive measures, lifestyle, genetics, actigraphy, voice/video
* **License:** CC BY-NC; follow HBN citation and DUA guidance
* **Reference:** Alexander et al., *Sci Data* 4(1), 1–26 (2017)
* **Diffusion methods (this repo SRC/FIB):** Multishell (b=1000, 2000; 64+64 dirs), TOPUP+eddy via TinyFSL + DSI Studio, RDI + GQI reconstruction (see release).
* **Typical uses:** Pediatric mental health, transdiagnostic phenotypes, method development for large pediatric data.

### GitHub one-line download (`hbn`)

**Linux / macOS**

```bash
curl -s https://api.github.com/repos/data-others/brain/releases/tags/hbn | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

**Windows PowerShell**

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-others/brain/releases/tags/hbn").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

---

## 13) Cambridge Centre for Ageing and Neuroscience (`cam-can`)

Large-scale **ageing** resource with rich cognitive and imaging data.

* **Participants:** Community adults across the adult lifespan
* **Data (this repo):**

  * FIB files (GQI reconstruction, ready for DSI Studio tracking)
  * SRC files available only to users with Cam-CAN approval (via private link on request)
* **Diffusion methods:** Multishell (b=1000 & 2000; 30+30 dirs), QC-checked b-table, GQI reconstruction (DSI Studio)
* **License:** Follows **original CamCAN agreement**: non-commercial, open-access publication, acknowledgement of CamCAN
* **Typical uses:** Ageing and connectomics, tract-specific analyses, method development on well-characterized adults.

### GitHub one-line download (`cam-can`)

**Linux / macOS**

```bash
curl -s https://api.github.com/repos/data-others/brain/releases/tags/cam-can | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

**Windows PowerShell**

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-others/brain/releases/tags/cam-can").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

---

## Quick Start

* Use the **Releases** tab to inspect per-dataset assets (archives, CSVs, FIB/SRC, metadata).
* Prefer the **one-line commands** above to mirror all assets for a given tag.
* For DSI Studio:

  * Load `.nii.gz` + `.bval` + `.bvec` **or** SRC/FIB as provided.
  * Run reconstruction (e.g., GQI/DTI), set QA/FA thresholds, then track/export.

> For reproducible pipelines, keep software versions and reconstruction parameters under version control with your outputs.

---

## Licensing & Attribution

* Each release retains its **original license / DUA** (e.g., CC BY, CC BY-NC, CC BY-NC-SA, BIRN, CC BY-SA, institutional DUA).
* Always **cite the original dataset and primary articles** listed in each section.
* If this aggregation is useful, you may add:
  *“Data access was facilitated via the `data-others/brain` repository.”*

---

## Notes & Caveats

* Some releases represent **partial** uploads or derived subsets (e.g., SRC/FIB only).
* Phenotypic and other sensitive data may require a **Data Use Agreement** (DUA) or site-specific approval.
* Anonymization / defacing policies differ across datasets; verify before face-related analyses.

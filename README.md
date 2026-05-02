# The Voynich Manuscript as a Hierarchical Formal Writing System

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19977084.svg)](https://doi.org/10.5281/zenodo.19977084)
![Status](https://img.shields.io/badge/status-research%20dossier-blue)
![License](https://img.shields.io/badge/license-CC%20BY--NC--ND%204.0-lightgrey)

**Author:** Marina Ofengeim  
**Project label:** HGN — Hierarchical Garza Notation  
**Archived version:** Research Dossier v1, May 2026  
**Zenodo DOI:** [10.5281/zenodo.19977084](https://doi.org/10.5281/zenodo.19977084)

---

## Overview

This repository supports an independent formal-first research project on the Voynich Manuscript.

The central working claim is **architectural, not decipherment-based**:

> At the current stage of evidence, the Voynich Manuscript is better modeled as a **hierarchical formal writing system** than as ordinary continuous prose, flat lexical accumulation, or simple pseudo-text.

The project studies the manuscript through formal units, positional roles, section-conditioned behavior, and page-layout structure. Semantic, historical-comparative, translation, and folio-level readings are treated as **secondary or exploratory layers** unless separately tested.

---

## Archived research dossier

The first public version of the project has been archived on Zenodo:

> **Ofengeim, Marina. _The Voynich Manuscript as a Hierarchical Formal Writing System: Hierarchical Garza Notation Research Dossier v1_. Zenodo, 2026.**  
> DOI: [10.5281/zenodo.19977084](https://doi.org/10.5281/zenodo.19977084)

The Zenodo record preserves the May 2026 state of the project, including the main architectural argument, methodological framework, working appendices, segmentation notes, interpretive workstreams, and reproducibility orientation.

---

## Core idea

The project follows a **formal-first methodology**:

1. define units of analysis;
2. test positional and distributional behavior;
3. test larger structural dependencies;
4. only then evaluate semantic, historical, or translation hypotheses.

This is intended to prevent premature conflation of:

- repetition with lexical identity;
- positional regularity with ordinary prose grammar;
- historical analogy with decipherment;
- interpretive plausibility with proof.

---

## Main architectural model

The central model is a nested hierarchy:

| Model | Description |
|---|---|
| **M0** | frequency-only baseline |
| **M1** | slot-conditioned model |
| **M2** | slot + section-conditioned model |
| **M3** | slot + section + layout model |
| **M4** | visual extension, retained as exploratory |

The main proof burden currently rests on the **M0 → M3 architectural ladder**, especially the section-conditioned step.

In the archived v1 dossier, the strongest reported architectural target is the prefix-level formal class layer:

| Metric | M0 | M3 | Direction |
|---|---:|---:|---|
| Accuracy | 0.4143 | 0.4226 | positive |
| Macro-F1 | 0.0732 | 0.1163 | positive |
| Log-loss | 1.6771 | 1.6477 | positive |

The gains are intentionally described as modest but structured. The claim is not that the manuscript has been deciphered, but that a hierarchical formal model carries more explanatory burden than flatter alternatives.

---

## Terminology

### HGN — Hierarchical Garza Notation

**HGN** is the current typological working label for the proposed system type:

- **Hierarchical** — because the main architecture is modeled through slot, section, and layout layers.
- **Garza** — used as a cautious typological name for a constrained, procedural, agglutinative-like notation hypothesis.
- **Notation** — because the manuscript is approached less as ordinary continuous prose and more as an operator-facing formal or procedural record.

This label is a working typological classification, not a claim of completed decipherment.

### RUMUZ protocol

**RUMUZ** is the project’s regime-dependent measurement framework for a small and internally heterogeneous corpus. It is used to route tests by data regime rather than flattening all manuscript zones into one ordinary-text benchmark.

### Knorozov-Dozen Protocol

The **Knorozov-Dozen Protocol** is a working positional translation and segmentation protocol. It is included as a controlled interpretive workflow, not as proof that lexical values have been established.

---

## Claim boundaries

### Public-safe claims

The current project supports the following bounded claims:

- the corpus shows slot-conditioned formal structure;
- section/page-domain assignment modulates slot behavior;
- layout/page type contributes additional structure beyond slot and section;
- hierarchical models most clearly outperform flatter alternatives on prefix-level formal targets;
- branch-level support is uneven and should not be collapsed into one uniform grammar.

### Claims not made

This project does **not** claim that:

- the Voynich Manuscript has been deciphered;
- exact lexical values have been established;
- historical etymologies are proven;
- translation tables are final;
- the visual layer is already decisive;
- all macro-domains carry equal evidence;
- the manuscript is ordinary natural-language prose.

---

## Evidence layers

The project separates evidence into zones:

| Layer | Status | Role |
|---|---|---|
| Architectural hierarchy | strongest current layer | main formal claim |
| Slot / section / layout modeling | established core direction | main evidence path |
| Formal class and family behavior | secondary support | helps characterize structure |
| Branch-level models | uneven but useful | herbal/biological stronger; pharma support-limited; cosmological mixed |
| Segmentation and translation protocols | working layer | interpretive workflow, not final proof |
| Historical comparators | exploratory / contextual | subordinate to formal evidence |
| Phi/Fibonacci signals | exploratory | retained as a bounded architectural signal, not a “golden bullet” |

---

## Provisional repository structure

This repository is intended to become a reviewer-facing and reproducibility-oriented companion to the Zenodo research dossier.

The structure below is **provisional**. It may change as files are added, reviewer packages are separated, new workstreams are stabilized, and further research clarifies which materials belong in the main repository, supplementary packages, or external archives. The directory plan should therefore be read as an initial organizing scaffold, not as a fixed final architecture.

```text
.
├── README.md
├── article/
│   └── Ofengeim_Marina_Voynich_HGN_Hierarchical_Garza_Notation_Research_Dossier_v1_May_2026.pdf
├── data/
│   ├── raw/
│   ├── normalized/
│   ├── mapping/
│   └── derived/
├── protocols/
│   ├── rumuz/
│   ├── knorozov_dozen/
│   ├── segmentation/
│   └── branch_tests/
├── scripts/
│   ├── run_all.sh
│   ├── preprocessing/
│   ├── modeling/
│   └── diagnostics/
├── outputs/
│   ├── tables/
│   ├── figures/
│   └── reports/
├── appendices/
├── notebooks/
├── citation/
│   ├── CITATION.cff
│   └── zenodo_record.md
└── LICENSE
```

As the project develops, some folders may be renamed, split, merged, or moved into separate reviewer packages. The Zenodo DOI remains the fixed archival reference for v1, while the GitHub repository may evolve as the active working and reproducibility space.

---

## Reproducibility orientation

The long-term goal of this repository is to allow independent readers to inspect and rerun:

- corpus normalization steps;
- slot / section / layout assignment tables;
- M0–M3 model comparisons;
- permutation and shuffled controls;
- branch-level diagnostics;
- segmentation batteries;
- figure and table generation;
- appendix provenance.

When code and data packages are added, the expected workflow will be documented here, for example:

```bash
git clone <repository-url>
cd <repository-name>
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
bash scripts/run_all.sh
```

Until the full reproducibility package is uploaded, the Zenodo dossier should be treated as the stable versioned reference.

---

## Suggested citation

```bibtex
@misc{ofengeim2026voynichhgn,
  author       = {Ofengeim, Marina},
  title        = {The Voynich Manuscript as a Hierarchical Formal Writing System: Hierarchical Garza Notation Research Dossier v1},
  year         = {2026},
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.19977084},
  url          = {https://doi.org/10.5281/zenodo.19977084},
  note         = {Version v1, May 2026}
}
```

---

## License

The archived dossier is licensed under:

**Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International  
(CC BY-NC-ND 4.0).**

This means the work may be shared with attribution, but may not be used commercially or distributed in modified form.

Future code files, if added, may receive a separate software license and will be marked explicitly.

---

## Project status

This is an active research project.

The current public goal is to preserve and develop the formal architecture, reproducibility packages, reviewer-facing materials, and bounded interpretive workstreams without presenting exploratory translation or historical layers as completed proof.


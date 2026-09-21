# PFOS targets and myocardial-infarction transcriptomes

Public supporting data and reproducibility materials for:

> Predicted PFOS targets and acute myocardial infarction transcriptomes: a network toxicology and nested machine-learning study

Authors: Honglei Cao, Hongyue Wang and Rongyuan Zhang.

## Repository contents

| File | Contents |
|---|---|
| `S1_Data.zip` | Standardized PFOS/MI evidence tables, machine-learning results, subset-selection locks, bootstrap analyses, enrichment results and figure source data |
| `S2_Data.zip` | Public code/model reproducibility bundle; third-party raw database exports excluded |
| `S3_Data.csv.gz` | GSE66360 normalized gene-level RMA matrix: 20,834 genes x 99 samples |
| `S4_Data.csv.gz` | GSE48060 normalized gene-level RMA matrix: 20,834 genes x 52 samples |
| `S5_Data.zip` | De-duplicated ALPL/PLAU docking reproducibility bundle, HSA/PFOS control, selected Fig4 display structures, source images, final figure exports and R assembly script |
| `THIRD_PARTY_SOURCES.csv` | URLs, access dates, queries, thresholds, standardized counts and redistribution status |
| `SHA256SUMS.csv` | File sizes and SHA-256 checksums |

## PFOS target provenance

PFOS target predictions were obtained from SwissTargetPrediction, SuperPred,
PharmMapper, STITCH and TargetNet between 26 April and 4 May 2026. Raw provider
exports are not redistributed. The public derived table records standardized human
gene symbols, per-source scores and membership indicators. The operational target
sets contained 423 broad targets, 141 targets passing at least one source-specific
high-confidence threshold and 74 targets supported by at least two sources.

## Transcriptomic data

GSE66360 and GSE48060 remain available from NCBI GEO. S3 and S4 are the processed
gene-level matrices used in the reported analyses. Sample identifiers are GEO GSM
accessions; this repository contains no direct participant identifiers.

## Docking interpretation

Docking poses and Vina scores are exploratory scoring-function outputs. The
prespecified top-ranked native-ligand redocking criterion was not met; the docking
files do not demonstrate experimental binding, specificity or functional modulation.
Figure 4 visualizes medoid top-ranked dry-pocket poses and recurrent contact distances
without changing this validation classification.

## Reuse and citation

See `DATA_LICENSE.md`, `CITATION.cff` and `THIRD_PARTY_SOURCES.csv`. Create a tagged
release and archive it with Zenodo before replacing the placeholders in
`DATA_AVAILABILITY.md` with the final repository URL and DOI.

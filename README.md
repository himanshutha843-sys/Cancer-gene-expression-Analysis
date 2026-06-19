# Breast Cancer Gene Expression Analysis

## Overview

This project performs a comprehensive transcriptomic analysis of breast cancer gene expression data using the GSE42568 dataset from the NCBI Gene Expression Omnibus (GEO). The objective is to identify differentially expressed genes, discover potential biomarkers, and investigate biological pathways associated with breast cancer progression.

---

## Dataset

**Dataset:** GSE42568 (NCBI GEO)

**Platform:** GPL570 – Affymetrix Human Genome U133 Plus 2.0 Array

### Dataset Statistics

* Total Samples: 121
* Breast Cancer Samples: 104
* Normal Breast Tissue Samples: 17
* Gene Probes: 54,675

---

## Project Workflow

### 1. Data Acquisition & Preprocessing

* Downloaded GEO Series Matrix data
* Parsed gene expression matrix
* Extracted sample metadata
* Constructed expression dataset for downstream analysis

### 2. Exploratory Data Analysis

* Principal Component Analysis (PCA)
* Sample clustering visualization
* Cancer vs Normal tissue separation analysis

### 3. Differential Expression Analysis

* Two-sample t-test
* Log Fold Change (logFC) calculation
* Benjamini–Hochberg False Discovery Rate (FDR) correction

### 4. Gene Annotation

* Probe-to-gene mapping using GPL570 annotation
* Gene symbol and functional annotation retrieval

### 5. Biomarker Discovery

Identification of highly dysregulated genes including:

* COL10A1
* NECTIN4
* MMP11
* FGFR3
* LRRC15
* HELLS

### 6. Pathway Enrichment Analysis

KEGG pathway enrichment performed using GSEApy/Enrichr.

Key enriched pathways include:

* Cell Cycle
* Focal Adhesion
* Autophagy
* FoxO Signaling Pathway
* Proteoglycans in Cancer
* p53 Signaling Pathway
* Cellular Senescence

---

## Key Results

### Differential Expression

* 17,922 significantly differentially expressed probes identified (FDR < 0.05)

### PCA Analysis

* Clear separation observed between breast cancer and normal samples.

### Top Biomarkers

* COL10A1 showed strong overexpression in tumor samples.
* MMP11 and LRRC15 were associated with extracellular matrix remodeling and tumor invasion.
* FGFR3 and NECTIN4 highlighted cancer-related signaling alterations.

### Pathway Analysis

The Cell Cycle pathway was the most significantly enriched pathway, indicating extensive dysregulation of proliferation-related genes in breast cancer tissues.

---

## Visualizations

* PCA Plot
* Volcano Plot
* Highlighted Volcano Plot
* Top Differentially Expressed Gene Heatmap
* Top 20 Biomarkers Bar Plot
* KEGG Pathway Enrichment Plot

---

## Technologies Used

* Python
* Pandas
* NumPy
* SciPy
* Statsmodels
* Matplotlib
* Seaborn
* Scikit-learn
* GSEApy

---

## Future Work

* Survival analysis using clinical datasets
* Breast cancer subtype classification
* Gene regulatory network analysis
* Drug-target discovery
* Machine learning-based cancer prediction models

---

## Author

Himanshu Thakur
B.Tech, Biosciences and Bioengineering
Indian Institute of Technology Guwahati

# Breast Cancer Gene Expression Analysis: Identification of Differentially Expressed Genes and Enriched Biological Pathways

## Abstract

Breast cancer remains one of the most prevalent malignancies worldwide. This study analyzes transcriptomic data from the GSE42568 dataset to identify genes and biological pathways associated with breast cancer. Differential expression analysis, gene annotation, and pathway enrichment analysis were performed on 121 breast tissue samples comprising 104 cancer and 17 normal samples. A total of 17,922 significantly differentially expressed probes were identified. Key biomarkers included COL10A1, NECTIN4, MMP11, FGFR3, LRRC15, and HELLS. Pathway enrichment analysis revealed significant involvement of Cell Cycle, Focal Adhesion, Autophagy, FoxO Signaling, and p53 Signaling pathways, highlighting major mechanisms underlying breast cancer progression.

## 1. Introduction

Breast cancer is a heterogeneous disease characterized by extensive molecular and genetic alterations. High-throughput gene expression profiling enables identification of dysregulated genes and pathways that contribute to tumor initiation and progression. This project investigates transcriptomic differences between breast cancer and normal breast tissue using publicly available microarray data.

## 2. Dataset Description

* Dataset: GSE42568
* Platform: GPL570
* Samples: 121
* Breast Cancer Samples: 104
* Normal Samples: 17
* Probes: 54,675

The dataset contains expression measurements from breast cancer biopsies and normal breast tissues obtained using the Affymetrix Human Genome U133 Plus 2.0 microarray platform.

## 3. Methodology

### 3.1 Data Preprocessing

* GEO series matrix extraction
* Expression matrix generation
* Sample labeling

### 3.2 Principal Component Analysis

PCA was applied to visualize global transcriptomic differences between cancer and normal tissues.

### 3.3 Differential Expression Analysis

* Two-sample t-tests
* Log fold-change computation
* Benjamini-Hochberg FDR correction

### 3.4 Gene Annotation

Probe IDs were mapped to gene symbols using GPL570 annotation files.

### 3.5 Pathway Enrichment Analysis

KEGG pathway enrichment was performed using GSEApy Enrichr.

## 4. Results

### 4.1 PCA Analysis

PCA demonstrated distinct clustering of breast cancer and normal samples, indicating significant transcriptomic differences.

### 4.2 Differential Expression Analysis

A total of 17,922 probes were significantly differentially expressed (FDR < 0.05).

### 4.3 Top Differentially Expressed Genes

| Gene    | logFC |
| ------- | ----- |
| COL10A1 | 3.59  |
| NECTIN4 | 1.86  |
| MMP11   | 3.40  |
| FGFR3   | 2.82  |
| LRRC15  | 3.64  |
| HELLS   | 2.11  |

### 4.4 Pathway Enrichment

Top enriched pathways:

1. Cell Cycle
2. Focal Adhesion
3. Autophagy
4. FoxO Signaling
5. Proteoglycans in Cancer
6. p53 Signaling Pathway

## 5. Discussion

The identified biomarkers are consistent with known mechanisms of breast cancer progression. COL10A1 and MMP11 are involved in extracellular matrix remodeling and tumor invasion, while FGFR3 participates in proliferative signaling. Enrichment of Cell Cycle and p53 signaling pathways further supports the biological relevance of the findings.

## 6. Conclusion

This study successfully identified significant transcriptomic alterations associated with breast cancer. Integration of differential expression analysis, gene annotation, and pathway enrichment revealed key biomarkers and pathways involved in disease progression. These findings provide a foundation for future biomarker discovery and computational oncology studies.

## References

1. Clarke C. et al. Carcinogenesis (2013).
2. NCBI GEO Database – GSE42568.
3. Affymetrix GPL570 Platform Annotation.
4. GSEApy Documentation.

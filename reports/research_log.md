Date: 17 june 2026
Dataset: GSE42568
What I learned: convert the micro array data to readable and editable data for 
               further analysis
               
Problems faced: dont know that much about pandas functions yet

Next steps: currently rows = genes
                      columns = samples

                      they need to interchange

======================================================================================
Date: 17 June 2026

Dataset:
GSE42568

Progress:
Loaded 54,675 probe measurements across 121 samples.
Created sample labels.
Performed PCA analysis.

Observation:
Cancer and normal samples showed (strong/moderate/weak)
separation in PCA space.

Next:
Differential Gene Expression Analysis.


=======================================================================================

Date : 18 June 2026

Dataset:
GSE42568

Progress:



# Research Log

## Project Title

Breast Cancer Gene Expression Analysis using Transcriptomic Data

---

## Objective

To identify differentially expressed genes and enriched biological pathways associated with breast cancer using publicly available transcriptomic datasets from NCBI GEO.

---

## Dataset Selection

Dataset Chosen:

* GSE42568

Reason:

* Publicly available breast cancer transcriptomic dataset.
* Contains both cancer and normal breast tissue samples.
* Suitable sample size for differential expression analysis.

---

## Day 1: Data Acquisition and Preprocessing

Completed:

* Downloaded GSE42568 series matrix file.
* Extracted expression matrix.
* Parsed GEO metadata.
* Identified sample labels.
* Constructed gene expression dataset.

Observations:

* Dataset contains 121 samples.
* 104 breast cancer samples.
* 17 normal breast tissue samples.

---

## Day 2: Exploratory Data Analysis

Completed:

* Principal Component Analysis (PCA).
* Sample visualization.

Results:

* Clear separation between cancer and normal samples.
* Distinct transcriptomic profiles observed.

Output:

* pca_breast_cancer.png

---

## Day 3: Differential Expression Analysis

Completed:

* Two-sample t-tests.
* Log Fold Change calculations.
* Benjamini-Hochberg FDR correction.

Results:

* 17,922 significant probes identified (FDR < 0.05).

Outputs:

* significant_genes.csv
* volcano_plot.png
* volcano_plot_highlighted.png

---

## Day 4: Gene Annotation

Completed:

* Downloaded GPL570 annotation file.
* Mapped probe identifiers to gene symbols.
* Generated annotated results table.

Outputs:

* significant_genes_annotated.csv
* top20_genes.csv

Key Genes:

* COL10A1
* NECTIN4
* MMP11
* FGFR3
* LRRC15
* HELLS

---

## Day 5: Biological Interpretation

Completed:

* Top biomarker investigation.
* Literature-supported interpretation of candidate genes.

Key Findings:

* COL10A1 associated with extracellular matrix remodeling.
* MMP11 linked to tumor invasion.
* FGFR3 involved in growth signaling.
* LRRC15 associated with tumor microenvironment remodeling.

---

## Day 6: Pathway Enrichment Analysis

Completed:

* KEGG pathway enrichment using GSEApy.

Significant Pathways:

1. Cell Cycle
2. Focal Adhesion
3. Autophagy
4. FoxO Signaling Pathway
5. Proteoglycans in Cancer
6. p53 Signaling Pathway

Output:

* pathway_enrichment.csv
* pathway_enrichment.png

---

## Current Status

Completed:

* Data Processing
* PCA
* Differential Expression
* Volcano Plot Analysis
* Heatmap Analysis
* Gene Annotation
* Biomarker Discovery
* Pathway Enrichment

Repository Status:
Version 1.0 Complete

---

## Future Work

* Survival analysis
* Gene regulatory network analysis
* Machine learning classification
* Drug target prediction
* Breast cancer subtype analysis
* Publication-style report preparation

---

## Author

Himanshu Thakur

B.Tech, Biosciences and Bioengineering

Indian Institute of Technology Guwahati


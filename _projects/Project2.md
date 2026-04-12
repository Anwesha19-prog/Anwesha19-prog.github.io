---
title: "RNA-seq Differential Expression SARS-CoV-2"
excerpt: "Project demonstrating RNA-seq DE analysis, metadata engineering, and QC in Python."
author_profile: true

date: 2026-04-10

# Shows a big banner image at the top (hero)
header:
  overlay_image: /assets/images/Projects/hero-project2.png
  overlay_filter: 0.35
  caption: "Figure: PCA for sample clustering."

# Shows a small thumbnail on the /projects/ grid page
teaser: /assets/images/Projects/hero-project2.png

# Optional: nice wide layout for projects with images
classes: wide

# If you want a table-of-contents on the right
toc: true
toc_sticky: true
---

## Overview

This project demonstrates an end-to-end RNA-seq differential expression (DE) workflow in Python using pydeseq2 (DESeq2-like negative binomial modeling). The notebook covers:
- loading and validating a raw count matrix
- constructing metadata from GEO annotations (Series Matrix)
- running DE with an explicit contrast
- QC/visualization (PCA, clustered heatmap)
- exporting results for downstream interpretation

- Links: [GitHub](https://github.com/Anwesha19-prog/RNA-seq-Differential-Expression)
- Status: Complete

## Why this project
This project asks which human genes change expression in SARS‑CoV‑2 positive vs negative samples (GSE152075) using a proper RNA‑seq DE workflow with pyDESeq2, producing interpretable QC and results visuals

## Highlights
- Differential expression (pydeseq2)
  - Count-based modeling using a negative binomial GLM
  - Multiple testing correction (FDR / adjusted p-values)
  - Results table extraction via DeseqStats(...).results_df

- QC and visualization
  - PCA to inspect global sample structure (and detect technical effects)
  - Heatmap / clustermap of top DE genes (pattern-level interpretation)

## Result
|Figure|
|---|
|![Volcano Plot]({{ site.baseurl }}/assets/images/Projects/project2-volcano.png)<br><small>*Figure 1: Volcano plot Tumor vs Normal*</small>|
|![PCA Plot]({{ site.baseurl }}/assets/images/Projects/project2-pca.png)<br><small>*Figure 2: PCA plot Tumor vs Normal*</small>|
|![Top Genes]({{ site.baseurl }}/assets/images/Projects/project2-topgenes.png)<br><small>*Figure 3: Top 20 genes based on p-value*</small>|

## How to run
git clone https://github.com/Anwesha19-prog/RNA-seq-Differential-Expression <br>
cd RNA-seq-Differential-Expression <br>
pip install pandas numpy matplotlib seaborn scikit-learn pydeseq2<br>
jupyter notebook Project-2_clean.ipynb

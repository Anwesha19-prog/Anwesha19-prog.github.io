---
title: "Multi omics integration (TCGA-BRCA)"
excerpt: "Project integrating TCGA-BRCA multi-omics profiles—gene expression (RNA-seq), DNA methylation (450K), and copy-number variation (CNV)."
author_profile: true

date: 2026-04-11

# Shows a big banner image at the top (hero)
header:
  overlay_image: /assets/images/Projects/project3-marker_expression_by_cluster.png
  overlay_filter: 0.35
  caption: "Figure: PCA for sample clustering."

# Shows a small thumbnail on the /projects/ grid page
teaser: /assets/images/Projects/project3-marker_expression_by_cluster.png

# Optional: nice wide layout for projects with images
classes: wide

# If you want a table-of-contents on the right
toc: true
toc_sticky: true
---

## Overview

This repository contains a single, end-to-end Python notebook that integrates The Cancer Genome Atlas (TCGA) Breast Cancer (BRCA) multi-omics profiles—gene expression (RNA-seq), DNA methylation (450K), and copy-number variation (CNV) — to discover unsupervised patient groups and interpret them biologically.

## Why this project

## Highlights

- Multi-omics data handling (RNA + methylation + CNV)
- Sample harmonization with TCGA barcodes
- Robust preprocessing and missing-value handling
- Dimensionality reduction (PCA) and integration (early integration of PCs)
- Unsupervised clustering with model selection (silhouette)
- Biological interpretation via:

    - canonical marker genes,
    - CNV driver loci inspection,
    - pathway enrichment (Hallmark)


## Result

|Figure|
|---|
|![CNV key genes]({{ site.baseurl }}/assets/images/Projects/project3-cnv-key-genes.png)<br><small>*Figure 1: CNV of key genes by cluster*</small>|
|![Embedding clusters]({{ site.baseurl }}/assets/images/Projects/project3-embedding_clusters.png)<br><small>*Figure 2: Integrated multi-omics embedding (colored by cluster)*</small>|
|![Marker expression]({{ site.baseurl }}/assets/images/Projects/project3-marker_expression_by_cluster.png)<br><small>*Figure 3: Marker gene expression by multi-omics cluster*</small>|
|![Survival rate]({{ site.baseurl }}/assets/images/Projects/project3-survival.png)<br><small>*Figure 4: Overall survival by multi-omics cluster (TCGA BRCA)*</small>|

## How to run

git clone https://github.com/Anwesha19-prog/TCGA-BRCA-Multi-Omics-Intergration <br>
cd TCGA-BRCA-Multi-Omics-Intergration <br>
python -m requirements.txt <br>
jupyter notebook Project-3.ipynb
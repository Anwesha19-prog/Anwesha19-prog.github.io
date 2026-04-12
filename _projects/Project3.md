---
title: "Multi omics integration (TCGA-BRCA)"
excerpt: "Project integrating TCGA-BRCA multi-omics profiles—gene expression (RNA-seq), DNA methylation (450K), and copy-number variation (CNV)."
author_profile: true

date: 2026-04-10

# Shows a big banner image at the top (hero)
header:
  overlay_image: /assets/images/Projects/hero-project3.png
  overlay_filter: 0.35
  caption: "Figure: PCA for sample clustering."

# Shows a small thumbnail on the /projects/ grid page
teaser: /assets/images/Projects/hero-project3.png

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

## How to run
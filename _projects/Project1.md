---
title: "Breast cancer microarray analysis"
excerpt: "Bioinformatics project demonstrating transcriptomics data wrangling + analysis."
date: 2026-04-10

# Shows a big banner image at the top (hero)
header:
  overlay_image: /assets/images/Projects/hero-project1.png
  overlay_filter: 0.35
  caption: "Figure: PCA for sample clustering."

# Shows a small thumbnail on the /projects/ grid page
teaser: /assets/images/Projects/hero-project1.png

# Optional: nice wide layout for projects with images
classes: wide

# If you want a table-of-contents on the right
toc: true
toc_sticky: true
---

## At a glance

### Overview
This notebook demonstrates an end-to-end gene expression analysis workflow starting from a raw GEO Series Matrix file. The focus is on a core real-world bioinformatics skill: turning “messy” public repository files into analysis-ready matrices and metadata, then performing basic differential expression and exploratory analysis.

Although the dataset is public and compact, the same workflow scales to large transcriptomics studies and is directly applicable in oncology pipelines.

- Links: [GitHub](https://github.com/Anwesha19-prog/Breast-Cancer-Microarray-Analysis).
- Status: Complete

## Why this project
This project demonstrates a reproducible end-to-end gene expression analysis workflow turning chaotic public repository data into analysis-ready matrices and metadata.

## Highlights
- Parsing GEO Series Matrix structure:
  - detecting !series_matrix_table_begin / !series_matrix_table_end
  - separating metadata lines from expression table
- Building a clean expression matrix:
  - rows = genes
  - columns = samples
- Extracting phenotype labels (Tumor vs Normal) from sample characteristics

## Results (put 1–2 key figures)
![Volcano Plot]({{ site.baseurl }}/assets/images/Projects/project1-volcano.png)

![Top Genes]({{ site.baseurl }}/assets/images/Projects/project1-topgenes.png)

## How to run
git clone https://github.com/Anwesha19-prog/Breast-Cancer-Microarray-Analysis <br>
cd Breast-Cancer-Microarray-Analysis <br>
pip install pandas numpy scipy matplotlib seaborn scikit-learn<br>
jupyter notebook Project-1_clean.ipynb

---
title: "3D-Spheroid-Image-Segmentation-Uptake-Analysis"
excerpt: "Project developed to identify spheroids from microscopic Images and analyze ICG uptake"
author_profile: true

date: 2023-10-10

# Shows a big banner image at the top (hero)
header:
  overlay_image: /assets/images/Projects/project4_hero.jpg
  overlay_filter: 0.35
  caption: "[Source](https://idea-bio.com/how-to-efficiently-conduct-3d-spheroid-imaging/)"

# Shows a small thumbnail on the /projects/ grid page
teaser: /assets/images/project4-hero.jpg

# Optional: nice wide layout for projects with images
classes: wide

# If you want a table-of-contents on the right
toc: true
toc_sticky: true
---

## Overview

Quantitative analysis of 3D spheroid/organoid microscopy images to measure morphology and fluorescence/intensity statistics in user-defined offset regions (e.g., shells/rings around a spheroid). Designed for both biologists (easy-to-run workflow, clear outputs) and image-analysis users (tunable segmentation parameters).

- Links: [Github](https://github.com/Anwesha19-prog/3D-Spheroid-Organoid_Analysis_Image_Analysis)
- Status: Complete

## Why this project

This project provides a simple MATLAB workflow to segment spheroid/organoid images and quantify ROI intensity metrics (including user-defined offset regions) with results exported to Excel for fast, reproducible analysis.

## Highlights

Given a single-channel .tif image containing a spheroid/organoid, the pipeline:

- Segments the spheroid region of interest (ROI)
- Optionally fills holes / removes small noise components
- Computes intensity metrics within the ROI and within regions defined by an offset length

![Image analysis pipeline]({{ site.baseurl }}/assets/images/Projects/project4_result.png)<br><small>*Figure 1: Sample image analysis pipeline*</small>

## Result

The program exports an Excel file including:
    - Offset value (μm)
    - Area of ROI (pixels)
    - Total / Integrated intensity
    - Mean intensity
    - Median intensity
    - Standard deviation of intensity
    - Maximum intensity

## How to run
- MATLAB (tested in a standard MATLAB environment)
- Input images must be TIF/TIFF (.tif) format
  > paCurrent workflow assumes images have equal height and width (square images), or at least the same pixel count in both directions.



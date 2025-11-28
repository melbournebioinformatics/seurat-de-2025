---
title: 'Introduction'
teaching: 10
exercises: 2
---

::::::::::::::::::::::::::::::::::::: questions

- How to perform differential expression analysis with Seurat?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

-   Gain more familiarity with standard scRNA-seq Quality Control (QC) steps.
-   Understand and get comfortable using various integration strategies (`harmoy` and `seuratCCA`).
-   Understand when and how to use all of the differential expression functions offered by Seurat: `FindMarkers()`, `FindConservedMarkers()`, and `FindAllMarkers()`.
-   Learn how to use differential expression tools meant for bulk data, like DESeq2, for single-cell 'pseudobulk' data and understand why you might choose this approach.
-   Learn different ways to visualise both in-built Seurat functions and  external packages like pheatmap.

::::::::::::::::::::::::::::::::::::::::::::::::


:::: callout

This tutorial is partially based on existing
material from:

* https://satijalab.org/seurat/articles/seurat5_integration
* https://satijalab.org/seurat/articles/de_vignette
* https://hbctraining.github.io/scRNA-seq_online/
* https://bookdown.org/ytliu13207/SingleCellMultiOmicsDataAnalysis/

::::

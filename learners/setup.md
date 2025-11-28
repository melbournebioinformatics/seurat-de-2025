---
title: Setup
---

:::: prereq

Some knowledge of R and scRNA-seq analysis is assumed. We recommend reviewing the following materials before the starting the materials:
- [Introduction to R](https://mbite.org/intro-to-r/)
- [10X single-cell RNA-seq analysis in R](https://mbite.org/tutorials/singlecell/)

Please see our [Intro to R](https://mbite.org/intro-to-r/) and [RNA-seq: counts to genes](https://mbite.org/intro-to-r/) workshops if you need a refresher.

::::


## Data Sets


[Click here to download the RData object](../episodes/data/ifnb.RData) that will be used for this workshop.


## Software Setup

## RStudio Setup

We use RStudio for coding in R.

[Click here and follow the instructions](https://posit.co/download/rstudio-desktop/) to install RStudio Desktop in your system.

::::::::::::::::: discussion

### R packages

**Run the code block below to install the packages needed for this
workshop.**

To check if installed properly, load each package in one at a time using
the `library()` function.


``` r
install.packages('Seurat')

if (!requireNamespace("remotes", quietly = TRUE)) {
  install.packages("remotes")
}
remotes::install_github("satijalab/seurat-data", quiet = TRUE)

if (!require("BiocManager", quietly = TRUE)) {
  install.packages("BiocManager")
}
BiocManager::install("DESeq2")
BiocManager::install("multtest") # dependency commonly missing
BiocManager::install(c("SingleR", "celldex"))
install.packages("harmony") # dependency needed for harmony analysis

install.packages("tidyverse")
install.packages("pheatmap")
install.packages("metap")
install.packages("ggplot2")


```


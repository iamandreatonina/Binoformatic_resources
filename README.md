# Bioninformatic Resources Project

Project in R for the course of Bioinformatic Resources, held by Alessandro Romanel (A.Y. 2022-2023).

Topic: Perform an analysis of the selected dataset representing RNA-seq count data extracted from different cancer datasets from the Cancer Genome Atlas (TCGA).

Dataset selected: [Thyroid carcinoma](https://github.com/iamandreatonina/Binoformatic_resources/tree/main/file)

[Report (both in Rmd and HTML) ](https://github.com/iamandreatonina/Binoformatic_resources/edit/main/Report)

## Authors 

Project developed by:
 * Andrea Tonina [@iamandreatonina](https://github.com/iamandreatonina)
 * Gloria Lugoboni [@GloriaLugoboni](https://github.com/GloriaLugoboni)

## Tasks 

* Load the RData file
* Extract only protein-coding genes
* Perform differential expression analysis using [`edgeR`](https://bioconductor.org/packages/release/bioc/html/edgeR.html) package and select up-b and down-regulated genes using a p-value cutoff of 0.01, a log fold change ratio >1.5 for up-regulated genes and < (-1.5) for down-regulated genes, and a log CPM >1. 


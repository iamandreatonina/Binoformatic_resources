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

* Load the RData file.
* Extract only protein-coding genes.
* Perform differential expression analysis using [`edgeR`](https://bioconductor.org/packages/release/bioc/html/edgeR.html) package and select up-b and down-regulated genes using a p-value cutoff of 0.01, a log fold change ratio >1.5 for up-regulated genes and < (-1.5) for down-regulated genes, and a log CPM >1.
* Perform gene set enrichment analysis using [`clusterProfiler`](https://bioconductor.org/packages/release/bioc/html/clusterProfiler.html).
* Visualize one pathway you find enriched using the upregulated gene list by utilizing [`pathview`](9https://www.bioconductor.org/packages/release/bioc/html/pathview.html).
* Identify which transcription factors (TFs) have enriched scores in the promoters of all up-regulated genes.
* Select one among the top enriched TFs, compute the empirical distributions of scores for all PWMs that you find in MotifDB for the selected TF, and determine for all of them the distribution (log2) threshold cutoff at 99.75%.
* Identify which up-regulated genes have a region in their promoter with binding scores above the computed thresholds for any of the previously selected PWMs.
9. Find PPI interactions among differentially expressed genes by using [STRING](https://string-db.org/) and export the network in TSV format.
10. Import the network by using [`igraph`](https://cran.r-project.org/web/packages/igraph/index.html) package and identify and plot the largest connected component ( we also decided to use [`ggnet2`](https://ggobi.github.io/ggally/reference/ggnet2.html) from [`GGally`](https://cran.r-project.org/web/packages/GGally/index.html) package).  


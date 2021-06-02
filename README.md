# **VTA snRNA-seq**


This page contains R code for analysis of single-nucleus RNA-seq (snRNA-seq) datasets from "_An atlas of transcriptionally defined cell populations in the rat ventral tegmental area_".  R objects containg UMAP coordindates and other metadata characteristics for the complete dataset and neuronal subclustering are available upon request. 


## **Study design**

This snRNA-seq dataset was generated from VTA punches from naive adult male and female Sprague Dawley rats.  

Datasets in this preprint used the 10X Genomics Chromium Single Cell Next GEM 3’ library construction kit to generate barcoded libraries for Illumina sequencing. For each dataset, we provide R Markdown and Word documents containing analysis parameters and code.  


## **Citation**

Phillips III, R.A.* Tuscher, J.J.*, Black, S.L., Ianov, L., & Day, J.J. (2021). An atlas of transcriptionally defined cell populations in the rat ventral tegmental area. *bioRxiv* DOI:
[Link]()


## **Links**

All Day lab resources may be found at the [Day Lab website](http://day-lab.org/resources)  
[Ratlas Shiny App](https://day-lab.shinyapps.io/ratlas/)  
[BioRxiv preprint](https://www.biorxiv.org/content/10.1101/2021.06.02.446737v1)  


## **Raw data**

GEO accession [GSE168156](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE168156)  


## **Source code**
All packages required for reproduction of this analysis are included in the session info section of the word doc included in this repository.
[Seurat v3.2.2](https://github.com/satijalab/seurat)  

## **Docker image**
A Docker image containing all depedencies needed to reproduce the analysis from the code present in this repository: [Day lab VTA Docker image](https://hub.docker.com/r/daylabprojects/daylab_rat_vta_snrna)

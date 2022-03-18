# **VTA snRNA-seq**


This page contains R code for analysis of single-nucleus RNA-seq (snRNA-seq) datasets from "_An atlas of transcriptionally defined cell populations in the rat ventral tegmental area_".  R objects containing UMAP coordinates and other metadata characteristics for the complete dataset and neuronal sub-clustering are available upon request. 


## **Study design**

This snRNA-seq dataset was generated from VTA punches from naive adult male and female Sprague Dawley rats.  

Datasets in this preprint used the 10X Genomics Chromium Single Cell Next GEM 3’ library construction kit to generate barcoded libraries for Illumina sequencing. For each dataset, we provide R Markdown and Word documents containing analysis parameters and code.  


## **Citation**

Phillips III, R.A.* Tuscher, J.J.*, Black, S.L., Ianov, L., & Day, J.J. (2021). An atlas of transcriptionally defined cell populations in the rat ventral tegmental area. *bioRxiv* DOI: 10.1101/2021.06.02.446737
[Link](https://www.biorxiv.org/content/10.1101/2021.06.02.446737v1)


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

The Dockerfile associated with this image can be found [here](https://github.com/Jeremy-Day-Lab/VTA_Dockerfiles/blob/master/Dockerfile_additional_seurat_dependencies/Dockerfile)

Overall this image contains the minimum dependencies to reproduce the Day lab VTA analysis code, and a number of additional Seurat dependencies which were not used in the analysis (e.g.: DESeq2, multtest, metap which are needed for specific differential expression parameters or functions such as `FindConservedMarkers`) but can aid in the utilization of the container for exploratory purposes.
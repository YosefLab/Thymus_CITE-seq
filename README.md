# Thymus_CITE-seq

## Single-cell multi-omic analysis of thymocyte development reveals drivers of CD4/CD8 lineage commitment
Zoë Steier, Dominik A. Aylard, Laura L. McIntyre, Isabel Baldwin, Esther Jeong Yoon Kim, Lydia K. Lutes, Can Ergen, Tse-Shun Huang, Ellen A. Robey, Nir Yosef, Aaron Streets

Nature Immunology, 2023. https://doi.org/10.1038/s41590-023-01584-0

This repository contains code for the analysis performed in this manuscript.

The CITE-seq data generated in this manuscript are accessible through GEO: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE186078.

The thymus CITE-seq data set can be explored interactively with Vision:
  - Positive selection subset: http://s133.cs.berkeley.edu:9001/Results.html
  - Full data set: http://s133.cs.berkeley.edu:9002/Results.html

## Analysis notebooks

* __totalVI_AllData/__ 
  * ```Filtering_thymus111.ipynb``` Data preparation and filtering prior to running totalVI on the full CITE-seq data set
  * ```totalVI_thymus111.ipynb``` Run totalVI on the full data set
    
* __totalVI_PositiveSelection/__ 
  * ```Filtering_thymus111_posselecting.ipynb``` Data preparation and filtering prior to running totalVI on the positive selection subset of the data
  * ```totalVI_thymus111_posselecting.ipynb```  Run totalVI on the positive selection subset of the data
    
* __Annotation/__ 
  * ```Annotation.ipynb``` Annotation of the full data set and the positive selection subset (run alongside the totalVI notebooks)
    
* __Pseudotime/__ 
  * ```Slingshot_thymus_posselecting_filtered.Rmd``` Run Slingshot to generate pseudotime (run alongside differential expression notebooks to plot DE results over pseudotime)
  * ```Pseudotime_plotting.Rmd``` Plotting of pseudotime results and in silico FACS analysis
    
* __Differential_Expression/__ 
  * ```totalVI_thymus111_DE_bintime.ipynb``` Run differential expression tests with totalVI and generate gene clusters
  * ```DE_analysis.Rmd``` Analyze differential expression results and perform trancription factor enrichment analysis

* __Multidimensional_Flow/__ 
  * ```Multidimensional_Flow.ipynb``` Multidimensional flow analysis
 
* __Vision/__ 
  * ```Vision_AllData.Rmd``` Run Vision to generate session for interactive exploration of the full CITE-seq data set
  * ```Vision_PositiveSelection.Rmd``` Run Vision to generate session for interactive exploration of the positive selection subset of the data

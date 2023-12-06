
<!-- README.md is generated from README.Rmd. Please edit that file -->

# 2023_Nicolosi-Gelis_et_al

## Overview

In this repository, you will find two tutorials:
<br/>i. one explaining how we processed metabarcoding data (rRNA 16S and 23S) to report on the genetic diversity of phytoplankton in four French peri-alpine lakes. 
<br/>ii. another explaining the subsequent statistical analyzes performed with metabarcoding data.

Data analysis was done using R version 4.2.1. This document was compiled with the rmarkdown package version 2.8. This tutorial is licensed under CC BY-NC-ND 4.0, which means you are free to share, copy and redistribute this tutorial in any medium or format under the terms of attribution of appropriate credit, non-commercial purposes and no derivatives.

The data were produced as part of the article:

>Nicolosi Gelis M.M., A. Canino, A. Bouchez, I. Domaizon, C. Laplace-Treyture, F. Rimet, B. Alric. Assessing the relevance of DNA metabarcoding compared to morphological identification for lake phytoplankton monitoring, submitted to the journal *Science of the Total Environment*.

## Utilization

i. We can access the script for bioinformatic analyzes [here](https://raw.githack.com/benalric/2023_Nicolosi-Gelis_STOTEN/main/DADA2_pipeline_phytoplankton_16S_23S.html)
<br/>ii. We can access the script for statistical analyzes [here](https://raw.githack.com/benalric/2023_Nicolosi-Gelis_STOTEN/main/Statistical_analysis_phytoplankton.html)

## Version of packages used to create the web application
```r
sessionInfo()

R version 4.2.1 (2022-06-23 ucrt)
Platform: x86_64-w64-mingw32/x64 (64-bit)
Running under: Windows 10 x64 (build 19044)

Matrix products: default

locale:
[1] LC_COLLATE=French_France.utf8  LC_CTYPE=French_France.utf8    LC_MONETARY=French_France.utf8 LC_NUMERIC=C                  
[5] LC_TIME=French_France.utf8    

attached base packages:
[1] stats4    stats     graphics  grDevices utils     datasets  methods   base     

other attached packages:
 [1] ShortRead_1.56.1            GenomicAlignments_1.34.0    SummarizedExperiment_1.28.0 Biobase_2.58.0             
 [5] MatrixGenerics_1.10.0       matrixStats_0.63.0          Rsamtools_2.14.0            GenomicRanges_1.50.1       
 [9] Biostrings_2.66.0           GenomeInfoDb_1.34.3         XVector_0.38.0              IRanges_2.32.0             
[13] S4Vectors_0.36.0            BiocParallel_1.32.3         BiocGenerics_0.44.0         dada2_1.26.0               
[17] Rcpp_1.0.9                  ggplot2_3.4.0               adegraphics_1.0-16          vegan_2.6-4                
[21] lattice_0.20-45             permute_0.9-7               tibble_3.1.8                ade4_1.7-20                
[25] DiagrammeR_1.0.9            tidyr_1.2.1                 dplyr_1.0.10               

loaded via a namespace (and not attached):
 [1] jsonlite_1.8.3         splines_4.2.1          RcppParallel_5.1.5     sp_1.5-1               latticeExtra_0.6-30   
 [6] GenomeInfoDbData_1.2.9 yaml_2.3.6             pillar_1.8.1           glue_1.6.2             digest_0.6.30         
[11] RColorBrewer_1.1-3     colorspace_2.0-3       plyr_1.8.8             htmltools_0.5.3        Matrix_1.5-3          
[16] pkgconfig_2.0.3        bookdown_0.30          zlibbioc_1.44.0        purrr_0.3.5            scales_1.2.1          
[21] jpeg_0.1-10            mgcv_1.8-40            generics_0.1.3         withr_2.5.0            cli_3.4.1             
[26] magrittr_2.0.3         crayon_1.5.2           deldir_1.0-6           evaluate_0.18          fansi_1.0.3           
[31] nlme_3.1-157           MASS_7.3-57            hwriter_1.3.2.1        rsconnect_0.8.29       tools_4.2.1           
[36] lifecycle_1.0.3        stringr_1.4.1          interp_1.1-3           munsell_0.5.0          DelayedArray_0.24.0   
[41] cluster_2.1.3          compiler_4.2.1         rlang_1.0.6            grid_4.2.1             RCurl_1.98-1.9        
[46] rstudioapi_0.14        htmlwidgets_1.5.4      visNetwork_2.1.2       bitops_1.0-7           rmarkdown_2.18        
[51] codetools_0.2-18       gtable_0.3.1           DBI_1.1.3              reshape2_1.4.4         R6_2.5.1              
[56] knitr_1.41             fastmap_1.1.0          utf8_1.2.2             KernSmooth_2.23-20     stringi_1.7.8         
[61] parallel_4.2.1         rmdformats_1.0.4       vctrs_0.5.1            png_0.1-8              tidyselect_1.2.0      
[66] xfun_0.35          
```

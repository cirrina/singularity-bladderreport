# singularity-bladderreport
Singularity container to use for uroscan bladderreport. Include R v3.4 and some extras.

This container will only include R, r packeges and other associated libraries that are needed to generate the bladder report.
It will not iclude software for RNAseq analysis.


The main goal is to get include following versions:
r-base=3.4.1 \
r-ranger=0.7.0 \
r-dplyr=0.7.4


Optinally:
r-knitr=1.16
vladsaveliev::r-kableextra=0.9.0
r-jsonlite=1.4

r-reshape=0.8.6
r-ggplot2=2.2.0
r-cowplot=0.9.1



  Also include
  - lynx

  

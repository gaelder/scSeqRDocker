# scSeqRDocker
Creation of a Docker image for single cell RNA sequencing with R using BioConductor and Seurat packages

# Why I'm not using a rocker image as a base.
Installation of the R package ddalpha is the source of this idiosyncracy. If I used the dockerhub image
of rocker/r-ver:3.5.0 my Ubuntu 16.04 OS would hang. However, if I built the rocker/r-ver:3.5.0 image
locally it would not. From there it seemed logical to append my other changes to my forked copy of the rockerimage.

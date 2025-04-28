
# morphogb

**Glioblastoma stem cell morphotypes convey distinct cell states and clinically relevant functions**

This repository contains the code to reproduce the analysis presented in Barelli *et al.*, 
"Glioblastoma stem cell morphotypes convey distinct cell states and clinically relevant functions".

### Transcriptomics Data Analysis with Nanostring GeoMX

The analysis was conducted using Python and various libraries. A complete environment for the 
analysis is available in the Docker container `nfdata/workbench:sc-1.2.2`, which can be found on DockerHub.
The relevant notebooks to reproduce the results and the figures of the article are contained in the 
`geomx` folder. The analysis is based on the Nanostring GeoMX data, which is contained in the
`geomx/data` folder.


An html version of the notebooks is accessible [here](https://KalebicLab.github.io/morphogb/).




## Preliminary exploration of geomx dataset

Links: [jupyter notebook](geomx/01_geomx_analysis.ipynb) and [html file](https://KalebicLab.github.io/morphogb/geomx/01_geomx_analysis.html).

This notebook contains a preliminary exploration of the spatial transcriptomics data,
including steps such as data loading, quality control, and exploratory dimensionality reduction.




## Differential expression analysis

Links: [jupyter notebook](geomx/02_geomx_differential_expression.ipynb) and [html file](https://KalebicLab.github.io/morphogb/geomx/02_geomx_differential_expression.html).

This notebook focuses on the differential expression analysis of the spatial transcriptomics data,
using PyDeseq2 for model definition and statistical testing. Differentially expressed genes are identified
and then further anlyzed with Over Representation Analysis (ORA) and Gene Set Enrichemnt Analyses (GSEA) 
to characterize their biological relevance.




## Biological Pathway Deconvolution

Links: [jupyter notebook](geomx/03_geomx_biolocal_pathway_deconvolution.ipynb) and [html file](https://KalebicLab.github.io/morphogb/geomx/03_geomx_biolocal_pathway_deconvolution.html).

This notebook applies the Biological Pathway Deconvolution (BPD) method using the single-sample 
Mann-Whitney-Wilcoxon Gene-Set Test (ss-MWWGST). This approach enables the characterization of 
spatial transcriptomics data by assessing the enrichment of various gene set databases,
while minimizing inter-patient variability.





---
*Note: this README file has been generated automatically.* <br>
*Please do not modify it directly but instead work on [this config file](resources/config.yaml).*



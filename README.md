
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

Links: [jupyter notebook](geomx/02_differential_expression_analysis.ipynb) and [html file](https://KalebicLab.github.io/morphogb/geomx/02_differential_expression_analysis.html).

This notebook focuses on the differential expression analysis of the spatial transcriptomics data,
using PyDeseq2 for model definition and statistical testing. Differentially expressed genes are identified
and then further anlyzed with Over Representation Analysis (ORA) and Gene Set Enrichemnt Analyses (GSEA) 
to characterize their biological relevance.




## Biological Pathway Deconvolution

Links: [jupyter notebook](geomx/03_biological_pathway_deconvolution.ipynb) and [html file](https://KalebicLab.github.io/morphogb/geomx/03_biological_pathway_deconvolution.html).

This notebook applies the Biological Pathway Deconvolution (BPD) method using the single-sample 
Mann-Whitney-Wilcoxon Gene-Set Test (ss-MWWGST). This approach enables the characterization of 
spatial transcriptomics data by assessing the enrichment of various gene set databases,
while minimizing inter-patient variability.




## Convert Richards 2021 dataset to h5ad

Links: [jupyter notebook](public_dataset_analysis/convert_Richards_2021_to_h5ad.ipynb) and [html file](https://KalebicLab.github.io/morphogb/public_dataset_analysis/convert_Richards_2021_to_h5ad.html).

This notebook converts the dataset as downloaded from the web into the `.h5ad`
format for downstream analysis.




## Convert Fazzari 2024 dataset to h5ad

Links: [jupyter notebook](public_dataset_analysis/convert_fazzari_2024_to_h5ad.ipynb) and [html file](https://KalebicLab.github.io/morphogb/public_dataset_analysis/convert_fazzari_2024_to_h5ad.html).

This notebook converts the dataset as downloaded from the web into the `.h5ad`
format for downstream analysis.




## Public dataset analysis – Neftel 2019

Links: [jupyter notebook](public_dataset_analysis/public_dataset_analysis_Neftel_2019.ipynb) and [html file](https://KalebicLab.github.io/morphogb/public_dataset_analysis/public_dataset_analysis_Neftel_2019.html).

This notebook plots relevant signatures and data from the Neftel 2019 dataset
and computes several gene signature scores.




## Public dataset analysis – Richards 2021

Links: [jupyter notebook](public_dataset_analysis/public_dataset_analysis_Richards_2021.ipynb) and [html file](https://KalebicLab.github.io/morphogb/public_dataset_analysis/public_dataset_analysis_Richards_2021.html).

This notebook plots relevant signatures and data from the Richards 2021 dataset
and computes several gene signature scores.




## Public dataset analysis – Fazzari 2024

Links: [jupyter notebook](public_dataset_analysis/public_dataset_analysis_Fazzari_2024.ipynb) and [html file](https://KalebicLab.github.io/morphogb/public_dataset_analysis/public_dataset_analysis_Fazzari_2024.html).

This notebook plots relevant signatures and data from the Fazzari dataset
and computes several gene signature scores.




## Gene lists comparison

Links: [jupyter notebook](public_dataset_analysis/gene_lists_comparison.ipynb) and [html file](https://KalebicLab.github.io/morphogb/public_dataset_analysis/gene_lists_comparison.html).

This notebook contains additional analysis on the relevant gene lists and
compares the different gene signatures used in the study.





---
*Note: this README file has been generated automatically.* <br>
*Please do not modify it directly but instead work on [this config file](resources/config.yaml).*



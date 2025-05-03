#TFM_BIO_2025

I'll upload the files I'll be working on to this repository.

- The "Data_check..." files are a first look at the Clinic, etc. files, where some unnecessary columns are removed. The resulting data frames are saved in Pickle format (they work better in Python when loading, and the data types are maintained).

- I started the imputation of zeros and the correction for sex and age for the FA matrices (Pre_processing_FA_Null_Age_Sex-HCB / NAPLES.ipynb).
You'll see that I've generated new folders in addition to those provided, where the corrected connectivity matrices are stored. The first lines of the file explain what I've done.

Apr 6

- Added a Pre_processing_FA_Corrected_Analysis_HCB / Naples that would cover all preprocessing:
- Imputation
- Covariates
- Normalization
- Combating
- Matrix visualizations by type

Apr 22

- Added all preprocessing for all layers (Pre_processing_...)
- Added generation of graph metrics per layer and multi-layer (Grap-Metrics...)

May 3

- Added all GNN strategies    
- Minor midificaitons in previous .ipynb files for better documentation and understanding of the steps done.

 
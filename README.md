#TFM_BIO_2025

Project Summary
- This repository contains all the notebooks and scripts used for the Master's Thesis on multimodal brain network analysis in Multiple Sclerosis (MS). All files are thoroughly documented and designed to be self-explanatory.

Contents and Workflow
- Data inspection and cleaning: The Data_check_... notebooks perform an initial exploration of the clinical and connectivity datasets. Unnecessary columns are removed, and the resulting cleaned DataFrames are saved in Pickle format to preserve data types and improve loading performance in Python.

- Preprocessing of FA matrices: The Pre_processing_FA_Null_Age_Sex_... notebooks apply imputation of zero values and linear correction for age and sex on FA connectivity matrices. New folders store the corrected matrices, and each step is documented at the beginning of the notebooks.

- Complete preprocessing pipeline: The Pre_processing_FA_Corrected_Analysis_... notebooks include the full preprocessing steps: Imputation of missing values, Covariate correction, Min-max normalization, Batch harmonization using ComBat, Matrix visualization before and after correction

- Added full preprocessing workflows for all layers (FA, GM, rsfMRI) and the generation of graph metrics (global and nodal) for both single-layer and multilayer networks.

- Integrated all Graph Neural Network (GNN) strategies, including training, evaluation, and interpretation. Minor improvements were made to existing notebooks for clarity and reproducibility. Multilayer data processing was finalized, including calculations and figures for each section.


Order to read the files:

1 - #Data_check_CLINIC_HCB-CLINIC_Naples.ipynb

2a - #Pre_processing_FA_Corrected_Analysis-HCB_new.ipynb
2b - #Pre_processing_FA_Corrected_Analysis-Naples_new.ipynb
2c - #Pre_processing_GM_Corrected_Analysis-NAPLES_new.ipynb
2d - #Pre_processing_GM_Corrected_Analysis_HCB_new.ipynb
2e - #Pre_processing_rsfMRI_Corrected_Analysis-HCB_new.ipynb
2f - #Pre_processing_rsfMRI_Corrected_Analysis-NAPLES_new.ipynb

3a - #Graph-Metrics_Generation-Layer_and_Multilayer.ipynb
3b - #Graph-Metrics-Analisys-Global-Layer-Layer.ipynb
3c - #Graph-Metrics-Analisys-Global-MultiLayer.ipynb
3d - #Graph-Metrics-Analisys-Nodal-Layer-Layer.ipynb
3e - #Graph-Metrics-Analisys-Nodal-MultiLayer.ipynb

4a - #ML_Intial_GNN-All-Sig_Naples_Layer.ipynb
4b - #ML_Intial_GNN-All-Sig_Naples_MLayer.ipynb
4c - #ML_Initial_GNN_HCB_AllLayers.ipynb

All these files are fully documented and are self-reading explainable. 


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
- Multilayer data was loaded with all the calcualtions, figures, etc. performed in each section.

 

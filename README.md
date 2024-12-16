# AITAC_Rep_Fall2024

### Attributions
This project incorporates code from AI-TAC (https://github.com/smaslova/AI-TAC), licensed under the MIT License.

Copyright (c) 2019 smaslova

This repository includes the codes from two different attempts to replicate the prediction of mouse immune cell ATAC-seq signal from peak sequences using data from the Immunological Genome Project: http://www.immgen.org/ (accession no. GSE100738), with reference from the OG AI-TAC repository.

1. Notebooks: Including notebooks and codes from the 2 attempts and intended innovations
   
- First_Attempt_RawData_Analysis.ipynb and First_Attempt_RawData_Analysis_V2.ipynb: Analysis of the raw data downloaded from the Immunological Genome Project website.
  Result: Failed to replicate the results due to 
- Second_Attempt_sample_data_Analysis: Use the available processed data of 100 NGUs from the original Github to train the available AI-TAC Model from the AI-TAC Repository by running:

python train_test_aitac.py model_name '../data/one_hot_seqs.npy' '../data/cell_type_array.npy' 

  Result: Succesfully trained the model and generated outputs.
- Noise Reduction

2. sample_data: (from AI-TAC) This folder contains examples of the data files that serve as input into the AI-TAC model.

- one_hot_seqs.npy - tensor of one-hot-encoded sequences of 100 ATAC-seq open chromatin regions (OCRs)
- cell_type_array.npy - matrix of normalized ATAC-seq peak values for the same 100 OCRs
- peak_names.npy - IDs of 100 OCRs in sample data
- cell_type_names.npy - names of the 81 cell types in ATAC-seq dataset, in the same order as the data in cell_type_array.npy
- filter_set99_index.txt - indices of 99 reproducible filters in the AI-TAC model

3. Outputs:
   Results from the second attempts

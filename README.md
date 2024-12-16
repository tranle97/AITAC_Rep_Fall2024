# AITAC_Rep_Fall2024

The original (OG) repository: https://github.com/smaslova/AI-TAC

This repository includes the codes from two different attempts to replicate the prediction of mouse immune cell ATAC-seq signal from peak sequences using data from the Immunological Genome Project: http://www.immgen.org/ (accession no. GSE100738), with reference from the OG AI-TAC repository.

1. Codes: Including codes from the 2 attempts and intended innovations
   
- First attempt: Analysis of the raw data downloaded from the Immunological Genome Project website.
  Result: Failed to replicate the results due to 
- Second attempt: Use the available processed data of 100 NGUs from the original Github to train the available AI-TAC Model from the OG repository.
  Result: Succesfully trained the model and
- Innovation: Noise Reduction.

2. sample_data: This folder contains examples of the data files that serve as input into the AI-TAC model.

- one_hot_seqs.npy - tensor of one-hot-encoded sequences of 100 ATAC-seq open chromatin regions (OCRs)
- cell_type_array.npy - matrix of normalized ATAC-seq peak values for the same 100 OCRs
- peak_names.npy - IDs of 100 OCRs in sample data
- cell_type_names.npy - names of the 81 cell types in ATAC-seq dataset, in the same order as the data in cell_type_array.npy
- filter_set99_index.txt - indices of 99 reproducible filters in the AI-TAC model

3. Output: Results from the second attempts

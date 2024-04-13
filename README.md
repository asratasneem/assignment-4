# Assignment-4


## Author
-Asra Tasneem Shaik

## Date
-04/12/2024

## Programming Language & Version
-Python

## Dependencies
-Pandas.
-gzip.
-Numpy.
-bz2 (This module offers a complete set of tools for compressing and decompressing data using the bzip2 compression algorithm).


## Description
- Data Extraction: Extracted upstream regulatory sequences from a compressed .bz2 file, where each sequence was associated with a distinct gene ID.
- Score Calculation: Implemented a sliding window technique to apply a weight matrix to each sequence, generating a cumulative score for possible binding sites.
- Sequence Evaluation: Calculated scores for each gene’s sequence by summing contributions from each position in the weight matrix and ranked the sequences accordingly.
- Gene Identification: Identified the top 30 gene IDs with the highest scores, highlighting those with potential binding sites closely matching the specified PSM.


## Input files
-E_coli_K12_MG1655.400_50

-argR-counts-matrix.txt


## Results
- The analysis identified the top 30 genes that are most likely to have binding sites similar to the profile specified in the weight matrix. These genes are prime candidates for further experimental validation to confirm regulatory interactions.

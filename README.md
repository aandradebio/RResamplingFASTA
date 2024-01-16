# Random Resampling Script

## Overview

This R script performs random resampling of sequences from a given FASTA file and saves each resampling into separate FASTA files. The script uses the Bioconductor's Biostrings package for sequence handling.

## Prerequisites

Make sure you have R installed on your system. You can download R from [https://www.r-project.org/](https://www.r-project.org/).

Install the Bioconductor's Biostrings package by running the following commands in R:

```R
if (!requireNamespace("BiocManager", quietly = TRUE))
  install.packages("BiocManager")
BiocManager::install("Biostrings")```

## Usage

```Rscript random_resampling.R input_fasta output_folder num_resamples num_sequences```

input_fasta: Path to the input FASTA file.
output_folder: Path to the output folder where resampled FASTA files will be saved.
num_resamples: Number of resamplings to perform.
num_sequences: Number of sequences to include in each resampling.

Example: Rscript random_resampling.R path/to/your/input.fasta path/to/your/output_folder 100 1500

## Output

The script will generate a specified number of resampled FASTA files in the specified output folder. Each file will contain the specified number of sequences randomly selected from the input FASTA file.

## Author

Amanda Araújo S. Andrade

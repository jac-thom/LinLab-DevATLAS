# About
This github repo hosts a copy of the code used to generate the scRNAseq results for the required DevATLAS manuscript submitted to Neuron in Fall 2024.<br>
While the manuscript is under review, raw data files are restricted to access only through the NCBI GEO accession reviewer token. 

# Reviewer information
Please note that samples GSM7696619-22 can be used as input to `001_Scanpy_preprocessing_DG`. GSE240350 supplemental files contain only cells that passed QC filters. <br>
Although the file names do not match exactly, the analysis pipeline beginning in `002_Seurat_preprocessing_DG` can be replicated by constructing a Seurat object from `GSE240350_mergedSamples_filteredCells_RNA_counts.csv` and `GSE240350_mergedSamples_filteredCells_cell_metadata.csv`.

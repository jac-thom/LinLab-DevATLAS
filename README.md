# About
This project outlines the code used to analyze the mouse DG scRNA-seq data presented in [Xue et al. 2024 bioRxiv](https://pmc.ncbi.nlm.nih.gov/articles/PMC10802351/). 
<br><br>
The RNA-seq data has been made publicly available at [GSE240350](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE240350).
<br><br>
Without the original package environment this code will not identically replicate the results presented in the manuscript.
<br><br>
```
LinLab-DevATLAS/
├── tools/
│   ├── args_list.csv
│   └── high_n_color_palette.csv
├── 001_Scanpy_preprocessing_DG.ipynb             # entry point if re-running GSE240350 FASTQ through cellranger 
├── 002_Seurat_preprocessing_DG.ipynb             # entry point if building Seurat from GSE240350 supp. files
├── 003_Seurat_clustering-gsea-pseudotime.ipynb
├── 004_tdT_analysis_MAST-GSEA.ipynb
└── README.md
```

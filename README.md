# About
This project outlines the code used to analyze the mouse DG scRNA-seq data presented in [Xue et al. 2024 bioRxiv](https://pmc.ncbi.nlm.nih.gov/articles/PMC10802351/). 
<br><br>
The RNA-seq data has been made publicly available at [GSE240350](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE240350).
<br><br>
Without the original package environment this code will not identically replicate the results presented in the manuscript. Therefore, key outputs from the analysis have been made available in `results` (see site map for descriptions).
<br><br>


```
LinLab-DevATLAS/
├── README.md
├── 001_Scanpy_preprocessing_DG.ipynb             # entry point if re-running GSE240350 FASTQ through cellranger 
├── 002_Seurat_preprocessing_DG.ipynb             # entry point if building Seurat from GSE240350 suppl files
├── 003_Seurat_clustering-gsea-pseudotime.ipynb   # exit point for GSE240350 supp. files
├── 004_tdT_analysis_MAST-GSEA.ipynb
├── results/ 
│   ├── 003_cluster/                              # RDS and CSV files related to cluster composition and marker genes
│   ├── 003_pseudotime/                           # CSV files related to pseudotime calculations
│   └── 004_DE/                                   # all DE results from 7904 pre-filtered genes expressed in at least 25% of GCs
└── tools/
    ├── args_list.csv
    └── high_n_color_palette.csv
```
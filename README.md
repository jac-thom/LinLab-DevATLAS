# About
`submission_code` contains the step-by-step analysis I performed on the developmental DevATLAS DG dataset for submission to Nature Methods in August 2023.
<br><br>
The Jupyter Notebook (`.ipynb`) files can be previewed in the github browser and can be forked/cloned to your local computer or the Syracuse VM so that you can reproduce the analysis. 

# Input files
Most data files needed to reproduce this analysis were too large for github and are thus available on the Syracuse VM at `/home/upstate/` within various subdirs.
### raw data
For input to:
> cellranger

The raw fastq files are found here: `/home/upstate/deliv_Lin_EXT_120120_raw`
### cellranger ouput
For input to:
> `001_Scanpy_preprocessing_DG.ipynb`

This pipeline can be reproduced from the cellranger output of the SH snRNAseq libraries. 
Compressed cellranger output for each of the four SH libraries used in this analysis are available here: `/home/upstate/LinLab-NGS_data/submission_data_GEO_Aug2023`

### cellranger postprocessing
For input to:
> `002_Seurat_preprocessing_DG.ipynb`

The outcome of cellranger postprocessing is the same for the SH dataset submitted for publication and the SH dataset utilized in my disseration. <br>
Therefore, if you want to run this pipeline without having to perform the cellranger or scanpy steps, you can use the compressed files found at `/home/upstate/LinLab-NGS_data/scRNAseq_pipeline/SH_raw.tar.gz`.

# Output files
Since the goal of providing this resource is to ease re-submission and not as a tutorial, I have also provided nearly every data object/ file generated in the pipeline.
### processed-data
For input to/ output from:
> `002_Seurat_preprocessing_DG.ipynb`
> `003_Seurat_clustering-gsea-pseudotime.ipynb`
> `004_tdT_analysis_MAST-GSEA.ipynb`

The Seurat objects and SingleCellExperiment objects utilized in this analysis can be found here:`/home/upstate/LinLab-NGS_data/submission_code/processed-data`.<br>
The idea is that if you want to reproduce or tweak the analysis, you can fork/clone this repo and copy the `processed-data` folder directly into your local/VM `submission_code` dir where it should integrate with the code already present in the notebook files.

### results
Output from:
> `002_Seurat_preprocessing_DG.ipynb`
> `003_Seurat_clustering-gsea-pseudotime.ipynb`
> `004_tdT_analysis_MAST-GSEA.ipynb`

These files were requested by Alex or are part of the analysis pipeline that must be saved. Luckily they are small enough to be hosted on github directly in the `submission_code/results` dir.
>[!NOTE]
>These files are not intended for direct submission to journals. They have not been formatted properly.
>If you are looking for the results files that are ready to be submitted to the journal, look in `LinLab-NGS/DevATLAS_submission/submission_data_GEO_Aug2023` for a handful of files and the complete file list stored at `/home/upstate/submission_data_GEO_Aug2023`.

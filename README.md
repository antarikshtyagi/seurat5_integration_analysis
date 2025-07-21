# seurat5_integration_analysis
This jupyter notebook uses seurat5 R-conda environment. This environment can be installed using the seurat5.yml file
To install this environment run the following commands in an interactive session:

1. module load miniconda
2. conda env create -f seurat5.yml
3. Since a R-conda repository is not available for easybio, run these three commands
	conda activate seurat5
	R
	install.packages("easybio", repos = c("https://person-c.r-universe.dev", "https://cloud.r-project.org"))
4. Update the new conda environment on McCleary by 
	ycrc_conda_env.sh update
5. Before starting the analysis, mkdir matrix and copy the cellRanger filtered_feature_bc_matrix folder to the "matrix" folder named by sample. for example
ls matrix
KO_filtered_feature_bc_matrix   WT_filtered_feature_bc_matrix

6. Start a jupyter session in Open On demand and select seurat5 in the drop down menu. 12 hours, 1 CPU, 100G
7. open the sc-RNAseq_seurat_integration.ipynb and follow the comments in the cells

################

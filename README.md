# CellInteractionScores

Dear reader,

Here's a simple procedure that we developped to predict pairwise cell-to-cell interactions from  bulk gene expression data.

The method considers each cell-cell interaction as a quantitative variable dependent on the relative expression values of the receptor and the ligand. The method works readily and robustly across different data sets and cell types because the expression values are encoded by their rank. The rank-based comparison generates a global and balanced picture of cell-to-cell interactomes without overemphasizing genes with extremely high expression values

For each pairs of cells, and each interaction in our Receptor Ligand DataBase (or any other R-L database of your choice), the script ranks the receptors and ligands  and then normalizes the sum of these two ranks so as to get a score ranging from 0 to 1. 

For datasets with multiple regulator cells (ligand providers) and/or regulated cells(receptors), cell-to-cellinteractomes generated with our method can be compared with each other with standard tools of statistical learning (e.g., PCA, clustering) to extract cell-type-specific features.
In the script, we further propose to use z-scores to identify interactions which are specific to certain pairs of interactors. 

We first used this method to predict potential interactions between hematopoietic progenitors and the bone marrow niche in mice, the paper is now published in Blood ([Mende, Jolly, Percin et al.](https://doi.org/10.1182/blood.2019000176)). Please refer to this paper when using this method.


Please do not hesitate to contact me if you have any questions regarding the method.

Cheers,


Adrien 

# Contact

a.jolly@dkfz-heidelberg.de


# Expression levels of NEDD8 and neddylation gene-signature in lung-cancer associated immune and non-immune populations

This repository contains the R script to reproduce bioinformatics analyses from the work by Jimenez-Lasheras et al. 2024. Using the single-cell lung cancer atlas by [Prazanowska et al 2023](https://www.nature.com/articles/s41597-023-02074-6), we first examined the expression of NEDD8 and a neddylation signature (Reactome) in tumor-associated immune and non-immune populations (Fig. 1a). Our results suggest an important role of NEDD8 during the differentiation of effector-like and proliferative CD8+ T cells, reaching expression levels comparable to cancer cells (Fig 1b). These results were confirmed for NEDD8 expression by interrogating three representative datasets of lung cancer [GSE131907](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE131907), melanoma [GSE115978](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE115978) and hepatocarcinoma [GSE125499](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE125449). 

The annotated R markdown file (nedd8_expression_v3_final.Rmd) interrogates the expression of both NEDD8 and the neddylation signature in naïve-like and effector-like CD8+ T cells in the above-mentioned datasets (Fig. 1c). Briefly, high-quality T cells were filtered using [scGate](https://github.com/carmonalab/scGate) and annotated using a [human CD8+ T cell](https://figshare.com/articles/dataset/ProjecTILs_human_reference_atlas_of_CD8_tumor-infiltrating_T_cells_CD8_TIL_version_1/23608308) reference map with [ProjecTILs](https://github.com/carmonalab/ProjecTILs). The expression of the neddylation signature from Reactome was evaluated using [UCell](https://github.com/carmonalab/UCell).

Fig. 1a. UMAP plot of immune and non-immune populations associated with lung cancer.
![LC_1_S2_minor-1](https://github.com/eprieto012/nedd8_APLab/assets/98150852/791ee874-c049-476b-8ab6-0a040a1f3728)

Fig. 1b. Violin plots showing the expression levels of the indicated markers (NEDD8 and NAE1) or the neddylation gene-signature (Reactome) in lung cancer-associated immune and non-immune populations.
![LC_1_S2_minor_vln-1](https://github.com/eprieto012/nedd8_APLab/assets/98150852/aa513366-8da7-43a1-96b1-b2b4f2888ea7)

Fig. 1c. Dot plots showing the mean expression levels of NEDD8 in 5-cell interactions (n=50) across the indicated types of cancer and phenotypes.
![plot_iter_nedd8-1](https://github.com/eprieto012/nedd8_APLab/assets/98150852/b6fc65b5-81c1-4e16-b86d-b09e2571a7ab)

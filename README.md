# Preprocessing perturbation data of Open Problems: single cell perturbation for NeurIPS 2023


## Motivation

In 2023, Open Problems hosted a competition with the aim of prediction how small modules affect gene expression profiles. See the [Kaggle
competition page](https://www.kaggle.com/competitions/open-problems-single-cell-perturbations/overview). However, the provided dataset contained serious biases, raised in [our previous report] (https://storage.googleapis.com/kaggle-forum-message-attachments/2559525/20057/OP2_Write_Up_JN_AP.pdf). In this study, we aimed at enhancing the quality of the perturbation data by addressing the potential biases. The notebook of the analysis can be found in the `notebooks`. The results of this analysis was contributed to post competition analysis report submitted to [NeurIPS 2023 competition
track](https://neurips.cc/virtual/2023/competition/66586). 


The analysis primarily focuses on the perturbation data, with an emphasis on identifying potential outliers. Extensive explanatory data analysis (EDA) was conducted on single-cell data, pseudobulked data, and the results of the differential expression (DE) analysis. Furthermore, the validity of cell type annotations was rigorously evaluated by cross-checking across donors, Leiden clusters, and biomarkers. Also, new cell type annotations were proposed using CellTypist, revealing higher consistency. Additionally, cluster-specific and compound-specific evaluations were carried out to pinpoint outliers. Subsequently, the single-cell data was pseudobulked and subjected to DE analysis using both the Voom+Limma and EdgeR pipelines 

In addition, in the folder 'src/task/methods`, there is the clean implementation of deep NN model proposed by our team which ranked the 20th place in the competition.


## Authors & contributors

| name              | roles  |
|:------------------|:-------|
| Jalil Nourisa     | author |


# Using gene expression to identify cancer type
Goal: Identifying cancer type based on gene expression and identifying the relevant genes in performing this task

Introduction: 
  There are tens of trillions of cells in the human body, and in their neucleas (core), they have the same DNA. DNA is just a long molecule that contains instructions for cells, and based on the cell type, each cell only reads and executes parts of these instructions. Each DNA can be split to several parts, known as genes, each containing one instruction. The human body contains about 30 thousand genes.
  The data used in this analysis, describes how each gene is expressed in cancer patients. The data belongs to patients suffering from one of these 5 types of cancer:
  - BRCA: Breast invasive carcinoma
  - KIRC: Kidney renal clear cell carcinoma
  - LUAD: Lung adenocarcinoma
  - PRAD: Prostate adenocarcinoma
  - COAD: Colon adenocarcinoma

Skills required:
  - Python programming
  - Understanding Numpy, Pandas, Matplotlib libraries
  - Understanding machine learning algorithms such as Random Forest, and Logistic regression
  - Feature selection
  - Dimentionality reduction
  - Data visualization and reporting
  - Very basic understanding of microbiology
  
Method:
  - Random Forest, and Logistic regression were used for classification of samples.
  - Random Forest was used for feature selection and identification of important genes.
  - PCA was used for dimentionality reduction in order to enable visualization.
  
Results:
  - Random Forest, and Logistic regression reached a classification accuracy of 100% which means that the initial data is enough to identify the type of cancer a patient has, and some of the features (genes) may not even be useful in performing this task.
  - Through feature selection, 100% classification accuracy was achieved by only using 22 features (genes), which means that these features have all the data we need to identify the cancer type in a patient. These genes were identified.
  - By using PCA, the minention of data was reduced to 2 which enabled visualization. Te visualization shows that COAD and LUAD have certain similarities in their gene expression. LUAD and BRCA also show similarities.

Data used from:
https://archive.ics.uci.edu/ml/datasets/gene+expression+cancer+RNA-Seq
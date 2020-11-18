# Project outlines
## Title
### Building a classification model of NGS RNA-seq data with MLseq.      
## Author
### Bo Cheng
## Overview 
### 1. In this project, I will try to use a machine learning package from Bioconductor to build a model which can predict breast cancer subtype. 
### 2. I will try to optimize model parameters and find a good classifier in MLSeq. I will also use 9 data sets from TCGA to train and test this model. six as training data, and three as testing data.
### 3. The main goal of this project is to have a taste of machine learning in R. So I may do many copy and paste, but I will give my understanding and opinions in the R notebook.
### 4. The original package link: https://www.bioconductor.org/packages/devel/bioc/vignettes/MLSeq/inst/doc/MLSeq.pdf
### 5. The original Vignettes/sample link: https://www.bioconductor.org/packages/devel/bioc/vignettes/MLInterfaces/inst/doc/MLprac2_2.pdf
## Data availability
### All data are available from [TCGA](https://portal.gdc.cancer.gov/exploration?filters=%7B%22op%22%3A%22and%22%2C%22content%22%3A%5B%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.disease_type%22%2C%22value%22%3A%5B%22ductal%20and%20lobular%20neoplasms%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.primary_site%22%2C%22value%22%3A%5B%22breast%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.project.program.name%22%2C%22value%22%3A%5B%22TCGA%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.project.project_id%22%2C%22value%22%3A%5B%22TCGA-BRCA%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.samples.sample_type%22%2C%22value%22%3A%5B%22primary%20tumor%22%5D%7D%7D%5D%7D)
### The dataset list(Case ID)
#### 1.he Training data and testing data are from TCGA, 40 datasets in total. Training datasets : testing datasets = 7:3
#### 2.When we download datasets from TCGA, we can add the htseq file into cart, and download them as a comprised file.
## Milestone1
### Progress
#### Accroding to the Vignette, I've input the data and converted the data to be right dataframes which are ready to do MLSeq. And the next step is to choose a model, do the Normalization and transformation, and use the normalized data to train model.
## Milestone2
### What I've done
#### 1.I use 28 datasets to training all the model offered by MLSeq, and use 12 dataset to test the model.
#### 2.I find out the best model I have now is "voomNSC", which has about 75% accuracy.
#### Below is the table of accuracy of the four models
Model | Accuracy 
----- | -------- 
voomNSC | 75%
plda | 50%
plda2 | 46.43%
svm | 53.57%
NSC | 51.85
nblda | 46.43%


#### 3.The possible biomarkers I found is:
ensembl_gene_id_version | entrezgene_id | description | hgnc_symbol
------------ | ------------- | ---------------- | -----------
ENSG00000124107.5	 | 6590 | secretory leukocyte peptidase inhibitor [Source:HGNC Symbol;Acc:HGNC:11092] | SLPI
ENSG00000198888.2 | 4535 | mitochondrially encoded NADH:ubiquinone oxidoreductase core subunit 1 [Source:HGNC Symbol;Acc:HGNC:7455] | MT-ND1
#### *This is selected possible biomarkers are from inner_join of voomNSC,plda, and plda2 model, there is no possible biomarkers selected from NSC model.
  
### What issues I found
#### 1.I found in the vignette is the "voomDLDA" method, which has errors for now I can't solve, so I just skip this method.
#### 2.Another thing is the model accuracy is low, maybe I need more dataset.
#### 3.For the HTML, I still can't make the HTML, the issue is from my input data function, I input my data once a time and print the table, so the HTML will contain so much table, so HTML does not work well.
## Deliverable
### I will use R MarkDown/Notebook/Jupyter to display a understandable codes.